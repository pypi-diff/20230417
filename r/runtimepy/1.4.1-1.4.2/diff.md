# Comparing `tmp/runtimepy-1.4.1.tar.gz` & `tmp/runtimepy-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.4.1.tar", last modified: Thu Apr 13 23:39:06 2023, max compression
+gzip compressed data, was "runtimepy-1.4.2.tar", last modified: Mon Apr 17 17:53:00 2023, max compression
```

## Comparing `runtimepy-1.4.1.tar` & `runtimepy-1.4.2.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 23:37:43.000000 runtimepy-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 23:39:06.059302 runtimepy-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-13 23:37:43.000000 runtimepy-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 23:37:43.000000 runtimepy-1.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.039302 runtimepy-1.4.1/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.031303 runtimepy-1.4.1/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.047303 runtimepy-1.4.1/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.051303 runtimepy-1.4.1/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.055302 runtimepy-1.4.1/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 23:37:43.000000 runtimepy-1.4.1/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.043302 runtimepy-1.4.1/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 23:39:06.000000 runtimepy-1.4.1/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:39:06.059302 runtimepy-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 23:37:43.000000 runtimepy-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:39:06.059302 runtimepy-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 23:37:43.000000 runtimepy-1.4.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 17:50:50.000000 runtimepy-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-17 17:53:00.284329 runtimepy-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-17 17:50:50.000000 runtimepy-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 17:50:50.000000 runtimepy-1.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.264329 runtimepy-1.4.2/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.268329 runtimepy-1.4.2/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.268329 runtimepy-1.4.2/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.268329 runtimepy-1.4.2/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.268329 runtimepy-1.4.2/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.272329 runtimepy-1.4.2/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.260329 runtimepy-1.4.2/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.272329 runtimepy-1.4.2/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.272329 runtimepy-1.4.2/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.272329 runtimepy-1.4.2/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/mixins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.276329 runtimepy-1.4.2/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.280329 runtimepy-1.4.2/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/task/basic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 17:50:50.000000 runtimepy-1.4.2/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.268329 runtimepy-1.4.2/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 17:53:00.000000 runtimepy-1.4.2/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:53:00.284329 runtimepy-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 17:50:50.000000 runtimepy-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:53:00.284329 runtimepy-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-17 17:50:50.000000 runtimepy-1.4.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-17 17:50:50.000000 runtimepy-1.4.2/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 17:50:50.000000 runtimepy-1.4.2/tests/test_resources.py
```

### Comparing `runtimepy-1.4.1/LICENSE` & `runtimepy-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/PKG-INFO` & `runtimepy-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.4.1
+Version: 1.4.2
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
+    hash=36f9aec8c2e9ae7d8015f17f7164d382
     =====================================
 -->
 
-# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.2](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.1/README.md` & `runtimepy-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
+    hash=36f9aec8c2e9ae7d8015f17f7164d382
     =====================================
 -->
 
-# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.2](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.1/pyproject.toml` & `runtimepy-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.4.1"
+version = "1.4.2"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.4.1/runtimepy/app.py` & `runtimepy-1.4.2/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/__init__.py` & `runtimepy-1.4.2/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/__init__.py` & `runtimepy-1.4.2/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/array.py` & `runtimepy-1.4.2/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/base.py` & `runtimepy-1.4.2/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/create.py` & `runtimepy-1.4.2/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/file.py` & `runtimepy-1.4.2/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/environment/names.py` & `runtimepy-1.4.2/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/channel/registry.py` & `runtimepy-1.4.2/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/codec/protocol/base.py` & `runtimepy-1.4.2/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/codec/protocol/json.py` & `runtimepy-1.4.2/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/commands/all.py` & `runtimepy-1.4.2/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/commands/arbiter.py` & `runtimepy-1.4.2/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/commands/tui.py` & `runtimepy-1.4.2/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.4.2/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.4.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,22 @@
       $ref: package://runtimepy/schemas/ClientConnectionConfig.yaml
 
   servers:
     type: array
     items:
       $ref: package://runtimepy/schemas/ServerConnectionConfig.yaml
 
+  # Runtime application or applications.
+  # defaults to: "runtimepy.net.apps.init_only"
   app:
-    # This is the default application.
-    # default: "runtimepy.net.apps.init_only"
-    type: string
+    oneOf:
+      - type: string
+      - type: array
+        items:
+          type: string
 
   # Application configuration data.
   config:
     type: object
 
   # A 'site' directory to add for discovering modules that may appear in other
   # parts of the configuration. If this isn't specified, the current directory
```

### Comparing `runtimepy-1.4.1/runtimepy/entry.py` & `runtimepy-1.4.2/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/enum/__init__.py` & `runtimepy-1.4.2/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/enum/registry.py` & `runtimepy-1.4.2/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/enum/type.py` & `runtimepy-1.4.2/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/mapping.py` & `runtimepy-1.4.2/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/mixins/enum.py` & `runtimepy-1.4.2/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/mixins/regex.py` & `runtimepy-1.4.2/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/__init__.py` & `runtimepy-1.4.2/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/base.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,36 +35,51 @@
     stack: _AsyncExitStack
     connections: ConnectionMap
     stop: _asyncio.Event
     config: _JsonObject
 
 
 NetworkApplication = _Callable[[AppInfo], _Awaitable[int]]
+NetworkApplicationlike = _Union[NetworkApplication, _List[NetworkApplication]]
 ServerTask = _Awaitable[None]
 
 
 async def init_only(app: AppInfo) -> int:
     """A network application that doesn't do anything."""
 
     del app
     return 0
 
 
+def normalize_app(
+    app: NetworkApplicationlike = None,
+) -> _List[NetworkApplication]:
+    """
+    Normalize some application parameter into a list of network applications.
+    """
+
+    if app is None:
+        app = [init_only]
+    elif not isinstance(app, list):
+        app = [app]
+    return app
+
+
 class BaseConnectionArbiter(_NamespaceMixin, _LoggerMixin):
     """
     A class implementing a base connection-manager for a broader application.
     """
 
     def __init__(
         self,
         manager: _ConnectionManager = None,
         stop_sig: _asyncio.Event = None,
         namespace: _Namespace = None,
         logger: _LoggerType = None,
-        app: NetworkApplication = init_only,
+        app: NetworkApplicationlike = None,
         config: _JsonObject = None,
     ) -> None:
         """Initialize this connection arbiter."""
 
         _LoggerMixin.__init__(self, logger=logger)
 
         if manager is None:
@@ -75,15 +90,15 @@
             stop_sig = _asyncio.Event()
         self.stop_sig = stop_sig
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
         # A fallback application. Set a class attribute so this can be more
         # easily externally updated.
-        self._app = app
+        self._apps: _List[NetworkApplication] = normalize_app(app)
 
         # Application configuration data.
         if config is None:
             config = {}
         self._config = config
 
         # Keep track of connection objects.
@@ -132,15 +147,15 @@
 
             result = True
 
         return result
 
     async def _entry(
         self,
-        app: NetworkApplication = None,
+        app: NetworkApplicationlike = None,
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """
         Ensures connections are given a chance to initialize, run the
         application, clean up connections and return the application's result.
         """
@@ -170,56 +185,66 @@
             # still alive after initialization.
             if not check_connections or not any(
                 x.disabled for x in self._connections.values()
             ):
                 async with _AsyncExitStack() as stack:
                     self.logger.info("Application starting.")
 
-                    if app is None:
-                        app = self._app
-
-                    result = await app(
-                        AppInfo(
-                            stack,
-                            self._connections,
-                            self.stop_sig,
-                            config if config is not None else self._config,
-                        )
+                    info = AppInfo(
+                        stack,
+                        self._connections,
+                        self.stop_sig,
+                        config if config is not None else self._config,
                     )
-                    self.logger.info("Application returned %d.", result)
+
+                    # Get application methods.
+                    apps = self._apps
+                    if app is not None:
+                        apps = normalize_app(app)
+
+                    result = 0
+                    for curr_app in apps:
+                        if result == 0:
+                            result = await curr_app(info)
+
+                            self.logger.info(
+                                "Application '%s' returned %d.",
+                                curr_app.__name__,
+                                result,
+                            )
 
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
             self.stop_sig.set()
 
         return result
 
     async def app(
         self,
-        app: NetworkApplication = None,
+        app: NetworkApplicationlike = None,
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """
         Run the application alongside the connection manager and server tasks.
         """
 
         result = await _asyncio.gather(
             self._entry(
-                app, check_connections=check_connections, config=config
+                app=app, check_connections=check_connections, config=config
             ),
             self.manager.manage(self.stop_sig),
             *self._servers,
         )
         return int(result[0])
 
     def run(
         self,
-        app: NetworkApplication = None,
+        app: NetworkApplicationlike = None,
         eloop: _asyncio.AbstractEventLoop = None,
         signals: _Iterable[int] = None,
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """Run the application until the stop signal is set."""
```

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/config.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/factory.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/factory.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/imports.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 A module extending capability of the connection arbiter using Python import
 machinery.
 """
 
 # built-in
 from importlib import import_module as _import_module
+from typing import List as _List
 from typing import Tuple as _Tuple
+from typing import Union as _Union
 
 # internal
 from runtimepy.net.arbiter.factory import (
     FactoryConnectionArbiter as _FactoryConnectionArbiter,
 )
 
 
@@ -28,21 +30,29 @@
 
 class ImportConnectionArbiter(_FactoryConnectionArbiter):
     """
     A class implementing extensions to the connection arbiter for working with
     arbitrary Python modules.
     """
 
-    def set_app(self, module_path: str) -> None:
+    def set_app(self, module_path: _Union[str, _List[str]]) -> None:
         """
         Attempt to update the application method from the provided string.
         """
 
-        module, app = import_str_and_item(module_path)
-        self._app = getattr(_import_module(module), app)
+        if isinstance(module_path, str):
+            module_path = [module_path]
+
+        # Load all application methods.
+        apps = []
+        for path in module_path:
+            module, app = import_str_and_item(path)
+            apps.append(getattr(_import_module(module), app))
+
+        self._apps = apps
 
     def register_module_factory(
         self, module_path: str, *namespaces: str, **kwargs
     ) -> bool:
         """Attempt to register a factory class based on its module path."""
 
         module, factory_class = import_str_and_item(module_path)
```

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/udp.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.4.2/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/connection.py` & `runtimepy-1.4.2/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/factories/__init__.py` & `runtimepy-1.4.2/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/manager.py` & `runtimepy-1.4.2/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/mixin.py` & `runtimepy-1.4.2/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/tcp/connection.py` & `runtimepy-1.4.2/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.4.2/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.4.2/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/udp/connection.py` & `runtimepy-1.4.2/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/util.py` & `runtimepy-1.4.2/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/net/websocket/connection.py` & `runtimepy-1.4.2/runtimepy/net/websocket/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 """
 
 from __future__ import annotations
 
 # built-in
 import asyncio as _asyncio
 from contextlib import asynccontextmanager as _asynccontextmanager
+from contextlib import suppress as _suppress
 from logging import getLogger as _getLogger
 from typing import AsyncIterator as _AsyncIterator
 from typing import Awaitable as _Awaitable
 from typing import Callable as _Callable
 from typing import Optional as _Optional
 from typing import Tuple as _Tuple
 from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # third-party
+from vcorelib.asyncio import log_exceptions as _log_exceptions
 import websockets
 from websockets.client import (
     WebSocketClientProtocol as _WebSocketClientProtocol,
 )
 from websockets.exceptions import ConnectionClosed as _ConnectionClosed
 from websockets.server import (
     WebSocketServerProtocol as _WebSocketServerProtocol,
@@ -105,14 +107,15 @@
         """
         A wrapper for passing in a websocket handler and initializing a
         connection.
         """
 
         async def _handler(protocol: _WebSocketServerProtocol) -> None:
             """A handler that runs the callers initialization function."""
+
             conn = cls(protocol)
             if init is None or await init(conn):
                 if manager is not None:
                     # Allow the connection manager to process this connection.
                     await manager.queue.put(conn)
 
                     # Wait for either the connection to be disabled, or for
@@ -123,17 +126,21 @@
 
                     # Wait for the event and cancel the task that didn't
                     # complete.
                     _, pending = await _asyncio.wait(
                         tasks,
                         return_when=_asyncio.FIRST_COMPLETED,
                     )
+
+                    # Cleaning up tasks is always a nightmare.
                     for task in pending:
                         task.cancel()
-                        await task
+                        with _suppress(_asyncio.CancelledError):
+                            await task
+                    _log_exceptions(pending, logger=conn.logger)
 
                 # If there's no connection manager, just process the
                 # connection here.
                 else:
                     await conn.process(stop_sig=stop_sig)
 
         return _handler
```

### Comparing `runtimepy-1.4.1/runtimepy/primitives/__init__.py` & `runtimepy-1.4.2/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/array.py` & `runtimepy-1.4.2/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/base.py` & `runtimepy-1.4.2/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/bool.py` & `runtimepy-1.4.2/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/byte_order.py` & `runtimepy-1.4.2/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/field/__init__.py` & `runtimepy-1.4.2/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/field/fields.py` & `runtimepy-1.4.2/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.4.2/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.4.2/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/float.py` & `runtimepy-1.4.2/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/int.py` & `runtimepy-1.4.2/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/string.py` & `runtimepy-1.4.2/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/type/__init__.py` & `runtimepy-1.4.2/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/type/base.py` & `runtimepy-1.4.2/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/type/float.py` & `runtimepy-1.4.2/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/primitives/type/int.py` & `runtimepy-1.4.2/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/registry/__init__.py` & `runtimepy-1.4.2/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/registry/bool.py` & `runtimepy-1.4.2/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/registry/item.py` & `runtimepy-1.4.2/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/registry/name.py` & `runtimepy-1.4.2/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/schemas.py` & `runtimepy-1.4.2/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/task/__init__.py` & `runtimepy-1.4.2/runtimepy/task/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/task/basic/__init__.py` & `runtimepy-1.4.2/runtimepy/task/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/tui/channels/__init__.py` & `runtimepy-1.4.2/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy/tui/task.py` & `runtimepy-1.4.2/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.4.2/runtimepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.4.1
+Version: 1.4.2
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1b0b047c6997f2915a3cf8fe7fc78ee4
+    hash=36f9aec8c2e9ae7d8015f17f7164d382
     =====================================
 -->
 
-# runtimepy ([1.4.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.4.2](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.4.1/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.4.2/runtimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/setup.py` & `runtimepy-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/tests/test_entry.py` & `runtimepy-1.4.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.4.1/tests/test_mapping.py` & `runtimepy-1.4.2/tests/test_mapping.py`

 * *Files identical despite different names*

