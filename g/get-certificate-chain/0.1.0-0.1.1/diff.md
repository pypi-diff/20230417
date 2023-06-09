# Comparing `tmp/get_certificate_chain-0.1.0.tar.gz` & `tmp/get_certificate_chain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_certificate_chain-0.1.0.tar", max compression
+gzip compressed data, was "get_certificate_chain-0.1.1.tar", max compression
```

## Comparing `get_certificate_chain-0.1.0.tar` & `get_certificate_chain-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     3580 2023-04-16 21:51:26.498276 get_certificate_chain-0.1.0/README.md
--rw-r--r--   0        0        0    13720 2023-04-16 21:39:56.386517 get_certificate_chain-0.1.0/get_certificate_chain.py
--rw-r--r--   0        0        0      733 2023-04-16 22:08:33.192960 get_certificate_chain-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     3964 2023-04-17 14:49:17.941113 get_certificate_chain-0.1.1/README.md
+-rw-r--r--   0        0        0    15843 2023-04-17 14:33:13.405779 get_certificate_chain-0.1.1/get_certificate_chain.py
+-rw-r--r--   0        0        0      733 2023-04-17 14:55:28.819742 get_certificate_chain-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.1/PKG-INFO
```

### Comparing `get_certificate_chain-0.1.0/LICENSE.md` & `get_certificate_chain-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.0/get_certificate_chain.py` & `get_certificate_chain-0.1.1/get_certificate_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,34 @@
 import glob
 import os
 import logging
 import re
 import ssl
 import socket
 import sys
-from typing import Any, Dict, List
-from urllib.request import urlopen, Request
+from typing import Any, Dict, List, Union
+from urllib.request import urlopen
 
 # Third-party library imports
 import argparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 CERT_CHAIN = []
 
 # Configure logging
 logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s [%(levelname)s] %(message)s"
+    level=logging.WARNING, format="%(asctime)s [%(levelname)s] %(message)s"
 )
 
 
+# parse arguments
 def parse_arguments():
     """
     Parse command line arguments.
 
     Returns:
         argparse.Namespace: Parsed arguments.
     """
@@ -61,384 +62,407 @@
         dest="domain",
         default="www.google.com",
         help="The hostname to connect to. (default: %(default)s)",
     )
     return parser.parse_args()
 
 
-def remove_cacert_pem():
-    """
-    Remove certificate files from the current directory.
-    """
-    for crt_file in glob.glob("*.crt"):
-        os.remove(crt_file)
-    for pem_file in glob.glob("*.pem"):
-        os.remove(pem_file)
-
-
-def get_cacert_pem():
-    """
-    Download the cacert.pem file from the curl.se website.
-    """
-    cacert_pem_url = "https://curl.se/ca/cacert.pem"
-    cacert_pem_file = "cacert.pem"
-    logging.info("Downloading %s to %s", cacert_pem_url, cacert_pem_file)
-    with urlopen(cacert_pem_url) as response, open(cacert_pem_file, "wb") as out_file:
-        if response.getcode() != 200:
-            logging.error(
-                "Error downloading %s. HTTP status code: %s",
-                cacert_pem_url,
-                response.getcode(),
-            )
+class SSLCertificateChainDownloader:
+    def __init__(self):
+        self.cert_chain = []
+
+    def remove_cacert_pem(self):
+        """
+        Remove certificate files from the current directory.
+        """
+        for crt_file in glob.glob("*.crt"):
+            os.remove(crt_file)
+        for pem_file in glob.glob("*.pem"):
+            os.remove(pem_file)
+
+    def get_cacert_pem(self):
+        """
+        Download the cacert.pem file from the curl.se website.
+        """
+        cacert_pem_url = "https://curl.se/ca/cacert.pem"
+        cacert_pem_file = "cacert.pem"
+        logging.info("Downloading %s to %s", cacert_pem_url, cacert_pem_file)
+        with urlopen(cacert_pem_url) as response, open(
+            cacert_pem_file, "wb"
+        ) as out_file:
+            if response.getcode() != 200:
+                logging.error(
+                    "Error downloading %s. HTTP status code: %s",
+                    cacert_pem_url,
+                    response.getcode(),
+                )
+                sys.exit(1)
+            data = response.read()
+            out_file.write(data)
+        logging.info("Downloaded %s to %s", cacert_pem_url, cacert_pem_file)
+
+    def check_domain(self) -> Dict[str, Any]:
+        """
+        Check and parse the domain provided by the user.
+
+        Args:
+            domain (str): The domain provided by the user.
+
+        Returns:
+            Dict[str, Any]: A dictionary containing the hostname and port.
+        """
+        hostname, _, port = self.domain.partition(":")
+        return {"hostname": hostname, "port": int(port) if port else 443}
+
+    def get_certificate(self, hostname: str, port: int) -> x509.Certificate:
+        """
+        Connect to a server and retrieve the SSL certificate.
+
+        Args:
+            hostname (str): The hostname to connect to.
+            port (int): The port to connect to.
+
+        Returns:
+            x509.Certificate: The SSL certificate of the server.
+        """
+        try:
+            context = ssl.create_default_context()
+            with socket.create_connection((hostname, port)) as sock:
+                with context.wrap_socket(sock, server_hostname=hostname) as ssl_socket:
+                    cert_pem = ssl.DER_cert_to_PEM_cert(ssl_socket.getpeercert(True))
+                    cert = x509.load_pem_x509_certificate(
+                        cert_pem.encode(), default_backend()
+                    )
+            return cert
+        except ConnectionRefusedError:
+            print(f"Connection refused to {hostname}:{port}")
+            sys.exit(1)
+        except ssl.SSLError as e:
+            print(f"SSL error: {e}")
+            sys.exit(1)
+        except socket.timeout:
+            print(f"Connection timed out to {hostname}:{port}")
+            sys.exit(1)
+        except socket.gaierror:
+            print(f"Hostname could not be resolved: {hostname}")
             sys.exit(1)
-        data = response.read()
-        out_file.write(data)
-    logging.info("Downloaded %s to %s", cacert_pem_url, cacert_pem_file)
-
-
-def check_domain(domain: str) -> Dict[str, Any]:
-    """
-    Check and parse the domain provided by the user.
-
-    Args:
-        domain (str): The domain provided by the user.
-
-    Returns:
-        Dict[str, Any]: A dictionary containing the hostname and port.
-    """
-    hostname, _, port = domain.partition(":")
-    return {"hostname": hostname, "port": int(port) if port else 443}
-
 
-def get_certificate(hostname: str, port: int) -> x509.Certificate:
-    """
-    Connect to a server and retrieve the SSL certificate.
+    def normalize_subject(self, subject: str) -> str:
+        """
+        Normalize the subject of a certificate.
+
+        Args:
+            subject (str): The subject of the certificate.
+
+        Returns:
+            str: The normalized subject.
+        """
+        return "_".join(
+            part.strip()
+            .replace("=", "_")
+            .replace(".", "_")
+            .replace(" ", "_")
+            .replace(",", "_")
+            for part in subject.split("/")
+            if part.strip()
+        )
 
-    Args:
-        hostname (str): The hostname to connect to.
-        port (int): The port to connect to.
+    def save_ssl_certificate(
+        self,
+        ssl_certificate: x509.Certificate,
+        file_name: str,
+    ) -> None:
+        """
+        Save an SSL certificate to a file.
+
+        Args:
+            ssl_certificate (x509.Certificate): The SSL certificate to save.
+            file_name (str): The file name to save the SSL certificate as.
+        """
+        with open(file_name, "wb") as f:
+            f.write(ssl_certificate.public_bytes(encoding=serialization.Encoding.PEM))
+
+    def write_chain_to_file(self, certificate_chain: List[x509.Certificate]) -> None:
+        """
+        Write a certificate chain to files.
+
+        Args:
+            certificate_chain (List[x509.Certificate]): The certificate chain to write to files.
+        """
+        for counter, certificate_item in enumerate(certificate_chain):
+            cert_subject = certificate_item.subject.rfc4514_string()
+            normalized_subject = self.normalize_subject(cert_subject)
+            ssl_certificate_filename = (
+                f"{len(certificate_chain) - 1 - counter}-{normalized_subject}.crt"
+            )
+            self.save_ssl_certificate(certificate_item, ssl_certificate_filename)
 
-    Returns:
-        x509.Certificate: The SSL certificate of the server.
-    """
-    try:
-        context = ssl.create_default_context()
-        with socket.create_connection((hostname, port)) as sock:
-            with context.wrap_socket(sock, server_hostname=hostname) as ssl_socket:
-                cert_pem = ssl.DER_cert_to_PEM_cert(ssl_socket.getpeercert(True))
+    def return_cert_aia(self, ssl_certificate: x509.Certificate) -> x509.Extensions:
+        """
+        Get the Authority Information Access (AIA) extension from a certificate.
+
+        Args:
+            ssl_certificate (x509.Certificate): The SSL certificate.
+
+        Returns:
+            x509.Extensions: The AIA extension or None if not found.
+        """
+        try:
+            aia = ssl_certificate.extensions.get_extension_for_oid(
+                ExtensionOID.AUTHORITY_INFORMATION_ACCESS
+            )
+            return aia
+        except x509.ExtensionNotFound:
+            return None
+
+    def get_certificate_from_uri(self, uri: str) -> x509.Certificate:
+        """
+        Retrieve a certificate from the given URI.
+
+        Args:
+            uri (str): The URI to get the certificate from.
+
+        Returns:
+            x509.Certificate: The certificate from the URI or None if there was an error.
+        """
+        try:
+            with urlopen(uri) as response:
+                if response.getcode() != 200:
+                    return None
+                aia_content = response.read()
+                ssl_certificate = ssl.DER_cert_to_PEM_cert(aia_content)
                 cert = x509.load_pem_x509_certificate(
-                    cert_pem.encode(), default_backend()
+                    ssl_certificate.encode("ascii"), default_backend()
                 )
-        return cert
-    except ConnectionRefusedError:
-        print(f"Connection refused to {hostname}:{port}")
-        sys.exit(1)
-    except ssl.SSLError as e:
-        print(f"SSL error: {e}")
-        sys.exit(1)
-    except socket.timeout:
-        print(f"Connection timed out to {hostname}:{port}")
-        sys.exit(1)
-    except socket.gaierror:
-        print(f"Hostname could not be resolved: {hostname}")
-        sys.exit(1)
-
-
-def normalize_subject(subject: str) -> str:
-    """
-    Normalize the subject of a certificate.
-
-    Args:
-        subject (str): The subject of the certificate.
-
-    Returns:
-        str: The normalized subject.
-    """
-    return "_".join(
-        part.strip()
-        .replace("=", "_")
-        .replace(".", "_")
-        .replace(" ", "_")
-        .replace(",", "_")
-        for part in subject.split("/")
-        if part.strip()
-    )
-
-
-def save_ssl_certificate(ssl_certificate: x509.Certificate, file_name: str) -> None:
-    """
-    Save an SSL certificate to a file.
-
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate to save.
-        file_name (str): The file name to save the SSL certificate as.
-    """
-    with open(file_name, "wb") as f:
-        f.write(ssl_certificate.public_bytes(encoding=serialization.Encoding.PEM))
-
-
-def write_chain_to_file(certificate_chain: List[x509.Certificate]) -> None:
-    """
-    Write a certificate chain to files.
-
-    Args:
-        certificate_chain (List[x509.Certificate]): The certificate chain to write to files.
-    """
-    for counter, certificate_item in enumerate(certificate_chain):
-        cert_subject = certificate_item.subject.rfc4514_string()
-        normalized_subject = normalize_subject(cert_subject)
-        ssl_certificate_filename = (
-            f"{len(certificate_chain) - 1 - counter}-{normalized_subject}.crt"
+                return cert
+        except Exception:
+            return None
+
+    def return_cert_aia_list(self, ssl_certificate: x509.Certificate) -> list:
+        """
+        Get the list of AIA URIs from a certificate.
+
+        Args:
+            ssl_certificate (x509.Certificate): The SSL certificate.
+
+        Returns:
+            list: A list of AIA URIs.
+        """
+        aia_uri_list = []
+
+        for extension in ssl_certificate.extensions:
+            cert_value = extension.value
+
+            if isinstance(cert_value, x509.AuthorityInformationAccess):
+                data_aia = [x for x in cert_value or []]
+                for item in data_aia:
+                    if item.access_method._name == "caIssuers":
+                        aia_uri_list.append(item.access_location._value)
+
+        return aia_uri_list
+
+    def return_cert_aki(self, ssl_certificate):
+        """
+        Get the Authority Key Identifier (AKI) from a certificate.
+
+        Args:
+            ssl_certificate (x509.Certificate): The SSL certificate.
+
+        Returns:
+            x509.AuthorityKeyIdentifier: The AKI extension or None if not found.
+        """
+        try:
+            cert_aki = ssl_certificate.extensions.get_extension_for_oid(
+                ExtensionOID.AUTHORITY_KEY_IDENTIFIER
+            )
+        except x509.extensions.ExtensionNotFound:
+            cert_aki = None
+        return cert_aki
+
+    def return_cert_ski(self, ssl_certificate):
+        """
+        Get the Subject Key Identifier (SKI) from a certificate.
+
+        Args:
+            ssl_certificate (x509.Certificate): The SSL certificate.
+
+        Returns:
+            x509.SubjectKeyIdentifier: The SKI extension.
+        """
+        cert_ski = ssl_certificate.extensions.get_extension_for_oid(
+            ExtensionOID.SUBJECT_KEY_IDENTIFIER
         )
-        save_ssl_certificate(certificate_item, ssl_certificate_filename)
 
+        return cert_ski
 
-def return_cert_aia(ssl_certificate: x509.Certificate) -> x509.Extensions:
-    """
-    Get the Authority Information Access (AIA) extension from a certificate.
+    def load_root_ca_cert_chain(
+        self,
+        filename: str = None,
+        ca_cert_text: str = None,
+    ) -> Dict[str, str]:
+        """
+        Load the root CA certificate chain from a file or text.
+
+        Args:
+            filename (str, optional): The file name containing the root CA certificates.
+            ca_cert_text (str, optional): The text containing the root CA certificates.
+
+        Returns:
+            Dict[str, str]: A dictionary containing the root CA certificates.
+        """
+        if filename is None and ca_cert_text is None:
+            raise ValueError("Either filename or ca_cert_text must be provided")
+
+        ca_root_store = {}
+
+        if filename:
+            with open(filename, "r") as f_ca_cert:
+                ca_cert_text = f_ca_cert.read()
+
+        lines = ca_cert_text.splitlines()
+        line_count = len(lines)
+        index = 0
 
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate.
+        while index < line_count:
+            current_line = lines[index]
 
-    Returns:
-        x509.Extensions: The AIA extension or None if not found.
-    """
-    try:
-        aia = ssl_certificate.extensions.get_extension_for_oid(
-            ExtensionOID.AUTHORITY_INFORMATION_ACCESS
-        )
-        return aia
-    except x509.ExtensionNotFound:
-        return None
+            if re.search(r"^-----BEGIN CERTIFICATE-----", current_line):
+                root_ca_cert = ""
+                index += 1
+                while index < line_count and not re.search(
+                    r"^-----END CERTIFICATE-----", lines[index]
+                ):
+                    root_ca_cert += lines[index] + "\n"
+                    index += 1
 
+                root_ca_cert += lines[index] + "\n"
+                index += 1
 
-def get_certificate_from_uri(uri: str) -> x509.Certificate:
-    """
-    Retrieve a certificate from the given URI.
+                cert = x509.load_pem_x509_certificate(
+                    root_ca_cert.encode(), default_backend()
+                )
+                root_ca_name = cert.subject.rfc4514_string()
 
-    Args:
-        uri (str): The URI to get the certificate from.
+                ca_root_store[root_ca_name] = root_ca_cert
+            else:
+                index += 1
 
-    Returns:
-        x509.Certificate: The certificate from the URI or None if there was an error.
-    """
-    try:
-        with urlopen(uri) as response:
-            if response.getcode() != 200:
-                return None
-            aia_content = response.read()
-            ssl_certificate = ssl.DER_cert_to_PEM_cert(aia_content)
-            cert = x509.load_pem_x509_certificate(
-                ssl_certificate.encode("ascii"), default_backend()
-            )
-            return cert
-    except Exception:
-        return None
+        print(f"Number of Root CA's loaded: {len(ca_root_store)}")
+        return ca_root_store
 
+    def walk_the_chain(
+        self,
+        ssl_certificate: x509.Certificate,
+        depth: int,
+        max_depth: int = 4,
+    ):
+        if depth <= max_depth:
+            cert_aki = self.return_cert_aki(ssl_certificate)
+            cert_ski = self.return_cert_ski(ssl_certificate)
 
-def return_cert_aia_list(ssl_certificate: x509.Certificate) -> list:
-    """
-    Get the list of AIA URIs from a certificate.
+            cert_aki_value = (
+                cert_aki._value.key_identifier if cert_aki is not None else None
+            )
+            cert_ski_value = cert_ski._value.digest
+            logging.info(
+                f"Depth: {depth} - AKI: {cert_aki_value} - SKI: {cert_ski_value}"
+            )
 
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate.
+            if cert_aki_value is not None:
+                aia_uri_list = self.return_cert_aia_list(ssl_certificate)
+                if aia_uri_list:
+                    for item in aia_uri_list:
+                        next_cert = self.get_certificate_from_uri(item)
+
+                        if next_cert is not None:
+                            self.cert_chain.append(next_cert)
+                            self.walk_the_chain(next_cert, depth + 1, max_depth)
+                        else:
+                            logging.warning("Could not retrieve certificate.")
+                            sys.exit(1)
+                else:
+                    logging.warning("Certificate didn't have AIA.")
+                    ca_root_store = self.load_root_ca_cert_chain("cacert.pem")
+                    root_ca_cn = None
+
+                    for root_ca in ca_root_store:
+                        try:
+                            root_ca_certificate_pem = ca_root_store[root_ca]
+                            root_ca_certificate = x509.load_pem_x509_certificate(
+                                root_ca_certificate_pem.encode("ascii")
+                            )
+                            root_ca_ski = self.return_cert_ski(root_ca_certificate)
+                            root_ca_ski_value = root_ca_ski._value.digest
 
-    Returns:
-        list: A list of AIA URIs.
-    """
-    aia_uri_list = []
+                            if root_ca_ski_value == cert_aki_value:
+                                root_ca_cn = root_ca
+                                self.cert_chain.append(root_ca_certificate)
+                                logging.info(
+                                    f"Root CA Found - {root_ca_cn}\nCERT_CHAIN - {self.cert_chain}"
+                                )
+                                break
+                        except x509.extensions.ExtensionNotFound:
+                            logging.info("Root CA didn't have a SKI. Skipping...")
+                            pass
 
-    for extension in ssl_certificate.extensions:
-        cert_value = extension.value
+                    if root_ca_cn is None:
+                        logging.error("Root CA NOT found.")
+                        sys.exit(1)
 
-        if isinstance(cert_value, x509.AuthorityInformationAccess):
-            data_aia = [x for x in cert_value or []]
-            for item in data_aia:
-                if item.access_method._name == "caIssuers":
-                    aia_uri_list.append(item.access_location._value)
+    def run(self, args: Union[argparse.Namespace, dict]):
+        if isinstance(args, argparse.Namespace):
+            self.domain = args.domain
+        elif isinstance(args, dict):
+            self.domain = args.get("domain")
+        else:
+            raise ValueError(
+                "Invalid argument type. Expected argparse.Namespace or dict."
+            )
 
-    return aia_uri_list
+        self.parsed_domain = self.check_domain()
 
+        if isinstance(args, argparse.Namespace):
+            remove_ca_files = args.remove_ca_files
+            get_ca_cert_pem = args.get_ca_cert_pem
+        else:
+            remove_ca_files = args.get("remove_ca_files")
+            get_ca_cert_pem = args.get("get_ca_cert_pem")
 
-def return_cert_aki(ssl_certificate):
-    """
-    Get the Authority Key Identifier (AKI) from a certificate.
+        if remove_ca_files:
+            self.remove_ca_files()
 
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate.
+        if get_ca_cert_pem:
+            self.get_ca_cert_pem()
 
-    Returns:
-        x509.AuthorityKeyIdentifier: The AKI extension or None if not found.
-    """
-    try:
-        cert_aki = ssl_certificate.extensions.get_extension_for_oid(
-            ExtensionOID.AUTHORITY_KEY_IDENTIFIER
+        ssl_certificate = self.get_certificate(
+            self.parsed_domain["hostname"], self.parsed_domain["port"]
         )
-    except x509.extensions.ExtensionNotFound:
-        cert_aki = None
-    return cert_aki
-
-
-def return_cert_ski(ssl_certificate):
-    """
-    Get the Subject Key Identifier (SKI) from a certificate.
 
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate.
+        aia = self.return_cert_aia(ssl_certificate)
 
-    Returns:
-        x509.SubjectKeyIdentifier: The SKI extension.
-    """
-    cert_ski = ssl_certificate.extensions.get_extension_for_oid(
-        ExtensionOID.SUBJECT_KEY_IDENTIFIER
-    )
-
-    return cert_ski
-
-
-def load_root_ca_cert_chain(
-    filename: str = None,
-    ca_cert_text: str = None,
-) -> Dict[str, str]:
-    """
-    Load the root CA certificate chain from a file or text.
-
-    Args:
-        filename (str, optional): The file name containing the root CA certificates.
-        ca_cert_text (str, optional): The text containing the root CA certificates.
-
-    Returns:
-        Dict[str, str]: A dictionary containing the root CA certificates.
-    """
-    if filename is None and ca_cert_text is None:
-        raise ValueError("Either filename or ca_cert_text must be provided")
-
-    ca_root_store = {}
-
-    if filename:
-        with open(filename, "r") as f_ca_cert:
-            ca_cert_text = f_ca_cert.read()
-
-    lines = ca_cert_text.splitlines()
-    line_count = len(lines)
-    index = 0
-
-    while index < line_count:
-        current_line = lines[index]
-
-        if re.search(r"^-----BEGIN CERTIFICATE-----", current_line):
-            root_ca_cert = ""
-            index += 1
-            while index < line_count and not re.search(
-                r"^-----END CERTIFICATE-----", lines[index]
-            ):
-                root_ca_cert += lines[index] + "\n"
-                index += 1
-
-            root_ca_cert += lines[index] + "\n"
-            index += 1
-
-            cert = x509.load_pem_x509_certificate(
-                root_ca_cert.encode(), default_backend()
+        if aia is not None and not self.return_cert_aia(ssl_certificate):
+            logging.error(
+                "Could not find AIA, possible decryption taking place upstream?"
             )
-            root_ca_name = cert.subject.rfc4514_string()
-
-            ca_root_store[root_ca_name] = root_ca_cert
-        else:
-            index += 1
+            sys.exit(1)
 
-    print(f"Number of Root CA's loaded: {len(ca_root_store)}")
-    return ca_root_store
+        self.cert_chain.append(ssl_certificate)
 
+        self.walk_the_chain(ssl_certificate, 1, max_depth=4)
 
-def walk_the_chain(ssl_certificate: x509.Certificate, depth: int, max_depth: int = 4):
-    """
-    Walk through the certificate chain and find the root CA.
+        self.write_chain_to_file(self.cert_chain)
 
-    Args:
-        ssl_certificate (x509.Certificate): The SSL certificate.
-        depth (int): The current depth in the certificate chain.
-        max_depth (int, optional): The maximum depth to search in the certificate chain.
-
-    """
-    if depth <= max_depth:
-        cert_aki = return_cert_aki(ssl_certificate)
-        cert_ski = return_cert_ski(ssl_certificate)
-
-        cert_aki_value = (
-            cert_aki._value.key_identifier if cert_aki is not None else None
-        )
-        cert_ski_value = cert_ski._value.digest
-        logging.info(f"Depth: {depth} - AKI: {cert_aki_value} - SKI: {cert_ski_value}")
-
-        if cert_aki_value is not None:
-            aia_uri_list = return_cert_aia_list(ssl_certificate)
-            if aia_uri_list:
-                for item in aia_uri_list:
-                    next_cert = get_certificate_from_uri(item)
-
-                    if next_cert is not None:
-                        CERT_CHAIN.append(next_cert)
-                        walk_the_chain(next_cert, depth + 1, max_depth)
-                    else:
-                        logging.warning("Could not retrieve certificate.")
-                        sys.exit(1)
-            else:
-                logging.warning("Certificate didn't have AIA.")
-                ca_root_store = load_root_ca_cert_chain("cacert.pem")
-                root_ca_cn = None
-
-                for root_ca in ca_root_store:
-                    try:
-                        root_ca_certificate_pem = ca_root_store[root_ca]
-                        root_ca_certificate = x509.load_pem_x509_certificate(
-                            root_ca_certificate_pem.encode("ascii")
-                        )
-                        root_ca_ski = return_cert_ski(root_ca_certificate)
-                        root_ca_ski_value = root_ca_ski._value.digest
-
-                        if root_ca_ski_value == cert_aki_value:
-                            root_ca_cn = root_ca
-                            CERT_CHAIN.append(root_ca_certificate)
-                            logging.info(
-                                f"Root CA Found - {root_ca_cn}\nCERT_CHAIN - {CERT_CHAIN}"
-                            )
-                            break
-                    except x509.extensions.ExtensionNotFound:
-                        logging.info("Root CA didn't have a SKI. Skipping...")
-                        pass
-
-                if root_ca_cn is None:
-                    logging.error("Root CA NOT found.")
-                    sys.exit(1)
+        logging.info("Certificate chain downloaded and saved.")
 
 
 def main() -> None:
     """
     Main function to execute the script. Parses arguments, retrieves the SSL certificate, walks the chain,
     and writes the certificate chain and PEM-encoded certificates.
     """
     args = parse_arguments()
-
-    domain = check_domain(args.domain)
-
-    ssl_certificate = get_certificate(domain["hostname"], domain["port"])
-
-    aia = return_cert_aia(ssl_certificate)
-
-    if aia is not None and not return_cert_aia(ssl_certificate):
-        print(
-            "ERROR - I could not find AIA. Possible decryption taking place upstream?"
-        )
-        sys.exit(1)
-
-    CERT_CHAIN.append(ssl_certificate)
-
-    walk_the_chain(ssl_certificate, 1, max_depth=4)
-
-    write_chain_to_file(CERT_CHAIN)
-
-    print("Certificate chain downloaded and saved.")
+    downloader = SSLCertificateChainDownloader()
+    downloader.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `get_certificate_chain-0.1.0/pyproject.toml` & `get_certificate_chain-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get_certificate_chain"
-version = "0.1.0"
+version = "0.1.1"
 description = "Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files."
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>", " TheScriptGuy <@nolanrumble>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

