# Comparing `tmp/oar-docker-1.6.3.dev0.tar.gz` & `tmp/oar-docker-1.6.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oar-docker-1.6.3.dev0.tar", last modified: Thu Jan  6 16:33:48 2022, max compression
+gzip compressed data, was "dist/oar-docker-1.6.4.dev0.tar", last modified: Mon Apr 17 14:58:14 2023, max compression
```

## Comparing `oar-docker-1.6.3.dev0.tar` & `oar-docker-1.6.4.dev0.tar`

### file list

```diff
@@ -1,240 +1,256 @@
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     8531 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/SOURCES.txt
--rw-r--r--   0 neyron    (1000) neyron    (1000)       10 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/top_level.txt
--rw-r--r--   0 neyron    (1000) neyron    (1000)       68 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/entry_points.txt
--rw-r--r--   0 neyron    (1000) neyron    (1000)        1 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/dependency_links.txt
--rw-r--r--   0 neyron    (1000) neyron    (1000)        1 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/not-zip-safe
--rw-r--r--   0 neyron    (1000) neyron    (1000)    22521 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/PKG-INFO
--rw-r--r--   0 neyron    (1000) neyron    (1000)       31 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oar_docker.egg-info/requires.txt
--rw-r--r--   0 neyron    (1000) neyron    (1000)       71 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/MANIFEST.in
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     4544 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/client.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     6708 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/utils.py
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/base/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1589 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/base/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      766 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1355 2019-10-11 15:50:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/systemd/oardocker-postgresql@9.6-main.service
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      322 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/frontend/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     7183 2020-03-31 16:17:40.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/frontend/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1103 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/frontend/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      569 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/node/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/create_resources.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/create_queues.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/mount_cow_volumes.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/prepare_oar_cgroup.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/oar_server.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/systemd-spawn-fcgi.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/configure_oar_ssh_keys.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/config/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     3893 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/config/sshd_config
--rw-r--r--   0 neyron    (1000) neyron    (1000)      250 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/config/rsyslog.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)      181 2019-10-11 15:50:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/config/tmpfiles_oardocker.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/custom_setup.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1031 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/split_ssh_pane
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      766 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/wait_ssh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)       64 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/exec_in_container
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1124 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/wait_pgsql
--rw-r--r--   0 neyron    (1000) neyron    (1000)      627 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/generate_ssh_keys.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)      305 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/create_users.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      233 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-ssh-keys.service
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      249 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-fix-mount.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      206 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker.target
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      237 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-mount-cow.service
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      231 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-sshd@.service
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      177 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-sshd.socket
--rw-r--r--   0 neyron    (1000) neyron    (1000)      197 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/systemd/oardocker-rsyslog.service
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      566 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/container-init
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)    17506 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/ps_mem
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      832 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/setuser
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     6477 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/custom_setup.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      422 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/systemd/oardocker-resources.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      395 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/systemd/oardocker-postgresql.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      264 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/systemd/oardocker-server.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      413 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/systemd/oardocker-queues.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/.gitignore
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/sbin/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      185 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/sbin/taillogs
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      271 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/sbin/oar_server_cmd
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/rsyslog/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/rsyslog/config/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      387 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/rsyslog/config/rsyslog.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/rsyslog/custom_setup.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     2148 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/nginx-default-site.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)      498 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/php5.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1867 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/nginx.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1462 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/motd
--rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/custom_setup.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      178 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.socket
--rw-r--r--   0 neyron    (1000) neyron    (1000)      109 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-nginx.socket
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oar-node.service.d/
--rw-r--r--   0 neyron    (1000) neyron    (1000)       36 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oar-node.service.d/override.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)      212 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      228 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-php.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      222 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-frontend.target
--rw-r--r--   0 neyron    (1000) neyron    (1000)      381 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-nginx.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)      162 2018-01-22 08:24:36.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-php.socket
--rw-r--r--   0 neyron    (1000) neyron    (1000)      599 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-apache.service
--rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/.gitignore
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     3244 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/custom_setup.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      340 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/systemd/oardocker-cgroup.service
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/systemd/oar-node.service.d/
--rw-r--r--   0 neyron    (1000) neyron    (1000)       36 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/systemd/oar-node.service.d/override.conf
--rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/.gitignore
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/base/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1567 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/base/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      766 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1650 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/systemd/oardocker-postgresql@13-main.service
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      323 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/frontend/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     7589 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/frontend/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1519 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/frontend/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      548 2022-01-06 16:12:28.000000 oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/node/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/base/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1589 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/base/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      756 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/server/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      321 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/frontend/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     7183 2020-03-31 16:17:58.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/frontend/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)      917 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/frontend/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      568 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/node/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      520 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/create_resources.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/create_queues.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/mount_cow_volumes.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/prepare_oar_cgroup.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/oar_server.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/systemd-spawn-fcgi.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/configure_oar_ssh_keys.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      572 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/server/configure_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)      692 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/server/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      194 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/frontend/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      582 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/frontend/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      191 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/node/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      634 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      282 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/server/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)      484 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/server/install_cigri.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      195 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      629 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1327 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/init_cigri.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)      257 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/start_cigri.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1564 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/install_cigri.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      269 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/node/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)       64 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/node/install_cigri.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)     2416 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/cigri/README.md
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      559 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/create_resources.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/create_queues.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/mount_cow_volumes.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/prepare_oar_cgroup.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/oar_server.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/systemd-spawn-fcgi.sh
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/configure_oar_ssh_keys.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      568 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/oarswitch-cli
--rw-r--r--   0 neyron    (1000) neyron    (1000)      849 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1880 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/configure_oar3.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      196 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)      568 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/oarswitch-cli
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1220 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)      480 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/configure_oar3.sh
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      193 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/node/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/manifest.json
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/base/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1567 2021-03-23 11:02:05.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/base/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      764 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/systemd/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1650 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/systemd/oardocker-postgresql@11-main.service
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/rsyslog/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      321 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/rsyslog/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/frontend/
--rwxr-xr-x   0 neyron    (1000) neyron    (1000)     7589 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/frontend/install_oar.sh
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1517 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/frontend/Dockerfile
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/node/
--rw-r--r--   0 neyron    (1000) neyron    (1000)      546 2021-10-21 08:22:39.000000 oar-docker-1.6.3.dev0/oardocker/templates/buster/images/node/Dockerfile
--rw-r--r--   0 neyron    (1000) neyron    (1000)     2306 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/cli.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     3130 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/state.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)    14903 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/actions.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     6356 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/context.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     2046 2021-10-21 08:13:13.000000 oar-docker-1.6.3.dev0/oardocker/compat.py
-drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/oardocker/commands/
--rw-r--r--   0 neyron    (1000) neyron    (1000)     3147 2020-03-30 22:24:45.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_start.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)      584 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_install.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1334 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_stop.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)      999 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_reset.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1833 2020-03-06 16:29:10.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_init.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)      757 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_exec.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     3532 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_logs.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1025 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_clean.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1862 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_status.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)      630 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_destroy.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     4133 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_build.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)      713 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/commands/cmd_connect.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)        0 2017-11-03 12:49:35.000000 oar-docker-1.6.3.dev0/oardocker/commands/__init__.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)       45 2021-10-21 08:58:26.000000 oar-docker-1.6.3.dev0/oardocker/__init__.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     7145 2019-10-02 19:59:09.000000 oar-docker-1.6.3.dev0/oardocker/container.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)       38 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/setup.cfg
--rw-r--r--   0 neyron    (1000) neyron    (1000)     1058 2021-10-21 08:13:13.000000 oar-docker-1.6.3.dev0/setup.py
--rw-r--r--   0 neyron    (1000) neyron    (1000)     6655 2020-03-30 23:48:41.000000 oar-docker-1.6.3.dev0/README.rst
--rw-r--r--   0 neyron    (1000) neyron    (1000)    10711 2021-10-21 08:58:25.000000 oar-docker-1.6.3.dev0/CHANGES.rst
--rw-r--r--   0 neyron    (1000) neyron    (1000)    22521 2022-01-06 16:33:48.000000 oar-docker-1.6.3.dev0/PKG-INFO
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     8924 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       10 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/top_level.txt
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       68 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/entry_points.txt
+-rw-r--r--   0 neyron    (1000) neyron    (1000)        1 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 neyron    (1000) neyron    (1000)        1 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/not-zip-safe
+-rw-r--r--   0 neyron    (1000) neyron    (1000)    23470 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/PKG-INFO
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       31 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oar_docker.egg-info/requires.txt
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       71 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/MANIFEST.in
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     4544 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/client.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     6708 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/utils.py
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/base/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1589 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/base/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      766 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1355 2019-10-11 15:50:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/systemd/oardocker-postgresql@9.6-main.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      322 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1103 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      569 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/create_resources.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/create_queues.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/mount_cow_volumes.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/prepare_oar_cgroup.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/oar_server.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/systemd-spawn-fcgi.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/configure_oar_ssh_keys.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/config/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     3893 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/config/sshd_config
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      250 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/config/rsyslog.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      181 2019-10-11 15:50:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/config/tmpfiles_oardocker.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/custom_setup.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1031 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/split_ssh_pane
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      766 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/wait_ssh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)       64 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/exec_in_container
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1124 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/wait_pgsql
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      627 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/generate_ssh_keys.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      305 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/create_users.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      233 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-ssh-keys.service
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      249 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-fix-mount.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      206 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker.target
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      237 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-mount-cow.service
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      231 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-sshd@.service
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      177 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-sshd.socket
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      197 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/systemd/oardocker-rsyslog.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      566 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/container-init
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)    17506 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/ps_mem
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      832 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/setuser
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     6760 2023-04-17 14:55:26.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/install_oar.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/custom_setup.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      422 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/systemd/oardocker-resources.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      395 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/systemd/oardocker-postgresql.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      264 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/systemd/oardocker-server.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      413 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/systemd/oardocker-queues.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/.gitignore
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/sbin/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      185 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/sbin/taillogs
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      271 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/sbin/oar_server_cmd
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/rsyslog/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/rsyslog/config/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      387 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/rsyslog/config/rsyslog.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/rsyslog/custom_setup.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     8096 2023-04-17 14:55:26.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/install_oar.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     2148 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/nginx-default-site.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      498 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/php5.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1867 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/nginx.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1462 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/motd
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/custom_setup.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      178 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.socket
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      109 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-nginx.socket
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oar-node.service.d/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       36 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oar-node.service.d/override.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      212 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      228 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-php.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/apache2.service.d/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       29 2022-07-27 15:48:47.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/apache2.service.d/override.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      222 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-frontend.target
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      381 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-nginx.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      162 2018-01-22 08:24:36.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-php.socket
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      599 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-apache.service
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/.gitignore
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     3794 2023-04-17 14:55:26.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/install_oar.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       42 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/custom_setup.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      340 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/oardocker-cgroup.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/oar-node.service.d/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       36 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/oar-node.service.d/override.conf
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/oar-node-script.service.d/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       36 2022-11-14 16:31:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/systemd/oar-node-script.service.d/override.conf
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       15 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/.gitignore
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/base/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1570 2022-05-10 07:50:18.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/base/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      766 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1650 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/systemd/oardocker-postgresql@13-main.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      323 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1519 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      548 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/base/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1589 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/base/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      756 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      321 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      917 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      568 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      520 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/create_resources.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/create_queues.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/mount_cow_volumes.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/prepare_oar_cgroup.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/oar_server.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/systemd-spawn-fcgi.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/configure_oar_ssh_keys.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      572 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/server/configure_oar.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      692 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      194 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      582 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      191 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      634 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      282 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/server/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      484 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/server/install_cigri.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      195 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      629 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1327 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/init_cigri.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      257 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/start_cigri.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1564 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/install_cigri.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      269 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/node/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       64 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/node/install_cigri.sh
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     2416 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/cigri/README.md
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      559 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     1294 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/create_resources.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      285 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/create_queues.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      690 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/mount_cow_volumes.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)     2246 2020-03-30 23:48:41.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/prepare_oar_cgroup.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      411 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/oar_server.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      397 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/systemd-spawn-fcgi.sh
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      615 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/configure_oar_ssh_keys.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      568 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/oarswitch-cli
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      849 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1880 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/configure_oar3.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      196 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/
+-rwxr-xr-x   0 neyron    (1000) neyron    (1000)      568 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/oarswitch-cli
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1220 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      480 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/configure_oar3.sh
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      193 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/base/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1570 2022-05-10 07:50:18.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/base/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      764 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1650 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/systemd/oardocker-postgresql@11-main.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      321 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1517 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      546 2021-10-21 08:22:39.000000 oar-docker-1.6.4.dev0/oardocker/templates/buster/images/node/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      632 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/manifest.json
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/base/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1570 2023-04-16 20:48:18.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/base/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/server/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      766 2023-04-16 21:10:58.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/server/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/server/systemd/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1650 2022-01-06 16:12:28.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/server/systemd/oardocker-postgresql@15-main.service
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/rsyslog/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      323 2023-04-16 21:11:37.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/rsyslog/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/frontend/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1519 2023-04-16 21:11:09.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/frontend/Dockerfile
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/node/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      548 2023-04-16 21:11:23.000000 oar-docker-1.6.4.dev0/oardocker/templates/bookworm/images/node/Dockerfile
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     2306 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/cli.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     3130 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/state.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)    14903 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/actions.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     6356 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/context.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     2046 2021-10-21 08:13:13.000000 oar-docker-1.6.4.dev0/oardocker/compat.py
+drwxr-xr-x   0 neyron    (1000) neyron    (1000)        0 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/oardocker/commands/
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     3147 2020-03-30 22:24:45.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_start.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      584 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_install.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1334 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_stop.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      999 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_reset.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1833 2020-03-06 16:29:10.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_init.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      757 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_exec.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     3532 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_logs.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1025 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_clean.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1862 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_status.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      630 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_destroy.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     4133 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_build.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)      713 2019-10-02 19:59:09.000000 oar-docker-1.6.4.dev0/oardocker/commands/cmd_connect.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)        0 2017-11-03 12:49:35.000000 oar-docker-1.6.4.dev0/oardocker/commands/__init__.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       45 2022-01-06 16:36:14.000000 oar-docker-1.6.4.dev0/oardocker/__init__.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     7157 2022-07-27 15:48:47.000000 oar-docker-1.6.4.dev0/oardocker/container.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)       38 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/setup.cfg
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     1058 2021-10-21 08:13:13.000000 oar-docker-1.6.4.dev0/setup.py
+-rw-r--r--   0 neyron    (1000) neyron    (1000)     7313 2022-12-01 16:56:26.000000 oar-docker-1.6.4.dev0/README.rst
+-rw-r--r--   0 neyron    (1000) neyron    (1000)    10794 2022-01-06 16:36:14.000000 oar-docker-1.6.4.dev0/CHANGES.rst
+-rw-r--r--   0 neyron    (1000) neyron    (1000)    23470 2023-04-17 14:58:14.000000 oar-docker-1.6.4.dev0/PKG-INFO
```

### Comparing `oar-docker-1.6.3.dev0/oar_docker.egg-info/SOURCES.txt` & `oar-docker-1.6.4.dev0/oar_docker.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,31 @@
 oardocker/commands/cmd_init.py
 oardocker/commands/cmd_install.py
 oardocker/commands/cmd_logs.py
 oardocker/commands/cmd_reset.py
 oardocker/commands/cmd_start.py
 oardocker/commands/cmd_status.py
 oardocker/commands/cmd_stop.py
+oardocker/templates/bookworm/manifest.json
+oardocker/templates/bookworm/images/base/Dockerfile
+oardocker/templates/bookworm/images/frontend/Dockerfile
+oardocker/templates/bookworm/images/node/Dockerfile
+oardocker/templates/bookworm/images/rsyslog/Dockerfile
+oardocker/templates/bookworm/images/server/Dockerfile
+oardocker/templates/bookworm/images/server/systemd/oardocker-postgresql@15-main.service
 oardocker/templates/bullseye/manifest.json
 oardocker/templates/bullseye/images/base/Dockerfile
 oardocker/templates/bullseye/images/frontend/Dockerfile
-oardocker/templates/bullseye/images/frontend/install_oar.sh
 oardocker/templates/bullseye/images/node/Dockerfile
 oardocker/templates/bullseye/images/rsyslog/Dockerfile
 oardocker/templates/bullseye/images/server/Dockerfile
 oardocker/templates/bullseye/images/server/systemd/oardocker-postgresql@13-main.service
 oardocker/templates/buster/manifest.json
 oardocker/templates/buster/images/base/Dockerfile
 oardocker/templates/buster/images/frontend/Dockerfile
-oardocker/templates/buster/images/frontend/install_oar.sh
 oardocker/templates/buster/images/node/Dockerfile
 oardocker/templates/buster/images/rsyslog/Dockerfile
 oardocker/templates/buster/images/server/Dockerfile
 oardocker/templates/buster/images/server/systemd/oardocker-postgresql@11-main.service
 oardocker/templates/cigri/README.md
 oardocker/templates/cigri/manifest.json
 oardocker/templates/cigri/images/frontend/Dockerfile
@@ -76,31 +81,34 @@
 oardocker/templates/common/images/base/systemd/oardocker-rsyslog.service
 oardocker/templates/common/images/base/systemd/oardocker-ssh-keys.service
 oardocker/templates/common/images/base/systemd/oardocker-sshd.socket
 oardocker/templates/common/images/base/systemd/oardocker-sshd@.service
 oardocker/templates/common/images/base/systemd/oardocker.target
 oardocker/templates/common/images/frontend/.gitignore
 oardocker/templates/common/images/frontend/custom_setup.sh
+oardocker/templates/common/images/frontend/install_oar.sh
 oardocker/templates/common/images/frontend/motd
 oardocker/templates/common/images/frontend/config/nginx-default-site.conf
 oardocker/templates/common/images/frontend/config/nginx.conf
 oardocker/templates/common/images/frontend/config/php5.conf
 oardocker/templates/common/images/frontend/systemd/oardocker-apache.service
 oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.service
 oardocker/templates/common/images/frontend/systemd/oardocker-fcgi.socket
 oardocker/templates/common/images/frontend/systemd/oardocker-frontend.target
 oardocker/templates/common/images/frontend/systemd/oardocker-nginx.service
 oardocker/templates/common/images/frontend/systemd/oardocker-nginx.socket
 oardocker/templates/common/images/frontend/systemd/oardocker-php.service
 oardocker/templates/common/images/frontend/systemd/oardocker-php.socket
+oardocker/templates/common/images/frontend/systemd/apache2.service.d/override.conf
 oardocker/templates/common/images/frontend/systemd/oar-node.service.d/override.conf
 oardocker/templates/common/images/node/.gitignore
 oardocker/templates/common/images/node/custom_setup.sh
 oardocker/templates/common/images/node/install_oar.sh
 oardocker/templates/common/images/node/systemd/oardocker-cgroup.service
+oardocker/templates/common/images/node/systemd/oar-node-script.service.d/override.conf
 oardocker/templates/common/images/node/systemd/oar-node.service.d/override.conf
 oardocker/templates/common/images/rsyslog/custom_setup.sh
 oardocker/templates/common/images/rsyslog/config/rsyslog.conf
 oardocker/templates/common/images/server/.gitignore
 oardocker/templates/common/images/server/custom_setup.sh
 oardocker/templates/common/images/server/install_oar.sh
 oardocker/templates/common/images/server/sbin/oar_server_cmd
@@ -128,15 +136,14 @@
 oardocker/templates/coorm/init-scripts/mount_cow_volumes.sh
 oardocker/templates/coorm/init-scripts/oar_server.sh
 oardocker/templates/coorm/init-scripts/prepare_oar_cgroup.sh
 oardocker/templates/coorm/init-scripts/systemd-spawn-fcgi.sh
 oardocker/templates/jessie/manifest.json
 oardocker/templates/jessie/images/base/Dockerfile
 oardocker/templates/jessie/images/frontend/Dockerfile
-oardocker/templates/jessie/images/frontend/install_oar.sh
 oardocker/templates/jessie/images/node/Dockerfile
 oardocker/templates/jessie/images/rsyslog/Dockerfile
 oardocker/templates/jessie/images/server/Dockerfile
 oardocker/templates/oar3-dev/manifest.json
 oardocker/templates/oar3-dev/images/frontend/Dockerfile
 oardocker/templates/oar3-dev/images/frontend/configure_oar3.sh
 oardocker/templates/oar3-dev/images/frontend/oarswitch-cli
@@ -151,12 +158,11 @@
 oardocker/templates/oar3-dev/init-scripts/mount_cow_volumes.sh
 oardocker/templates/oar3-dev/init-scripts/oar_server.sh
 oardocker/templates/oar3-dev/init-scripts/prepare_oar_cgroup.sh
 oardocker/templates/oar3-dev/init-scripts/systemd-spawn-fcgi.sh
 oardocker/templates/stretch/manifest.json
 oardocker/templates/stretch/images/base/Dockerfile
 oardocker/templates/stretch/images/frontend/Dockerfile
-oardocker/templates/stretch/images/frontend/install_oar.sh
 oardocker/templates/stretch/images/node/Dockerfile
 oardocker/templates/stretch/images/rsyslog/Dockerfile
 oardocker/templates/stretch/images/server/Dockerfile
 oardocker/templates/stretch/images/server/systemd/oardocker-postgresql@9.6-main.service
```

### Comparing `oar-docker-1.6.3.dev0/oar_docker.egg-info/PKG-INFO` & `oar-docker-1.6.4.dev0/oar_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: oar-docker
-Version: 1.6.3.dev0
+Version: 1.6.4.dev0
 Summary: Manage a small OAR developpement cluster with docker.
 Home-page: https://oar.imag.fr/wiki:oar-docker
 Author: Salem Harrache
 Author-email: salem@harrache.info
 License: UNKNOWN
 Description: Build your own OAR cluster with docker
         --------------------------------------
@@ -18,16 +18,16 @@
         
         oar-docker is a set of docker images especially configured for deploying
         your own OAR cluster. The main idea is to have a mini development cluster with
         a frontend, a server and some nodes that launch in just a few seconds on a
         simple laptop.
         
         
-        Why use oar-docker ?
-        --------------------
+        Why use oar-docker?
+        -------------------
         
         Various case scenarios may affect you:
          - Quickly test OAR on a cluster
          - Gain time: a ten-node cluster (or more) is launched in just a
            few seconds and is cleaned in less than a second.
          - Save resources: docker allows the user to pool the node between
            various systems, resource utilization is thus considerably reduced.
@@ -37,14 +37,15 @@
         
         Installation
         ------------
         
         Requirements:
           - python >= 2.7
           - docker >= 1.3
+          - cgroup v1
         
         You can install, upgrade, uninstall oar-docker with these commands::
         
           $ pip install [--user] oar-docker
           $ pip install [--user] --upgrade oar-docker
           $ pip uninstall oar-docker
         
@@ -167,14 +168,33 @@
         
         oardocker ≥ 1.6.0 does not create the ``/dev/oar_cgroups_links/`` and ``/dev/cpuset`` in ``oardocker install``, to let OAR take care of it so that the concerned part of ``job_resource_manager_cgroup.pl`` is actually tested.
         
         This breaks ``job_resource_manager_cgroup.pl`` before OAR 2.5.9+g5k5. See ``.oardocker/init-scripts/prepare_oar_cgroup.sh`` to revert to the old behaviour, by setting::
         
             CREATE_OAR_CGROUPS_LINKS=yes
         
+        The oardocker on Debian setup
+        -----------------------------
+        To use oardocker on a Debian 11 (bullseye) system, one must activate Linux cgroup v1. This can be achieved by including in the linux kernel cmdline: `systemd.legacy_systemd_cgroup_controller=true` (add those options to your bootloader configuration).
+        
+        Using a python3 venv
+        --------------------
+        oardocker can be installed in a python3 venv::
+        
+          $ python3 -m venv oardocker
+          $ cd oardocker
+          $ . bin/activate
+          $ pip install oar-docker
+          $ oardocker init -e bullseye
+          $ oardocker build
+          $ oardocker install path/to/oar/git/repository
+          $ oardocker start
+          $ oardocker connect
+          $ ...
+        
         Network services
         ----------------
         
         By default, oardocker forwards the 80 and 6667 TCP ports to the frontend
         container, for the OAR web services. To add other TCP ports forwarding to
         the frontend, modify the ``.oardocker/manifest.json`` file, adding extra lines
         in the ``net_services`` array. For instance::
@@ -205,19 +225,25 @@
         Besides, the private ssh key used is also insecured since it is public (you can
         find it in the sources).
         
         
         oar-docker CHANGELOG
         ====================
         
-        Version 1.6.3.dev0
+        Version 1.6.4.dev0
         ------------------
         
         **unreleased**
         
+        Version 1.6.3
+        -------------
+        
+        Released on January 06th 2022
+        - add bullseye support
+        
         Version 1.6.2
         -------------
         
         Released on October 21st 2021
         - update docker image recipes for Debian buster: use buster instead of stable as the release name, add the man package
         - add support for the oar-node and oar-server systemd native unit files
         - fix python3 collections callable
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/client.py` & `oar-docker-1.6.4.dev0/oardocker/client.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/utils.py` & `oar-docker-1.6.4.dev0/oardocker/utils.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/base/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/server/systemd/oardocker-postgresql@9.6-main.service` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/server/systemd/oardocker-postgresql@9.6-main.service`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/frontend/install_oar.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/install_oar.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-#!/bin/bash -x
+#!/bin/bash
 set -e
 
+IFS='.' read DEBIAN_VERSION DEBIAN_VERSION_MINOR < /etc/debian_version
+
 TMPDIR=$(mktemp -d --tmpdir install_oar.XXXXXXXX)
 SRCDIR="$TMPDIR/src"
 
+if [ ${DEBIAN_VERSION} -ge '11' ]; then
+    export SYSTEMD_INIT=true
+fi
+
 mkdir -p $SRCDIR
 
 on_exit() {
     mountpoint -q $SRCDIR && umount $SRCDIR || true
     rm -rf $TMPDIR
 }
 
-trap "{ on_exit; kill 0; }" EXIT
+#trap "{ on_exit; kill 0; }" EXIT
+trap on_exit EXIT
 
 fail() {
     echo $@ 1>&2
     exit 1
 }
 
 if [ -d "$1"  ]; then
     GIT_SRC="$(readlink -m $1)"
     RWSRCDIR="$TMPDIR/src-rw"
     mkdir -p $RWSRCDIR
     unionfs-fuse -o cow -o allow_other,use_ino,suid,dev,nonempty $RWSRCDIR=RW:$GIT_SRC=RO $SRCDIR
     pushd $SRCDIR
+    if [ ${DEBIAN_VERSION} -ge '11' ]; then
+        git config --global --add safe.directory $SRCDIR
+    fi
     git clean -Xfd
     BRANCH="$(git rev-parse --abbrev-ref HEAD)"
     VERSION="$(git describe --tags)"
     COMMENT="OAR ${VERSION} (git branch ${BRANCH})"
     popd
     [ -n "${VERSION}" ] || fail "error: fail to retrieve OAR version"
 else
@@ -39,15 +49,15 @@
     else
         TARBALL="$(readlink -m $TARBALL)"
     fi
 
     # extract version from OAR2 or OAR3
     if tar -tf $TARBALL --wildcards "*/setup.py"; then
         VERSION=$(tar xfz $TARBALL --wildcards "*/oar/__init__.py" --to-command "grep -e '__version__ '" | sed -e "s/^[^']\+'\(.\+\)'$/\1/" )
-    else    
+    else
         VERSION=$(tar xfz $TARBALL --wildcards "*/sources/core/common-libs/lib/OAR/Version.pm" --to-command "grep -e 'my \$OARVersion'" | sed -e 's/^[^"]\+"\(.\+\)";$/\1/')
     fi
 
     COMMENT="OAR ${VERSION} (tarball)"
     tar xf $TARBALL -C $SRCDIR
     [ -n "${VERSION}" ] || fail "error: fail to retrieve OAR version"
     SRCDIR=$SRCDIR/oar-${VERSION}
@@ -81,23 +91,30 @@
 fi
 
 if [ -f /usr/local/share/doc/oar-node/examples/init.d/oar-node ]; then
     cat /usr/local/share/doc/oar-node/examples/init.d/oar-node > /etc/init.d/oar-node
     chmod +x  /etc/init.d/oar-node
 fi
 
-
 if [ -f /usr/local/share/oar/oar-node/default/oar-node ]; then
     cat /usr/local/share/oar/oar-node/default/oar-node > /etc/default/oar-node
 fi
 
 if [ -f /usr/local/share/doc/oar-node/examples/default/oar-node ]; then
     cat /usr/local/share/doc/oar-node/examples/default/oar-node > /etc/default/oar-node
 fi
 
+# Copy systemd unit
+if [ -f /usr/local/share/oar/oar-node/systemd/oar-node.service ]; then
+    mkdir -p /usr/local/lib/systemd/system
+    cat /usr/local/share/oar/oar-node/systemd/oar.target > /usr/local/lib/systemd/system/oar.target
+    cat /usr/local/share/oar/oar-node/systemd/oar-node.service > /usr/local/lib/systemd/system/oar-node.service
+    cat /usr/local/share/oar/oar-node/systemd/oar-node-script.service > /usr/local/lib/systemd/system/oar-node-script.service
+fi
+
 # Adapt oar.conf
 sed -e 's/^LOG_LEVEL\=\"2\"/LOG_LEVEL\=\"3\"/' -i /etc/oar/oar.conf
 sed -e 's/^DB_HOSTNAME\=.*/DB_HOSTNAME\=\"server\"/' -i /etc/oar/oar.conf
 sed -e 's/^SERVER_HOSTNAME\=.*/SERVER_HOSTNAME\=\"server\"/' -i /etc/oar/oar.conf
 sed -e 's/^#\(TAKTUK_CMD\=\"\/usr\/bin\/taktuk \-t 30 \-s\".*\)/\1/' -i /etc/oar/oar.conf
 sed -e 's/^#\(PINGCHECKER_TAKTUK_ARG_COMMAND\=\"broadcast exec timeout 5 kill 9 \[ true \]\".*\)/\1/' -i /etc/oar/oar.conf
 sed -e 's/^\(DB_TYPE\)=.*/\1="Pg"/' -i /etc/oar/oar.conf
@@ -166,9 +183,15 @@
 sed -i "s/\$conf\['extra_login_security'\] = true;/\$conf\['extra_login_security'\] = false;/g" /etc/phppgadmin/config.inc.php
 sed -i "s/\$conf\['servers'\]\[0\]\['host'\] = 'localhost';/\$conf\['servers'\]\[0\]\['host'\] = 'server';/g" /etc/phppgadmin/config.inc.php
 sed -i "s/Require local/Require all granted/" /etc/apache2/conf-available/phppgadmin.conf
 
 # Disable all sysvinit services
 ls /etc/init.d/* | xargs -I {} basename {} | xargs -I {} systemctl disable {} 2> /dev/null || true
 
+# Enable oar-node systemd unit
+if [ -f /usr/local/share/oar/oar-node/systemd/oar-node.service ]; then
+    systemctl enable oar-node
+    systemctl enable oar-node-script
+fi
+
 echo "$VERSION" | tee /oar_version
 echo "$COMMENT"
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/stretch/images/node/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/stretch/images/node/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/create_resources.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/create_resources.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/mount_cow_volumes.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/mount_cow_volumes.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/prepare_oar_cgroup.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/prepare_oar_cgroup.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/init-scripts/configure_oar_ssh_keys.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/init-scripts/configure_oar_ssh_keys.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/config/sshd_config` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/config/sshd_config`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/split_ssh_pane` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/split_ssh_pane`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/wait_ssh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/wait_ssh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/bin/wait_pgsql` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/bin/wait_pgsql`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/generate_ssh_keys.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/generate_ssh_keys.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/container-init` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/container-init`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/ps_mem` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/ps_mem`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/base/sbin/setuser` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/base/sbin/setuser`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/server/install_oar.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/server/install_oar.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 #!/bin/bash
 set -e
 
 IFS='.' read DEBIAN_VERSION DEBIAN_VERSION_MINOR < /etc/debian_version
 
 TMPDIR=$(mktemp -d --tmpdir install_oar.XXXXXXXX)
 SRCDIR="$TMPDIR/src"
-export SYSTEMD_INIT=true
+
+if [ ${DEBIAN_VERSION} -ge '11' ]; then
+    export SYSTEMD_INIT=true
+fi
 
 mkdir -p $SRCDIR
 
 on_exit() {
     mountpoint -q $SRCDIR && umount $SRCDIR || true
     rm -rf $TMPDIR
 }
 
-trap "{ on_exit; kill 0; }" EXIT
+#trap "{ on_exit; kill 0; }" EXIT
+trap on_exit EXIT
 
 fail() {
     echo $@ 1>&2
     exit 1
 }
 
 if [ -d "$1"  ]; then
     GIT_SRC="$(readlink -m $1)"
     RWSRCDIR="$TMPDIR/src-rw"
     mkdir -p $RWSRCDIR
     unionfs-fuse -o cow -o allow_other,use_ino,suid,dev,nonempty $RWSRCDIR=RW:$GIT_SRC=RO $SRCDIR
     pushd $SRCDIR
+    if [ ${DEBIAN_VERSION} -ge '11' ]; then
+        git config --global --add safe.directory $SRCDIR
+    fi
     git clean -Xfd
     BRANCH="$(git rev-parse --abbrev-ref HEAD)"
     VERSION="$(git describe --tags)"
     COMMENT="OAR ${VERSION} (git branch ${BRANCH})"
     popd
     [ -n "${VERSION}" ] || fail "error: fail to retrieve OAR version"
 else
@@ -39,14 +46,15 @@
     if [ ! -r "$TARBALL" ]; then
         curl $TARBALL -o $TMPDIR/oar-tarball.tar.gz
         TARBALL=$TMPDIR/oar-tarball.tar.gz
     else
         TARBALL="$(readlink -m $TARBALL)"
     fi
 
+    # extract version from OAR2 or OAR3
     if tar -tf $TARBALL --wildcards "*/setup.py"; then
         VERSION=$(tar xfz $TARBALL --wildcards "*/oar/__init__.py" --to-command "grep -e '__version__ '" | sed -e "s/^[^']\+'\(.\+\)'$/\1/" )
     else
         VERSION=$(tar xfz $TARBALL --wildcards "*/sources/core/common-libs/lib/OAR/Version.pm" --to-command "grep -e 'my \$OARVersion'" | sed -e 's/^[^"]\+"\(.\+\)";$/\1/')
     fi
 
     COMMENT="OAR ${VERSION} (tarball)"
@@ -132,14 +140,16 @@
     POSTGRESQL_VERSION="9.4"
 elif [ ${DEBIAN_VERSION} = '9' ]; then
     POSTGRESQL_VERSION="9.6"
 elif [ ${DEBIAN_VERSION} = '10' ]; then
     POSTGRESQL_VERSION="11"
 elif [ ${DEBIAN_VERSION} = '11' ]; then
     POSTGRESQL_VERSION="13"
+elif [ ${DEBIAN_VERSION} = '12' ]; then
+    POSTGRESQL_VERSION="15"
 else
     POSTGRESQL_VERSION="9.1"
 fi
 
 echo "Configure PostgreSQL to listen for remote connections"
 sed -i "s/#listen_addresses = 'localhost'/listen_addresses = '*'/" /etc/postgresql/$POSTGRESQL_VERSION/main/postgresql.conf
 echo "Configure PostgreSQL to accept remote connections (from any host):"
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/nginx-default-site.conf` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/nginx-default-site.conf`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/config/nginx.conf` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/config/nginx.conf`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/motd` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/motd`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-apache.service` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/frontend/systemd/oardocker-apache.service`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/common/images/node/install_oar.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/common/images/node/install_oar.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 #!/bin/bash
 set -e
 
+IFS='.' read DEBIAN_VERSION DEBIAN_VERSION_MINOR < /etc/debian_version
+
 TMPDIR=$(mktemp -d --tmpdir install_oar.XXXXXXXX)
 SRCDIR="$TMPDIR/src"
-export SYSTEMD_INIT=true
+
+if [ ${DEBIAN_VERSION} -ge '11' ]; then
+    export SYSTEMD_INIT=true
+fi
 
 mkdir -p $SRCDIR
 
 on_exit() {
     mountpoint -q $SRCDIR && umount $SRCDIR || true
     rm -rf $TMPDIR
 }
 
-trap "{ on_exit; kill 0; }" EXIT
+#trap "{ on_exit; kill 0; }" EXIT
+trap on_exit EXIT
 
 fail() {
     echo $@ 1>&2
     exit 1
 }
 
 if [ -d "$1"  ]; then
     GIT_SRC="$(readlink -m $1)"
     RWSRCDIR="$TMPDIR/src-rw"
     mkdir -p $RWSRCDIR
     unionfs-fuse -o cow -o allow_other,use_ino,suid,dev,nonempty $RWSRCDIR=RW:$GIT_SRC=RO $SRCDIR
     pushd $SRCDIR
+    if [ ${DEBIAN_VERSION} -ge '11' ]; then
+        git config --global --add safe.directory $SRCDIR
+    fi
     git clean -Xfd
     BRANCH="$(git rev-parse --abbrev-ref HEAD)"
     VERSION="$(git describe --tags)"
     COMMENT="OAR ${VERSION} (git branch ${BRANCH})"
     popd
     [ -n "${VERSION}" ] || fail "error: fail to retrieve OAR version"
 else
@@ -37,20 +46,21 @@
     if [ ! -r "$TARBALL" ]; then
         curl $TARBALL -o $TMPDIR/oar-tarball.tar.gz
         TARBALL=$TMPDIR/oar-tarball.tar.gz
     else
         TARBALL="$(readlink -m $TARBALL)"
     fi
 
+    # extract version from OAR2 or OAR3
     if tar -tf $TARBALL --wildcards "*/setup.py"; then
         VERSION=$(tar xfz $TARBALL --wildcards "*/oar/__init__.py" --to-command "grep -e '__version__ '" | sed -e "s/^[^']\+'\(.\+\)'$/\1/" )
-    else    
+    else
         VERSION=$(tar xfz $TARBALL --wildcards "*/sources/core/common-libs/lib/OAR/Version.pm" --to-command "grep -e 'my \$OARVersion'" | sed -e 's/^[^"]\+"\(.\+\)";$/\1/')
     fi
-    
+
     COMMENT="OAR ${VERSION} (tarball)"
     tar xf $TARBALL -C $SRCDIR
     [ -n "${VERSION}" ] || fail "error: fail to retrieve OAR version"
     SRCDIR=$SRCDIR/oar-${VERSION}
 fi
 
 MAJOR_VERSION=$(echo $VERSION | sed -e 's/\([0-9]\).*/\1/')
@@ -67,38 +77,40 @@
 # Copy initd scripts
 if [ -f /usr/local/share/oar/oar-node/init.d/oar-node ]; then
     cat /usr/local/share/oar/oar-node/init.d/oar-node > /etc/init.d/oar-node
     chmod +x  /etc/init.d/oar-node
 fi
 
 if [ -f /usr/local/share/doc/oar-node/examples/init.d/oar-node ]; then
-    cat /usr/local/share/oar/oar-node/init.d/oar-node > /etc/init.d/oar-node
+    cat /usr/local/share/doc/oar-node/examples/init.d/oar-node > /etc/init.d/oar-node
     chmod +x  /etc/init.d/oar-node
 fi
 
-
 if [ -f /usr/local/share/oar/oar-node/default/oar-node ]; then
     cat /usr/local/share/oar/oar-node/default/oar-node > /etc/default/oar-node
 fi
 
 if [ -f /usr/local/share/doc/oar-node/examples/default/oar-node ]; then
     cat /usr/local/share/doc/oar-node/examples/default/oar-node > /etc/default/oar-node
 fi
 
 # Copy systemd unit
 if [ -f /usr/local/share/oar/oar-node/systemd/oar-node.service ]; then
     mkdir -p /usr/local/lib/systemd/system
+    cat /usr/local/share/oar/oar-node/systemd/oar.target > /usr/local/lib/systemd/system/oar.target
     cat /usr/local/share/oar/oar-node/systemd/oar-node.service > /usr/local/lib/systemd/system/oar-node.service
+    cat /usr/local/share/oar/oar-node/systemd/oar-node-script.service > /usr/local/lib/systemd/system/oar-node-script.service
 fi
 
 sed -e 's/^#\(GET_CURRENT_CPUSET_CMD.*oardocker.*\)/\1/' -i /etc/oar/oar.conf
 
 # Disable all sysvinit services
 ls /etc/init.d/* | xargs -I {} basename {} | xargs -I {} systemctl disable {} 2> /dev/null || true
 
 # Enable oar-node systemd unit
 if [ -f /usr/local/share/oar/oar-node/systemd/oar-node.service ]; then
     systemctl enable oar-node
+    systemctl enable oar-node-script
 fi
 
 echo "$VERSION" | tee /oar_version
 echo "$COMMENT"
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/base/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/base/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     DEBIAN_PRIORITY=critical \
     DEBCONF_NOWARNINGS=yes \
     COLOR=green
 
 RUN echo "export COLOR=green" > /etc/hostname.color
 
 RUN apt-get update
-RUN apt-get install -y man
+RUN apt-get install -y man jq
 
 ## rsyslog sender
 COPY config/rsyslog.conf /etc/rsyslog.conf
 
 ## configure sshd daemon
 ADD config/sshd_config /etc/ssh/sshd_config
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/server/systemd/oardocker-postgresql@13-main.service` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/server/systemd/oardocker-postgresql@13-main.service`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/bullseye/images/node/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/bullseye/images/node/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/jessie/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/jessie/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/base/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/jessie/images/node/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/jessie/images/node/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/create_resources.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/create_resources.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/mount_cow_volumes.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/mount_cow_volumes.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/prepare_oar_cgroup.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/prepare_oar_cgroup.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/init-scripts/configure_oar_ssh_keys.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/init-scripts/configure_oar_ssh_keys.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/server/configure_oar.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/server/configure_oar.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/coorm/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/coorm/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/cigri/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/cigri/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/init_cigri.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/init_cigri.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/cigri/images/frontend/install_cigri.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/cigri/images/frontend/install_cigri.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/cigri/README.md` & `oar-docker-1.6.4.dev0/oardocker/templates/cigri/README.md`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/create_resources.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/create_resources.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/mount_cow_volumes.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/mount_cow_volumes.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/prepare_oar_cgroup.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/prepare_oar_cgroup.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/init-scripts/configure_oar_ssh_keys.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/init-scripts/configure_oar_ssh_keys.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/oarswitch-cli` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/oarswitch-cli`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/server/configure_oar3.sh` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/server/configure_oar3.sh`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/oarswitch-cli` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/oarswitch-cli`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/oar3-dev/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/oar3-dev/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/manifest.json` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/manifest.json`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/images/base/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/images/base/Dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     DEBIAN_PRIORITY=critical \
     DEBCONF_NOWARNINGS=yes \
     COLOR=green
 
 RUN echo "export COLOR=green" > /etc/hostname.color
 
 RUN apt-get update
-RUN apt-get install -y man
+RUN apt-get install -y man jq
 
 ## rsyslog sender
 COPY config/rsyslog.conf /etc/rsyslog.conf
 
 ## configure sshd daemon
 ADD config/sshd_config /etc/ssh/sshd_config
```

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/images/server/systemd/oardocker-postgresql@11-main.service` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/images/server/systemd/oardocker-postgresql@11-main.service`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/images/frontend/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/images/frontend/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/templates/buster/images/node/Dockerfile` & `oar-docker-1.6.4.dev0/oardocker/templates/buster/images/node/Dockerfile`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/cli.py` & `oar-docker-1.6.4.dev0/oardocker/cli.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/state.py` & `oar-docker-1.6.4.dev0/oardocker/state.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/actions.py` & `oar-docker-1.6.4.dev0/oardocker/actions.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/context.py` & `oar-docker-1.6.4.dev0/oardocker/context.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/compat.py` & `oar-docker-1.6.4.dev0/oardocker/compat.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_start.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_install.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_stop.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_stop.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_reset.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_reset.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_init.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_exec.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_logs.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_logs.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_clean.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_status.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_destroy.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_destroy.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_build.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_build.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/commands/cmd_connect.py` & `oar-docker-1.6.4.dev0/oardocker/commands/cmd_connect.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/oardocker/container.py` & `oar-docker-1.6.4.dev0/oardocker/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         binds = options.pop('binds', None)
         volumes_from = options.pop('volumes_from', [])
         network_name = options.pop('network_name', None)
 
         host_config_kwargs = {
             "tmpfs": {'/run/lock': '', '/run': '', '/tmp': ''},
             "security_opt": ['seccomp:unconfined'],
-            "cap_add": ["SYS_ADMIN", "MKNOD"],
+            "cap_add": ["SYS_ADMIN", "SYS_NICE", "MKNOD"],
         }
         if binds:
             host_config_kwargs['binds'] = binds
         if privileged:
             host_config_kwargs['privileged'] = privileged
         if port_bindings:
             host_config_kwargs['port_bindings'] = port_bindings
```

### Comparing `oar-docker-1.6.3.dev0/setup.py` & `oar-docker-1.6.4.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `oar-docker-1.6.3.dev0/README.rst` & `oar-docker-1.6.4.dev0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 oar-docker is a set of docker images especially configured for deploying
 your own OAR cluster. The main idea is to have a mini development cluster with
 a frontend, a server and some nodes that launch in just a few seconds on a
 simple laptop.
 
 
-Why use oar-docker ?
---------------------
+Why use oar-docker?
+-------------------
 
 Various case scenarios may affect you:
  - Quickly test OAR on a cluster
  - Gain time: a ten-node cluster (or more) is launched in just a
    few seconds and is cleaned in less than a second.
  - Save resources: docker allows the user to pool the node between
    various systems, resource utilization is thus considerably reduced.
@@ -29,14 +29,15 @@
 
 Installation
 ------------
 
 Requirements:
   - python >= 2.7
   - docker >= 1.3
+  - cgroup v1
 
 You can install, upgrade, uninstall oar-docker with these commands::
 
   $ pip install [--user] oar-docker
   $ pip install [--user] --upgrade oar-docker
   $ pip uninstall oar-docker
 
@@ -159,14 +160,33 @@
 
 oardocker ≥ 1.6.0 does not create the ``/dev/oar_cgroups_links/`` and ``/dev/cpuset`` in ``oardocker install``, to let OAR take care of it so that the concerned part of ``job_resource_manager_cgroup.pl`` is actually tested.
 
 This breaks ``job_resource_manager_cgroup.pl`` before OAR 2.5.9+g5k5. See ``.oardocker/init-scripts/prepare_oar_cgroup.sh`` to revert to the old behaviour, by setting::
 
     CREATE_OAR_CGROUPS_LINKS=yes
 
+The oardocker on Debian setup
+-----------------------------
+To use oardocker on a Debian 11 (bullseye) system, one must activate Linux cgroup v1. This can be achieved by including in the linux kernel cmdline: `systemd.legacy_systemd_cgroup_controller=true` (add those options to your bootloader configuration).
+
+Using a python3 venv
+--------------------
+oardocker can be installed in a python3 venv::
+
+  $ python3 -m venv oardocker
+  $ cd oardocker
+  $ . bin/activate
+  $ pip install oar-docker
+  $ oardocker init -e bullseye
+  $ oardocker build
+  $ oardocker install path/to/oar/git/repository
+  $ oardocker start
+  $ oardocker connect
+  $ ...
+
 Network services
 ----------------
 
 By default, oardocker forwards the 80 and 6667 TCP ports to the frontend
 container, for the OAR web services. To add other TCP ports forwarding to
 the frontend, modify the ``.oardocker/manifest.json`` file, adding extra lines
 in the ``net_services`` array. For instance::
```

### Comparing `oar-docker-1.6.3.dev0/CHANGES.rst` & `oar-docker-1.6.4.dev0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 oar-docker CHANGELOG
 ====================
 
-Version 1.6.3.dev0
+Version 1.6.4.dev0
 ------------------
 
 **unreleased**
 
+Version 1.6.3
+-------------
+
+Released on January 06th 2022
+- add bullseye support
+
 Version 1.6.2
 -------------
 
 Released on October 21st 2021
 - update docker image recipes for Debian buster: use buster instead of stable as the release name, add the man package
 - add support for the oar-node and oar-server systemd native unit files
 - fix python3 collections callable
```

### Comparing `oar-docker-1.6.3.dev0/PKG-INFO` & `oar-docker-1.6.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: oar-docker
-Version: 1.6.3.dev0
+Version: 1.6.4.dev0
 Summary: Manage a small OAR developpement cluster with docker.
 Home-page: https://oar.imag.fr/wiki:oar-docker
 Author: Salem Harrache
 Author-email: salem@harrache.info
 License: UNKNOWN
 Description: Build your own OAR cluster with docker
         --------------------------------------
@@ -18,16 +18,16 @@
         
         oar-docker is a set of docker images especially configured for deploying
         your own OAR cluster. The main idea is to have a mini development cluster with
         a frontend, a server and some nodes that launch in just a few seconds on a
         simple laptop.
         
         
-        Why use oar-docker ?
-        --------------------
+        Why use oar-docker?
+        -------------------
         
         Various case scenarios may affect you:
          - Quickly test OAR on a cluster
          - Gain time: a ten-node cluster (or more) is launched in just a
            few seconds and is cleaned in less than a second.
          - Save resources: docker allows the user to pool the node between
            various systems, resource utilization is thus considerably reduced.
@@ -37,14 +37,15 @@
         
         Installation
         ------------
         
         Requirements:
           - python >= 2.7
           - docker >= 1.3
+          - cgroup v1
         
         You can install, upgrade, uninstall oar-docker with these commands::
         
           $ pip install [--user] oar-docker
           $ pip install [--user] --upgrade oar-docker
           $ pip uninstall oar-docker
         
@@ -167,14 +168,33 @@
         
         oardocker ≥ 1.6.0 does not create the ``/dev/oar_cgroups_links/`` and ``/dev/cpuset`` in ``oardocker install``, to let OAR take care of it so that the concerned part of ``job_resource_manager_cgroup.pl`` is actually tested.
         
         This breaks ``job_resource_manager_cgroup.pl`` before OAR 2.5.9+g5k5. See ``.oardocker/init-scripts/prepare_oar_cgroup.sh`` to revert to the old behaviour, by setting::
         
             CREATE_OAR_CGROUPS_LINKS=yes
         
+        The oardocker on Debian setup
+        -----------------------------
+        To use oardocker on a Debian 11 (bullseye) system, one must activate Linux cgroup v1. This can be achieved by including in the linux kernel cmdline: `systemd.legacy_systemd_cgroup_controller=true` (add those options to your bootloader configuration).
+        
+        Using a python3 venv
+        --------------------
+        oardocker can be installed in a python3 venv::
+        
+          $ python3 -m venv oardocker
+          $ cd oardocker
+          $ . bin/activate
+          $ pip install oar-docker
+          $ oardocker init -e bullseye
+          $ oardocker build
+          $ oardocker install path/to/oar/git/repository
+          $ oardocker start
+          $ oardocker connect
+          $ ...
+        
         Network services
         ----------------
         
         By default, oardocker forwards the 80 and 6667 TCP ports to the frontend
         container, for the OAR web services. To add other TCP ports forwarding to
         the frontend, modify the ``.oardocker/manifest.json`` file, adding extra lines
         in the ``net_services`` array. For instance::
@@ -205,19 +225,25 @@
         Besides, the private ssh key used is also insecured since it is public (you can
         find it in the sources).
         
         
         oar-docker CHANGELOG
         ====================
         
-        Version 1.6.3.dev0
+        Version 1.6.4.dev0
         ------------------
         
         **unreleased**
         
+        Version 1.6.3
+        -------------
+        
+        Released on January 06th 2022
+        - add bullseye support
+        
         Version 1.6.2
         -------------
         
         Released on October 21st 2021
         - update docker image recipes for Debian buster: use buster instead of stable as the release name, add the man package
         - add support for the oar-node and oar-server systemd native unit files
         - fix python3 collections callable
```

