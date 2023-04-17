# Comparing `tmp/yubikey_manager-5.0.1.tar.gz` & `tmp/yubikey_manager-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yubikey_manager-5.0.1.tar", max compression
+gzip compressed data, was "yubikey_manager-5.1.0.tar", max compression
```

## Comparing `yubikey_manager-5.0.1.tar` & `yubikey_manager-5.1.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1322 2021-04-12 07:23:08.055259 yubikey_manager-5.0.1/COPYING
--rw-r--r--   0        0        0    15218 2023-01-17 10:30:26.662008 yubikey_manager-5.0.1/NEWS
--rw-r--r--   0        0        0     7475 2023-01-17 10:29:18.625743 yubikey_manager-5.0.1/README.adoc
--rw-r--r--   0        0        0     1510 2023-01-17 10:30:26.663007 yubikey_manager-5.0.1/man/ykman.1
--rw-r--r--   0        0        0     1246 2023-01-17 10:30:26.665258 yubikey_manager-5.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-12 07:23:08.071963 yubikey_manager-5.0.1/tests/__init__.py
--rw-r--r--   0        0        0      195 2021-04-12 07:23:08.072538 yubikey_manager-5.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-04-12 07:23:08.073691 yubikey_manager-5.0.1/tests/device/__init__.py
--rw-r--r--   0        0        0        0 2021-04-12 07:23:08.074843 yubikey_manager-5.0.1/tests/device/cli/__init__.py
--rw-r--r--   0        0        0     1092 2023-01-17 10:29:18.636875 yubikey_manager-5.0.1/tests/device/cli/conftest.py
--rw-r--r--   0        0        0        0 2021-04-12 07:23:08.077727 yubikey_manager-5.0.1/tests/device/cli/piv/__init__.py
--rw-r--r--   0        0        0      215 2021-04-12 07:23:08.078879 yubikey_manager-5.0.1/tests/device/cli/piv/conftest.py
--rw-r--r--   0        0        0      733 2023-01-17 10:29:18.637873 yubikey_manager-5.0.1/tests/device/cli/piv/test_fips.py
--rw-r--r--   0        0        0    10295 2023-01-17 10:29:18.638870 yubikey_manager-5.0.1/tests/device/cli/piv/test_generate_cert_and_csr.py
--rw-r--r--   0        0        0    15795 2023-01-17 10:29:18.639867 yubikey_manager-5.0.1/tests/device/cli/piv/test_key_management.py
--rw-r--r--   0        0        0     5502 2021-04-12 07:23:08.083487 yubikey_manager-5.0.1/tests/device/cli/piv/test_management_key.py
--rw-r--r--   0        0        0     1303 2021-04-12 07:23:08.084654 yubikey_manager-5.0.1/tests/device/cli/piv/test_misc.py
--rw-r--r--   0        0        0     1691 2023-01-17 10:29:18.640864 yubikey_manager-5.0.1/tests/device/cli/piv/test_pin_puk.py
--rw-r--r--   0        0        0     3057 2023-01-17 10:29:18.641945 yubikey_manager-5.0.1/tests/device/cli/piv/test_read_write_object.py
--rw-r--r--   0        0        0      325 2021-04-12 07:23:08.088672 yubikey_manager-5.0.1/tests/device/cli/piv/util.py
--rw-r--r--   0        0        0      311 2023-01-17 10:29:18.641945 yubikey_manager-5.0.1/tests/device/cli/test_aliases.py
--rw-r--r--   0        0        0     8495 2023-01-17 10:29:18.642944 yubikey_manager-5.0.1/tests/device/cli/test_config.py
--rw-r--r--   0        0        0      816 2023-01-17 10:29:18.643941 yubikey_manager-5.0.1/tests/device/cli/test_misc.py
--rw-r--r--   0        0        0    11351 2023-01-17 10:29:18.643941 yubikey_manager-5.0.1/tests/device/cli/test_oath.py
--rw-r--r--   0        0        0     5304 2023-01-17 10:29:18.644937 yubikey_manager-5.0.1/tests/device/cli/test_openpgp.py
--rw-r--r--   0        0        0    23421 2023-01-17 10:29:18.645936 yubikey_manager-5.0.1/tests/device/cli/test_otp.py
--rw-r--r--   0        0        0     2379 2023-01-17 10:29:18.646934 yubikey_manager-5.0.1/tests/device/condition.py
--rw-r--r--   0        0        0     2708 2023-01-17 10:29:18.647931 yubikey_manager-5.0.1/tests/device/conftest.py
--rw-r--r--   0        0        0      276 2021-04-12 07:23:08.096732 yubikey_manager-5.0.1/tests/device/test_ccid.py
--rw-r--r--   0        0        0     2022 2023-01-17 10:29:18.647931 yubikey_manager-5.0.1/tests/device/test_fips_u2f_commands.py
--rw-r--r--   0        0        0      694 2023-01-17 10:29:18.648928 yubikey_manager-5.0.1/tests/device/test_interfaces.py
--rw-r--r--   0        0        0     8019 2023-01-17 10:29:18.648928 yubikey_manager-5.0.1/tests/device/test_oath.py
--rw-r--r--   0        0        0     3619 2023-01-17 10:29:18.649925 yubikey_manager-5.0.1/tests/device/test_openpgp.py
--rw-r--r--   0        0        0     5163 2023-01-17 10:29:18.650923 yubikey_manager-5.0.1/tests/device/test_otp.py
--rw-r--r--   0        0        0    21962 2023-01-17 10:29:18.650923 yubikey_manager-5.0.1/tests/device/test_piv.py
--rw-r--r--   0        0        0      887 2021-04-12 07:23:08.104219 yubikey_manager-5.0.1/tests/files/rsa_1024_key.pem
--rw-r--r--   0        0        0      735 2021-04-12 07:23:08.104795 yubikey_manager-5.0.1/tests/files/rsa_2048_cert.der
--rw-r--r--   0        0        0     1050 2021-04-12 07:23:08.105947 yubikey_manager-5.0.1/tests/files/rsa_2048_cert.pem
--rw-r--r--   0        0        0     1088 2021-04-12 07:23:08.107100 yubikey_manager-5.0.1/tests/files/rsa_2048_cert_metadata.pem
--rw-r--r--   0        0        0     1679 2021-04-12 07:23:08.108252 yubikey_manager-5.0.1/tests/files/rsa_2048_key.pem
--rw-r--r--   0        0        0     2469 2021-04-12 07:23:08.109407 yubikey_manager-5.0.1/tests/files/rsa_2048_key_cert.pfx
--rw-r--r--   0        0        0     2469 2021-04-12 07:23:08.109979 yubikey_manager-5.0.1/tests/files/rsa_2048_key_cert_encrypted.pfx
--rw-r--r--   0        0        0     1751 2021-04-12 07:23:08.111131 yubikey_manager-5.0.1/tests/files/rsa_2048_key_encrypted.pem
--rw-r--r--   0        0        0     5490 2023-01-17 10:30:26.665258 yubikey_manager-5.0.1/tests/test_device.py
--rw-r--r--   0        0        0      153 2021-04-12 07:23:08.112859 yubikey_manager-5.0.1/tests/test_management.py
--rw-r--r--   0        0        0     3971 2023-01-17 10:29:18.652009 yubikey_manager-5.0.1/tests/test_oath.py
--rw-r--r--   0        0        0     2420 2023-01-17 10:29:18.653008 yubikey_manager-5.0.1/tests/test_piv.py
--rw-r--r--   0        0        0    21312 2021-04-12 07:23:08.115739 yubikey_manager-5.0.1/tests/test_scancodes.py
--rw-r--r--   0        0        0     6105 2023-01-17 10:29:18.654005 yubikey_manager-5.0.1/tests/test_util.py
--rw-r--r--   0        0        0     1302 2021-04-12 07:23:08.118618 yubikey_manager-5.0.1/tests/util.py
--rw-r--r--   0        0        0     1394 2023-01-17 10:30:26.666255 yubikey_manager-5.0.1/ykman/__init__.py
--rw-r--r--   0        0        0     1371 2023-01-17 10:29:18.656000 yubikey_manager-5.0.1/ykman/_cli/__init__.py
--rw-r--r--   0        0        0    12603 2023-01-17 10:29:18.656997 yubikey_manager-5.0.1/ykman/_cli/__main__.py
--rw-r--r--   0        0        0     5554 2023-01-17 10:29:18.656997 yubikey_manager-5.0.1/ykman/_cli/aliases.py
--rw-r--r--   0        0        0     6279 2023-01-17 10:29:18.658040 yubikey_manager-5.0.1/ykman/_cli/apdu.py
--rw-r--r--   0        0        0    17796 2023-01-17 10:29:18.658550 yubikey_manager-5.0.1/ykman/_cli/config.py
--rwxr-xr-x   0        0        0    26006 2023-01-17 10:29:18.659459 yubikey_manager-5.0.1/ykman/_cli/fido.py
--rw-r--r--   0        0        0     6970 2023-01-17 10:29:18.659459 yubikey_manager-5.0.1/ykman/_cli/info.py
--rw-r--r--   0        0        0    22389 2023-01-17 10:29:18.660459 yubikey_manager-5.0.1/ykman/_cli/oath.py
--rw-r--r--   0        0        0    18280 2023-01-17 10:29:18.661542 yubikey_manager-5.0.1/ykman/_cli/openpgp.py
--rw-r--r--   0        0        0    27317 2023-01-17 10:29:18.661542 yubikey_manager-5.0.1/ykman/_cli/otp.py
--rw-r--r--   0        0        0    35614 2023-01-17 10:29:18.662541 yubikey_manager-5.0.1/ykman/_cli/piv.py
--rw-r--r--   0        0        0     3341 2023-01-17 10:29:18.663538 yubikey_manager-5.0.1/ykman/_cli/script.py
--rw-r--r--   0        0        0     8842 2023-01-17 10:29:18.663538 yubikey_manager-5.0.1/ykman/_cli/util.py
--rw-r--r--   0        0        0    23287 2023-01-17 10:30:26.667258 yubikey_manager-5.0.1/ykman/_openpgp.py
--rw-r--r--   0        0        0     2050 2023-01-17 10:29:18.664535 yubikey_manager-5.0.1/ykman/base.py
--rw-r--r--   0        0        0    10548 2023-01-17 10:29:18.665532 yubikey_manager-5.0.1/ykman/device.py
--rw-r--r--   0        0        0     7069 2023-01-17 10:29:18.666530 yubikey_manager-5.0.1/ykman/diagnostics.py
--rw-r--r--   0        0        0     3558 2021-04-12 07:23:08.140507 yubikey_manager-5.0.1/ykman/fido.py
--rw-r--r--   0        0        0     3772 2023-01-17 10:29:18.666530 yubikey_manager-5.0.1/ykman/hid/__init__.py
--rw-r--r--   0        0        0     2136 2023-01-17 10:29:18.667527 yubikey_manager-5.0.1/ykman/hid/base.py
--rw-r--r--   0        0        0    10151 2023-01-17 10:29:18.668525 yubikey_manager-5.0.1/ykman/hid/freebsd.py
--rw-r--r--   0        0        0     4307 2023-01-17 10:29:18.668525 yubikey_manager-5.0.1/ykman/hid/linux.py
--rw-r--r--   0        0        0     9838 2023-01-17 10:29:18.669522 yubikey_manager-5.0.1/ykman/hid/macos.py
--rw-r--r--   0        0        0    11199 2023-01-17 10:29:18.670519 yubikey_manager-5.0.1/ykman/hid/windows.py
--rw-r--r--   0        0        0     2763 2023-01-17 10:29:18.670519 yubikey_manager-5.0.1/ykman/logging.py
--rw-r--r--   0        0        0     2322 2023-01-17 10:29:18.671517 yubikey_manager-5.0.1/ykman/logging_setup.py
--rw-r--r--   0        0        0     2173 2021-04-12 07:23:08.148000 yubikey_manager-5.0.1/ykman/oath.py
--rw-r--r--   0        0        0     7246 2023-01-17 10:29:18.672599 yubikey_manager-5.0.1/ykman/otp.py
--rw-r--r--   0        0        0     6186 2023-01-17 10:29:18.672599 yubikey_manager-5.0.1/ykman/pcsc/__init__.py
--rw-r--r--   0        0        0    22554 2023-01-17 10:29:18.674172 yubikey_manager-5.0.1/ykman/piv.py
--rw-r--r--   0        0        0        0 2023-01-17 10:29:18.674172 yubikey_manager-5.0.1/ykman/py.typed
--rw-r--r--   0        0        0     1907 2021-04-12 07:23:08.153756 yubikey_manager-5.0.1/ykman/scancodes/__init__.py
--rw-r--r--   0        0        0     3405 2021-04-12 07:23:08.154908 yubikey_manager-5.0.1/ykman/scancodes/bepo.py
--rw-r--r--   0        0        0     3343 2021-04-12 07:23:08.155484 yubikey_manager-5.0.1/ykman/scancodes/de.py
--rw-r--r--   0        0        0     3287 2021-04-12 07:23:08.156639 yubikey_manager-5.0.1/ykman/scancodes/fr.py
--rw-r--r--   0        0        0     3351 2021-04-12 07:23:08.157787 yubikey_manager-5.0.1/ykman/scancodes/it.py
--rw-r--r--   0        0        0     2172 2021-04-12 07:23:08.158362 yubikey_manager-5.0.1/ykman/scancodes/modhex.py
--rw-r--r--   0        0        0     3312 2021-04-12 07:23:08.159515 yubikey_manager-5.0.1/ykman/scancodes/norman.py
--rw-r--r--   0        0        0     3306 2021-04-12 07:23:08.160673 yubikey_manager-5.0.1/ykman/scancodes/uk.py
--rw-r--r--   0        0        0     3305 2021-04-12 07:23:08.161243 yubikey_manager-5.0.1/ykman/scancodes/us.py
--rw-r--r--   0        0        0     7636 2023-01-17 10:29:18.674172 yubikey_manager-5.0.1/ykman/scripting.py
--rw-r--r--   0        0        0     4031 2023-01-17 10:29:18.675169 yubikey_manager-5.0.1/ykman/settings.py
--rw-r--r--   0        0        0     6063 2023-01-17 10:29:18.676166 yubikey_manager-5.0.1/ykman/util.py
--rw-r--r--   0        0        0     1371 2021-04-12 07:23:08.164123 yubikey_manager-5.0.1/yubikit/__init__.py
--rw-r--r--   0        0        0    10457 2023-01-17 10:29:18.677162 yubikey_manager-5.0.1/yubikit/core/__init__.py
--rw-r--r--   0        0        0     1593 2023-01-17 10:29:18.677162 yubikey_manager-5.0.1/yubikit/core/fido.py
--rw-r--r--   0        0        0     9552 2023-01-17 10:29:18.678161 yubikey_manager-5.0.1/yubikit/core/otp.py
--rw-r--r--   0        0        0     6922 2023-01-17 10:29:18.679159 yubikey_manager-5.0.1/yubikit/core/smartcard.py
--rw-r--r--   0        0        0     1642 2023-01-17 10:29:18.679159 yubikey_manager-5.0.1/yubikit/logging.py
--rw-r--r--   0        0        0    17699 2023-01-17 10:29:18.680156 yubikey_manager-5.0.1/yubikit/management.py
--rw-r--r--   0        0        0    14147 2023-01-17 10:29:18.680156 yubikey_manager-5.0.1/yubikit/oath.py
--rwxr-xr-x   0        0        0    28832 2023-01-17 10:30:26.668252 yubikey_manager-5.0.1/yubikit/piv.py
--rw-r--r--   0        0        0        0 2023-01-17 10:29:18.681153 yubikey_manager-5.0.1/yubikit/py.typed
--rw-r--r--   0        0        0    15477 2023-01-17 10:30:26.669247 yubikey_manager-5.0.1/yubikit/support.py
--rw-r--r--   0        0        0    29215 2023-01-17 10:29:18.683227 yubikey_manager-5.0.1/yubikit/yubiotp.py
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 yubikey_manager-5.0.1/setup.py
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 yubikey_manager-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/COPYING
+-rw-r--r--   0        0        0    15548 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/NEWS
+-rw-r--r--   0        0        0     7452 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/README.adoc
+-rw-r--r--   0        0        0     1508 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/man/ykman.1
+-rw-r--r--   0        0        0     1246 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/cli/__init__.py
+-rw-r--r--   0        0        0     1092 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/cli/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/cli/piv/__init__.py
+-rw-r--r--   0        0        0      215 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/cli/piv/conftest.py
+-rw-r--r--   0        0        0      733 2023-04-17 07:17:04.765138 yubikey_manager-5.1.0/tests/device/cli/piv/test_fips.py
+-rw-r--r--   0        0        0    10295 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_generate_cert_and_csr.py
+-rw-r--r--   0        0        0    15795 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_key_management.py
+-rw-r--r--   0        0        0     5502 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_management_key.py
+-rw-r--r--   0        0        0     1303 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_misc.py
+-rw-r--r--   0        0        0     1691 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_pin_puk.py
+-rw-r--r--   0        0        0     3057 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/test_read_write_object.py
+-rw-r--r--   0        0        0      325 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/piv/util.py
+-rw-r--r--   0        0        0      311 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_aliases.py
+-rw-r--r--   0        0        0     8495 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_config.py
+-rw-r--r--   0        0        0      816 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_misc.py
+-rw-r--r--   0        0        0    11351 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_oath.py
+-rw-r--r--   0        0        0     5304 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_openpgp.py
+-rw-r--r--   0        0        0    23421 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/cli/test_otp.py
+-rw-r--r--   0        0        0     2379 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/condition.py
+-rw-r--r--   0        0        0     2708 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/conftest.py
+-rw-r--r--   0        0        0      276 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_ccid.py
+-rw-r--r--   0        0        0     2022 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_fips_u2f_commands.py
+-rw-r--r--   0        0        0      694 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_interfaces.py
+-rw-r--r--   0        0        0     8019 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_oath.py
+-rw-r--r--   0        0        0     6723 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_openpgp.py
+-rw-r--r--   0        0        0     5163 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_otp.py
+-rw-r--r--   0        0        0    21962 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/device/test_piv.py
+-rw-r--r--   0        0        0      887 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_1024_key.pem
+-rw-r--r--   0        0        0      735 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_cert.der
+-rw-r--r--   0        0        0     1050 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_cert.pem
+-rw-r--r--   0        0        0     1088 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_cert_metadata.pem
+-rw-r--r--   0        0        0     1679 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_key.pem
+-rw-r--r--   0        0        0     2469 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_key_cert.pfx
+-rw-r--r--   0        0        0     2469 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_key_cert_encrypted.pfx
+-rw-r--r--   0        0        0     1751 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/files/rsa_2048_key_encrypted.pem
+-rw-r--r--   0        0        0     5490 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_device.py
+-rw-r--r--   0        0        0      153 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_management.py
+-rw-r--r--   0        0        0     3971 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_oath.py
+-rw-r--r--   0        0        0     2420 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_piv.py
+-rw-r--r--   0        0        0    21312 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_scancodes.py
+-rw-r--r--   0        0        0     6105 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/test_util.py
+-rw-r--r--   0        0        0     1302 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/tests/util.py
+-rw-r--r--   0        0        0     1394 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/__init__.py
+-rw-r--r--   0        0        0    12603 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/__main__.py
+-rw-r--r--   0        0        0     5554 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/aliases.py
+-rw-r--r--   0        0        0     6279 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/apdu.py
+-rw-r--r--   0        0        0    17796 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/config.py
+-rwxr-xr-x   0        0        0    26006 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/fido.py
+-rw-r--r--   0        0        0     6970 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/info.py
+-rw-r--r--   0        0        0    22389 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/oath.py
+-rw-r--r--   0        0        0    17018 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/openpgp.py
+-rw-r--r--   0        0        0    27317 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/otp.py
+-rw-r--r--   0        0        0    38384 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/piv.py
+-rw-r--r--   0        0        0     3341 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/script.py
+-rw-r--r--   0        0        0     9236 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/_cli/util.py
+-rw-r--r--   0        0        0     2050 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/base.py
+-rw-r--r--   0        0        0    10548 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/device.py
+-rw-r--r--   0        0        0     7089 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/diagnostics.py
+-rw-r--r--   0        0        0     3558 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/fido.py
+-rw-r--r--   0        0        0     3772 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/base.py
+-rw-r--r--   0        0        0    10151 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/freebsd.py
+-rw-r--r--   0        0        0     4307 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/linux.py
+-rw-r--r--   0        0        0     9838 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/macos.py
+-rw-r--r--   0        0        0    11199 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/hid/windows.py
+-rw-r--r--   0        0        0     2763 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/logging.py
+-rw-r--r--   0        0        0     2322 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/logging_setup.py
+-rw-r--r--   0        0        0     2173 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/oath.py
+-rw-r--r--   0        0        0     2518 2023-04-17 07:17:04.769138 yubikey_manager-5.1.0/ykman/openpgp.py
+-rw-r--r--   0        0        0     7239 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/otp.py
+-rw-r--r--   0        0        0     6186 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/pcsc/__init__.py
+-rw-r--r--   0        0        0    22734 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/piv.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/py.typed
+-rw-r--r--   0        0        0     1907 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/__init__.py
+-rw-r--r--   0        0        0     3405 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/bepo.py
+-rw-r--r--   0        0        0     3343 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/de.py
+-rw-r--r--   0        0        0     3287 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/fr.py
+-rw-r--r--   0        0        0     3351 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/it.py
+-rw-r--r--   0        0        0     2172 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/modhex.py
+-rw-r--r--   0        0        0     3312 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/norman.py
+-rw-r--r--   0        0        0     3306 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/uk.py
+-rw-r--r--   0        0        0     3305 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scancodes/us.py
+-rw-r--r--   0        0        0     7636 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/scripting.py
+-rw-r--r--   0        0        0     4031 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/settings.py
+-rw-r--r--   0        0        0     6063 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/ykman/util.py
+-rw-r--r--   0        0        0     1371 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/__init__.py
+-rw-r--r--   0        0        0    10457 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/core/__init__.py
+-rw-r--r--   0        0        0     1593 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/core/fido.py
+-rw-r--r--   0        0        0     9552 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/core/otp.py
+-rw-r--r--   0        0        0     7083 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/core/smartcard.py
+-rw-r--r--   0        0        0     1642 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/logging.py
+-rw-r--r--   0        0        0    17699 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/management.py
+-rw-r--r--   0        0        0    14147 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/oath.py
+-rw-r--r--   0        0        0    53812 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/openpgp.py
+-rwxr-xr-x   0        0        0    29081 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/piv.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/py.typed
+-rw-r--r--   0        0        0    15689 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/support.py
+-rw-r--r--   0        0        0    29215 2023-04-17 07:17:04.773138 yubikey_manager-5.1.0/yubikit/yubiotp.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yubikey_manager-5.1.0/PKG-INFO
```

### Comparing `yubikey_manager-5.0.1/COPYING` & `yubikey_manager-5.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/NEWS` & `yubikey_manager-5.1.0/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+* Version 5.1.0 (released 2023-04-17)
+ ** Add OpenPGP functionality to supported API.
+ ** Add PIV key info command to CLI.
+ ** PIV: Support signing prehashed data via API.
+ ** Bugfix: Fix signing PIV certificates/CSRs with key that always requires PIN.
+ ** Bugfix: Fix incorrect display name detection for certain keys over NFC.
+
 * Version 5.0.1 (released 2023-01-17)
  ** Bugfix: Fix the interactive confirmation prompt for some CLI commands.
  ** Bugfix: OpenPGP Signature PIN policy values were swapped.
  ** Bugfix: FIDO: Handle discoverable credentials that are missing name or displayName.
  ** Add support for Python 3.11.
  ** Remove extra whitespace characters from CLI into command output.
```

### Comparing `yubikey_manager-5.0.1/README.adoc` & `yubikey_manager-5.1.0/README.adoc`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 On Linux platforms you will need `pcscd` installed and running to be able to
 communicate with a YubiKey over the SmartCard interface. Additionally, you may
 need to set permissions for your user to access YubiKeys via the HID interfaces.
 More information available link:doc/Device_Permissions.adoc[here].
 
 Some of the libraries used by yubikey-manager have C-extensions, and may require
 additional dependencies to build, such as http://www.swig.org/[swig] and
-potentially https://pcsclite.alioth.debian.org/pcsclite.html[PCSC lite].
+potentially https://pcsclite.apdu.fr/[PCSC lite].
 
 === Pre-build packages
 Pre-built packages specific to your platform may be available from Yubico or
 third parties. Please refer to your platforms native package manager for
 detailed instructions on how to install, if available.
 
 ==== Windows
```

### Comparing `yubikey_manager-5.0.1/man/ykman.1` & `yubikey_manager-5.1.0/man/ykman.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH YKMAN "1" "January 2023" "ykman 5.0.1" "User Commands"
+.TH YKMAN "1" "April 2023" "ykman 5.1.0" "User Commands"
 .SH NAME
 ykman \- YubiKey Manager (ykman)
 .SH SYNOPSIS
 .B ykman
 [\fI\,OPTIONS\/\fR] \fI\,COMMAND \/\fR[\fI\,ARGS\/\fR]...
 .SH DESCRIPTION
 .PP
```

### Comparing `yubikey_manager-5.0.1/pyproject.toml` & `yubikey_manager-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yubikey-manager"
-version = "5.0.1"
+version = "5.1.0"
 description = "Tool for managing your YubiKey configuration."
 authors = ["Dain Nilsson <dain@yubico.com>"]
 license = "BSD"
 homepage = "https://github.com/Yubico/yubikey-manager"
 repository = "https://github.com/Yubico/yubikey-manager"
 keywords = ["yubikey", "yubiotp", "piv", "fido"]
 classifiers = [
@@ -24,15 +24,15 @@
   { include = "yubikit" },
   { include = "ykman" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-cryptography = ">=3.0, <42"
+cryptography = ">=3.0, <43"
 pyscard = "^2.0"
 fido2 = "^1.0"
 click = "^8.0"
 pywin32 = {version = ">=223", platform = "win32"}
 keyring = "^23.4"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `yubikey_manager-5.0.1/tests/device/cli/conftest.py` & `yubikey_manager-5.1.0/tests/device/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_fips.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_fips.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_generate_cert_and_csr.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_generate_cert_and_csr.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_key_management.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_key_management.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_management_key.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_management_key.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_misc.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_misc.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_pin_puk.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_pin_puk.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/piv/test_read_write_object.py` & `yubikey_manager-5.1.0/tests/device/cli/piv/test_read_write_object.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/test_config.py` & `yubikey_manager-5.1.0/tests/device/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/test_misc.py` & `yubikey_manager-5.1.0/tests/device/cli/test_misc.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/test_oath.py` & `yubikey_manager-5.1.0/tests/device/cli/test_oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/test_openpgp.py` & `yubikey_manager-5.1.0/tests/device/cli/test_openpgp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/cli/test_otp.py` & `yubikey_manager-5.1.0/tests/device/cli/test_otp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/condition.py` & `yubikey_manager-5.1.0/tests/device/condition.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/conftest.py` & `yubikey_manager-5.1.0/tests/device/conftest.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/test_fips_u2f_commands.py` & `yubikey_manager-5.1.0/tests/device/test_fips_u2f_commands.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/test_interfaces.py` & `yubikey_manager-5.1.0/tests/device/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/test_oath.py` & `yubikey_manager-5.1.0/tests/device/test_oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/test_otp.py` & `yubikey_manager-5.1.0/tests/device/test_otp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/device/test_piv.py` & `yubikey_manager-5.1.0/tests/device/test_piv.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_1024_key.pem` & `yubikey_manager-5.1.0/tests/files/rsa_1024_key.pem`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_cert.der` & `yubikey_manager-5.1.0/tests/files/rsa_2048_cert.der`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_cert.pem` & `yubikey_manager-5.1.0/tests/files/rsa_2048_cert.pem`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_cert_metadata.pem` & `yubikey_manager-5.1.0/tests/files/rsa_2048_cert_metadata.pem`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_key.pem` & `yubikey_manager-5.1.0/tests/files/rsa_2048_key.pem`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_key_cert.pfx` & `yubikey_manager-5.1.0/tests/files/rsa_2048_key_cert.pfx`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_key_cert_encrypted.pfx` & `yubikey_manager-5.1.0/tests/files/rsa_2048_key_cert_encrypted.pfx`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/files/rsa_2048_key_encrypted.pem` & `yubikey_manager-5.1.0/tests/files/rsa_2048_key_encrypted.pem`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/test_device.py` & `yubikey_manager-5.1.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/test_oath.py` & `yubikey_manager-5.1.0/tests/test_oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/test_piv.py` & `yubikey_manager-5.1.0/tests/test_piv.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/test_scancodes.py` & `yubikey_manager-5.1.0/tests/test_scancodes.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/test_util.py` & `yubikey_manager-5.1.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/tests/util.py` & `yubikey_manager-5.1.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/__init__.py` & `yubikey_manager-5.1.0/yubikit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2015 Yubico AB
+# Copyright (c) 2020 Yubico AB
 # All rights reserved.
 #
 #   Redistribution and use in source and binary forms, with or
 #   without modification, are permitted provided that the following
 #   conditions are met:
 #
 #    1. Redistributions of source code must retain the above copyright
@@ -20,9 +20,7 @@
 # INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
-
-__version__ = "5.0.1"
```

### Comparing `yubikey_manager-5.0.1/ykman/_cli/__init__.py` & `yubikey_manager-5.1.0/ykman/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/__main__.py` & `yubikey_manager-5.1.0/ykman/_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/aliases.py` & `yubikey_manager-5.1.0/ykman/_cli/aliases.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/apdu.py` & `yubikey_manager-5.1.0/ykman/_cli/apdu.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/config.py` & `yubikey_manager-5.1.0/ykman/_cli/config.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/fido.py` & `yubikey_manager-5.1.0/ykman/_cli/fido.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/info.py` & `yubikey_manager-5.1.0/ykman/_cli/info.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/oath.py` & `yubikey_manager-5.1.0/ykman/_cli/oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/openpgp.py` & `yubikey_manager-5.1.0/ykman/_cli/openpgp.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,67 +21,44 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-import logging
-import click
+from yubikit.core.smartcard import ApduError, SW, SmartCardConnection
+from yubikit.openpgp import OpenPgpSession, UIF, PIN_POLICY, KEY_REF as _KEY_REF
 from ..util import parse_certificates, parse_private_key
-from .._openpgp import (
-    OpenPgpController,
-    KEY_SLOT,
-    TOUCH_MODE,
-    PIN_POLICY,
-    get_openpgp_info,
-)
+from ..openpgp import get_openpgp_info
 from .util import (
     CliFail,
     click_force_option,
     click_format_option,
     click_postpone_execution,
     click_prompt,
     click_group,
     EnumChoice,
     pretty_print,
 )
-
-from yubikit.core.smartcard import ApduError, SW, SmartCardConnection
+from enum import IntEnum
+import logging
+import click
 
 logger = logging.getLogger(__name__)
 
 
-def one_of(data):
-    def inner(ctx, param, key):
-        if key is not None:
-            return data[key]
-
-    return inner
-
-
-def get_or_fail(data):
-    def inner(key):
-        if key in data:
-            return data[key]
-        raise ValueError(
-            f"Invalid value: {key}. Must be one of: {', '.join(data.keys())}"
-        )
+class KEY_REF(IntEnum):
+    SIG = 0x01
+    DEC = 0x02
+    AUT = 0x03
+    ATT = 0x81
+    ENC = 0x02  # Alias for backwards compatibility, will be removed in ykman 6
 
-    return inner
-
-
-def int_in_range(minval, maxval):
-    def inner(val):
-        intval = int(val)
-        if minval <= intval <= maxval:
-            return intval
-        raise ValueError(f"Invalid value: {intval}. Must be in range {minval}-{maxval}")
-
-    return inner
+    def __getattribute__(self, name: str):
+        return _KEY_REF(self).__getattribute__(name)
 
 
 def _fname(fobj):
     return getattr(fobj, "name", fobj)
 
 
 @click_group(connections=[SmartCardConnection])
@@ -100,25 +77,25 @@
     \b
       Require touch to use the authentication key:
       $ ykman openpgp keys set-touch aut on
     """
     dev = ctx.obj["device"]
     conn = dev.open_connection(SmartCardConnection)
     ctx.call_on_close(conn.close)
-    ctx.obj["controller"] = OpenPgpController(conn)
+    ctx.obj["session"] = OpenPgpSession(conn)
 
 
 @openpgp.command()
 @click.pass_context
 def info(ctx):
     """
     Display general status of the OpenPGP application.
     """
-    controller = ctx.obj["controller"]
-    click.echo("\n".join(pretty_print(get_openpgp_info(controller))))
+    session = ctx.obj["session"]
+    click.echo("\n".join(pretty_print(get_openpgp_info(session))))
 
 
 @openpgp.command()
 @click_force_option
 @click.pass_context
 def reset(ctx, force):
     """
@@ -131,15 +108,15 @@
         "WARNING! This will delete all stored OpenPGP keys and data and restore "
         "factory settings. Proceed?",
         abort=True,
         err=True,
     )
 
     click.echo("Resetting OpenPGP data, don't remove the YubiKey...")
-    ctx.obj["controller"].reset()
+    ctx.obj["session"].reset()
     logger.info("OpenPGP application data reset")
     click.echo("Success! All data has been cleared and default PINs are set.")
     echo_default_pins()
 
 
 def echo_default_pins():
     click.echo("PIN:         123456")
@@ -165,31 +142,30 @@
 @click.pass_context
 def set_pin_retries(
     ctx, admin_pin, user_pin_retries, reset_code_retries, admin_pin_retries, force
 ):
     """
     Set the number of retry attempts for the User PIN, Reset Code, and Admin PIN.
     """
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
-    resets_pins = controller.version < (4, 0, 0)
+    resets_pins = session.version < (4, 0, 0)
     if resets_pins:
         click.echo("WARNING: Setting PIN retries will reset the values for all 3 PINs!")
     if force or click.confirm(
         f"Set PIN retry counters to: {user_pin_retries} {reset_code_retries} "
         f"{admin_pin_retries}?",
         abort=True,
         err=True,
     ):
-
-        controller.verify_admin(admin_pin)
-        controller.set_pin_retries(
+        session.verify_admin(admin_pin)
+        session.set_pin_attempts(
             user_pin_retries, reset_code_retries, admin_pin_retries
         )
         logger.info("Number of PIN/Reset Code/Admin PIN retries set")
 
         if resets_pins:
             click.echo("Default PINs are set.")
             echo_default_pins()
@@ -203,82 +179,82 @@
     """
     Change the User PIN.
 
     The PIN has a minimum length of 6, and supports any type of
     alphanumeric characters.
     """
 
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if pin is None:
         pin = click_prompt("Enter PIN", hide_input=True)
 
     if new_pin is None:
         new_pin = click_prompt(
             "New PIN",
             hide_input=True,
             confirmation_prompt=True,
         )
 
-    controller.change_pin(pin, new_pin)
+    session.change_pin(pin, new_pin)
 
 
 @access.command("change-reset-code")
 @click.option("-a", "--admin-pin", help="Admin PIN")
 @click.option("-r", "--reset-code", help="a new Reset Code")
 @click.pass_context
 def change_reset_code(ctx, admin_pin, reset_code):
     """
     Change the Reset Code.
 
     The Reset Code has a minimum length of 6, and supports any type of
     alphanumeric characters.
     """
 
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
     if reset_code is None:
         reset_code = click_prompt(
             "New Reset Code",
             hide_input=True,
             confirmation_prompt=True,
         )
 
-    controller.verify_admin(admin_pin)
-    controller.change_reset_code(reset_code)
+    session.verify_admin(admin_pin)
+    session.set_reset_code(reset_code)
 
 
 @access.command("change-admin-pin")
 @click.option("-a", "--admin-pin", help="current Admin PIN")
 @click.option("-n", "--new-admin-pin", help="new Admin PIN")
 @click.pass_context
 def change_admin(ctx, admin_pin, new_admin_pin):
     """
     Change the Admin PIN.
 
     The Admin PIN has a minimum length of 8, and supports any type of
     alphanumeric characters.
     """
 
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
     if new_admin_pin is None:
         new_admin_pin = click_prompt(
             "New Admin PIN",
             hide_input=True,
             confirmation_prompt=True,
         )
 
-    controller.change_admin(admin_pin, new_admin_pin)
+    session.change_admin(admin_pin, new_admin_pin)
 
 
 @access.command("unblock-pin")
 @click.option(
     "-a", "--admin-pin", help='admin PIN (use "-" as a value to prompt for input)'
 )
 @click.option("-r", "--reset-code", help="Reset Code")
@@ -291,15 +267,15 @@
     If the PIN is lost or blocked you can reset it to a new value using either the
     Reset Code OR the Admin PIN.
 
     The new PIN has a minimum length of 6, and supports any type of
     alphanumeric characters.
     """
 
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if reset_code is not None and admin_pin is not None:
         raise CliFail(
             "Invalid options: Only one of --reset-code and --admin-pin may be used."
         )
 
     if admin_pin == "-":
@@ -312,16 +288,16 @@
         new_pin = click_prompt(
             "New PIN",
             hide_input=True,
             confirmation_prompt=True,
         )
 
     if admin_pin:
-        controller.verify_admin(admin_pin)
-    controller.reset_pin(new_pin, reset_code)
+        session.verify_admin(admin_pin)
+    session.reset_pin(new_pin, reset_code)
 
 
 @access.command("set-signature-policy")
 @click.argument("policy", metavar="POLICY", type=EnumChoice(PIN_POLICY))
 @click.option("-a", "--admin-pin", help="Admin PIN for OpenPGP")
 @click.pass_context
 def set_signature_policy(ctx, policy, admin_pin):
@@ -331,34 +307,34 @@
     The Signature PIN policy is used to control whether the PIN is
     always required when using the Signature key, or if it is required
     only once per session.
 
     \b
     POLICY  signature PIN policy to set (always, once)
     """
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
     try:
-        controller.verify_admin(admin_pin)
-        controller.set_signature_pin_policy(policy)
+        session.verify_admin(admin_pin)
+        session.set_signature_pin_policy(policy)
     except Exception:
         raise CliFail("Failed to set new Signature PIN policy")
 
 
 @openpgp.group("keys")
 def keys():
     """Manage private keys."""
 
 
 @keys.command("set-touch")
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT))
-@click.argument("policy", metavar="POLICY", type=EnumChoice(TOUCH_MODE))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF))
+@click.argument("policy", metavar="POLICY", type=EnumChoice(UIF))
 @click.option("-a", "--admin-pin", help="Admin PIN for OpenPGP")
 @click_force_option
 @click.pass_context
 def set_touch(ctx, key, policy, admin_pin, force):
     """
     Set the touch policy for OpenPGP keys.
 
@@ -373,120 +349,113 @@
     On              touch required
     Fixed           touch required, can't be disabled without deleting the private key
     Cached          touch required, cached for 15s after use
     Cached-Fixed    touch required, cached for 15s after use, can't be disabled
                     without deleting the private key
 
     \b
-    KEY     key slot to set (sig, enc, aut or att)
+    KEY     key slot to set (sig, dec, aut or att)
     POLICY  touch policy to set (on, off, fixed, cached or cached-fixed)
     """
-    controller = ctx.obj["controller"]
-
+    session = ctx.obj["session"]
     policy_name = policy.name.lower().replace("_", "-")
 
-    if policy not in controller.supported_touch_policies:
-        raise CliFail(f"Touch policy {policy_name} not supported by this YubiKey.")
-
-    if key == KEY_SLOT.ATT and not controller.supports_attestation:
-        raise CliFail("Attestation is not supported by this YubiKey.")
-
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
     prompt = f"Set touch policy of {key.name} key to {policy_name}?"
     if policy.is_fixed:
         prompt = (
             "WARNING: This touch policy cannot be changed without deleting the "
             + "corresponding key slot!\n"
             + prompt
         )
 
     if force or click.confirm(prompt, abort=True, err=True):
         try:
-            controller.verify_admin(admin_pin)
-            controller.set_touch(key, policy)
+            session.verify_admin(admin_pin)
+            session.set_uif(key, policy)
             logger.info(f"Touch policy for slot {key.name} set")
         except ApduError as e:
             if e.sw == SW.SECURITY_CONDITION_NOT_SATISFIED:
                 raise CliFail("Touch policy not allowed.")
             raise CliFail("Failed to set touch policy.")
 
 
 @keys.command("import")
 @click.option("-a", "--admin-pin", help="Admin PIN for OpenPGP")
 @click.pass_context
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF))
 @click.argument("private-key", type=click.File("rb"), metavar="PRIVATE-KEY")
 def import_key(ctx, key, private_key, admin_pin):
     """
     Import a private key (ONLY SUPPORTS ATTESTATION KEY).
 
     Import a private key for OpenPGP attestation.
 
     \b
     PRIVATE-KEY  file containing the private key (use '-' to use stdin)
     """
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
-    if key != KEY_SLOT.ATT:
+    if key != KEY_REF.ATT:
         ctx.fail("Importing keys is only supported for the Attestation slot.")
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
     try:
         private_key = parse_private_key(private_key.read(), password=None)
     except Exception:
         raise CliFail("Failed to parse private key.")
     try:
-        controller.verify_admin(admin_pin)
-        controller.import_key(key, private_key)
+        session.verify_admin(admin_pin)
+        session.put_key(key, private_key)
         logger.info(f"Private key imported for slot {key.name}")
     except Exception:
         raise CliFail("Failed to import attestation key.")
 
 
 @keys.command()
 @click.pass_context
 @click.option("-P", "--pin", help="PIN code")
 @click_format_option
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT, hidden=[KEY_SLOT.ATT]))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF, hidden=[KEY_REF.ATT]))
 @click.argument("certificate", type=click.File("wb"), metavar="CERTIFICATE")
 def attest(ctx, key, certificate, pin, format):
     """
     Generate a attestation certificate for a key.
 
     Attestation is used to show that an asymmetric key was generated on the
     YubiKey and therefore doesn't exist outside the device.
 
     \b
-    KEY          key slot to attest (sig, enc, aut)
+    KEY          key slot to attest (sig, dec, aut)
     CERTIFICATE  file to write attestation certificate to (use '-' to use stdout)
     """
 
-    controller = ctx.obj["controller"]
+    session = ctx.obj["session"]
 
     if not pin:
         pin = click_prompt("Enter PIN", hide_input=True)
 
     try:
-        cert = controller.read_certificate(key)
+        cert = session.get_certificate(key)
     except ValueError:
         cert = None
 
     if not cert or click.confirm(
         f"There is already data stored in the certificate slot for {key.value}, "
         "do you want to overwrite it?"
     ):
-        touch_policy = controller.get_touch(KEY_SLOT.ATT)
-        if touch_policy in [TOUCH_MODE.ON, TOUCH_MODE.FIXED]:
+        touch_policy = session.get_uif(KEY_REF.ATT)
+        if touch_policy in [UIF.ON, UIF.FIXED]:
             click.echo("Touch the YubiKey sensor...")
         try:
-            controller.verify_pin(pin)
-            cert = controller.attest(key)
+            session.verify_pin(pin)
+            cert = session.attest_key(key)
             certificate.write(cert.public_bytes(encoding=format))
             logger.info(
                 f"Attestation certificate for slot {key.name} written to "
                 f"{_fname(certificate)}"
             )
         except Exception:
             raise CliFail("Attestation failed")
@@ -497,89 +466,80 @@
     """
     Manage certificates.
     """
 
 
 @certificates.command("export")
 @click.pass_context
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF))
 @click_format_option
 @click.argument("certificate", type=click.File("wb"), metavar="CERTIFICATE")
 def export_certificate(ctx, key, format, certificate):
     """
     Export an OpenPGP certificate.
 
     \b
-    KEY          key slot to read from (sig, enc, aut, or att)
+    KEY          key slot to read from (sig, dec, aut, or att)
     CERTIFICATE  file to write certificate to (use '-' to use stdout)
     """
-    controller = ctx.obj["controller"]
-
-    if controller.version < (5, 2, 0) and key != KEY_SLOT.AUT:
-        raise CliFail(f"Certificate slot {key.name} requires YubiKey 5.2.0 or later.")
+    session = ctx.obj["session"]
 
     try:
-        cert = controller.read_certificate(key)
+        cert = session.get_certificate(key)
     except ValueError:
         raise CliFail(f"Failed to read certificate from slot {key.name}")
     certificate.write(cert.public_bytes(encoding=format))
     logger.info(f"Certificate for slot {key.name} exported to {_fname(certificate)}")
 
 
 @certificates.command("delete")
 @click.option("-a", "--admin-pin", help="Admin PIN for OpenPGP")
 @click.pass_context
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF))
 def delete_certificate(ctx, key, admin_pin):
     """
     Delete an OpenPGP certificate.
 
     \b
-    KEY         Key slot to delete certificate from (sig, enc, aut, or att).
+    KEY         Key slot to delete certificate from (sig, dec, aut, or att).
     """
-    controller = ctx.obj["controller"]
-
-    if controller.version < (5, 2, 0) and key != KEY_SLOT.AUT:
-        raise CliFail(f"Certificate slot {key.name} requires YubiKey 5.2.0 or later.")
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
     try:
-        controller.verify_admin(admin_pin)
-        controller.delete_certificate(key)
+        session.verify_admin(admin_pin)
+        session.delete_certificate(key)
         logger.info(f"Certificate for slot {key.name} deleted")
     except Exception:
         raise CliFail("Failed to delete certificate.")
 
 
 @certificates.command("import")
 @click.option("-a", "--admin-pin", help="Admin PIN for OpenPGP")
 @click.pass_context
-@click.argument("key", metavar="KEY", type=EnumChoice(KEY_SLOT))
+@click.argument("key", metavar="KEY", type=EnumChoice(KEY_REF))
 @click.argument("cert", type=click.File("rb"), metavar="CERTIFICATE")
 def import_certificate(ctx, key, cert, admin_pin):
     """
     Import an OpenPGP certificate.
 
     \b
-    KEY          key slot to import certificate to (sig, enc, aut, or att)
+    KEY          key slot to import certificate to (sig, dec, aut, or att)
     CERTIFICATE  file containing the certificate (use '-' to use stdin)
     """
-    controller = ctx.obj["controller"]
-
-    if controller.version < (5, 2, 0) and key != KEY_SLOT.AUT:
-        raise CliFail(f"Certificate slot {key.name} requires YubiKey 5.2.0 or later.")
+    session = ctx.obj["session"]
 
     if admin_pin is None:
         admin_pin = click_prompt("Enter Admin PIN", hide_input=True)
 
     try:
         certs = parse_certificates(cert.read(), password=None)
     except Exception:
         raise CliFail("Failed to parse certificate.")
     if len(certs) != 1:
         raise CliFail("Can only import one certificate.")
     try:
-        controller.verify_admin(admin_pin)
-        controller.import_certificate(key, certs[0])
+        session.verify_admin(admin_pin)
+        session.put_certificate(key, certs[0])
     except Exception:
         raise CliFail("Failed to import certificate")
```

### Comparing `yubikey_manager-5.0.1/ykman/_cli/otp.py` & `yubikey_manager-5.1.0/ykman/_cli/otp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/piv.py` & `yubikey_manager-5.1.0/ykman/_cli/piv.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     click_prompt,
     prompt_timeout,
     EnumChoice,
     pretty_print,
 )
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.backends import default_backend
+
 import click
 import datetime
 import logging
 
 
 logger = logging.getLogger(__name__)
 
@@ -651,14 +652,46 @@
         raise CliFail("Attestation failed.")
     certificate.write(cert.public_bytes(encoding=format))
     logger.info(
         f"Attestation certificate for slot {slot} written to {_fname(certificate)}"
     )
 
 
+@keys.command("info")
+@click.pass_context
+@click_slot_argument
+def metadata(ctx, slot):
+    """
+    Show metadata about a private key.
+
+    This will show what type of key is stored in a specific slot,
+    whether it was imported into the YubiKey, or generated on-chip,
+    and what the PIN and Touch policies are for using the key.
+
+    \b
+    SLOT        PIV slot of the private key
+    """
+
+    session = ctx.obj["session"]
+    try:
+        metadata = session.get_slot_metadata(slot)
+        info = {
+            "Key slot": slot,
+            "Algorithm": metadata.key_type.name,
+            "Origin": "GENERATED" if metadata.generated else "IMPORTED",
+            "PIN required for use": metadata.pin_policy.name,
+            "Touch required for use": metadata.touch_policy.name,
+        }
+        click.echo("\n".join(pretty_print(info)))
+    except ApduError as e:
+        if e.sw == SW.REFERENCE_DATA_NOT_FOUND:
+            raise CliFail(f"No key stored in slot {slot}.")
+        raise e
+
+
 @keys.command()
 @click.pass_context
 @click_format_option
 @click_slot_argument
 @click.option(
     "-v",
     "--verify",
@@ -681,42 +714,42 @@
     require the PIN to be provided.
 
     \b
     SLOT        PIV slot of the private key
     PUBLIC-KEY  file to write the public key to (use '-' to use stdout)
     """
     session = ctx.obj["session"]
-
     try:  # Prefer metadata if available
         public_key = session.get_slot_metadata(slot).public_key
         logger.debug("Public key read from YubiKey")
     except ApduError as e:
         if e.sw == SW.REFERENCE_DATA_NOT_FOUND:
-            raise CliFail(f"No key stored in slot {slot.name}.")
+            raise CliFail(f"No key stored in slot {slot}.")
+        raise CliFail(f"Unable to export public key from slot {slot}.")
     except NotSupportedError:
         try:  # Try attestation
             public_key = session.attest_key(slot).public_key()
             logger.debug("Public key read using attestation")
         except (NotSupportedError, ApduError):
             try:  # Read from stored certificate
                 public_key = session.get_certificate(slot).public_key()
                 logger.debug("Public key read from stored certificate")
                 if verify:  # Only needed when read from certificate
 
                     def do_verify():
-                        with prompt_timeout():
+                        with prompt_timeout(timeout=1.0):
                             if not check_key(session, slot, public_key):
                                 raise CliFail(
                                     "This public key is not tied to the private key in "
-                                    f"the {slot.name} slot."
+                                    f"slot {slot}."
                                 )
 
                     _verify_pin_if_needed(ctx, session, do_verify, pin)
             except ApduError:
-                raise CliFail(f"Unable to export public key from slot {slot.name}.")
+                raise CliFail(f"Unable to export public key from slot {slot}.")
 
     key_encoding = format
     public_key_output.write(
         public_key.public_bytes(
             encoding=key_encoding,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
         )
@@ -786,21 +819,39 @@
         cert_to_import = leafs[0]
     else:
         cert_to_import = certs[0]
 
     _ensure_authenticated(ctx, pin, management_key)
 
     if verify:
+        public_key = cert_to_import.public_key()
+
+        try:
+            metadata = session.get_slot_metadata(slot)
+            if metadata.pin_policy in (PIN_POLICY.ALWAYS, PIN_POLICY.ONCE):
+                pivman = ctx.obj["pivman_data"]
+                _verify_pin(ctx, session, pivman, pin)
+
+            if metadata.touch_policy in (TOUCH_POLICY.ALWAYS, TOUCH_POLICY.CACHED):
+                timeout = 0.0
+            else:
+                timeout = None
+        except ApduError as e:
+            if e.sw == SW.REFERENCE_DATA_NOT_FOUND:
+                raise CliFail("No private key in slot {slot}")
+            raise e
+        except NotSupportedError:
+            timeout = 1.0
 
         def do_verify():
-            with prompt_timeout():
-                if not check_key(session, slot, cert_to_import.public_key()):
+            with prompt_timeout(timeout=timeout):
+                if not check_key(session, slot, public_key):
                     raise CliFail(
-                        "This certificate is not tied to the private key in the "
-                        f"{slot.name} slot."
+                        "The public key of the certificate does not match the "
+                        f"private key in slot {slot}"
                     )
 
         _verify_pin_if_needed(ctx, session, do_verify, pin)
 
     session.put_certificate(slot, cert_to_import)
     session.put_object(OBJECT_ID.CHUID, generate_chuid())
 
@@ -863,28 +914,42 @@
     the YubiKey. A private key must already be present in the corresponding key slot.
 
     \b
     SLOT            PIV slot of the certificate
     PUBLIC-KEY      file containing a public key (use '-' to use stdin)
     """
     session = ctx.obj["session"]
-    _ensure_authenticated(ctx, pin, management_key, require_pin_and_key=True)
+
+    try:
+        metadata = session.get_slot_metadata(slot)
+        if metadata.touch_policy in (TOUCH_POLICY.ALWAYS, TOUCH_POLICY.CACHED):
+            timeout = 0.0
+        else:
+            timeout = None
+    except ApduError as e:
+        if e.sw == SW.REFERENCE_DATA_NOT_FOUND:
+            raise CliFail("No private key in slot {slot}")
+    except NotSupportedError:
+        timeout = 1.0
 
     data = public_key.read()
     public_key = serialization.load_pem_public_key(data, default_backend())
 
     now = datetime.datetime.utcnow()
     valid_to = now + datetime.timedelta(days=valid_days)
 
     if "=" not in subject:
         # Old style, common name only.
         subject = "CN=" + subject
 
+    # This verifies PIN, make sure next action is sign
+    _ensure_authenticated(ctx, pin, management_key, require_pin_and_key=True)
+
     try:
-        with prompt_timeout():
+        with prompt_timeout(timeout=timeout):
             cert = generate_self_signed_certificate(
                 session, slot, public_key, subject, now, valid_to, hash_algorithm
             )
         session.put_certificate(slot, cert)
         session.put_object(OBJECT_ID.CHUID, generate_chuid())
     except ApduError:
         raise CliFail("Certificate generation failed.")
@@ -914,25 +979,39 @@
     \b
     SLOT        PIV slot of the certificate
     PUBLIC-KEY  file containing a public key (use '-' to use stdin)
     CSR         file to write CSR to (use '-' to use stdout)
     """
     session = ctx.obj["session"]
     pivman = ctx.obj["pivman_data"]
-    _verify_pin(ctx, session, pivman, pin)
 
     data = public_key.read()
     public_key = serialization.load_pem_public_key(data, default_backend())
 
     if "=" not in subject:
         # Old style, common name only.
         subject = "CN=" + subject
 
     try:
-        with prompt_timeout():
+        metadata = session.get_slot_metadata(slot)
+        if metadata.touch_policy in (TOUCH_POLICY.ALWAYS, TOUCH_POLICY.CACHED):
+            timeout = 0.0
+        else:
+            timeout = None
+    except ApduError as e:
+        if e.sw == SW.REFERENCE_DATA_NOT_FOUND:
+            raise CliFail("No private key in slot {slot}")
+    except NotSupportedError:
+        timeout = 1.0
+
+    # This verifies PIN, make sure next action is sign
+    _verify_pin(ctx, session, pivman, pin)
+
+    try:
+        with prompt_timeout(timeout=timeout):
             csr = generate_csr(session, slot, public_key, subject, hash_algorithm)
     except ApduError:
         raise CliFail("Certificate Signing Request generation failed.")
 
     csr_output.write(csr.public_bytes(encoding=serialization.Encoding.PEM))
     logger.info(f"CSR for slot {slot} written to {_fname(csr_output)}")
 
@@ -1147,14 +1226,15 @@
 
 
 def _verify_pin_if_needed(ctx, session, func, pin=None, no_prompt=False):
     try:
         return func()
     except ApduError as e:
         if e.sw == SW.SECURITY_CONDITION_NOT_SATISFIED:
+            logger.debug("Command failed due to PIN required, verifying and retrying")
             pivman = ctx.obj["pivman_data"]
             _verify_pin(ctx, session, pivman, pin, no_prompt)
         else:
             raise
     return func()
```

### Comparing `yubikey_manager-5.0.1/ykman/_cli/script.py` & `yubikey_manager-5.1.0/ykman/_cli/script.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/_cli/util.py` & `yubikey_manager-5.1.0/ykman/_cli/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,24 +103,39 @@
     Use an enum's member names as the definition for a choice option.
 
     Enum member names MUST be all uppercase. Options are not case sensitive.
     Underscores in enum names are translated to dashes in the option choice.
     """
 
     def __init__(self, choices_enum, hidden=[]):
+        self.choices_names = [
+            v.name.replace("_", "-") for v in choices_enum if v not in hidden
+        ]
         super().__init__(
-            [v.name.replace("_", "-") for v in choices_enum if v not in hidden],
+            self.choices_names,
             case_sensitive=False,
         )
+        self.hidden = hidden
         self.choices_enum = choices_enum
 
     def convert(self, value, param, ctx):
         if isinstance(value, self.choices_enum):
             return value
-        name = super().convert(value, param, ctx).replace("-", "_")
+
+        try:
+            # Allow aliases
+            self.choices = [
+                k.replace("_", "-")
+                for k, v in self.choices_enum.__members__.items()
+                if v not in self.hidden
+            ]
+            name = super().convert(value, param, ctx).replace("-", "_")
+        finally:
+            self.choices = self.choices_names
+
         return self.choices_enum[name]
 
 
 def click_callback(invoke_on_missing=False):
     def wrap(f):
         @functools.wraps(f)
         def inner(ctx, param, val):
```

### Comparing `yubikey_manager-5.0.1/ykman/_openpgp.py` & `yubikey_manager-5.1.0/ykman/piv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2015 Yubico AB
+# Copyright (c) 2017 Yubico AB
 # All rights reserved.
 #
 #   Redistribution and use in source and binary forms, with or
 #   without modification, are permitted provided that the following
 #   conditions are met:
 #
 #    1. Redistributions of source code must retain the above copyright
@@ -21,676 +21,655 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-"""
-Classes and functions for interacting with the OpenPGP application on a YubiKey.
 
-WARNING: This file is not part of the stable API, and thus changes to is can occur
-without a major version increase of the project.
-
-Keep this in mind when using these classes for scripting purposes!
-"""
-
-from yubikit.core import (
-    Tlv,
-    NotSupportedError,
-    require_version,
-    int2bytes,
-    bytes2int,
-)
-from yubikit.core.smartcard import (
-    SmartCardConnection,
-    SmartCardProtocol,
-    ApduError,
-    AID,
-    SW,
+from yubikit.core import Tlv, BadResponseError, NotSupportedError
+from yubikit.core.smartcard import ApduError, SW
+from yubikit.piv import (
+    PivSession,
+    SLOT,
+    OBJECT_ID,
+    KEY_TYPE,
+    MANAGEMENT_KEY_TYPE,
+    ALGORITHM,
+    TAG_LRC,
 )
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
+from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.serialization import (
-    Encoding,
-    PrivateFormat,
-    NoEncryption,
-)
-from cryptography.hazmat.primitives.asymmetric import rsa, ec
-
-from enum import Enum, IntEnum, unique
-from dataclasses import dataclass
-from typing import Optional, Tuple
-import time
-import struct
+from cryptography.hazmat.primitives.asymmetric import rsa, ec, padding
+from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from cryptography.hazmat.backends import default_backend
+from cryptography.x509.oid import NameOID
+from collections import OrderedDict
+from datetime import datetime
 import logging
+import struct
+import os
+import re
 
-from typing import NamedTuple
-
-logger = logging.getLogger(__name__)
-
+from typing import Union, Mapping, Optional, List, Dict, Type, Any, cast
 
-class _KeySlot(NamedTuple):
-    value: str
-    indx: int
-    key_id: int
-    fingerprint: int
-    gen_time: int
-    uif: int  # touch policy
-    crt: bytes  # Control Reference Template
-
-
-@unique
-class KEY_SLOT(_KeySlot, Enum):  # type: ignore  # noqa: N801
-    SIG = _KeySlot("SIGNATURE", 1, 0xC1, 0xC7, 0xCE, 0xD6, Tlv(0xB6))
-    ENC = _KeySlot("ENCRYPTION", 2, 0xC2, 0xC8, 0xCF, 0xD7, Tlv(0xB8))
-    AUT = _KeySlot("AUTHENTICATION", 3, 0xC3, 0xC9, 0xD0, 0xD8, Tlv(0xA4))
-    ATT = _KeySlot(
-        "ATTESTATION", 4, 0xDA, 0xDB, 0xDD, 0xD9, Tlv(0xB6, Tlv(0x84, b"\x81"))
-    )
 
+logger = logging.getLogger(__name__)
 
-@unique
-class TOUCH_MODE(IntEnum):  # noqa: N801
-    OFF = 0x00
-    ON = 0x01
-    FIXED = 0x02
-    CACHED = 0x03
-    CACHED_FIXED = 0x04
 
-    @property
-    def is_fixed(self):
-        return "FIXED" in self.name
+OBJECT_ID_PIVMAN_DATA = 0x5FFF00
+OBJECT_ID_PIVMAN_PROTECTED_DATA = OBJECT_ID.PRINTED  # Use slot for printed information.
 
-    def __str__(self):
-        if self == TOUCH_MODE.OFF:
-            return "Off"
-        elif self == TOUCH_MODE.ON:
-            return "On"
-        elif self == TOUCH_MODE.FIXED:
-            return "On (fixed)"
-        elif self == TOUCH_MODE.CACHED:
-            return "Cached"
-        elif self == TOUCH_MODE.CACHED_FIXED:
-            return "Cached (fixed)"
-
-
-@unique
-class PIN_POLICY(IntEnum):  # noqa: N801
-    ALWAYS = 0x00
-    ONCE = 0x01
-
-    def __str__(self):
-        name = self.name
-        return name[0] + name[1:].lower()
-
-
-@unique
-class INS(IntEnum):  # noqa: N801
-    VERIFY = 0x20
-    CHANGE_PIN = 0x24
-    RESET_RETRY_COUNTER = 0x2C
-    ACTIVATE = 0x44
-    GENERATE_ASYM = 0x47
-    SELECT_DATA = 0xA5
-    SEND_REMAINING = 0xC0
-    GET_DATA = 0xCA
-    PUT_DATA = 0xDA
-    PUT_DATA_ODD = 0xDB
-    TERMINATE = 0xE6
-    GET_VERSION = 0xF1
-    SET_PIN_RETRIES = 0xF2
-    GET_ATTESTATION = 0xFB
-
-
-class PinRetries(NamedTuple):
-    pin: int
-    reset: int
-    admin: int
-
-
-PW1 = 0x81
-PW2 = 0x82  # Resetting Code
-PW3 = 0x83
-INVALID_PIN = b"\0" * 8
-TOUCH_METHOD_BUTTON = 0x20
-
-
-@unique
-class DO(IntEnum):
-    AID = 0x4F
-    PW_STATUS = 0xC4
-    RESETTING_CODE = 0xD3
-    KDF = 0xF9
-    ATT_CERTIFICATE = 0xFC
-    CARDHOLDER_CERTIFICATE = 0x7F21
-
-
-@unique
-class OID(bytes, Enum):
-    SECP256R1 = b"\x2a\x86\x48\xce\x3d\x03\x01\x07"
-    SECP256K1 = b"\x2b\x81\x04\x00\x0a"
-    SECP384R1 = b"\x2b\x81\x04\x00\x22"
-    SECP521R1 = b"\x2b\x81\x04\x00\x23"
-    BRAINPOOLP256R1 = b"\x2b\x24\x03\x03\x02\x08\x01\x01\x07"
-    BRAINPOOLP384R1 = b"\x2b\x24\x03\x03\x02\x08\x01\x01\x0b"
-    BRAINPOOLP512R1 = b"\x2b\x24\x03\x03\x02\x08\x01\x01\x0d"
-    X25519 = b"\x2b\x06\x01\x04\x01\x97\x55\x01\x05\x01"
-    ED25519 = b"\x2b\x06\x01\x04\x01\xda\x47\x0f\x01"
 
-    @classmethod
-    def for_name(cls, name):
-        try:
-            return getattr(cls, name.upper())
-        except AttributeError:
-            raise ValueError("Unsupported curve: " + name)
-
-
-def _get_curve_name(key):
-    if isinstance(key, ec.EllipticCurvePrivateKey):
-        return key.curve.name
-    cls_name = key.__class__.__name__
-    if "Ed25519" in cls_name:
-        return "ed25519"
-    if "X25519" in cls_name:
-        return "x25519"
-    raise ValueError("Unsupported private key")
-
-
-def _format_rsa_attributes(key_size):
-    return struct.pack(">BHHB", 0x01, key_size, 32, 0)
-
-
-def _format_ec_attributes(key_slot, curve_name):
-    if curve_name in ("ed25519", "x25519"):
-        algorithm = b"\x16"
-    elif key_slot == KEY_SLOT.ENC:
-        algorithm = b"\x12"
-    else:
-        algorithm = b"\x13"
-    return algorithm + OID.for_name(curve_name)
-
-
-def _get_key_attributes(key, key_slot):
-    if isinstance(key, rsa.RSAPrivateKeyWithSerialization):
-        if key.private_numbers().public_numbers.e != 65537:
-            raise ValueError("RSA keys with e != 65537 are not supported!")
-        return _format_rsa_attributes(key.key_size)
-    curve_name = _get_curve_name(key)
-    return _format_ec_attributes(key_slot, curve_name)
-
-
-def _get_key_template(key, key_slot, crt=False):
-    def _pack_tlvs(tlvs):
-        header = b""
-        body = b""
-        for tlv in tlvs:
-            header += tlv[: -tlv.length]
-            body += tlv.value
-        return Tlv(0x7F48, header) + Tlv(0x5F48, body)
-
-    values: Tuple[Tlv, ...]
-
-    if isinstance(key, rsa.RSAPrivateKeyWithSerialization):
-        rsa_numbers = key.private_numbers()
-        ln = (key.key_size // 8) // 2
-
-        e = Tlv(0x91, b"\x01\x00\x01")  # e=65537
-        p = Tlv(0x92, int2bytes(rsa_numbers.p, ln))
-        q = Tlv(0x93, int2bytes(rsa_numbers.q, ln))
-        values = (e, p, q)
-        if crt:
-            dp = Tlv(0x94, int2bytes(rsa_numbers.dmp1, ln))
-            dq = Tlv(0x95, int2bytes(rsa_numbers.dmq1, ln))
-            qinv = Tlv(0x96, int2bytes(rsa_numbers.iqmp, ln))
-            n = Tlv(0x97, int2bytes(rsa_numbers.public_numbers.n, 2 * ln))
-            values += (dp, dq, qinv, n)
-
-    elif isinstance(key, ec.EllipticCurvePrivateKeyWithSerialization):
-        ec_numbers = key.private_numbers()
-        ln = key.key_size // 8
-
-        privkey = Tlv(0x92, int2bytes(ec_numbers.private_value, ln))
-        values = (privkey,)
-
-    elif _get_curve_name(key) in ("ed25519", "x25519"):
-        privkey = Tlv(
-            0x92, key.private_bytes(Encoding.Raw, PrivateFormat.Raw, NoEncryption())
-        )
-        values = (privkey,)
+_NAME_ATTRIBUTES = {
+    "CN": NameOID.COMMON_NAME,
+    "L": NameOID.LOCALITY_NAME,
+    "ST": NameOID.STATE_OR_PROVINCE_NAME,
+    "O": NameOID.ORGANIZATION_NAME,
+    "OU": NameOID.ORGANIZATIONAL_UNIT_NAME,
+    "C": NameOID.COUNTRY_NAME,
+    "STREET": NameOID.STREET_ADDRESS,
+    "DC": NameOID.DOMAIN_COMPONENT,
+    "UID": NameOID.USER_ID,
+}
 
-    return Tlv(0x4D, key_slot.crt + _pack_tlvs(values))
 
+_ESCAPED = "\\\"+,'<> #="
 
-@unique
-class HashAlgorithm(IntEnum):
-    SHA256 = 0x08
-    SHA512 = 0x0A
 
-    def create_digest(self):
-        algorithm = getattr(hashes, self.name)
-        return hashes.Hash(algorithm(), default_backend())
+def _parse(value: str) -> List[List[str]]:
+    remaining = list(value)
+    name = []
+    entry = []
+    buf = ""
+    hexbuf = b""
+    while remaining:
+        c = remaining.pop(0)
+        if c == "\\":
+            c1 = remaining.pop(0)
+            if c1 in _ESCAPED:
+                c = c1
+            else:
+                c2 = remaining.pop(0)
+                hexbuf += bytes.fromhex(c1 + c2)
+                try:
+                    c = hexbuf.decode()
+                    hexbuf = b""
+                except UnicodeDecodeError:
+                    continue  # Possibly multi-byte, expect more hex
+        elif c in ",+":
+            entry.append(buf)
+            buf = ""
+            if c == ",":
+                name.append(entry)
+                entry = []
+            continue
+        if hexbuf:
+            raise ValueError("Invalid UTF-8 data")
+        buf += c
+    entry.append(buf)
+    name.append(entry)
+    return name
+
+
+_DOTTED_STRING_RE = re.compile(r"\d(\.\d+)+")
+
+
+def parse_rfc4514_string(value: str) -> x509.Name:
+    """Parses an RFC 4514 string into a x509.Name.
+
+    See: https://tools.ietf.org/html/rfc4514.html
+    """
+    name = _parse(value)
+    attributes: List[x509.RelativeDistinguishedName] = []
+    for entry in name:
+        parts = []
+        for part in entry:
+            if "=" not in part:
+                raise ValueError("Invalid RFC 4514 string")
+            k, v = part.split("=", 1)
+            if k in _NAME_ATTRIBUTES:
+                attr = _NAME_ATTRIBUTES[k]
+            elif _DOTTED_STRING_RE.fullmatch(k):
+                attr = x509.ObjectIdentifier(k)
+            else:
+                raise ValueError(f"Unsupported attribute: '{k}'")
+            parts.append(x509.NameAttribute(attr, v))
+        attributes.insert(0, x509.RelativeDistinguishedName(parts))
+
+    return x509.Name(attributes)
+
+
+def _dummy_key(algorithm):
+    if algorithm == KEY_TYPE.RSA1024:
+        return rsa.generate_private_key(65537, 1024, default_backend())  # nosec
+    if algorithm == KEY_TYPE.RSA2048:
+        return rsa.generate_private_key(65537, 2048, default_backend())
+    if algorithm == KEY_TYPE.ECCP256:
+        return ec.generate_private_key(ec.SECP256R1(), default_backend())
+    if algorithm == KEY_TYPE.ECCP384:
+        return ec.generate_private_key(ec.SECP384R1(), default_backend())
+    raise ValueError("Invalid algorithm")
+
+
+def derive_management_key(pin: str, salt: bytes) -> bytes:
+    """Derive a management key from the users PIN and a salt.
+
+    NOTE: This method of derivation is deprecated! Protect the management key using
+    PivmanProtectedData instead.
+    """
+    kdf = PBKDF2HMAC(hashes.SHA1(), 24, salt, 10000, default_backend())  # nosec
+    return kdf.derive(pin.encode("utf-8"))
+
+
+def generate_random_management_key(algorithm: MANAGEMENT_KEY_TYPE) -> bytes:
+    """Generates a new random management key."""
+    return os.urandom(algorithm.key_len)
+
+
+class PivmanData:
+    def __init__(self, raw_data: bytes = Tlv(0x80)):
+        data = Tlv.parse_dict(Tlv(raw_data).value)
+        self._flags = struct.unpack(">B", data[0x81])[0] if 0x81 in data else None
+        self.salt = data.get(0x82)
+        self.pin_timestamp = struct.unpack(">I", data[0x83]) if 0x83 in data else None
+
+    def _get_flag(self, mask: int) -> bool:
+        return bool((self._flags or 0) & mask)
+
+    def _set_flag(self, mask: int, value: bool) -> None:
+        if value:
+            self._flags = (self._flags or 0) | mask
+        elif self._flags is not None:
+            self._flags &= ~mask
 
+    @property
+    def puk_blocked(self) -> bool:
+        return self._get_flag(0x01)
 
-@unique
-class KdfAlgorithm(IntEnum):
-    NONE = 0x00
-    KDF_ITERSALTED_S2K = 0x03
+    @puk_blocked.setter
+    def puk_blocked(self, value: bool) -> None:
+        self._set_flag(0x01, value)
 
+    @property
+    def mgm_key_protected(self) -> bool:
+        return self._get_flag(0x02)
 
-def _kdf_none(pin, salt, hash_algorithm, iteration_count):
-    return pin
+    @mgm_key_protected.setter
+    def mgm_key_protected(self, value: bool) -> None:
+        self._set_flag(0x02, value)
 
+    @property
+    def has_protected_key(self) -> bool:
+        return self.has_derived_key or self.has_stored_key
 
-def _kdf_itersalted_s2k(pin, salt, hash_algorithm, iteration_count):
-    data = salt + pin
-    digest = hash_algorithm.create_digest()
-    # Although the field is called "iteration count", it's actually
-    # the number of bytes to be passed to the hash function, which
-    # is called only once. Go figure!
-    data_count, trailing_bytes = divmod(iteration_count, len(data))
-    for _ in range(data_count):
-        digest.update(data)
-    digest.update(data[:trailing_bytes])
-    return digest.finalize()
+    @property
+    def has_derived_key(self) -> bool:
+        return self.salt is not None
 
+    @property
+    def has_stored_key(self) -> bool:
+        return self.mgm_key_protected
 
-_KDFS = {
-    KdfAlgorithm.NONE: _kdf_none,
-    KdfAlgorithm.KDF_ITERSALTED_S2K: _kdf_itersalted_s2k,
-}
+    def get_bytes(self) -> bytes:
+        data = b""
+        if self._flags is not None:
+            data += Tlv(0x81, struct.pack(">B", self._flags))
+        if self.salt is not None:
+            data += Tlv(0x82, self.salt)
+        if self.pin_timestamp is not None:
+            data += Tlv(0x83, struct.pack(">I", self.pin_timestamp))
+        return Tlv(0x80, data)
+
+
+class PivmanProtectedData:
+    def __init__(self, raw_data: bytes = Tlv(0x88)):
+        data = Tlv.parse_dict(Tlv(raw_data).value)
+        self.key = data.get(0x89)
+
+    def get_bytes(self) -> bytes:
+        data = b""
+        if self.key is not None:
+            data += Tlv(0x89, self.key)
+        return Tlv(0x88, data)
+
+
+def get_pivman_data(session: PivSession) -> PivmanData:
+    """Reads out the Pivman data from a YubiKey."""
+    logger.debug("Reading pivman data")
+    try:
+        return PivmanData(session.get_object(OBJECT_ID_PIVMAN_DATA))
+    except ApduError as e:
+        if e.sw == SW.FILE_NOT_FOUND:
+            # No data there, initialise a new object.
+            logger.debug("No data, initializing blank")
+            return PivmanData()
+        raise
+
+
+def get_pivman_protected_data(session: PivSession) -> PivmanProtectedData:
+    """Reads out the Pivman protected data from a YubiKey.
+
+    This function requires PIN verification prior to being called.
+    """
+    logger.debug("Reading protected pivman data")
+    try:
+        return PivmanProtectedData(session.get_object(OBJECT_ID_PIVMAN_PROTECTED_DATA))
+    except ApduError as e:
+        if e.sw == SW.FILE_NOT_FOUND:
+            # No data there, initialise a new object.
+            logger.debug("No data, initializing blank")
+            return PivmanProtectedData()
+        raise
+
+
+def pivman_set_mgm_key(
+    session: PivSession,
+    new_key: bytes,
+    algorithm: MANAGEMENT_KEY_TYPE,
+    touch: bool = False,
+    store_on_device: bool = False,
+) -> None:
+    """Set a new management key, while keeping PivmanData in sync."""
+    pivman = get_pivman_data(session)
+    pivman_prot = None
 
+    if store_on_device or (not store_on_device and pivman.has_stored_key):
+        # Ensure we have access to protected data before overwriting key
+        try:
+            pivman_prot = get_pivman_protected_data(session)
+        except Exception:
+            logger.debug("Failed to initialize protected pivman data", exc_info=True)
+            if store_on_device:
+                raise
 
-def _parse_int(data, tag, func=lambda x: x, default=None):
-    return func(int.from_bytes(data[tag], "big")) if tag in data else default
+    # Set the new management key
+    session.set_management_key(algorithm, new_key, touch)
 
+    if pivman.has_derived_key:
+        # Clear salt for old derived keys.
+        logger.debug("Clearing salt in pivman data")
+        pivman.salt = None
+
+    # Set flag for stored or not stored key.
+    pivman.mgm_key_protected = store_on_device
+
+    # Update readable pivman data
+    session.put_object(OBJECT_ID_PIVMAN_DATA, pivman.get_bytes())
+
+    if pivman_prot is not None:
+        if store_on_device:
+            # Store key in protected pivman data
+            logger.debug("Storing key in protected pivman data")
+            pivman_prot.key = new_key
+            session.put_object(OBJECT_ID_PIVMAN_PROTECTED_DATA, pivman_prot.get_bytes())
+        elif pivman_prot.key:
+            # If new key should not be stored and there is an old stored key,
+            # try to clear it.
+            logger.debug("Clearing old key in protected pivman data")
+            try:
+                pivman_prot.key = None
+                session.put_object(
+                    OBJECT_ID_PIVMAN_PROTECTED_DATA,
+                    pivman_prot.get_bytes(),
+                )
+            except ApduError:
+                logger.debug("No PIN provided, can't clear key...", exc_info=True)
 
-@dataclass
-class KdfData:
-    kdf_algorithm: KdfAlgorithm
-    hash_algorithm: Optional[HashAlgorithm]
-    iteration_count: Optional[int]
-    pw1_salt_bytes: Optional[bytes]
-    pw2_salt_bytes: Optional[bytes]
-    pw3_salt_bytes: Optional[bytes]
-    pw1_initial_hash: Optional[bytes]
-    pw3_initial_hash: Optional[bytes]
-
-    def process(self, pw, pin):
-        kdf = _KDFS[self.kdf_algorithm]
-        if pw == PW1:
-            salt = self.pw1_salt_bytes
-        elif pw == PW2:
-            salt = self.pw2_salt_bytes or self.pw1_salt_bytes
-        elif pw == PW3:
-            salt = self.pw3_salt_bytes or self.pw1_salt_bytes
-        else:
-            raise ValueError("Invalid value for pw")
-        return kdf(pin, salt, self.hash_algorithm, self.iteration_count)
 
-    @classmethod
-    def parse(cls, data: bytes) -> "KdfData":
-        fields = Tlv.parse_dict(data)
-        return cls(
-            _parse_int(fields, 0x81, KdfAlgorithm, KdfAlgorithm.NONE),
-            _parse_int(fields, 0x82, HashAlgorithm),
-            _parse_int(fields, 0x83),
-            fields.get(0x84),
-            fields.get(0x85),
-            fields.get(0x86),
-            fields.get(0x87),
-            fields.get(0x88),
+def pivman_change_pin(session: PivSession, old_pin: str, new_pin: str) -> None:
+    """Change the PIN, while keeping PivmanData in sync."""
+    session.change_pin(old_pin, new_pin)
+
+    pivman = get_pivman_data(session)
+    if pivman.has_derived_key:
+        logger.debug("Has derived management key, update for new PIN")
+        session.authenticate(
+            MANAGEMENT_KEY_TYPE.TDES,
+            derive_management_key(old_pin, cast(bytes, pivman.salt)),
         )
+        session.verify_pin(new_pin)
+        new_salt = os.urandom(16)
+        new_key = derive_management_key(new_pin, new_salt)
+        session.set_management_key(MANAGEMENT_KEY_TYPE.TDES, new_key)
+        pivman.salt = new_salt
+        session.put_object(OBJECT_ID_PIVMAN_DATA, pivman.get_bytes())
 
 
-class OpenPgpController(object):
-    def __init__(self, connection: SmartCardConnection):
-        protocol = SmartCardProtocol(connection)
-        self._app = protocol
+def list_certificates(session: PivSession) -> Mapping[SLOT, Optional[x509.Certificate]]:
+    """Reads out and parses stored certificates.
+
+    Only certificates which are successfully parsed are returned.
+    """
+    certs = OrderedDict()
+    for slot in set(SLOT) - {SLOT.ATTESTATION}:
         try:
-            protocol.select(AID.OPENPGP)
-        except ApduError as e:
-            if e.sw in (SW.NO_INPUT_DATA, SW.CONDITIONS_NOT_SATISFIED):
-                protocol.send_apdu(0, INS.ACTIVATE, 0, 0)
-                protocol.select(AID.OPENPGP)
-            else:
-                raise
-        self._version = self._read_version()
+            certs[slot] = session.get_certificate(slot)
+        except ApduError:
+            pass
+        except BadResponseError:
+            certs[slot] = None  # type: ignore
+
+    return certs
+
+
+def check_key(
+    session: PivSession,
+    slot: SLOT,
+    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
+) -> bool:
+    """Check that a given public key corresponds to the private key in a slot.
+
+    This will create a signature using the private key, so the PIN must be verified
+    prior to calling this function if the PIN policy requires it.
+    """
+    try:
+        test_data = b"test"
+        logger.debug(
+            "Testing private key by creating a test signature, and verifying it"
+        )
 
-    @property
-    def version(self):
-        return self._version
+        test_sig = session.sign(
+            slot,
+            KEY_TYPE.from_public_key(public_key),
+            test_data,
+            hashes.SHA256(),
+            padding.PKCS1v15(),  # Only used for RSA
+        )
 
-    def _get_data(self, do):
-        return self._app.send_apdu(0, INS.GET_DATA, do >> 8, do & 0xFF)
+        if isinstance(public_key, rsa.RSAPublicKey):
+            public_key.verify(
+                test_sig,
+                test_data,
+                padding.PKCS1v15(),
+                hashes.SHA256(),
+            )
+        elif isinstance(public_key, ec.EllipticCurvePublicKey):
+            public_key.verify(test_sig, test_data, ec.ECDSA(hashes.SHA256()))
+        else:
+            raise ValueError("Unknown key type: " + type(public_key))
+        return True
 
-    def _put_data(self, do, data):
-        self._app.send_apdu(0, INS.PUT_DATA, do >> 8, do & 0xFF, data)
+    except ApduError as e:
+        if e.sw in (SW.INCORRECT_PARAMETERS, SW.WRONG_PARAMETERS_P1P2):
+            logger.debug(f"Couldn't create signature: SW={e.sw:04x}")
+            return False
+        raise
+
+    except InvalidSignature:
+        logger.debug("Signature verification failed")
+        return False
+
+
+def generate_chuid() -> bytes:
+    """Generates a CHUID (Cardholder Unique Identifier)."""
+    # Non-Federal Issuer FASC-N
+    # [9999-9999-999999-0-1-0000000000300001]
+    FASC_N = (
+        b"\xd4\xe7\x39\xda\x73\x9c\xed\x39\xce\x73\x9d\x83\x68"
+        + b"\x58\x21\x08\x42\x10\x84\x21\xc8\x42\x10\xc3\xeb"
+    )
+    # Expires on: 2030-01-01
+    EXPIRY = b"\x32\x30\x33\x30\x30\x31\x30\x31"
 
-    def _select_certificate(self, key_slot):
-        try:
-            require_version(self.version, (5, 2, 0))
-            data: bytes = Tlv(0x60, Tlv(0x5C, b"\x7f\x21"))
-            if self.version <= (5, 4, 3):
-                # These use a non-standard byte in the command.
-                data = b"\x06" + data  # 6 is the length of the data.
-            self._app.send_apdu(
-                0,
-                INS.SELECT_DATA,
-                3 - key_slot.indx,
-                0x04,
-                data,
-            )
-        except NotSupportedError:
-            if key_slot == KEY_SLOT.AUT:
-                return  # Older version still support AUT, which is the default slot.
-            raise
-
-    def _read_version(self):
-        bcd_hex = self._app.send_apdu(0, INS.GET_VERSION, 0, 0).hex()
-        return tuple(int(bcd_hex[i : i + 2]) for i in range(0, 6, 2))
-
-    def get_openpgp_version(self):
-        data = self._get_data(DO.AID)
-        return data[6], data[7]
-
-    def get_remaining_pin_tries(self):
-        data = self._get_data(DO.PW_STATUS)
-        return PinRetries(*data[4:7])
+    return (
+        Tlv(0x30, FASC_N)
+        + Tlv(0x34, os.urandom(16))
+        + Tlv(0x35, EXPIRY)
+        + Tlv(0x3E)
+        + Tlv(TAG_LRC)
+    )
 
-    def get_signature_pin_policy(self):
-        data = self._get_data(DO.PW_STATUS)
 
-        try:
-            return PIN_POLICY(data[0])
-        except ValueError:
-            return PIN_POLICY.ONCE
+def generate_ccc() -> bytes:
+    """Generates a CCC (Card Capability Container)."""
+    return (
+        Tlv(0xF0, b"\xa0\x00\x00\x01\x16\xff\x02" + os.urandom(14))
+        + Tlv(0xF1, b"\x21")
+        + Tlv(0xF2, b"\x21")
+        + Tlv(0xF3)
+        + Tlv(0xF4, b"\x00")
+        + Tlv(0xF5, b"\x10")
+        + Tlv(0xF6)
+        + Tlv(0xF7)
+        + Tlv(0xFA)
+        + Tlv(0xFB)
+        + Tlv(0xFC)
+        + Tlv(0xFD)
+        + Tlv(TAG_LRC)
+    )
 
-    def set_signature_pin_policy(self, pin_policy):
-        """Requires Admin PIN verification."""
-        data = struct.pack(">B", pin_policy)
 
-        self._put_data(DO.PW_STATUS, data)
+def get_piv_info(session: PivSession):
+    """Get human readable information about the PIV configuration."""
+    pivman = get_pivman_data(session)
+    info: Dict[str, Any] = {
+        "PIV version": session.version,
+    }
+    lines: List[Any] = [info]
 
-    def _block_pins(self):
-        retries = self.get_remaining_pin_tries()
+    try:
+        pin_data = session.get_pin_metadata()
+        if pin_data.default_value:
+            lines.append("WARNING: Using default PIN!")
+        tries_str = "%d/%d" % (pin_data.attempts_remaining, pin_data.total_attempts)
+    except NotSupportedError:
+        # Largest possible number of PIN tries to get back is 15
+        tries = session.get_pin_attempts()
+        tries_str = "15 or more" if tries == 15 else str(tries)
+    info["PIN tries remaining"] = tries_str
+    if pivman.puk_blocked:
+        lines.append("PUK is blocked")
+
+    try:
+        metadata = session.get_management_key_metadata()
+        if metadata.default_value:
+            lines.append("WARNING: Using default Management key!")
+        key_type = metadata.key_type
+    except NotSupportedError:
+        key_type = MANAGEMENT_KEY_TYPE.TDES
+    info["Management key algorithm"] = key_type.name
+
+    if pivman.has_derived_key:
+        lines.append("Management key is derived from PIN.")
+    if pivman.has_stored_key:
+        lines.append("Management key is stored on the YubiKey, protected by PIN.")
+
+    objects: Dict[str, Any] = {}
+    lines.append(objects)
+    try:
+        objects["CHUID"] = session.get_object(OBJECT_ID.CHUID)
+    except ApduError as e:
+        if e.sw == SW.FILE_NOT_FOUND:
+            objects["CHUID"] = "No data available"
+
+    try:
+        objects["CCC"] = session.get_object(OBJECT_ID.CAPABILITY)
+    except ApduError as e:
+        if e.sw == SW.FILE_NOT_FOUND:
+            objects["CCC"] = "No data available"
+
+    for slot, cert in list_certificates(session).items():
+        cert_data: Dict[str, Any] = {}
+        objects[f"Slot {slot}"] = cert_data
+        if cert:
+            try:
+                # Try to read out full DN, fallback to only CN.
+                # Support for DN was added in crytography 2.5
+                subject_dn = cert.subject.rfc4514_string()
+                issuer_dn = cert.issuer.rfc4514_string()
+                print_dn = True
+            except AttributeError:
+                print_dn = False
+                logger.debug("Failed to read DN, falling back to only CNs")
+                cn = cert.subject.get_attributes_for_oid(x509.NameOID.COMMON_NAME)
+                subject_cn = cn[0].value if cn else "None"
+                cn = cert.issuer.get_attributes_for_oid(x509.NameOID.COMMON_NAME)
+                issuer_cn = cn[0].value if cn else "None"
+            except ValueError as e:
+                # Malformed certificates may throw ValueError
+                logger.debug("Failed parsing certificate", exc_info=True)
+                cert_data["Error"] = f"Malformed certificate: {e}"
+                continue
 
-        for _ in range(retries.pin):
+            fingerprint = cert.fingerprint(hashes.SHA256()).hex()
             try:
-                self._app.send_apdu(0, INS.VERIFY, 0, PW1, INVALID_PIN)
-            except ApduError:
-                pass
-        for _ in range(retries.admin):
+                key_algo = KEY_TYPE.from_public_key(cert.public_key()).name
+            except ValueError:
+                key_algo = "Unsupported"
+            serial = cert.serial_number
             try:
-                self._app.send_apdu(0, INS.VERIFY, 0, PW3, INVALID_PIN)
-            except ApduError:
-                pass
-
-    def reset(self):
-        if self.version < (1, 0, 6):
-            raise ValueError("Resetting OpenPGP data requires version 1.0.6 or later.")
-        self._block_pins()
-        self._app.send_apdu(0, INS.TERMINATE, 0, 0)
-        self._app.send_apdu(0, INS.ACTIVATE, 0, 0)
-
-    def _get_kdf(self):
-        try:
-            data = self._get_data(DO.KDF)
-        except ApduError:
-            data = b""
-        return KdfData.parse(data)
-
-    def _verify(self, pw, pin):
-        try:
-            pin = self._get_kdf().process(pw, pin.encode())
-            self._app.send_apdu(0, INS.VERIFY, 0, pw, pin)
-        except ApduError:
-            pw_remaining = self.get_remaining_pin_tries()[pw - PW1]
-            raise ValueError(f"Invalid PIN, {pw_remaining} tries remaining.")
-
-    def verify_pin(self, pin):
-        self._verify(PW1, pin)
-
-    def verify_admin(self, admin_pin):
-        self._verify(PW3, admin_pin)
-
-    def _change(self, pw, pin, new_pin):
-        try:
-            pin = self._get_kdf().process(pw, pin.encode())
-            new_pin = self._get_kdf().process(pw, new_pin.encode())
-            self._app.send_apdu(0, INS.CHANGE_PIN, 0, pw, pin + new_pin)
-        except ApduError as e:
-            if e.sw == SW.CONDITIONS_NOT_SATISFIED:
-                raise ValueError("Conditions of use not satisfied.")
+                not_before: Optional[datetime] = cert.not_valid_before
+            except ValueError:
+                logger.debug("Failed reading not_valid_before", exc_info=True)
+                not_before = None
+            try:
+                not_after: Optional[datetime] = cert.not_valid_after
+            except ValueError:
+                logger.debug("Failed reading not_valid_after", exc_info=True)
+                not_after = None
+
+            # Print out everything
+            cert_data["Algorithm"] = key_algo
+            if print_dn:
+                cert_data["Subject DN"] = subject_dn
+                cert_data["Issuer DN"] = issuer_dn
             else:
-                pw_remaining = self.get_remaining_pin_tries()[pw - PW1]
-                raise ValueError(f"Invalid PIN, {pw_remaining} tries remaining.")
-
-    def change_pin(self, pin, new_pin):
-        self._change(PW1, pin, new_pin)
-
-    def change_admin(self, admin_pin, new_admin_pin):
-        self._change(PW3, admin_pin, new_admin_pin)
-
-    def change_reset_code(self, reset_code):
-        data = self._get_kdf().process(PW2, reset_code.encode())
-        self._put_data(DO.RESETTING_CODE, data)
-
-    def reset_pin(self, new_pin, reset_code=None):
-        p1 = 2
-        data = self._get_kdf().process(PW1, new_pin.encode())
-        if reset_code:
-            rc = self._get_kdf().process(PW2, reset_code.encode())
-            p1 = 0
-            data = rc + data
+                cert_data["Subject CN"] = subject_cn
+                cert_data["Issuer CN"] = issuer_cn
+            cert_data["Serial"] = serial
+            cert_data["Fingerprint"] = fingerprint
+            if not_before:
+                cert_data["Not before"] = not_before.isoformat()
+            if not_after:
+                cert_data["Not after"] = not_after.isoformat()
+        else:
+            cert_data["Error"] = "Failed to parse certificate"
 
-        try:
-            self._app.send_apdu(0, INS.RESET_RETRY_COUNTER, p1, PW1, data)
-        except ApduError as e:
-            if e.sw == SW.CONDITIONS_NOT_SATISFIED:
-                raise ValueError("Conditions of use not satisfied.")
-            else:
-                reset_remaining = self.get_remaining_pin_tries().reset
-                raise ValueError(
-                    f"Invalid Reset Code, {reset_remaining} tries remaining."
-                )
+    return lines
 
-    @property
-    def supported_touch_policies(self):
-        if self.version < (4, 2, 0):
-            return []
-        if self.version < (5, 2, 1):
-            return [TOUCH_MODE.ON, TOUCH_MODE.OFF, TOUCH_MODE.FIXED]
-        if self.version >= (5, 2, 1):
-            return [
-                TOUCH_MODE.ON,
-                TOUCH_MODE.OFF,
-                TOUCH_MODE.FIXED,
-                TOUCH_MODE.CACHED,
-                TOUCH_MODE.CACHED_FIXED,
-            ]
 
-    @property
-    def supports_attestation(self):
-        return self.version >= (5, 2, 1)
+_AllowedHashTypes = Union[
+    hashes.SHA224,
+    hashes.SHA256,
+    hashes.SHA384,
+    hashes.SHA512,
+    hashes.SHA3_224,
+    hashes.SHA3_256,
+    hashes.SHA3_384,
+    hashes.SHA3_512,
+]
+
+
+def sign_certificate_builder(
+    session: PivSession,
+    slot: SLOT,
+    key_type: KEY_TYPE,
+    builder: x509.CertificateBuilder,
+    hash_algorithm: Type[_AllowedHashTypes] = hashes.SHA256,
+) -> x509.Certificate:
+    """Sign a Certificate."""
+    logger.debug("Signing a certificate")
+    dummy_key = _dummy_key(key_type)
+    cert = builder.sign(dummy_key, hash_algorithm(), default_backend())
+
+    sig = session.sign(
+        slot,
+        key_type,
+        cert.tbs_certificate_bytes,
+        hash_algorithm(),
+        padding.PKCS1v15(),  # Only used for RSA
+    )
 
-    def get_touch(self, key_slot):
-        if not self.supported_touch_policies:
-            raise ValueError("Touch policy is available on YubiKey 4 or later.")
-        if key_slot == KEY_SLOT.ATT and not self.supports_attestation:
-            raise ValueError("Attestation key not available on this device.")
-        data = self._get_data(key_slot.uif)
-        return TOUCH_MODE(data[0])
-
-    def set_touch(self, key_slot, mode):
-        """Requires Admin PIN verification."""
-        if not self.supported_touch_policies:
-            raise ValueError("Touch policy is available on YubiKey 4 or later.")
-        if mode not in self.supported_touch_policies:
-            raise ValueError("Touch policy not available on this device.")
-        self._put_data(key_slot.uif, struct.pack(">BB", mode, TOUCH_METHOD_BUTTON))
-
-    def set_pin_retries(self, pw1_tries, pw2_tries, pw3_tries):
-        """Requires Admin PIN verification."""
-        if (1, 0, 0) <= self.version < (1, 0, 7):  # For YubiKey NEO
-            raise ValueError(
-                "Setting PIN retry counters requires version 1.0.7 or later."
-            )
-        if (4, 0, 0) <= self.version < (4, 3, 1):  # For YubiKey 4
-            raise ValueError(
-                "Setting PIN retry counters requires version 4.3.1 or later."
-            )
-        self._app.send_apdu(
-            0,
-            INS.SET_PIN_RETRIES,
-            0,
-            0,
-            struct.pack(">BBB", pw1_tries, pw2_tries, pw3_tries),
-        )
+    seq = Tlv.parse_list(Tlv.unpack(0x30, cert.public_bytes(Encoding.DER)))
+    # Replace signature, add unused bits = 0
+    seq[2] = Tlv(seq[2].tag, b"\0" + sig)
+    # Re-assemble sequence
+    der = Tlv(0x30, b"".join(seq))
+
+    return x509.load_der_x509_certificate(der, default_backend())
+
+
+def sign_csr_builder(
+    session: PivSession,
+    slot: SLOT,
+    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
+    builder: x509.CertificateSigningRequestBuilder,
+    hash_algorithm: Type[_AllowedHashTypes] = hashes.SHA256,
+) -> x509.CertificateSigningRequest:
+    """Sign a CSR."""
+    logger.debug("Signing a CSR")
+    key_type = KEY_TYPE.from_public_key(public_key)
+    dummy_key = _dummy_key(key_type)
+    csr = builder.sign(dummy_key, hash_algorithm(), default_backend())
+    seq = Tlv.parse_list(Tlv.unpack(0x30, csr.public_bytes(Encoding.DER)))
+
+    # Replace public key
+    pub_format = (
+        PublicFormat.PKCS1
+        if key_type.algorithm == ALGORITHM.RSA
+        else PublicFormat.SubjectPublicKeyInfo
+    )
+    dummy_bytes = dummy_key.public_key().public_bytes(Encoding.DER, pub_format)
+    pub_bytes = public_key.public_bytes(Encoding.DER, pub_format)
+    seq[0] = Tlv(seq[0].replace(dummy_bytes, pub_bytes))
+
+    sig = session.sign(
+        slot,
+        key_type,
+        seq[0],
+        hash_algorithm(),
+        padding.PKCS1v15(),  # Only used for RSA
+    )
 
-    def read_certificate(self, key_slot):
-        if key_slot == KEY_SLOT.ATT:
-            require_version(self.version, (5, 2, 0))
-            data = self._get_data(DO.ATT_CERTIFICATE)
-        else:
-            self._select_certificate(key_slot)
-            data = self._get_data(DO.CARDHOLDER_CERTIFICATE)
-        if not data:
-            raise ValueError("No certificate found!")
-        return x509.load_der_x509_certificate(data, default_backend())
-
-    def import_certificate(self, key_slot, certificate):
-        """Requires Admin PIN verification."""
-        cert_data = certificate.public_bytes(Encoding.DER)
-        if key_slot == KEY_SLOT.ATT:
-            require_version(self.version, (5, 2, 0))
-            self._put_data(DO.ATT_CERTIFICATE, cert_data)
-        else:
-            self._select_certificate(key_slot)
-            self._put_data(DO.CARDHOLDER_CERTIFICATE, cert_data)
+    # Replace signature, add unused bits = 0
+    seq[2] = Tlv(seq[2].tag, b"\0" + sig)
+    # Re-assemble sequence
+    der = Tlv(0x30, b"".join(seq))
+
+    return x509.load_der_x509_csr(der, default_backend())
+
+
+def generate_self_signed_certificate(
+    session: PivSession,
+    slot: SLOT,
+    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
+    subject_str: str,
+    valid_from: datetime,
+    valid_to: datetime,
+    hash_algorithm: Type[_AllowedHashTypes] = hashes.SHA256,
+) -> x509.Certificate:
+    """Generate a self-signed certificate using a private key in a slot."""
+    logger.debug("Generating a self-signed certificate")
+    key_type = KEY_TYPE.from_public_key(public_key)
+
+    subject = parse_rfc4514_string(subject_str)
+    builder = (
+        x509.CertificateBuilder()
+        .public_key(public_key)
+        .subject_name(subject)
+        .issuer_name(subject)  # Same as subject on self-signed certificate.
+        .serial_number(x509.random_serial_number())
+        .not_valid_before(valid_from)
+        .not_valid_after(valid_to)
+    )
 
-    def import_key(self, key_slot, key, fingerprint=None, timestamp=None):
-        """Requires Admin PIN verification."""
-        if self.version >= (4, 0, 0):
-            attributes = _get_key_attributes(key, key_slot)
-            self._put_data(key_slot.key_id, attributes)
-
-        template = _get_key_template(key, key_slot, self.version < (4, 0, 0))
-        self._app.send_apdu(0, INS.PUT_DATA_ODD, 0x3F, 0xFF, template)
-
-        if fingerprint is not None:
-            self._put_data(key_slot.fingerprint, fingerprint)
-
-        if timestamp is not None:
-            self._put_data(key_slot.gen_time, struct.pack(">I", timestamp))
-
-    def generate_rsa_key(self, key_slot, key_size, timestamp=None):
-        """Requires Admin PIN verification."""
-        if (4, 2, 0) <= self.version < (4, 3, 5):
-            raise NotSupportedError("RSA key generation not supported on this YubiKey")
-
-        if timestamp is None:
-            timestamp = int(time.time())
-
-        neo = self.version < (4, 0, 0)
-        if not neo:
-            attributes = _format_rsa_attributes(key_size)
-            self._put_data(key_slot.key_id, attributes)
-        elif key_size != 2048:
-            raise ValueError("Unsupported key size!")
-        resp = self._app.send_apdu(0, INS.GENERATE_ASYM, 0x80, 0x00, key_slot.crt)
-
-        data = Tlv.parse_dict(Tlv.unpack(0x7F49, resp))
-        numbers = rsa.RSAPublicNumbers(bytes2int(data[0x82]), bytes2int(data[0x81]))
-
-        self._put_data(key_slot.gen_time, struct.pack(">I", timestamp))
-        # TODO: Calculate and write fingerprint
-
-        return numbers.public_key(default_backend())
-
-    def generate_ec_key(self, key_slot, curve_name, timestamp=None):
-        require_version(self.version, (5, 2, 0))
-        """Requires Admin PIN verification."""
-        if timestamp is None:
-            timestamp = int(time.time())
-
-        attributes = _format_ec_attributes(key_slot, curve_name)
-        self._put_data(key_slot.key_id, attributes)
-        resp = self._app.send_apdu(0, INS.GENERATE_ASYM, 0x80, 0x00, key_slot.crt)
-
-        data = Tlv.parse_dict(Tlv.unpack(0x7F49, resp))
-        pubkey_enc = data[0x86]
-
-        self._put_data(key_slot.gen_time, struct.pack(">I", timestamp))
-        # TODO: Calculate and write fingerprint
-
-        if curve_name == "x25519":
-            # Added in 2.0
-            from cryptography.hazmat.primitives.asymmetric import x25519
-
-            return x25519.X25519PublicKey.from_public_bytes(pubkey_enc)
-        if curve_name == "ed25519":
-            # Added in 2.6
-            from cryptography.hazmat.primitives.asymmetric import ed25519
-
-            return ed25519.Ed25519PublicKey.from_public_bytes(pubkey_enc)
-
-        curve = getattr(ec, curve_name.upper())
-        return ec.EllipticCurvePublicKey.from_encoded_point(curve(), pubkey_enc)
-
-    def delete_key(self, key_slot):
-        """Requires Admin PIN verification."""
-        if self.version < (4, 0, 0):
-            # Import over the key
-            self.import_key(
-                key_slot,
-                rsa.generate_private_key(65537, 2048, default_backend()),
-                b"\0" * 20,
-                0,
-            )
-        else:
-            # Delete key by changing the key attributes twice.
-            self._put_data(key_slot.key_id, _format_rsa_attributes(4096))
-            self._put_data(key_slot.key_id, _format_rsa_attributes(2048))
-
-    def delete_certificate(self, key_slot):
-        """Requires Admin PIN verification."""
-        if key_slot == KEY_SLOT.ATT:
-            require_version(self.version, (5, 2, 0))
-            self._put_data(DO.ATT_CERTIFICATE, b"")
-        else:
-            self._select_certificate(key_slot)
-            self._put_data(DO.CARDHOLDER_CERTIFICATE, b"")
+    return sign_certificate_builder(session, slot, key_type, builder, hash_algorithm)
 
-    def attest(self, key_slot):
-        """Requires User PIN verification."""
-        require_version(self.version, (5, 2, 0))
-        self._app.send_apdu(0x80, INS.GET_ATTESTATION, key_slot.indx, 0)
-        return self.read_certificate(key_slot)
-
-
-def get_openpgp_info(controller: OpenPgpController):
-    """Get human readable information about the OpenPGP configuration."""
-    retries = controller.get_remaining_pin_tries()
-    data = {
-        "OpenPGP version": "%d.%d" % controller.get_openpgp_version(),
-        "Application version": "%d.%d.%d" % controller.version,
-        "PIN tries remaining": retries.pin,
-        "Reset code tries remaining": retries.reset,
-        "Admin PIN tries remaining": retries.admin,
-        "Require PIN for signature": controller.get_signature_pin_policy(),
-    }
 
-    # Touch only available on YK4 and later
-    if controller.version >= (4, 2, 6):
-        touch = {
-            "Signature key": controller.get_touch(KEY_SLOT.SIG),
-            "Encryption key": controller.get_touch(KEY_SLOT.ENC),
-            "Authentication key": controller.get_touch(KEY_SLOT.AUT),
-        }
-        if controller.supports_attestation:
-            touch["Attestation key"] = controller.get_touch(KEY_SLOT.ATT)
-        data["Touch policies"] = touch
+def generate_csr(
+    session: PivSession,
+    slot: SLOT,
+    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
+    subject_str: str,
+    hash_algorithm: Type[_AllowedHashTypes] = hashes.SHA256,
+) -> x509.CertificateSigningRequest:
+    """Generate a CSR using a private key in a slot."""
+    logger.debug("Generating a CSR")
+    builder = x509.CertificateSigningRequestBuilder().subject_name(
+        parse_rfc4514_string(subject_str)
+    )
 
-    return data
+    return sign_csr_builder(session, slot, public_key, builder, hash_algorithm)
```

### Comparing `yubikey_manager-5.0.1/ykman/base.py` & `yubikey_manager-5.1.0/ykman/base.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/device.py` & `yubikey_manager-5.1.0/ykman/device.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/diagnostics.py` & `yubikey_manager-5.1.0/ykman/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from . import __version__ as ykman_version
 from .util import get_windows_version
 from .pcsc import list_readers, list_devices as list_ccid_devices
 from .hid import list_otp_devices, list_ctap_devices
 from .piv import get_piv_info
-from ._openpgp import OpenPgpController, get_openpgp_info
+from .openpgp import get_openpgp_info
 
 from yubikit.core.smartcard import SmartCardConnection
 from yubikit.core.fido import FidoConnection
 from yubikit.core.otp import OtpConnection
 from yubikit.management import ManagementSession
 from yubikit.yubiotp import YubiOtpSession
 from yubikit.piv import PivSession
 from yubikit.oath import OathSession
+from yubikit.openpgp import OpenPgpSession
 from yubikit.support import read_info, get_name
 from fido2.ctap import CtapError
 from fido2.ctap2 import Ctap2, ClientPin
 
 from dataclasses import asdict
 from datetime import datetime
 from typing import List, Dict, Any
@@ -76,15 +77,15 @@
         return get_piv_info(piv)
     except Exception as e:
         return f"PIV not accessible {e!r}"
 
 
 def openpgp_info(conn):
     try:
-        openpgp = OpenPgpController(conn)
+        openpgp = OpenPgpSession(conn)
         return get_openpgp_info(openpgp)
     except Exception as e:
         return f"OpenPGP not accessible {e!r}"
 
 
 def oath_info(conn):
     try:
```

### Comparing `yubikey_manager-5.0.1/ykman/fido.py` & `yubikey_manager-5.1.0/ykman/fido.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/__init__.py` & `yubikey_manager-5.1.0/ykman/hid/__init__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/base.py` & `yubikey_manager-5.1.0/ykman/hid/base.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/freebsd.py` & `yubikey_manager-5.1.0/ykman/hid/freebsd.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/linux.py` & `yubikey_manager-5.1.0/ykman/hid/linux.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/macos.py` & `yubikey_manager-5.1.0/ykman/hid/macos.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/hid/windows.py` & `yubikey_manager-5.1.0/ykman/hid/windows.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/logging.py` & `yubikey_manager-5.1.0/ykman/logging.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/logging_setup.py` & `yubikey_manager-5.1.0/ykman/logging_setup.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/oath.py` & `yubikey_manager-5.1.0/ykman/oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/otp.py` & `yubikey_manager-5.1.0/ykman/otp.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     serial: int,
     public_id: bytes,
     private_id: bytes,
     key: bytes,
     access_code: Optional[bytes] = None,
     timestamp: Optional[datetime] = None,
 ) -> str:
-    """Produces a CSV line in the "Yubico" format (ycfg)."""
+    """Produces a CSV line in the "Yubico" format."""
     ts = timestamp or datetime.now()
     return ",".join(
         [
             str(serial),
             modhex_encode(public_id),
             private_id.hex(),
             key.hex(),
```

### Comparing `yubikey_manager-5.0.1/ykman/pcsc/__init__.py` & `yubikey_manager-5.1.0/ykman/pcsc/__init__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/piv.py` & `yubikey_manager-5.1.0/yubikit/management.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017 Yubico AB
+# Copyright (c) 2020 Yubico AB
 # All rights reserved.
 #
 #   Redistribution and use in source and binary forms, with or
 #   without modification, are permitted provided that the following
 #   conditions are met:
 #
 #    1. Redistributions of source code must retain the above copyright
@@ -21,643 +21,502 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-
-from yubikit.core import Tlv, BadResponseError, NotSupportedError
-from yubikit.core.smartcard import ApduError, SW
-from yubikit.piv import (
-    PivSession,
-    SLOT,
-    OBJECT_ID,
-    KEY_TYPE,
-    MANAGEMENT_KEY_TYPE,
-    ALGORITHM,
-    TAG_LRC,
+from .core import (
+    bytes2int,
+    int2bytes,
+    require_version,
+    Version,
+    Tlv,
+    TRANSPORT,
+    USB_INTERFACE,
+    NotSupportedError,
+    BadResponseError,
+    ApplicationNotAvailableError,
 )
-
-from cryptography import x509
-from cryptography.exceptions import InvalidSignature
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import rsa, ec, padding
-from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
-from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-from cryptography.hazmat.backends import default_backend
-from cryptography.x509.oid import NameOID
-from collections import OrderedDict
-from datetime import datetime
-import logging
+from .core.otp import (
+    check_crc,
+    OtpConnection,
+    OtpProtocol,
+    STATUS_OFFSET_PROG_SEQ,
+    CommandRejectedError,
+)
+from .core.fido import FidoConnection
+from .core.smartcard import AID, SmartCardConnection, SmartCardProtocol
+from fido2.hid import CAPABILITY as CTAP_CAPABILITY
+
+from enum import IntEnum, IntFlag, unique
+from dataclasses import dataclass
+from typing import Optional, Union, Mapping
+import abc
 import struct
-import os
-import re
+import logging
 
-from typing import Union, Mapping, Optional, List, Dict, Type, Any, cast
+logger = logging.getLogger(__name__)
 
 
-logger = logging.getLogger(__name__)
+@unique
+class CAPABILITY(IntFlag):
+    """YubiKey Application identifiers."""
+
+    OTP = 0x01
+    U2F = 0x02
+    FIDO2 = 0x200
+    OATH = 0x20
+    PIV = 0x10
+    OPENPGP = 0x08
+    HSMAUTH = 0x100
+
+    def __str__(self):
+        name = "|".join(c.name or str(c) for c in CAPABILITY if c in self)
+        return f"{name}: {hex(self)}"
 
+    @property
+    def display_name(self):
+        if self == CAPABILITY.U2F:
+            return "FIDO U2F"
+        elif self == CAPABILITY.OPENPGP:
+            return "OpenPGP"
+        elif self == CAPABILITY.HSMAUTH:
+            return "YubiHSM Auth"
+        return self.name or ", ".join(c.display_name for c in CAPABILITY if c in self)
 
-OBJECT_ID_PIVMAN_DATA = 0x5FFF00
-OBJECT_ID_PIVMAN_PROTECTED_DATA = OBJECT_ID.PRINTED  # Use slot for printed information.
+    @property
+    def usb_interfaces(self) -> USB_INTERFACE:
+        ifaces = USB_INTERFACE(0)
+        if self & CAPABILITY.OTP:
+            ifaces |= USB_INTERFACE.OTP
+        if self & (CAPABILITY.U2F | CAPABILITY.FIDO2):
+            ifaces |= USB_INTERFACE.FIDO
+        if self & (
+            CAPABILITY.OATH | CAPABILITY.PIV | CAPABILITY.OPENPGP | CAPABILITY.HSMAUTH
+        ):
+            ifaces |= USB_INTERFACE.CCID
+        return ifaces
+
+
+@unique
+class FORM_FACTOR(IntEnum):
+    """YubiKey device form factors."""
+
+    UNKNOWN = 0x00
+    USB_A_KEYCHAIN = 0x01
+    USB_A_NANO = 0x02
+    USB_C_KEYCHAIN = 0x03
+    USB_C_NANO = 0x04
+    USB_C_LIGHTNING = 0x05
+    USB_A_BIO = 0x06
+    USB_C_BIO = 0x07
+
+    def __str__(self):
+        if self == FORM_FACTOR.USB_A_KEYCHAIN:
+            return "Keychain (USB-A)"
+        elif self == FORM_FACTOR.USB_A_NANO:
+            return "Nano (USB-A)"
+        elif self == FORM_FACTOR.USB_C_KEYCHAIN:
+            return "Keychain (USB-C)"
+        elif self == FORM_FACTOR.USB_C_NANO:
+            return "Nano (USB-C)"
+        elif self == FORM_FACTOR.USB_C_LIGHTNING:
+            return "Keychain (USB-C, Lightning)"
+        elif self == FORM_FACTOR.USB_A_BIO:
+            return "Bio (USB-A)"
+        elif self == FORM_FACTOR.USB_C_BIO:
+            return "Bio (USB-C)"
+        else:
+            return "Unknown"
 
+    @classmethod
+    def from_code(cls, code: int) -> "FORM_FACTOR":
+        if code and not isinstance(code, int):
+            raise ValueError(f"Invalid form factor code: {code}")
+        code &= 0xF
+        return cls(code) if code in cls.__members__.values() else cls.UNKNOWN
+
+
+@unique
+class DEVICE_FLAG(IntFlag):
+    """Configuration flags."""
+
+    REMOTE_WAKEUP = 0x40
+    EJECT = 0x80
+
+
+TAG_USB_SUPPORTED = 0x01
+TAG_SERIAL = 0x02
+TAG_USB_ENABLED = 0x03
+TAG_FORM_FACTOR = 0x04
+TAG_VERSION = 0x05
+TAG_AUTO_EJECT_TIMEOUT = 0x06
+TAG_CHALRESP_TIMEOUT = 0x07
+TAG_DEVICE_FLAGS = 0x08
+TAG_APP_VERSIONS = 0x09
+TAG_CONFIG_LOCK = 0x0A
+TAG_UNLOCK = 0x0B
+TAG_REBOOT = 0x0C
+TAG_NFC_SUPPORTED = 0x0D
+TAG_NFC_ENABLED = 0x0E
+
+
+@dataclass
+class DeviceConfig:
+    """Management settings for YubiKey which can be configured by the user."""
+
+    enabled_capabilities: Mapping[TRANSPORT, CAPABILITY]
+    auto_eject_timeout: Optional[int]
+    challenge_response_timeout: Optional[int]
+    device_flags: Optional[DEVICE_FLAG]
+
+    def get_bytes(
+        self,
+        reboot: bool,
+        cur_lock_code: Optional[bytes] = None,
+        new_lock_code: Optional[bytes] = None,
+    ) -> bytes:
+        buf = b""
+        if reboot:
+            buf += Tlv(TAG_REBOOT)
+        if cur_lock_code:
+            buf += Tlv(TAG_UNLOCK, cur_lock_code)
+        usb_enabled = self.enabled_capabilities.get(TRANSPORT.USB)
+        if usb_enabled is not None:
+            buf += Tlv(TAG_USB_ENABLED, int2bytes(usb_enabled, 2))
+        nfc_enabled = self.enabled_capabilities.get(TRANSPORT.NFC)
+        if nfc_enabled is not None:
+            buf += Tlv(TAG_NFC_ENABLED, int2bytes(nfc_enabled, 2))
+        if self.auto_eject_timeout is not None:
+            buf += Tlv(TAG_AUTO_EJECT_TIMEOUT, int2bytes(self.auto_eject_timeout, 2))
+        if self.challenge_response_timeout is not None:
+            buf += Tlv(TAG_CHALRESP_TIMEOUT, int2bytes(self.challenge_response_timeout))
+        if self.device_flags is not None:
+            buf += Tlv(TAG_DEVICE_FLAGS, int2bytes(self.device_flags))
+        if new_lock_code:
+            buf += Tlv(TAG_CONFIG_LOCK, new_lock_code)
+        if len(buf) > 0xFF:
+            raise NotSupportedError("DeviceConfiguration too large")
+        return int2bytes(len(buf)) + buf
+
+
+@dataclass
+class DeviceInfo:
+    """Information about a YubiKey readable using the ManagementSession."""
+
+    config: DeviceConfig
+    serial: Optional[int]
+    version: Version
+    form_factor: FORM_FACTOR
+    supported_capabilities: Mapping[TRANSPORT, CAPABILITY]
+    is_locked: bool
+    is_fips: bool = False
+    is_sky: bool = False
+
+    def has_transport(self, transport: TRANSPORT) -> bool:
+        return transport in self.supported_capabilities
+
+    @classmethod
+    def parse(cls, encoded: bytes, default_version: Version) -> "DeviceInfo":
+        if len(encoded) - 1 != encoded[0]:
+            raise BadResponseError("Invalid length")
+        data = Tlv.parse_dict(encoded[1:])
+        locked = data.get(TAG_CONFIG_LOCK) == b"\1"
+        serial = bytes2int(data.get(TAG_SERIAL, b"\0")) or None
+        ff_value = bytes2int(data.get(TAG_FORM_FACTOR, b"\0"))
+        form_factor = FORM_FACTOR.from_code(ff_value)
+        fips = bool(ff_value & 0x80)
+        sky = bool(ff_value & 0x40)
+        if TAG_VERSION in data:
+            version = Version.from_bytes(data[TAG_VERSION])
+        else:
+            version = default_version
+        auto_eject_to = bytes2int(data.get(TAG_AUTO_EJECT_TIMEOUT, b"\0"))
+        chal_resp_to = bytes2int(data.get(TAG_CHALRESP_TIMEOUT, b"\0"))
+        flags = DEVICE_FLAG(bytes2int(data.get(TAG_DEVICE_FLAGS, b"\0")))
 
-_NAME_ATTRIBUTES = {
-    "CN": NameOID.COMMON_NAME,
-    "L": NameOID.LOCALITY_NAME,
-    "ST": NameOID.STATE_OR_PROVINCE_NAME,
-    "O": NameOID.ORGANIZATION_NAME,
-    "OU": NameOID.ORGANIZATIONAL_UNIT_NAME,
-    "C": NameOID.COUNTRY_NAME,
-    "STREET": NameOID.STREET_ADDRESS,
-    "DC": NameOID.DOMAIN_COMPONENT,
-    "UID": NameOID.USER_ID,
-}
-
-
-_ESCAPED = "\\\"+,'<> #="
-
-
-def _parse(value: str) -> List[List[str]]:
-    remaining = list(value)
-    name = []
-    entry = []
-    buf = ""
-    hexbuf = b""
-    while remaining:
-        c = remaining.pop(0)
-        if c == "\\":
-            c1 = remaining.pop(0)
-            if c1 in _ESCAPED:
-                c = c1
-            else:
-                c2 = remaining.pop(0)
-                hexbuf += bytes.fromhex(c1 + c2)
-                try:
-                    c = hexbuf.decode()
-                    hexbuf = b""
-                except UnicodeDecodeError:
-                    continue  # Possibly multi-byte, expect more hex
-        elif c in ",+":
-            entry.append(buf)
-            buf = ""
-            if c == ",":
-                name.append(entry)
-                entry = []
-            continue
-        if hexbuf:
-            raise ValueError("Invalid UTF-8 data")
-        buf += c
-    entry.append(buf)
-    name.append(entry)
-    return name
-
-
-_DOTTED_STRING_RE = re.compile(r"\d(\.\d+)+")
-
-
-def parse_rfc4514_string(value: str) -> x509.Name:
-    """Parses an RFC 4514 string into a x509.Name.
-
-    See: https://tools.ietf.org/html/rfc4514.html
-    """
-    name = _parse(value)
-    attributes: List[x509.RelativeDistinguishedName] = []
-    for entry in name:
-        parts = []
-        for part in entry:
-            if "=" not in part:
-                raise ValueError("Invalid RFC 4514 string")
-            k, v = part.split("=", 1)
-            if k in _NAME_ATTRIBUTES:
-                attr = _NAME_ATTRIBUTES[k]
-            elif _DOTTED_STRING_RE.fullmatch(k):
-                attr = x509.ObjectIdentifier(k)
-            else:
-                raise ValueError(f"Unsupported attribute: '{k}'")
-            parts.append(x509.NameAttribute(attr, v))
-        attributes.insert(0, x509.RelativeDistinguishedName(parts))
-
-    return x509.Name(attributes)
-
-
-def _dummy_key(algorithm):
-    if algorithm == KEY_TYPE.RSA1024:
-        return rsa.generate_private_key(65537, 1024, default_backend())  # nosec
-    if algorithm == KEY_TYPE.RSA2048:
-        return rsa.generate_private_key(65537, 2048, default_backend())
-    if algorithm == KEY_TYPE.ECCP256:
-        return ec.generate_private_key(ec.SECP256R1(), default_backend())
-    if algorithm == KEY_TYPE.ECCP384:
-        return ec.generate_private_key(ec.SECP384R1(), default_backend())
-    raise ValueError("Invalid algorithm")
-
-
-def derive_management_key(pin: str, salt: bytes) -> bytes:
-    """Derive a management key from the users PIN and a salt.
-
-    NOTE: This method of derivation is deprecated! Protect the management key using
-    PivmanProtectedData instead.
-    """
-    kdf = PBKDF2HMAC(hashes.SHA1(), 24, salt, 10000, default_backend())  # nosec
-    return kdf.derive(pin.encode("utf-8"))
-
-
-def generate_random_management_key(algorithm: MANAGEMENT_KEY_TYPE) -> bytes:
-    """Generates a new random management key."""
-    return os.urandom(algorithm.key_len)
-
-
-class PivmanData:
-    def __init__(self, raw_data: bytes = Tlv(0x80)):
-        data = Tlv.parse_dict(Tlv(raw_data).value)
-        self._flags = struct.unpack(">B", data[0x81])[0] if 0x81 in data else None
-        self.salt = data.get(0x82)
-        self.pin_timestamp = struct.unpack(">I", data[0x83]) if 0x83 in data else None
-
-    def _get_flag(self, mask: int) -> bool:
-        return bool((self._flags or 0) & mask)
-
-    def _set_flag(self, mask: int, value: bool) -> None:
-        if value:
-            self._flags = (self._flags or 0) | mask
-        elif self._flags is not None:
-            self._flags &= ~mask
+        supported = {}
+        enabled = {}
 
-    @property
-    def puk_blocked(self) -> bool:
-        return self._get_flag(0x01)
+        if version == (4, 2, 4):  # Doesn't report correctly
+            supported[TRANSPORT.USB] = CAPABILITY(0x3F)
+        else:
+            supported[TRANSPORT.USB] = CAPABILITY(bytes2int(data[TAG_USB_SUPPORTED]))
+        if TAG_USB_ENABLED in data:  # From YK 5.0.0
+            if not ((4, 0, 0) <= version < (5, 0, 0)):  # Broken on YK4
+                enabled[TRANSPORT.USB] = CAPABILITY(bytes2int(data[TAG_USB_ENABLED]))
+        if TAG_NFC_SUPPORTED in data:  # YK with NFC
+            supported[TRANSPORT.NFC] = CAPABILITY(bytes2int(data[TAG_NFC_SUPPORTED]))
+            enabled[TRANSPORT.NFC] = CAPABILITY(bytes2int(data[TAG_NFC_ENABLED]))
+
+        return cls(
+            DeviceConfig(enabled, auto_eject_to, chal_resp_to, flags),
+            serial,
+            version,
+            form_factor,
+            supported,
+            locked,
+            fips,
+            sky,
+        )
 
-    @puk_blocked.setter
-    def puk_blocked(self, value: bool) -> None:
-        self._set_flag(0x01, value)
 
-    @property
-    def mgm_key_protected(self) -> bool:
-        return self._get_flag(0x02)
+_MODES = [
+    USB_INTERFACE.OTP,  # 0x00
+    USB_INTERFACE.CCID,  # 0x01
+    USB_INTERFACE.OTP | USB_INTERFACE.CCID,  # 0x02
+    USB_INTERFACE.FIDO,  # 0x03
+    USB_INTERFACE.OTP | USB_INTERFACE.FIDO,  # 0x04
+    USB_INTERFACE.FIDO | USB_INTERFACE.CCID,  # 0x05
+    USB_INTERFACE.OTP | USB_INTERFACE.FIDO | USB_INTERFACE.CCID,  # 0x06
+]
+
+
+@dataclass(init=False, repr=False)
+class Mode:
+    """YubiKey USB Mode configuration for use with YubiKey NEO and 4."""
 
-    @mgm_key_protected.setter
-    def mgm_key_protected(self, value: bool) -> None:
-        self._set_flag(0x02, value)
+    code: int
+    interfaces: USB_INTERFACE
 
-    @property
-    def has_protected_key(self) -> bool:
-        return self.has_derived_key or self.has_stored_key
+    def __init__(self, interfaces: USB_INTERFACE):
+        try:
+            self.code = _MODES.index(interfaces)
+            self.interfaces = USB_INTERFACE(interfaces)
+        except ValueError:
+            raise ValueError("Invalid mode!")
+
+    def __repr__(self):
+        return "+".join(t.name or str(t) for t in USB_INTERFACE if t in self.interfaces)
+
+    @classmethod
+    def from_code(cls, code: int) -> "Mode":
+        # Mode is determined from the lowest 3 bits
+        try:
+            return cls(_MODES[code & 0b00000111])
+        except IndexError:
+            raise ValueError("Invalid mode code")
 
-    @property
-    def has_derived_key(self) -> bool:
-        return self.salt is not None
 
-    @property
-    def has_stored_key(self) -> bool:
-        return self.mgm_key_protected
+SLOT_DEVICE_CONFIG = 0x11
+SLOT_YK4_CAPABILITIES = 0x13
+SLOT_YK4_SET_DEVICE_INFO = 0x15
 
-    def get_bytes(self) -> bytes:
-        data = b""
-        if self._flags is not None:
-            data += Tlv(0x81, struct.pack(">B", self._flags))
-        if self.salt is not None:
-            data += Tlv(0x82, self.salt)
-        if self.pin_timestamp is not None:
-            data += Tlv(0x83, struct.pack(">I", self.pin_timestamp))
-        return Tlv(0x80, data)
-
-
-class PivmanProtectedData:
-    def __init__(self, raw_data: bytes = Tlv(0x88)):
-        data = Tlv.parse_dict(Tlv(raw_data).value)
-        self.key = data.get(0x89)
-
-    def get_bytes(self) -> bytes:
-        data = b""
-        if self.key is not None:
-            data += Tlv(0x89, self.key)
-        return Tlv(0x88, data)
-
-
-def get_pivman_data(session: PivSession) -> PivmanData:
-    """Reads out the Pivman data from a YubiKey."""
-    logger.debug("Reading pivman data")
-    try:
-        return PivmanData(session.get_object(OBJECT_ID_PIVMAN_DATA))
-    except ApduError as e:
-        if e.sw == SW.FILE_NOT_FOUND:
-            # No data there, initialise a new object.
-            logger.debug("No data, initializing blank")
-            return PivmanData()
-        raise
-
-
-def get_pivman_protected_data(session: PivSession) -> PivmanProtectedData:
-    """Reads out the Pivman protected data from a YubiKey.
-
-    This function requires PIN verification prior to being called.
-    """
-    logger.debug("Reading protected pivman data")
-    try:
-        return PivmanProtectedData(session.get_object(OBJECT_ID_PIVMAN_PROTECTED_DATA))
-    except ApduError as e:
-        if e.sw == SW.FILE_NOT_FOUND:
-            # No data there, initialise a new object.
-            logger.debug("No data, initializing blank")
-            return PivmanProtectedData()
-        raise
-
-
-def pivman_set_mgm_key(
-    session: PivSession,
-    new_key: bytes,
-    algorithm: MANAGEMENT_KEY_TYPE,
-    touch: bool = False,
-    store_on_device: bool = False,
-) -> None:
-    """Set a new management key, while keeping PivmanData in sync."""
-    pivman = get_pivman_data(session)
-    pivman_prot = None
 
-    if store_on_device or (not store_on_device and pivman.has_stored_key):
-        # Ensure we have access to protected data before overwriting key
-        try:
-            pivman_prot = get_pivman_protected_data(session)
-        except Exception:
-            logger.debug("Failed to initialize protected pivman data", exc_info=True)
-            if store_on_device:
-                raise
+class _Backend(abc.ABC):
+    version: Version
 
-    # Set the new management key
-    session.set_management_key(algorithm, new_key, touch)
+    @abc.abstractmethod
+    def close(self) -> None:
+        ...
 
-    if pivman.has_derived_key:
-        # Clear salt for old derived keys.
-        logger.debug("Clearing salt in pivman data")
-        pivman.salt = None
-
-    # Set flag for stored or not stored key.
-    pivman.mgm_key_protected = store_on_device
-
-    # Update readable pivman data
-    session.put_object(OBJECT_ID_PIVMAN_DATA, pivman.get_bytes())
-
-    if pivman_prot is not None:
-        if store_on_device:
-            # Store key in protected pivman data
-            logger.debug("Storing key in protected pivman data")
-            pivman_prot.key = new_key
-            session.put_object(OBJECT_ID_PIVMAN_PROTECTED_DATA, pivman_prot.get_bytes())
-        elif pivman_prot.key:
-            # If new key should not be stored and there is an old stored key,
-            # try to clear it.
-            logger.debug("Clearing old key in protected pivman data")
-            try:
-                pivman_prot.key = None
-                session.put_object(
-                    OBJECT_ID_PIVMAN_PROTECTED_DATA,
-                    pivman_prot.get_bytes(),
-                )
-            except ApduError:
-                logger.debug("No PIN provided, can't clear key...", exc_info=True)
+    @abc.abstractmethod
+    def set_mode(self, data: bytes) -> None:
+        ...
 
+    @abc.abstractmethod
+    def read_config(self) -> bytes:
+        ...
 
-def pivman_change_pin(session: PivSession, old_pin: str, new_pin: str) -> None:
-    """Change the PIN, while keeping PivmanData in sync."""
-    session.change_pin(old_pin, new_pin)
-
-    pivman = get_pivman_data(session)
-    if pivman.has_derived_key:
-        logger.debug("Has derived management key, update for new PIN")
-        session.authenticate(
-            MANAGEMENT_KEY_TYPE.TDES,
-            derive_management_key(old_pin, cast(bytes, pivman.salt)),
-        )
-        session.verify_pin(new_pin)
-        new_salt = os.urandom(16)
-        new_key = derive_management_key(new_pin, new_salt)
-        session.set_management_key(MANAGEMENT_KEY_TYPE.TDES, new_key)
-        pivman.salt = new_salt
-        session.put_object(OBJECT_ID_PIVMAN_DATA, pivman.get_bytes())
+    @abc.abstractmethod
+    def write_config(self, config: bytes) -> None:
+        ...
 
 
-def list_certificates(session: PivSession) -> Mapping[SLOT, Optional[x509.Certificate]]:
-    """Reads out and parses stored certificates.
-
-    Only certificates which are successfully parsed are returned.
-    """
-    certs = OrderedDict()
-    for slot in set(SLOT) - {SLOT.ATTESTATION}:
+class _ManagementOtpBackend(_Backend):
+    def __init__(self, otp_connection):
+        self.protocol = OtpProtocol(otp_connection)
+        self.version = self.protocol.version
+        if (1, 0, 0) <= self.version < (3, 0, 0):
+            raise ApplicationNotAvailableError()
+
+    def close(self):
+        self.protocol.close()
+
+    def set_mode(self, data):
+        empty = self.protocol.read_status()[STATUS_OFFSET_PROG_SEQ] == 0
         try:
-            certs[slot] = session.get_certificate(slot)
-        except ApduError:
-            pass
-        except BadResponseError:
-            certs[slot] = None  # type: ignore
-
-    return certs
-
-
-def check_key(
-    session: PivSession,
-    slot: SLOT,
-    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
-) -> bool:
-    """Check that a given public key corresponds to the private key in a slot.
-
-    This will create a signature using the private key, so the PIN must be verified
-    prior to calling this function if the PIN policy requires it.
-    """
-    try:
-        test_data = b"test"
-        logger.debug(
-            "Testing private key by creating a test signature, and verifying it"
-        )
+            self.protocol.send_and_receive(SLOT_DEVICE_CONFIG, data)
+        except CommandRejectedError:
+            if empty:
+                return  # ProgSeq isn't updated by set mode when empty
+            raise
+
+    def read_config(self):
+        response = self.protocol.send_and_receive(SLOT_YK4_CAPABILITIES)
+        r_len = response[0]
+        if check_crc(response[: r_len + 1 + 2]):
+            return response[: r_len + 1]
+        raise BadResponseError("Invalid checksum")
+
+    def write_config(self, config):
+        self.protocol.send_and_receive(SLOT_YK4_SET_DEVICE_INFO, config)
+
+
+INS_READ_CONFIG = 0x1D
+INS_WRITE_CONFIG = 0x1C
+INS_SET_MODE = 0x16
+P1_DEVICE_CONFIG = 0x11
+
+
+class _ManagementSmartCardBackend(_Backend):
+    def __init__(self, smartcard_connection):
+        self.protocol = SmartCardProtocol(smartcard_connection)
+        try:
+            select_bytes = self.protocol.select(AID.MANAGEMENT)
+            if select_bytes[-2:] == b"\x90\x00":
+                # YubiKey Edge incorrectly appends SW twice.
+                select_bytes = select_bytes[:-2]
+            select_str = select_bytes.decode()
+            self.version = Version.from_string(select_str)
+            # For YubiKey NEO, we use the OTP application for further commands
+            if self.version[0] == 3:
+                # Workaround to "de-select" on NEO, otherwise it gets stuck.
+                self.protocol.connection.send_and_receive(b"\xa4\x04\x00\x08")
+                self.protocol.select(AID.OTP)
+        except ApplicationNotAvailableError:
+            if smartcard_connection.transport == TRANSPORT.NFC:
+                # Probably NEO over NFC
+                status = self.protocol.select(AID.OTP)
+                self.version = Version.from_bytes(status[:3])
+            else:
+                raise
 
-        test_sig = session.sign(
-            slot,
-            KEY_TYPE.from_public_key(public_key),
-            test_data,
-            hashes.SHA256(),
-            padding.PKCS1v15(),  # Only used for RSA
-        )
+    def close(self):
+        self.protocol.close()
 
-        if isinstance(public_key, rsa.RSAPublicKey):
-            public_key.verify(
-                test_sig,
-                test_data,
-                padding.PKCS1v15(),
-                hashes.SHA256(),
-            )
-        elif isinstance(public_key, ec.EllipticCurvePublicKey):
-            public_key.verify(test_sig, test_data, ec.ECDSA(hashes.SHA256()))
+    def set_mode(self, data):
+        if self.version[0] == 3:  # Using the OTP application
+            self.protocol.send_apdu(0, 0x01, SLOT_DEVICE_CONFIG, 0, data)
         else:
-            raise ValueError("Unknown key type: " + type(public_key))
-        return True
+            self.protocol.send_apdu(0, INS_SET_MODE, P1_DEVICE_CONFIG, 0, data)
 
-    except ApduError as e:
-        if e.sw in (SW.INCORRECT_PARAMETERS, SW.WRONG_PARAMETERS_P1P2):
-            logger.debug(f"Couldn't create signature: SW={e.sw:04x}")
-            return False
-        raise
-
-    except InvalidSignature:
-        logger.debug("Signature verification failed")
-        return False
-
-
-def generate_chuid() -> bytes:
-    """Generates a CHUID (Cardholder Unique Identifier)."""
-    # Non-Federal Issuer FASC-N
-    # [9999-9999-999999-0-1-0000000000300001]
-    FASC_N = (
-        b"\xd4\xe7\x39\xda\x73\x9c\xed\x39\xce\x73\x9d\x83\x68"
-        + b"\x58\x21\x08\x42\x10\x84\x21\xc8\x42\x10\xc3\xeb"
-    )
-    # Expires on: 2030-01-01
-    EXPIRY = b"\x32\x30\x33\x30\x30\x31\x30\x31"
-
-    return (
-        Tlv(0x30, FASC_N)
-        + Tlv(0x34, os.urandom(16))
-        + Tlv(0x35, EXPIRY)
-        + Tlv(0x3E)
-        + Tlv(TAG_LRC)
-    )
-
-
-def generate_ccc() -> bytes:
-    """Generates a CCC (Card Capability Container)."""
-    return (
-        Tlv(0xF0, b"\xa0\x00\x00\x01\x16\xff\x02" + os.urandom(14))
-        + Tlv(0xF1, b"\x21")
-        + Tlv(0xF2, b"\x21")
-        + Tlv(0xF3)
-        + Tlv(0xF4, b"\x00")
-        + Tlv(0xF5, b"\x10")
-        + Tlv(0xF6)
-        + Tlv(0xF7)
-        + Tlv(0xFA)
-        + Tlv(0xFB)
-        + Tlv(0xFC)
-        + Tlv(0xFD)
-        + Tlv(TAG_LRC)
-    )
-
-
-def get_piv_info(session: PivSession):
-    """Get human readable information about the PIV configuration."""
-    pivman = get_pivman_data(session)
-    info: Dict[str, Any] = {
-        "PIV version": session.version,
-    }
-    lines: List[Any] = [info]
-
-    try:
-        pin_data = session.get_pin_metadata()
-        if pin_data.default_value:
-            lines.append("WARNING: Using default PIN!")
-        tries_str = "%d/%d" % (pin_data.attempts_remaining, pin_data.total_attempts)
-    except NotSupportedError:
-        # Largest possible number of PIN tries to get back is 15
-        tries = session.get_pin_attempts()
-        tries_str = "15 or more" if tries == 15 else str(tries)
-    info["PIN tries remaining"] = tries_str
-    if pivman.puk_blocked:
-        lines.append("PUK is blocked")
-
-    try:
-        metadata = session.get_management_key_metadata()
-        if metadata.default_value:
-            lines.append("WARNING: Using default Management key!")
-        key_type = metadata.key_type
-    except NotSupportedError:
-        key_type = MANAGEMENT_KEY_TYPE.TDES
-    info["Management key algorithm"] = key_type
-
-    if pivman.has_derived_key:
-        lines.append("Management key is derived from PIN.")
-    if pivman.has_stored_key:
-        lines.append("Management key is stored on the YubiKey, protected by PIN.")
-
-    objects: Dict[str, Any] = {}
-    lines.append(objects)
-    try:
-        objects["CHUID"] = session.get_object(OBJECT_ID.CHUID)
-    except ApduError as e:
-        if e.sw == SW.FILE_NOT_FOUND:
-            objects["CHUID"] = "No data available"
-
-    try:
-        objects["CCC"] = session.get_object(OBJECT_ID.CAPABILITY)
-    except ApduError as e:
-        if e.sw == SW.FILE_NOT_FOUND:
-            objects["CCC"] = "No data available"
-
-    for slot, cert in list_certificates(session).items():
-        cert_data: Dict[str, Any] = {}
-        objects[f"Slot {slot:02x}"] = cert_data
-        if cert:
-            try:
-                # Try to read out full DN, fallback to only CN.
-                # Support for DN was added in crytography 2.5
-                subject_dn = cert.subject.rfc4514_string()
-                issuer_dn = cert.issuer.rfc4514_string()
-                print_dn = True
-            except AttributeError:
-                print_dn = False
-                logger.debug("Failed to read DN, falling back to only CNs")
-                cn = cert.subject.get_attributes_for_oid(x509.NameOID.COMMON_NAME)
-                subject_cn = cn[0].value if cn else "None"
-                cn = cert.issuer.get_attributes_for_oid(x509.NameOID.COMMON_NAME)
-                issuer_cn = cn[0].value if cn else "None"
-            except ValueError as e:
-                # Malformed certificates may throw ValueError
-                logger.debug("Failed parsing certificate", exc_info=True)
-                cert_data["Error"] = f"Malformed certificate: {e}"
-                continue
-
-            fingerprint = cert.fingerprint(hashes.SHA256()).hex()
-            try:
-                key_algo = KEY_TYPE.from_public_key(cert.public_key()).name
-            except ValueError:
-                key_algo = "Unsupported"
-            serial = cert.serial_number
-            try:
-                not_before: Optional[datetime] = cert.not_valid_before
-            except ValueError:
-                logger.debug("Failed reading not_valid_before", exc_info=True)
-                not_before = None
-            try:
-                not_after: Optional[datetime] = cert.not_valid_after
-            except ValueError:
-                logger.debug("Failed reading not_valid_after", exc_info=True)
-                not_after = None
-
-            # Print out everything
-            cert_data["Algorithm"] = key_algo
-            if print_dn:
-                cert_data["Subject DN"] = subject_dn
-                cert_data["Issuer DN"] = issuer_dn
-            else:
-                cert_data["Subject CN"] = subject_cn
-                cert_data["Issuer CN"] = issuer_cn
-            cert_data["Serial"] = serial
-            cert_data["Fingerprint"] = fingerprint
-            if not_before:
-                cert_data["Not before"] = not_before.isoformat()
-            if not_after:
-                cert_data["Not after"] = not_after.isoformat()
+    def read_config(self):
+        return self.protocol.send_apdu(0, INS_READ_CONFIG, 0, 0)
+
+    def write_config(self, config):
+        self.protocol.send_apdu(0, INS_WRITE_CONFIG, 0, 0, config)
+
+
+CTAP_VENDOR_FIRST = 0x40
+CTAP_YUBIKEY_DEVICE_CONFIG = CTAP_VENDOR_FIRST
+CTAP_READ_CONFIG = CTAP_VENDOR_FIRST + 2
+CTAP_WRITE_CONFIG = CTAP_VENDOR_FIRST + 3
+
+
+class _ManagementCtapBackend(_Backend):
+    def __init__(self, fido_connection):
+        self.ctap = fido_connection
+        version = fido_connection.device_version
+        if version[0] < 4:  # Prior to YK4 this was not firmware version
+            if not (
+                version[0] == 0 and fido_connection.capabilities & CTAP_CAPABILITY.CBOR
+            ):
+                version = (3, 0, 0)  # Guess that it's a NEO
+        self.version = Version(*version)
+
+    def close(self):
+        self.ctap.close()
+
+    def set_mode(self, data):
+        self.ctap.call(CTAP_YUBIKEY_DEVICE_CONFIG, data)
+
+    def read_config(self):
+        return self.ctap.call(CTAP_READ_CONFIG)
+
+    def write_config(self, config):
+        self.ctap.call(CTAP_WRITE_CONFIG, config)
+
+
+class ManagementSession:
+    def __init__(
+        self, connection: Union[OtpConnection, SmartCardConnection, FidoConnection]
+    ):
+        if isinstance(connection, OtpConnection):
+            self.backend: _Backend = _ManagementOtpBackend(connection)
+        elif isinstance(connection, SmartCardConnection):
+            self.backend = _ManagementSmartCardBackend(connection)
+        elif isinstance(connection, FidoConnection):
+            self.backend = _ManagementCtapBackend(connection)
         else:
-            cert_data["Error"] = "Failed to parse certificate"
+            raise TypeError("Unsupported connection type")
+        logger.debug(
+            "Management session initialized for "
+            f"connection={type(connection).__name__}, version={self.version}"
+        )
 
-    return lines
+    def close(self) -> None:
+        self.backend.close()
 
+    @property
+    def version(self) -> Version:
+        return self.backend.version
 
-def sign_certificate_builder(
-    session: PivSession,
-    slot: SLOT,
-    key_type: KEY_TYPE,
-    builder: x509.CertificateBuilder,
-    hash_algorithm: Type[hashes.HashAlgorithm] = hashes.SHA256,
-) -> x509.Certificate:
-    """Sign a Certificate."""
-    logger.debug("Signing a certificate")
-    dummy_key = _dummy_key(key_type)
-    cert = builder.sign(dummy_key, hash_algorithm(), default_backend())
-
-    sig = session.sign(
-        slot,
-        key_type,
-        cert.tbs_certificate_bytes,
-        hash_algorithm(),
-        padding.PKCS1v15(),  # Only used for RSA
-    )
-
-    seq = Tlv.parse_list(Tlv.unpack(0x30, cert.public_bytes(Encoding.DER)))
-    # Replace signature, add unused bits = 0
-    seq[2] = Tlv(seq[2].tag, b"\0" + sig)
-    # Re-assemble sequence
-    der = Tlv(0x30, b"".join(seq))
-
-    return x509.load_der_x509_certificate(der, default_backend())
-
-
-def sign_csr_builder(
-    session: PivSession,
-    slot: SLOT,
-    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
-    builder: x509.CertificateSigningRequestBuilder,
-    hash_algorithm: Type[hashes.HashAlgorithm] = hashes.SHA256,
-) -> x509.CertificateSigningRequest:
-    """Sign a CSR."""
-    logger.debug("Signing a CSR")
-    key_type = KEY_TYPE.from_public_key(public_key)
-    dummy_key = _dummy_key(key_type)
-    csr = builder.sign(dummy_key, hash_algorithm(), default_backend())
-    seq = Tlv.parse_list(Tlv.unpack(0x30, csr.public_bytes(Encoding.DER)))
-
-    # Replace public key
-    pub_format = (
-        PublicFormat.PKCS1
-        if key_type.algorithm == ALGORITHM.RSA
-        else PublicFormat.SubjectPublicKeyInfo
-    )
-    dummy_bytes = dummy_key.public_key().public_bytes(Encoding.DER, pub_format)
-    pub_bytes = public_key.public_bytes(Encoding.DER, pub_format)
-    seq[0] = Tlv(seq[0].replace(dummy_bytes, pub_bytes))
-
-    sig = session.sign(
-        slot,
-        key_type,
-        seq[0],
-        hash_algorithm(),
-        padding.PKCS1v15(),  # Only used for RSA
-    )
-
-    # Replace signature, add unused bits = 0
-    seq[2] = Tlv(seq[2].tag, b"\0" + sig)
-    # Re-assemble sequence
-    der = Tlv(0x30, b"".join(seq))
-
-    return x509.load_der_x509_csr(der, default_backend())
-
-
-def generate_self_signed_certificate(
-    session: PivSession,
-    slot: SLOT,
-    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
-    subject_str: str,
-    valid_from: datetime,
-    valid_to: datetime,
-    hash_algorithm: Type[hashes.HashAlgorithm] = hashes.SHA256,
-) -> x509.Certificate:
-    """Generate a self-signed certificate using a private key in a slot."""
-    logger.debug("Generating a self-signed certificate")
-    key_type = KEY_TYPE.from_public_key(public_key)
-
-    subject = parse_rfc4514_string(subject_str)
-    builder = (
-        x509.CertificateBuilder()
-        .public_key(public_key)
-        .subject_name(subject)
-        .issuer_name(subject)  # Same as subject on self-signed certificate.
-        .serial_number(x509.random_serial_number())
-        .not_valid_before(valid_from)
-        .not_valid_after(valid_to)
-    )
-
-    return sign_certificate_builder(session, slot, key_type, builder, hash_algorithm)
-
-
-def generate_csr(
-    session: PivSession,
-    slot: SLOT,
-    public_key: Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey],
-    subject_str: str,
-    hash_algorithm: Type[hashes.HashAlgorithm] = hashes.SHA256,
-) -> x509.CertificateSigningRequest:
-    """Generate a CSR using a private key in a slot."""
-    logger.debug("Generating a CSR")
-    builder = x509.CertificateSigningRequestBuilder().subject_name(
-        parse_rfc4514_string(subject_str)
-    )
+    def read_device_info(self) -> DeviceInfo:
+        require_version(self.version, (4, 1, 0))
+        return DeviceInfo.parse(self.backend.read_config(), self.version)
+
+    def write_device_config(
+        self,
+        config: Optional[DeviceConfig] = None,
+        reboot: bool = False,
+        cur_lock_code: Optional[bytes] = None,
+        new_lock_code: Optional[bytes] = None,
+    ) -> None:
+        require_version(self.version, (5, 0, 0))
+        if cur_lock_code is not None and len(cur_lock_code) != 16:
+            raise ValueError("Lock code must be 16 bytes")
+        if new_lock_code is not None and len(new_lock_code) != 16:
+            raise ValueError("Lock code must be 16 bytes")
+        config = config or DeviceConfig({}, None, None, None)
+        logger.debug(
+            f"Writing device config: {config}, reboot: {reboot}, "
+            f"current lock code: {cur_lock_code is not None}, "
+            f"new lock code: {new_lock_code is not None}"
+        )
+        self.backend.write_config(
+            config.get_bytes(reboot, cur_lock_code, new_lock_code)
+        )
+        logger.info("Device config written")
 
-    return sign_csr_builder(session, slot, public_key, builder, hash_algorithm)
+    def set_mode(
+        self,
+        mode: Mode,
+        chalresp_timeout: int = 0,
+        auto_eject_timeout: Optional[int] = None,
+    ) -> None:
+        logger.debug(
+            f"Set mode: {mode}, chalresp_timeout: {chalresp_timeout}, "
+            f"auto_eject_timeout: {auto_eject_timeout}"
+        )
+        if self.version >= (5, 0, 0):
+            # Translate into DeviceConfig
+            usb_enabled = CAPABILITY(0)
+            if USB_INTERFACE.OTP in mode.interfaces:
+                usb_enabled |= CAPABILITY.OTP
+            if USB_INTERFACE.CCID in mode.interfaces:
+                usb_enabled |= CAPABILITY.OATH | CAPABILITY.PIV | CAPABILITY.OPENPGP
+            if USB_INTERFACE.FIDO in mode.interfaces:
+                usb_enabled |= CAPABILITY.U2F | CAPABILITY.FIDO2
+            logger.debug(f"Delegating to DeviceConfig with usb_enabled: {usb_enabled}")
+            # N.B: reboot=False, since we're using the older set_mode command
+            self.write_device_config(
+                DeviceConfig(
+                    {TRANSPORT.USB: usb_enabled},
+                    auto_eject_timeout,
+                    chalresp_timeout,
+                    None,
+                )
+            )
+        else:
+            code = mode.code
+            if auto_eject_timeout is not None:
+                if mode.interfaces == USB_INTERFACE.CCID:
+                    code |= DEVICE_FLAG.EJECT
+                else:
+                    raise ValueError("Touch-eject only applicable for mode: CCID")
+            self.backend.set_mode(
+                # N.B. This is little endian!
+                struct.pack("<BBH", code, chalresp_timeout, auto_eject_timeout or 0)
+            )
+            logger.info("Mode configuration written")
```

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/__init__.py` & `yubikey_manager-5.1.0/ykman/scancodes/__init__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/bepo.py` & `yubikey_manager-5.1.0/ykman/scancodes/bepo.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/de.py` & `yubikey_manager-5.1.0/ykman/scancodes/de.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/fr.py` & `yubikey_manager-5.1.0/ykman/scancodes/fr.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/it.py` & `yubikey_manager-5.1.0/ykman/scancodes/it.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/modhex.py` & `yubikey_manager-5.1.0/ykman/scancodes/modhex.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/norman.py` & `yubikey_manager-5.1.0/ykman/scancodes/norman.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/uk.py` & `yubikey_manager-5.1.0/ykman/scancodes/uk.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scancodes/us.py` & `yubikey_manager-5.1.0/ykman/scancodes/us.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/scripting.py` & `yubikey_manager-5.1.0/ykman/scripting.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/settings.py` & `yubikey_manager-5.1.0/ykman/settings.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/ykman/util.py` & `yubikey_manager-5.1.0/ykman/util.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/__init__.py` & `yubikey_manager-5.1.0/ykman/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020 Yubico AB
+# Copyright (c) 2015 Yubico AB
 # All rights reserved.
 #
 #   Redistribution and use in source and binary forms, with or
 #   without modification, are permitted provided that the following
 #   conditions are met:
 #
 #    1. Redistributions of source code must retain the above copyright
@@ -20,7 +20,9 @@
 # INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
+
+__version__ = "5.1.0"
```

### Comparing `yubikey_manager-5.0.1/yubikit/core/__init__.py` & `yubikey_manager-5.1.0/yubikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/core/fido.py` & `yubikey_manager-5.1.0/yubikit/core/fido.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/core/otp.py` & `yubikey_manager-5.1.0/yubikit/core/otp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/core/smartcard.py` & `yubikey_manager-5.1.0/yubikit/core/smartcard.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,20 +116,26 @@
 
 INS_SEND_REMAINING = 0xC0
 SW1_HAS_MORE_DATA = 0x61
 
 SHORT_APDU_MAX_CHUNK = 0xFF
 
 
-def _encode_short_apdu(cla, ins, p1, p2, data):
-    return struct.pack(">BBBBB", cla, ins, p1, p2, len(data)) + data
+def _encode_short_apdu(cla, ins, p1, p2, data, le=0):
+    buf = struct.pack(">BBBBB", cla, ins, p1, p2, len(data)) + data
+    if le:
+        buf += struct.pack(">B", le)
+    return buf
 
 
-def _encode_extended_apdu(cla, ins, p1, p2, data):
-    return struct.pack(">BBBBBH", cla, ins, p1, p2, 0, len(data)) + data
+def _encode_extended_apdu(cla, ins, p1, p2, data, le=0):
+    buf = struct.pack(">BBBBBH", cla, ins, p1, p2, 0, len(data)) + data
+    if le:
+        buf += struct.pack(">H", le)
+    return buf
 
 
 class SmartCardProtocol:
     def __init__(
         self,
         smartcard_connection: SmartCardConnection,
         ins_send_remaining: int = INS_SEND_REMAINING,
@@ -159,15 +165,15 @@
                 SW.INVALID_INSTRUCTION,
                 SW.WRONG_PARAMETERS_P1P2,
             ):
                 raise ApplicationNotAvailableError()
             raise
 
     def send_apdu(
-        self, cla: int, ins: int, p1: int, p2: int, data: bytes = b""
+        self, cla: int, ins: int, p1: int, p2: int, data: bytes = b"", le: int = 0
     ) -> bytes:
         if (
             self._touch_workaround
             and self._last_long_resp > 0
             and time() - self._last_long_resp < 2
         ):
             logger.debug("Sending dummy APDU as touch workaround")
@@ -176,25 +182,25 @@
             )  # Dummy APDU, returns error
             self._last_long_resp = 0
 
         if self.apdu_format is ApduFormat.SHORT:
             while len(data) > SHORT_APDU_MAX_CHUNK:
                 chunk, data = data[:SHORT_APDU_MAX_CHUNK], data[SHORT_APDU_MAX_CHUNK:]
                 response, sw = self.connection.send_and_receive(
-                    _encode_short_apdu(0x10 | cla, ins, p1, p2, chunk)
+                    _encode_short_apdu(0x10 | cla, ins, p1, p2, chunk, le)
                 )
                 if sw != SW.OK:
                     raise ApduError(response, sw)
             response, sw = self.connection.send_and_receive(
-                _encode_short_apdu(cla, ins, p1, p2, data)
+                _encode_short_apdu(cla, ins, p1, p2, data, le)
             )
             get_data = _encode_short_apdu(0, self._ins_send_remaining, 0, 0, b"")
         elif self.apdu_format is ApduFormat.EXTENDED:
             response, sw = self.connection.send_and_receive(
-                _encode_extended_apdu(cla, ins, p1, p2, data)
+                _encode_extended_apdu(cla, ins, p1, p2, data, le)
             )
             get_data = _encode_extended_apdu(0, self._ins_send_remaining, 0, 0, b"")
         else:
             raise TypeError("Invalid ApduFormat set")
 
         # Read chained response
         buf = b""
```

### Comparing `yubikey_manager-5.0.1/yubikit/logging.py` & `yubikey_manager-5.1.0/yubikit/logging.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/oath.py` & `yubikey_manager-5.1.0/yubikit/oath.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/yubikit/piv.py` & `yubikey_manager-5.1.0/yubikit/piv.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.constant_time import bytes_eq
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from cryptography.hazmat.primitives.asymmetric import rsa, ec
 from cryptography.hazmat.primitives.asymmetric.padding import AsymmetricPadding
+from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
 from cryptography.hazmat.backends import default_backend
 
 from dataclasses import dataclass
 from enum import Enum, IntEnum, unique
 from typing import Optional, Union, Type, cast
 
 import logging
@@ -172,14 +173,17 @@
     RETIRED17 = 0x92
     RETIRED18 = 0x93
     RETIRED19 = 0x94
     RETIRED20 = 0x95
 
     ATTESTATION = 0xF9
 
+    def __str__(self) -> str:
+        return f"{self:02X} ({self.name})"
+
 
 @unique
 class OBJECT_ID(IntEnum):
     CAPABILITY = 0x5FC107
     CHUID = 0x5FC102
     AUTHENTICATION = 0x5FC105  # cert for 9a key
     FINGERPRINTS = 0x5FC103
@@ -349,17 +353,20 @@
     @property
     def public_key(self):
         return _parse_device_public_key(self.key_type, self.public_key_encoded)
 
 
 def _pad_message(key_type, message, hash_algorithm, padding):
     if key_type.algorithm == ALGORITHM.EC:
-        h = hashes.Hash(hash_algorithm, default_backend())
-        h.update(message)
-        hashed = h.finalize()
+        if isinstance(hash_algorithm, Prehashed):
+            hashed = message
+        else:
+            h = hashes.Hash(hash_algorithm, default_backend())
+            h.update(message)
+            hashed = h.finalize()
         byte_len = key_type.bit_len // 8
         if len(hashed) < byte_len:
             return hashed.rjust(byte_len // 8, b"\0")
         return hashed[:byte_len]
     elif key_type.algorithm == ALGORITHM.RSA:
         # Sign with a dummy key, then encrypt the signature to get the padded message
         e = 65537
```

### Comparing `yubikey_manager-5.0.1/yubikit/support.py` & `yubikey_manager-5.1.0/yubikit/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,24 +364,28 @@
             return True
     return False
 
 
 def get_name(info: DeviceInfo, key_type: Optional[YUBIKEY]) -> str:
     """Determine the product name of a YubiKey"""
     usb_supported = info.supported_capabilities[TRANSPORT.USB]
+
+    # Guess the key type (over NFC)
     if not key_type:
-        if info.serial is None and _fido_only(usb_supported):
-            key_type = YUBIKEY.SKY
-        elif info.version[0] == 3:
+        if info.version[0] == 3:
             key_type = YUBIKEY.NEO
+        elif info.serial is None and _fido_only(usb_supported):
+            key_type = YUBIKEY.SKY if info.version < (5, 2, 8) else YUBIKEY.YK4
         else:
             key_type = YUBIKEY.YK4
 
+    # Generic name based on key type alone
     device_name = key_type.value
 
+    # Improved name based on configuration
     if key_type == YUBIKEY.SKY:
         if CAPABILITY.FIDO2 not in usb_supported:
             device_name = "FIDO U2F Security Key"  # SKY 1
         if info.has_transport(TRANSPORT.NFC):
             device_name = "Security Key NFC"
     elif key_type == YUBIKEY.YK4:
         major_version = info.version[0]
@@ -397,14 +401,15 @@
                 device_name = "YubiKey Edge"
             else:
                 device_name = "YubiKey 4"
 
         if _is_preview(info.version):
             device_name = "YubiKey Preview"
         elif info.version >= (5, 1, 0):
+            # Dynamic name building for YK5
             is_nano = info.form_factor in (
                 FORM_FACTOR.USB_A_NANO,
                 FORM_FACTOR.USB_C_NANO,
             )
             is_bio = info.form_factor in (FORM_FACTOR.USB_A_BIO, FORM_FACTOR.USB_C_BIO)
             is_c = info.form_factor in (  # Does NOT include Ci
                 FORM_FACTOR.USB_C_KEYCHAIN,
```

### Comparing `yubikey_manager-5.0.1/yubikit/yubiotp.py` & `yubikey_manager-5.1.0/yubikit/yubiotp.py`

 * *Files identical despite different names*

### Comparing `yubikey_manager-5.0.1/PKG-INFO` & `yubikey_manager-5.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yubikey-manager
-Version: 5.0.1
+Version: 5.1.0
 Summary: Tool for managing your YubiKey configuration.
 Home-page: https://github.com/Yubico/yubikey-manager
 License: BSD
 Keywords: yubikey,yubiotp,piv,fido
 Author: Dain Nilsson
 Author-email: dain@yubico.com
 Requires-Python: >=3.7,<4.0
@@ -16,13 +16,13 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: cryptography (>=3.0,<42)
+Requires-Dist: cryptography (>=3.0,<43)
 Requires-Dist: fido2 (>=1.0,<2.0)
 Requires-Dist: keyring (>=23.4,<24.0)
 Requires-Dist: pyscard (>=2.0,<3.0)
-Requires-Dist: pywin32 (>=223); sys_platform == "win32"
+Requires-Dist: pywin32 (>=223) ; sys_platform == "win32"
 Project-URL: Repository, https://github.com/Yubico/yubikey-manager
```

