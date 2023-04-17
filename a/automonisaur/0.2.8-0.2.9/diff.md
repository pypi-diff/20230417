# Comparing `tmp/automonisaur-0.2.8.tar.gz` & `tmp/automonisaur-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.2.8.tar", last modified: Fri Feb 25 19:52:27 2022, max compression
+gzip compressed data, was "automonisaur-0.2.9.tar", last modified: Fri Feb 25 21:39:47 2022, max compression
```

## Comparing `automonisaur-0.2.8.tar` & `automonisaur-0.2.9.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 19:52:27.699388 automonisaur-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-02-25 19:52:23.000000 automonisaur-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.683388 automonisaur-0.2.8/automon/
--rwxr-xr-x   0 runner    (1001) docker     (121)       31 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (121)      112 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1235 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/asyncio/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/asyncio_.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/grok/
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/grok/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      357 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/os/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/os/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1796 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/subprocess/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/helpers/threading/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/threading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1672 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/threading/initialize_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2145 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/helpers/threading/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10770 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/flask/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/flask/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/flask/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/flask/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/flask/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.687388 automonisaur-0.2.8/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3587 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (121)       29 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/minio/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/minio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/minio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/neo4j/
--rwxr-xr-x   0 runner    (1001) docker     (121)       64 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/cypher.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/neo4j/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/requests/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/requests/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/requests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/selenium/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/selenium/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/selenium/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/selenium/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/slack/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/bots.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10992 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/slack/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.691388 automonisaur-0.2.8/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3716 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/phantom_unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17233 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/integrations/vds/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (121)       84 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/core/test_sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/integrations/airport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/airport/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/airport/test_airport_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.695388 automonisaur-0.2.8/automon/tests/integrations/minio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/minio/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/minio/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/automon/tests/integrations/neo4j/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/automon/tests/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/nmap/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/nmap/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/automon/tests/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/sentryio/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/sentryio/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/automon/tests/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/splunk_soar/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/splunk_soar/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_datascience.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_geoip.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_selenium.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_shodan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_splunk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-25 19:52:23.000000 automonisaur-0.2.8/automon/tests/integrations/test_vds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 19:52:27.699388 automonisaur-0.2.8/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 19:52:27.000000 automonisaur-0.2.8/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-02-25 19:52:27.000000 automonisaur-0.2.8/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 19:52:27.000000 automonisaur-0.2.8/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-25 19:52:27.000000 automonisaur-0.2.8/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 19:52:27.699388 automonisaur-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-02-25 19:52:23.000000 automonisaur-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 21:39:47.465043 automonisaur-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-02-25 21:39:42.000000 automonisaur-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.449042 automonisaur-0.2.9/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       31 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      112 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1235 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio/loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio_.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/grok/
+-rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/grok/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      357 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/os/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/os/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1796 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/threading/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1672 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/initialize_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2145 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10770 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/flask/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3587 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6070 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/minio/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/neo4j/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       64 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/results.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/requests/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/selenium/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/browser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/slack/
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/bots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10992 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3716 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10147 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/phantom_unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17233 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       84 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/airport/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/test_airport_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/minio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_datascience.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_geoip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_selenium.py
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_shodan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_splunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_swift.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_vds.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 21:39:47.465043 automonisaur-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-02-25 21:39:42.000000 automonisaur-0.2.9/setup.py
```

### Comparing `automonisaur-0.2.8/PKG-INFO` & `automonisaur-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Description: ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
```

### Comparing `automonisaur-0.2.8/README.md` & `automonisaur-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/assertions.py` & `automonisaur-0.2.9/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/asyncio_.py` & `automonisaur-0.2.9/automon/helpers/asyncio_.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/grok/__init__.py` & `automonisaur-0.2.9/automon/helpers/grok/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/markdown.py` & `automonisaur-0.2.9/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/networking.py` & `automonisaur-0.2.9/automon/helpers/networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/regex.py` & `automonisaur-0.2.9/automon/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/sanitation.py` & `automonisaur-0.2.9/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/sleeper.py` & `automonisaur-0.2.9/automon/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/subprocess/run.py` & `automonisaur-0.2.9/automon/helpers/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/threading/initialize_threading.py` & `automonisaur-0.2.9/automon/helpers/threading/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/helpers/threading/worker_thread.py` & `automonisaur-0.2.9/automon/helpers/threading/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.2.9/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.2.9/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.2.9/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/cryptocurrency/robinhood.py` & `automonisaur-0.2.9/automon/integrations/cryptocurrency/robinhood.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.2.9/automon/integrations/datascience/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/elasticsearch/client.py` & `automonisaur-0.2.9/automon/integrations/elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/elasticsearch/config.py` & `automonisaur-0.2.9/automon/integrations/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.2.9/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.2.9/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.2.9/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/flask/auth.py` & `automonisaur-0.2.9/automon/integrations/flask/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/flask/config.py` & `automonisaur-0.2.9/automon/integrations/flask/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.2.9/automon/integrations/google/gmail/v1/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.2.9/automon/integrations/google/gmail/v1/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/ldap/client.py` & `automonisaur-0.2.9/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/mac/airport/airport.py` & `automonisaur-0.2.9/automon/integrations/mac/airport/airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/mac/airport/scan.py` & `automonisaur-0.2.9/automon/integrations/mac/airport/scan.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.2.9/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/minio/client.py` & `automonisaur-0.2.9/automon/integrations/minio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/minio/config.py` & `automonisaur-0.2.9/automon/integrations/minio/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/neo4j/client.py` & `automonisaur-0.2.9/automon/integrations/neo4j/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/neo4j/clientAsync.py` & `automonisaur-0.2.9/automon/integrations/neo4j/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/neo4j/config.py` & `automonisaur-0.2.9/automon/integrations/neo4j/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/neo4j/cypher.py` & `automonisaur-0.2.9/automon/integrations/neo4j/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/neo4j/results.py` & `automonisaur-0.2.9/automon/integrations/neo4j/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/nmap/client.py` & `automonisaur-0.2.9/automon/integrations/nmap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/nmap/config.py` & `automonisaur-0.2.9/automon/integrations/nmap/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/nmap/output.py` & `automonisaur-0.2.9/automon/integrations/nmap/output.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.2.9/automon/integrations/openvpn/openvpn.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/requests/client.py` & `automonisaur-0.2.9/automon/integrations/requests/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/selenium/actions.py` & `automonisaur-0.2.9/automon/integrations/selenium/actions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/selenium/browser.py` & `automonisaur-0.2.9/automon/integrations/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/selenium/config.py` & `automonisaur-0.2.9/automon/integrations/selenium/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/sentryio/client.py` & `automonisaur-0.2.9/automon/integrations/sentryio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/sentryio/config.py` & `automonisaur-0.2.9/automon/integrations/sentryio/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/shodan/__init__.py` & `automonisaur-0.2.9/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/bots.py` & `automonisaur-0.2.9/automon/integrations/slack/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/client.py` & `automonisaur-0.2.9/automon/integrations/slack/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/clientAsync.py` & `automonisaur-0.2.9/automon/integrations/slack/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/config.py` & `automonisaur-0.2.9/automon/integrations/slack/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/error.py` & `automonisaur-0.2.9/automon/integrations/slack/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/slack_formatting.py` & `automonisaur-0.2.9/automon/integrations/slack/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/slack/slack_logger.py` & `automonisaur-0.2.9/automon/integrations/slack/slack_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.2.9/automon/integrations/snmp/generate_maps.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk/client.py` & `automonisaur-0.2.9/automon/integrations/splunk/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk/config.py` & `automonisaur-0.2.9/automon/integrations/splunk/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk/helpers.py` & `automonisaur-0.2.9/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/client.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class SplunkSoarClient:
     def __init__(self, host: str = None,
                  user: str = None,
                  password: str = None,
                  config: SplunkSoarConfig = None):
-        """Phantom Client"""
+        """Splunk SOAR Client"""
 
         self.config = config or SplunkSoarConfig(host=host, user=user, password=password)
         self.client = Requests(headers=self.config.headers)
 
         self.action_run = None
         self.app = None
         self.app_run = None
```

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/common.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/common.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/config.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 
 class SplunkSoarConfig:
     def __init__(self, host: str = None,
                  user: str = None,
                  password: str = None,
                  auth_token: str = None):
-        """Phantom Config"""
+        """Splunk SOAR Config"""
 
-        self.host = host or environ('PHANTOM_HOST')
-        self.user = user or environ('PHANTOM_USER')
-        self.password = password or environ('PHANTOM_PASSWORD')
+        self.host = host or environ('SPLUNK_SOAR_HOST')
+        self.user = user or environ('SPLUNK_SOAR_USER')
+        self.password = password or environ('SPLUNK_SOAR_PASSWORD')
         self.auth = (self.user, self.password)
-        self.auth_token = auth_token or environ('PHANTOM_AUTH_TOKEN')
+        self.auth_token = auth_token or environ('SPLUNK_SOAR_AUTH_TOKEN')
 
         self.headers = {'ph-auth-token': self.auth_token}
 
         if not self.host:
-            log.warn(f'missing PHANTOM_HOST')
+            log.warn(f'missing SPLUNK_SOAR_HOST')
 
     def __repr__(self):
         return f'{self.__dict__}'
 
     def isReady(self):
         if self.host:
             return True
```

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/container.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/container.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/rest/urls.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/rest/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.2.9/automon/integrations/splunk_soar/rules.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/swift/client.py` & `automonisaur-0.2.9/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/swift/config.py` & `automonisaur-0.2.9/automon/integrations/swift/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/swift/error.py` & `automonisaur-0.2.9/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/swift/iterables.py` & `automonisaur-0.2.9/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/vds/client.py` & `automonisaur-0.2.9/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/integrations/vds/config.py` & `automonisaur-0.2.9/automon/integrations/vds/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/log/logger.py` & `automonisaur-0.2.9/automon/log/logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_assertions.py` & `automonisaur-0.2.9/automon/tests/core/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_logger.py` & `automonisaur-0.2.9/automon/tests/core/test_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_networking.py` & `automonisaur-0.2.9/automon/tests/core/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_runner.py` & `automonisaur-0.2.9/automon/tests/core/test_runner.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_sanitation.py` & `automonisaur-0.2.9/automon/tests/core/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/core/test_sleeper.py` & `automonisaur-0.2.9/automon/tests/core/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/airport/test_airport.py` & `automonisaur-0.2.9/automon/tests/integrations/airport/test_airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/airport/test_airport_neo4j.py` & `automonisaur-0.2.9/automon/tests/integrations/airport/test_airport_neo4j.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch.py` & `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py` & `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/minio/test_minio_client.py` & `automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_client.py` & `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_config.py` & `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/neo4j/test_neo4j_cypher.py` & `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/nmap/test_nmap_client.py` & `automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/sentryio/test_sentryio.py` & `automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/sentryio/test_sentryio_callback.py` & `automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio_callback.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/splunk_soar/test_soar_client.py` & `automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_crypto.py` & `automonisaur-0.2.9/automon/tests/integrations/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_datascience.py` & `automonisaur-0.2.9/automon/tests/integrations/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_flask.py` & `automonisaur-0.2.9/automon/tests/integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_requests.py` & `automonisaur-0.2.9/automon/tests/integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_selenium.py` & `automonisaur-0.2.9/automon/tests/integrations/test_selenium.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_slack.py` & `automonisaur-0.2.9/automon/tests/integrations/test_slack.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_splunk.py` & `automonisaur-0.2.9/automon/tests/integrations/test_splunk.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automon/tests/integrations/test_swift.py` & `automonisaur-0.2.9/automon/tests/integrations/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/automonisaur.egg-info/PKG-INFO` & `automonisaur-0.2.9/automonisaur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Description: ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
```

### Comparing `automonisaur-0.2.8/automonisaur.egg-info/SOURCES.txt` & `automonisaur-0.2.9/automonisaur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.8/setup.py` & `automonisaur-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.2.8",
+    version="0.2.9",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
```

