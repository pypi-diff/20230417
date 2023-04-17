# Comparing `tmp/PlexTraktSync-0.26.0.tar.gz` & `tmp/PlexTraktSync-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-npnpeg_h/PlexTraktSync-0.26.0.tar", last modified: Mon Apr 17 14:01:15 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-mdcu90ke/PlexTraktSync-0.26.1.tar", last modified: Mon Apr 17 14:03:48 2023, max compression
```

## Comparing `PlexTraktSync-0.26.0.tar` & `PlexTraktSync-0.26.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:01:04.000000 PlexTraktSync-0.26.0/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 14:01:06.000000 PlexTraktSync-0.26.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:01:15.000000 PlexTraktSync-0.26.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-17 14:01:03.000000 PlexTraktSync-0.26.0/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:03:40.000000 PlexTraktSync-0.26.1/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 14:03:42.000000 PlexTraktSync-0.26.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.0/LICENSE` & `PlexTraktSync-0.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/PKG-INFO` & `PlexTraktSync-0.26.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.0
+Version: 0.26.1
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.0/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.0
+Version: 0.26.1
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.0/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 charset-normalizer==3.1.0
 click==8.1.3
 deprecated==1.2.13
 inquirerpy==0.3.4
 oauthlib==3.2.2
 plexapi==4.13.4
 prompt-toolkit==3.0.38
-pygments==2.14.0
+pygments==2.15.0
 python-dotenv==0.21.1
-python-git-info==0.8.2
+python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.20
+pytrakt==3.4.21
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests==2.28.2
-rich==13.3.3
+rich==13.3.4
 tqdm==4.65.0
 urllib3==1.26.15
 wcwidth==0.2.6
 websocket-client==1.5.1
 
 [:python_version <= "3.7"]
 backports.cached-property==1.0.2
```

### Comparing `PlexTraktSync-0.26.0/README.md` & `PlexTraktSync-0.26.1/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/cli.py` & `PlexTraktSync-0.26.1/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.1/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.1/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.1/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.1/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.1/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.1/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.1/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.1/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.1/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.1/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/logging.py` & `PlexTraktSync-0.26.1/plextraktsync/logging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/media.py` & `PlexTraktSync-0.26.1/plextraktsync/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from plexapi.exceptions import PlexApiException
 from requests import RequestException
 from trakt.errors import TraktException
 
 from plextraktsync.decorators.cached_property import cached_property
 from plextraktsync.factory import logger
 from plextraktsync.trakt.TraktLookup import TraktLookup
+from rich.markup import escape
 
 if TYPE_CHECKING:
     from plextraktsync.plex.PlexApi import PlexApi
     from plextraktsync.plex.PlexGuid import PlexGuid
     from plextraktsync.plex.PlexLibraryItem import PlexLibraryItem
     from plextraktsync.trakt.TraktApi import TraktApi
     from plextraktsync.trakt.TraktItem import TraktItem
@@ -44,14 +45,20 @@
     @property
     def title(self):
         if self.plex:
             return self.plex.title
 
         return f"{self.trakt.title} ({self.trakt.year})"
 
+    @property
+    def title_link(self):
+        link = self.plex_api.media_url(self.plex)
+
+        return f"[link={link}][green]{escape(self.title)}[/][/]"
+
     @cached_property
     def media_type(self):
         return self.trakt.media_type
 
     @cached_property
     def type(self):
         """
```

### Comparing `PlexTraktSync-0.26.0/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.1/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,16 @@
     """
     Plex API class abstracting common data access and dealing with requests cache.
     """
 
     def __init__(self, plex: PlexServer):
         self.plex = plex
 
-    @cached_property
-    def plex_base_url(self):
-        return f"https://app.plex.tv/desktop/#!/server/{self.plex.machineIdentifier}"
+    def plex_base_url(self, section="server"):
+        return f"https://app.plex.tv/desktop/#!/{section}/{self.plex.machineIdentifier}"
 
     @property
     def plex_discover_base_url(self):
         return "https://app.plex.tv/desktop/#!/provider/tv.plex.provider.discover"
 
     @flatten_list
     def movie_sections(self, library=None) -> list[PlexLibrarySection]:
@@ -82,15 +81,15 @@
             return None
 
         self.fetch_item.cache_clear()
 
         return self.fetch_item(key)
 
     def media_url(self, m: PlexLibraryItem, discover=False):
-        base_url = self.plex_discover_base_url if m.is_discover or discover else self.plex_base_url
+        base_url = self.plex_discover_base_url if m.is_discover or discover else self.plex_base_url("server")
         key = f"/library/metadata/{m.item.guid.rsplit('/', 1)[-1]}" if discover else m.item.key
 
         return f"{base_url}/details?key={key}"
 
     def download(self, m: SubtitleStream | MediaPart, **kwargs):
         url = self.plex.url(m.key)
         token = self.plex._token
```

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibrarySection.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING
 
 from plexapi import X_PLEX_CONTAINER_SIZE
 from plexapi.exceptions import NotFound
 
 from plextraktsync.decorators.retry import retry
 from plextraktsync.plex.PlexLibraryItem import PlexLibraryItem
+from rich.markup import escape
 
 if TYPE_CHECKING:
     from plexapi.library import LibrarySection
 
     from plextraktsync.plex.PlexApi import PlexApi
     from plextraktsync.plex.types import PlexMedia
 
@@ -30,14 +31,25 @@
     def type(self):
         return self.section.type
 
     @property
     def title(self):
         return self.section.title
 
+    @property
+    def link(self):
+        """ Return Plex App URL for this section """
+        base_url = self.plex.plex_base_url("media")
+
+        return f"{base_url}/com.plexapp.plugins.library?source={self.section.key}"
+
+    @property
+    def title_link(self):
+        return f"[link={self.link}][green]{escape(self.title)}[/][/]"
+
     def find_by_title(self, name: str):
         try:
             return self.section.get(name)
         except NotFound:
             return None
 
     def search(self, **kwargs):
```

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.1/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.1/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.1/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.1/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.1/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.1/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.1/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/sync.py` & `PlexTraktSync-0.26.1/plextraktsync/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,32 +118,33 @@
     def sync_collection(self, m: Media, dry_run=False):
         if not self.config.plex_to_trakt["collection"]:
             return
 
         if m.is_collected:
             return
 
-        logger.info(f"Adding to collection: '{m.title}'")
+        logger.info(f"Adding to collection: {m.title_link}", extra={"markup": True})
+
         if not dry_run:
             m.add_to_collection()
 
     def sync_ratings(self, m: Media, dry_run=False):
         if not self.config.sync_ratings:
             return
 
         if m.plex_rating is m.trakt_rating:
             return
 
         # If two-way rating sync, Plex rating takes precedence over Trakt rating
         if m.plex_rating is not None and self.config.plex_to_trakt["ratings"]:
-            logger.info(f"Rating '{m.title}' with {m.plex_rating} on Trakt")
+            logger.info(f"Rating {m.title_link} with {m.plex_rating} on Trakt", extra={"markup": True})
             if not dry_run:
                 m.trakt_rate()
         elif m.trakt_rating is not None and self.config.trakt_to_plex["ratings"]:
-            logger.info(f"Rating '{m.title}' with {m.trakt_rating} on Plex")
+            logger.info(f"Rating {m.title_link} with {m.trakt_rating} on Plex", extra={"markup": True})
             if not dry_run:
                 m.plex_rate()
 
     def sync_watched(self, m: Media, dry_run=False):
         if not self.config.sync_watched_status:
             return
 
@@ -157,58 +158,58 @@
             if m.is_episode and m.watched_before_reset:
                 show = m.plex.item.show()
                 logger.info(f"Show '{show.title}' has been reset in trakt at {m.show_reset_at}.")
                 logger.info(f"Marking '{show.title}' as unwatched in Plex.")
                 if not dry_run:
                     m.reset_show()
             else:
-                logger.info(f"Marking as watched in Trakt: '{m.title}'")
+                logger.info(f"Marking as watched in Trakt: {m.title_link}", extra={"markup": True})
                 if not dry_run:
                     m.mark_watched_trakt()
         elif m.watched_on_trakt:
             if not self.config.trakt_to_plex["watched_status"]:
                 return
-            logger.info(f"Marking as watched in Plex: '{m.title}'")
+            logger.info(f"Marking as watched in Plex: {m.title_link}", extra={"markup": True})
             if not dry_run:
                 m.mark_watched_plex()
 
     def watchlist_sync_item(self, m: Media, dry_run=False):
         if m.plex is None:
             if self.config.update_plex_wl:
-                logger.info(f"Skipping '{m.title}' from Trakt watchlist because not found in Plex Discover")
+                logger.info(f"Skipping {m.title_link} from Trakt watchlist because not found in Plex Discover", extra={"markup": True})
             elif self.config.update_trakt_wl:
-                logger.info(f"Removing '{m.title}' from Trakt watchlist")
+                logger.info(f"Removing {m.title_link} from Trakt watchlist", extra={"markup": True})
                 if not dry_run:
                     m.remove_from_trakt_watchlist()
             return
 
         if m in self.plex_wl:
             if m not in self.trakt_wl:
                 if self.config.update_trakt_wl:
-                    logger.info(f"Adding '{m.title}' to Trakt watchlist")
+                    logger.info(f"Adding {m.title_link} to Trakt watchlist", extra={"markup": True})
                     if not dry_run:
                         m.add_to_trakt_watchlist()
                 else:
-                    logger.info(f"Removing '{m.title}' from Plex watchlist")
+                    logger.info(f"Removing {m.title_link} from Plex watchlist", extra={"markup": True})
                     if not dry_run:
                         m.remove_from_plex_watchlist()
             else:
                 # Plex Online search is inaccurate, and it doesn't offer search by id.
                 # Remove known match from trakt watchlist, so that the search would not be attempted.
                 # Example, trakt id 187634 where title mismatches:
                 #  - "The Vortex": https://trakt.tv/movies/the-vortex-2012
                 #  - "Big Bad Bugs": https://app.plex.tv/desktop/#!/provider/tv.plex.provider.vod/details?key=%2Flibrary%2Fmetadata%2F60185c5891c237002b37653d
                 del self.trakt_wl[m]
         elif m in self.trakt_wl:
             if self.config.update_plex_wl:
-                logger.info(f"Adding '{m.title}' to Plex watchlist")
+                logger.info(f"Adding {m.title_link} to Plex watchlist", extra={"markup": True})
                 if not dry_run:
                     m.add_to_plex_watchlist()
             else:
-                logger.info(f"Removing '{m.title}' from Trakt watchlist")
+                logger.info(f"Removing {m.title_link} from Trakt watchlist", extra={"markup": True})
                 if not dry_run:
                     m.remove_from_trakt_watchlist()
 
     def sync_watchlist(self, walker: Walker, dry_run=False):
         # NOTE: Plex watchlist sync removes matching items from trakt lists
         # See the comment above around "del self.trakt_wl[m]"
         for m in walker.media_from_plexlist(self.plex_wl):
```

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.1/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.1/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.1/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.1/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.1/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.1/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.1/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.1/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.1/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.1/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/walker.py` & `PlexTraktSync-0.26.1/plextraktsync/walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,20 +241,20 @@
     def plan(self):
         return WalkPlanner(self.plex, self.config).plan()
 
     @property
     def is_partial(self):
         return self.config.is_partial
 
-    def print_plan(self, print=print):
+    def print_plan(self, print):
         if self.plan.movie_sections:
-            print(f"Sync Movie sections: {[x.title for x in self.plan.movie_sections]}")
+            print(f"Sync Movie sections: {[x.title_link for x in self.plan.movie_sections]}", extra={"markup": True})
 
         if self.plan.show_sections:
-            print(f"Sync Show sections: {[x.title for x in self.plan.show_sections]}")
+            print(f"Sync Show sections: {[x.title_link for x in self.plan.show_sections]}", extra={"markup": True})
 
         if self.plan.movies:
             print(f"Sync Movies: {[x.title for x in self.plan.movies]}")
 
         if self.plan.shows:
             print(f"Sync Shows: {[x.title for x in self.plan.shows]}")
 
@@ -318,20 +318,20 @@
                 continue
 
             me.show = show
             yield me
 
     def media_from_sections(self, sections: list[PlexLibrarySection]) -> Generator[PlexLibraryItem, Any, None]:
         for section in sections:
-            with measure_time(f"{section.title} processed"):
+            with measure_time(f"{section.title_link} processed", extra={"markup": True}):
                 total = len(section)
                 it = self.progressbar(
                     section.items(total),
                     total=total,
-                    desc=f"Processing {section.title}",
+                    desc=f"Processing {section.title_link}",
                 )
                 yield from it
 
     def media_from_items(self, libtype: str, items: list) -> Generator[PlexLibraryItem, Any, None]:
         it = self.progressbar(items, desc=f"Processing {libtype}s")
         for m in it:
             yield PlexLibraryItem(m, self.plex)
```

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.1/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/requirements.txt` & `PlexTraktSync-0.26.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 markdown-it-py==2.2.0; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 platformdirs==3.2.0; python_version >= '3.7'
 plexapi==4.13.4
 prompt-toolkit==3.0.38
-pygments==2.14.0
+pygments==2.15.0
 python-dotenv==0.21.1
-python-git-info==0.8.2
+python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.20
+pytrakt==3.4.21
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests-oauthlib==1.3.1; python_version >= '3.4'
 requests==2.28.2
-rich==13.3.3
+rich==13.3.4
 six==1.16.0; python_version >= '3.4'
 tqdm==4.65.0
 url-normalize==1.4.3; python_version >= '3.6'
 urllib3==1.26.15
 wcwidth==0.2.6
 websocket-client==1.5.1
 wrapt==1.15.0; python_version >= '3.5'
```

### Comparing `PlexTraktSync-0.26.0/setup.cfg` & `PlexTraktSync-0.26.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.1/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_config.py` & `PlexTraktSync-0.26.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_events.py` & `PlexTraktSync-0.26.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_new_agent.py` & `PlexTraktSync-0.26.1/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_timer.py` & `PlexTraktSync-0.26.1/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.1/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.1/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.0/tests/test_walker.py` & `PlexTraktSync-0.26.1/tests/test_walker.py`

 * *Files identical despite different names*

