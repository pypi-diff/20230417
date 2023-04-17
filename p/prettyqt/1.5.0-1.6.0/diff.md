# Comparing `tmp/prettyqt-1.5.0.tar.gz` & `tmp/prettyqt-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyqt-1.5.0.tar", max compression
+gzip compressed data, was "prettyqt-1.6.0.tar", max compression
```

## Comparing `prettyqt-1.5.0.tar` & `prettyqt-1.6.0.tar`

### file list

```diff
@@ -1,749 +1,749 @@
--rw-r--r--   0        0        0     1078 2023-04-13 13:11:05.673482 prettyqt-1.5.0/LICENSE
--rw-r--r--   0        0        0     2746 2023-04-13 13:11:05.673482 prettyqt-1.5.0/docs/index.md
--rw-r--r--   0        0        0      687 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/__init__.py
--rw-r--r--   0        0        0      122 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      860 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/__pyinstaller/hook-prettyqt.py
--rw-r--r--   0        0        0      517 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/__init__.py
--rw-r--r--   0        0        0      334 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/bluetoothaddress.py
--rw-r--r--   0        0        0     2635 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
--rw-r--r--   0        0        0     1421 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
--rw-r--r--   0        0        0     1872 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/bluetoothserviceinfo.py
--rw-r--r--   0        0        0    11927 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/bluetooth/bluetoothuuid.py
--rw-r--r--   0        0        0     1792 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/abstractaxis.py
--rw-r--r--   0        0        0     1603 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/abstractbarseries.py
--rw-r--r--   0        0        0      554 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/abstractseries.py
--rw-r--r--   0        0        0      517 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/barcategoryaxis.py
--rw-r--r--   0        0        0      177 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/barseries.py
--rw-r--r--   0        0        0      932 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/barset.py
--rw-r--r--   0        0        0     1648 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/boxset.py
--rw-r--r--   0        0        0      609 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/candlestickset.py
--rw-r--r--   0        0        0     1767 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/categoryaxis.py
--rw-r--r--   0        0        0     5315 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/chart.py
--rw-r--r--   0        0        0     5665 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/chartview.py
--rw-r--r--   0        0        0      381 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/datetimeaxis.py
--rw-r--r--   0        0        0      197 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/horizontalbarseries.py
--rw-r--r--   0        0        0      217 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/horizontalpercentbarseries.py
--rw-r--r--   0        0        0      217 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/horizontalstackedbarseries.py
--rw-r--r--   0        0        0     2742 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/legend.py
--rw-r--r--   0        0        0      673 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/lineseries.py
--rw-r--r--   0        0        0      178 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/logvalueaxis.py
--rw-r--r--   0        0        0      191 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/percentbarseries.py
--rw-r--r--   0        0        0     2038 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/pieslice.py
--rw-r--r--   0        0        0      739 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/polarchart.py
--rw-r--r--   0        0        0      176 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/scatterseries.py
--rw-r--r--   0        0        0      191 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/stackedbarseries.py
--rw-r--r--   0        0        0     1044 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/valueaxis.py
--rw-r--r--   0        0        0     1219 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/charts/xyseries.py
--rw-r--r--   0        0        0    50840 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/constants/__init__.py
--rw-r--r--   0        0        0     8711 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/_calendar.py
--rw-r--r--   0        0        0     2000 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/_datetime.py
--rw-r--r--   0        0        0    16492 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/_locale.py
--rw-r--r--   0        0        0      478 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/_time.py
--rw-r--r--   0        0        0     3286 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstractanimation.py
--rw-r--r--   0        0        0      186 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstracteventdispatcher.py
--rw-r--r--   0        0        0     5236 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstractitemmodel.py
--rw-r--r--   0        0        0      250 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstractlistmodel.py
--rw-r--r--   0        0        0      146 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstractnativeeventfilter.py
--rw-r--r--   0        0        0      254 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstractproxymodel.py
--rw-r--r--   0        0        0      254 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/abstracttablemodel.py
--rw-r--r--   0        0        0     2060 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/animationgroup.py
--rw-r--r--   0        0        0      533 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/basictimer.py
--rw-r--r--   0        0        0      154 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/buffer.py
--rw-r--r--   0        0        0      173 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/bytearray.py
--rw-r--r--   0        0        0      369 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/bytearraymatcher.py
--rw-r--r--   0        0        0      959 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/collator.py
--rw-r--r--   0        0        0      126 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/collatorsortkey.py
--rw-r--r--   0        0        0      324 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/commandlineoption.py
--rw-r--r--   0        0        0     2231 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/commandlineparser.py
--rw-r--r--   0        0        0      211 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/concatenatetablesproxymodel.py
--rw-r--r--   0        0        0     3729 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/coreapplication.py
--rw-r--r--   0        0        0     2038 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/cryptographichash.py
--rw-r--r--   0        0        0     3426 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/datastream.py
--rw-r--r--   0        0        0      470 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/date.py
--rw-r--r--   0        0        0      766 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/deadlinetimer.py
--rw-r--r--   0        0        0     1153 2023-04-13 13:11:05.673482 prettyqt-1.5.0/prettyqt/core/debug.py
--rw-r--r--   0        0        0     4467 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/dir.py
--rw-r--r--   0        0        0      949 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/diriterator.py
--rw-r--r--   0        0        0     4527 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/easingcurve.py
--rw-r--r--   0        0        0      918 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/elapsedtimer.py
--rw-r--r--   0        0        0     7128 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/event.py
--rw-r--r--   0        0        0     1225 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/eventloop.py
--rw-r--r--   0        0        0      191 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/file.py
--rw-r--r--   0        0        0     3694 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/filedevice.py
--rw-r--r--   0        0        0     1492 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/fileinfo.py
--rw-r--r--   0        0        0      560 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/fileselector.py
--rw-r--r--   0        0        0      879 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/filesystemwatcher.py
--rw-r--r--   0        0        0      188 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/identityproxymodel.py
--rw-r--r--   0        0        0     1379 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/iodevice.py
--rw-r--r--   0        0        0      122 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/itemselection.py
--rw-r--r--   0        0        0      176 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/itemselectionmodel.py
--rw-r--r--   0        0        0      696 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/itemselectionrange.py
--rw-r--r--   0        0        0     1677 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/jsondocument.py
--rw-r--r--   0        0        0      538 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/jsonvalue.py
--rw-r--r--   0        0        0      730 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/keycombination.py
--rw-r--r--   0        0        0     1248 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/library.py
--rw-r--r--   0        0        0     1585 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/libraryinfo.py
--rw-r--r--   0        0        0     1868 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/line.py
--rw-r--r--   0        0        0     1997 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/linef.py
--rw-r--r--   0        0        0      810 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/lockfile.py
--rw-r--r--   0        0        0      708 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/margins.py
--rw-r--r--   0        0        0      713 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/marginsf.py
--rw-r--r--   0        0        0     1110 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/metaenum.py
--rw-r--r--   0        0        0     1423 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/metamethod.py
--rw-r--r--   0        0        0     3903 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/metaobject.py
--rw-r--r--   0        0        0      511 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/metaproperty.py
--rw-r--r--   0        0        0     5404 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/metatype.py
--rw-r--r--   0        0        0     1802 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/mimedata.py
--rw-r--r--   0        0        0      948 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/mimedatabase.py
--rw-r--r--   0        0        0      208 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/mimetype.py
--rw-r--r--   0        0        0      176 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/modelindex.py
--rw-r--r--   0        0        0      336 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/mutex.py
--rw-r--r--   0        0        0     3583 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/object.py
--rw-r--r--   0        0        0     2562 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/operatingsystemversion.py
--rw-r--r--   0        0        0      356 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/parallelanimationgroup.py
--rw-r--r--   0        0        0      253 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/pauseanimation.py
--rw-r--r--   0        0        0      338 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/persistentmodelindex.py
--rw-r--r--   0        0        0      811 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/pluginloader.py
--rw-r--r--   0        0        0      349 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/point.py
--rw-r--r--   0        0        0      353 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/pointf.py
--rw-r--r--   0        0        0     4839 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/process.py
--rw-r--r--   0        0        0     1340 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/processenvironment.py
--rw-r--r--   0        0        0      774 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/propertyanimation.py
--rw-r--r--   0        0        0      126 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/randomgenerator.py
--rw-r--r--   0        0        0      231 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/randomgenerator64.py
--rw-r--r--   0        0        0      878 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/rect.py
--rw-r--r--   0        0        0      442 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/rectf.py
--rw-r--r--   0        0        0     6495 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/regularexpression.py
--rw-r--r--   0        0        0     2625 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/regularexpressionmatch.py
--rw-r--r--   0        0        0      613 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/regularexpressionmatchiterator.py
--rw-r--r--   0        0        0     1702 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/resource.py
--rw-r--r--   0        0        0      112 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/runnable.py
--rw-r--r--   0        0        0      160 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/savefile.py
--rw-r--r--   0        0        0      281 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/semaphore.py
--rw-r--r--   0        0        0      202 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/sequentialanimationgroup.py
--rw-r--r--   0        0        0     6990 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/settings.py
--rw-r--r--   0        0        0      122 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/signalblocker.py
--rw-r--r--   0        0        0      451 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/signalmapper.py
--rw-r--r--   0        0        0     1124 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/size.py
--rw-r--r--   0        0        0     1142 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/sizef.py
--rw-r--r--   0        0        0      471 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/slot.py
--rw-r--r--   0        0        0      930 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/socketnotifier.py
--rw-r--r--   0        0        0     2681 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/sortfilterproxymodel.py
--rw-r--r--   0        0        0     2622 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/standardpaths.py
--rw-r--r--   0        0        0     1184 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/storageinfo.py
--rw-r--r--   0        0        0      339 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/stringlistmodel.py
--rw-r--r--   0        0        0      980 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/temporarydir.py
--rw-r--r--   0        0        0      164 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/temporaryfile.py
--rw-r--r--   0        0        0     2583 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/textboundaryfinder.py
--rw-r--r--   0        0        0     3862 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/textstream.py
--rw-r--r--   0        0        0      108 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/thread.py
--rw-r--r--   0        0        0      160 2023-04-13 13:11:05.677482 prettyqt-1.5.0/prettyqt/core/threadpool.py
--rw-r--r--   0        0        0     2318 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/timeline.py
--rw-r--r--   0        0        0     1770 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/timer.py
--rw-r--r--   0        0        0     2198 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/timezone.py
--rw-r--r--   0        0        0     1722 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/translator.py
--rw-r--r--   0        0        0      190 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/transposeproxymodel.py
--rw-r--r--   0        0        0     3968 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/url.py
--rw-r--r--   0        0        0      770 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/urlquery.py
--rw-r--r--   0        0        0     1837 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/uuid.py
--rw-r--r--   0        0        0     1501 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/variantanimation.py
--rw-r--r--   0        0        0     2614 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/versionnumber.py
--rw-r--r--   0        0        0     2614 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/core/xmlstreamreader.py
--rw-r--r--   0        0        0      253 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_animations/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_animations/bounceanimation.py
--rw-r--r--   0        0        0      644 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_animations/fadeinanimation.py
--rw-r--r--   0        0        0      978 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_animations/slideanimation.py
--rw-r--r--   0        0        0      535 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/__init__.py
--rw-r--r--   0        0        0      887 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/buttondelegate.py
--rw-r--r--   0        0        0     1001 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/checkboxdelegate.py
--rw-r--r--   0        0        0     2570 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/icondelegate.py
--rw-r--r--   0        0        0      596 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/nofocusdelegate.py
--rw-r--r--   0        0        0     1474 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/progressbardelegate.py
--rw-r--r--   0        0        0     4789 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/radiodelegate.py
--rw-r--r--   0        0        0     2574 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/renderlinkdelegate.py
--rw-r--r--   0        0        0     6634 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_delegates/stardelegate.py
--rw-r--r--   0        0        0      735 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/__init__.py
--rw-r--r--   0        0        0     5965 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/columnitemmodel.py
--rw-r--r--   0        0        0     3285 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/importlibdistributionmodel.py
--rw-r--r--   0        0        0     4175 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/jsonmodel.py
--rw-r--r--   0        0        0     3083 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/listmixin.py
--rw-r--r--   0        0        0     2562 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/modelmixin.py
--rw-r--r--   0        0        0     2298 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/nesteditem.py
--rw-r--r--   0        0        0     2177 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/nestedmodel.py
--rw-r--r--   0        0        0     2126 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/regexmatchesmodel.py
--rw-r--r--   0        0        0     1698 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/selectionmixin.py
--rw-r--r--   0        0        0     5288 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/storageinfomodel.py
--rw-r--r--   0        0        0     2858 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py
--rw-r--r--   0        0        0      635 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/__init__.py
--rw-r--r--   0        0        0     2060 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/compositevalidator.py
--rw-r--r--   0        0        0     1114 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/integervalidator.py
--rw-r--r--   0        0        0      704 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/notemptyvalidator.py
--rw-r--r--   0        0        0      700 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/notzerovalidator.py
--rw-r--r--   0        0        0      620 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/pathvalidator.py
--rw-r--r--   0        0        0     1554 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/regexpatternvalidator.py
--rw-r--r--   0        0        0     3143 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_validators/regexvalidators.py
--rw-r--r--   0        0        0     2704 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/booldicttoolbutton.py
--rw-r--r--   0        0        0     7718 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/borderlayout.py
--rw-r--r--   0        0        0     3046 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/codeeditor.py
--rw-r--r--   0        0        0     2588 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/collapsibleframe.py
--rw-r--r--   0        0        0     2468 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/colorchooserbutton.py
--rw-r--r--   0        0        0     7462 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/completionwidget.py
--rw-r--r--   0        0        0    17651 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/dataset.py
--rw-r--r--   0        0        0     2219 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/elidedlabel.py
--rw-r--r--   0        0        0     3429 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/expandableline.py
--rw-r--r--   0        0        0     3194 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/filechooserbutton.py
--rw-r--r--   0        0        0     2155 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/flagselectionwidget.py
--rw-r--r--   0        0        0     3847 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/flowlayout.py
--rw-r--r--   0        0        0     2156 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/fontchooserbutton.py
--rw-r--r--   0        0        0     9381 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/framelesswindow.py
--rw-r--r--   0        0        0     5371 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/iconbrowser.py
--rw-r--r--   0        0        0     1311 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/iconlabel.py
--rw-r--r--   0        0        0     1661 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/iconwidget.py
--rw-r--r--   0        0        0     1292 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/image.py
--rw-r--r--   0        0        0      644 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/imageviewer.py
--rw-r--r--   0        0        0     1931 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/inputandslider.py
--rw-r--r--   0        0        0     2106 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/joystickbutton.py
--rw-r--r--   0        0        0     4165 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/labeledslider.py
--rw-r--r--   0        0        0     1214 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/listinput.py
--rw-r--r--   0        0        0     8209 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/logtextedit.py
--rw-r--r--   0        0        0      738 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/mappedcheckbox.py
--rw-r--r--   0        0        0     2388 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/markdownwidget.py
--rw-r--r--   0        0        0     6576 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/menurecentfiles.py
--rw-r--r--   0        0        0    18898 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/notification.py
--rw-r--r--   0        0        0     1038 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/optionalwidget.py
--rw-r--r--   0        0        0     1332 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/popupinfo.py
--rw-r--r--   0        0        0      145 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/__init__.py
--rw-r--r--   0        0        0      431 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/__main__.py
--rw-r--r--   0        0        0     1039 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/quick_ref.py
--rw-r--r--   0        0        0    19388 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/ref.html
--rw-r--r--   0        0        0     6186 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
--rw-r--r--   0        0        0     3145 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/regexinput.py
--rw-r--r--   0        0        0    10698 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/roundprogressbar.py
--rw-r--r--   0        0        0     4284 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/selectionwidget.py
--rw-r--r--   0        0        0     6345 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/sidebarwidget.py
--rw-r--r--   0        0        0     1036 2023-04-13 13:11:05.681482 prettyqt-1.5.0/prettyqt/custom_widgets/singlelinetextedit.py
--rw-r--r--   0        0        0    18739 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/spanslider.py
--rw-r--r--   0        0        0     1286 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/standardiconswidget.py
--rw-r--r--   0        0        0     2313 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/stringornumberwidget.py
--rw-r--r--   0        0        0     1774 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/subsequencecompleter.py
--rw-r--r--   0        0        0     8034 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/timeline.py
--rw-r--r--   0        0        0     9009 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/custom_widgets/waitingspinner.py
--rw-r--r--   0        0        0      255 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/eventfilters/__init__.py
--rw-r--r--   0        0        0     2613 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/eventfilters/animatedtooltipeventfilter.py
--rw-r--r--   0        0        0      751 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/eventfilters/hovericoneventfilter.py
--rw-r--r--   0        0        0     7915 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/__init__.py
--rw-r--r--   0        0        0     1051 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/abstractfileiconprovider.py
--rw-r--r--   0        0        0     1269 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/abstracttextdocumentlayout.py
--rw-r--r--   0        0        0      235 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/bitmap.py
--rw-r--r--   0        0        0     1451 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/brush.py
--rw-r--r--   0        0        0     2490 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/clipboard.py
--rw-r--r--   0        0        0     7636 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/color.py
--rw-r--r--   0        0        0     3045 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/colorspace.py
--rw-r--r--   0        0        0      485 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/conicalgradient.py
--rw-r--r--   0        0        0     1255 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/cursor.py
--rw-r--r--   0        0        0      439 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/desktopservices.py
--rw-r--r--   0        0        0     1094 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/doublevalidator.py
--rw-r--r--   0        0        0      973 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/drag.py
--rw-r--r--   0        0        0     9049 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/font.py
--rw-r--r--   0        0        0     4694 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/fontdatabase.py
--rw-r--r--   0        0        0      243 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/fontinfo.py
--rw-r--r--   0        0        0      889 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/fontmetrics.py
--rw-r--r--   0        0        0      719 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/fontmetricsf.py
--rw-r--r--   0        0        0     5331 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/gradient.py
--rw-r--r--   0        0        0     5027 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/guiapplication.py
--rw-r--r--   0        0        0     3986 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/icon.py
--rw-r--r--   0        0        0     4053 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/iconengine.py
--rw-r--r--   0        0        0     1630 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/image.py
--rw-r--r--   0        0        0     3778 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/imageiohandler.py
--rw-r--r--   0        0        0     3838 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/imagereader.py
--rw-r--r--   0        0        0     2791 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/imagewriter.py
--rw-r--r--   0        0        0     1315 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/inputmethod.py
--rw-r--r--   0        0        0      921 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/intvalidator.py
--rw-r--r--   0        0        0     6154 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/keysequence.py
--rw-r--r--   0        0        0      636 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/lineargradient.py
--rw-r--r--   0        0        0      302 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/matrix4x4.py
--rw-r--r--   0        0        0     1969 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/movie.py
--rw-r--r--   0        0        0      297 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pagedpaintdevice.py
--rw-r--r--   0        0        0     2923 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pagelayout.py
--rw-r--r--   0        0        0     7804 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pagesize.py
--rw-r--r--   0        0        0     1676 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/paintdevice.py
--rw-r--r--   0        0        0      319 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/paintdevicewindow.py
--rw-r--r--   0        0        0     7794 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/painter.py
--rw-r--r--   0        0        0     2425 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/painterpath.py
--rw-r--r--   0        0        0     1641 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/painterpathstroker.py
--rw-r--r--   0        0        0     5907 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/palette.py
--rw-r--r--   0        0        0     1026 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pdfwriter.py
--rw-r--r--   0        0        0     2841 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pen.py
--rw-r--r--   0        0        0      471 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/picture.py
--rw-r--r--   0        0        0     4827 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pixmap.py
--rw-r--r--   0        0        0      796 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/pixmapcache.py
--rw-r--r--   0        0        0     3489 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/polygon.py
--rw-r--r--   0        0        0     4325 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/polygonf.py
--rw-r--r--   0        0        0      898 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/radialgradient.py
--rw-r--r--   0        0        0      220 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/rasterwindow.py
--rw-r--r--   0        0        0     1145 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/region.py
--rw-r--r--   0        0        0     1290 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/regularexpressionvalidator.py
--rw-r--r--   0        0        0     2963 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/screen.py
--rw-r--r--   0        0        0     1291 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/sessionmanager.py
--rw-r--r--   0        0        0     6203 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/standarditem.py
--rw-r--r--   0        0        0     4778 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/standarditemmodel.py
--rw-r--r--   0        0        0     2225 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/statictext.py
--rw-r--r--   0        0        0     1146 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/stylehints.py
--rw-r--r--   0        0        0     1303 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/surface.py
--rw-r--r--   0        0        0     1352 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/syntaxhighlighter.py
--rw-r--r--   0        0        0     5255 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textblock.py
--rw-r--r--   0        0        0      623 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textblockgroup.py
--rw-r--r--   0        0        0      536 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textblockuserdata.py
--rw-r--r--   0        0        0     4878 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textcharformat.py
--rw-r--r--   0        0        0     5551 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textcursor.py
--rw-r--r--   0        0        0     8932 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textdocument.py
--rw-r--r--   0        0        0      949 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textdocumentfragment.py
--rw-r--r--   0        0        0     1062 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textdocumentwriter.py
--rw-r--r--   0        0        0     3262 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textformat.py
--rw-r--r--   0        0        0      534 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textframe.py
--rw-r--r--   0        0        0     3627 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textframeformat.py
--rw-r--r--   0        0        0      297 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textimageformat.py
--rw-r--r--   0        0        0      517 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textlayout.py
--rw-r--r--   0        0        0      725 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textlength.py
--rw-r--r--   0        0        0     1649 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textline.py
--rw-r--r--   0        0        0     1327 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textlistformat.py
--rw-r--r--   0        0        0      445 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textobject.py
--rw-r--r--   0        0        0      199 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textobjectinterface.py
--rw-r--r--   0        0        0     1560 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/textoption.py
--rw-r--r--   0        0        0     4104 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/texttablecellformat.py
--rw-r--r--   0        0        0     2482 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/transform.py
--rw-r--r--   0        0        0      640 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/undocommand.py
--rw-r--r--   0        0        0      356 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/undogroup.py
--rw-r--r--   0        0        0      957 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/undostack.py
--rw-r--r--   0        0        0      755 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/validator.py
--rw-r--r--   0        0        0      575 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/vector3d.py
--rw-r--r--   0        0        0      578 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/vector4d.py
--rw-r--r--   0        0        0     2338 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/gui/window.py
--rw-r--r--   0        0        0    10227 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/animation.py
--rw-r--r--   0        0        0     3079 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/awesomefileiconprovider.py
--rw-r--r--   0        0        0      539 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/awesomequickimageprovider.py
--rw-r--r--   0        0        0      832 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/chariconengine.py
--rw-r--r--   0        0        0    10996 2023-04-13 13:11:05.685483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/codicon-charmap.json
--rw-r--r--   0        0        0    68076 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/codicon.ttf
--rw-r--r--   0        0        0     7924 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
--rw-r--r--   0        0        0    79556 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
--rw-r--r--   0        0        0    11206 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
--rw-r--r--   0        0        0   134316 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
--rw-r--r--   0        0        0     3947 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
--rw-r--r--   0        0        0    33692 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
--rw-r--r--   0        0        0    25663 2023-04-13 13:11:05.689483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
--rw-r--r--   0        0        0   203644 2023-04-13 13:11:05.693483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
--rw-r--r--   0        0        0   200215 2023-04-13 13:11:05.693483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
--rw-r--r--   0        0        0  1026284 2023-04-13 13:11:05.701483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
--rw-r--r--   0        0        0   216192 2023-04-13 13:11:05.701483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
--rw-r--r--   0        0        0  1108672 2023-04-13 13:11:05.705483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
--rw-r--r--   0        0        0   151941 2023-04-13 13:11:05.705483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/phosphor-charmap.json
--rw-r--r--   0        0        0  1392088 2023-04-13 13:11:05.713483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/phosphor.ttf
--rw-r--r--   0        0        0    72655 2023-04-13 13:11:05.713483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/remixicon-charmap.json
--rw-r--r--   0        0        0   403056 2023-04-13 13:11:05.717483 prettyqt-1.5.0/prettyqt/iconprovider/fonts/remixicon.ttf
--rw-r--r--   0        0        0     8417 2023-04-13 13:11:05.717483 prettyqt-1.5.0/prettyqt/iconprovider/iconic_font.py
--rw-r--r--   0        0        0     2468 2023-04-13 13:11:05.717483 prettyqt-1.5.0/prettyqt/iconprovider/svgbuffericonengine.py
--rw-r--r--   0        0        0   154232 2023-04-13 13:11:05.717483 prettyqt-1.5.0/prettyqt/localization/language_ar.qm
--rw-r--r--   0        0        0   155315 2023-04-13 13:11:05.717483 prettyqt-1.5.0/prettyqt/localization/language_bg.qm
--rw-r--r--   0        0        0   178552 2023-04-13 13:11:05.721483 prettyqt-1.5.0/prettyqt/localization/language_ca.qm
--rw-r--r--   0        0        0   151054 2023-04-13 13:11:05.721483 prettyqt-1.5.0/prettyqt/localization/language_cs.qm
--rw-r--r--   0        0        0   179910 2023-04-13 13:11:05.721483 prettyqt-1.5.0/prettyqt/localization/language_da.qm
--rw-r--r--   0        0        0   212675 2023-04-13 13:11:05.721483 prettyqt-1.5.0/prettyqt/localization/language_de.qm
--rw-r--r--   0        0        0   154543 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_es.qm
--rw-r--r--   0        0        0    97872 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_fa.qm
--rw-r--r--   0        0        0   174500 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_fi.qm
--rw-r--r--   0        0        0   154190 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_fr.qm
--rw-r--r--   0        0        0   183091 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_gd.qm
--rw-r--r--   0        0        0   108600 2023-04-13 13:11:05.725483 prettyqt-1.5.0/prettyqt/localization/language_gl.qm
--rw-r--r--   0        0        0   130568 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_he.qm
--rw-r--r--   0        0        0   150033 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_hu.qm
--rw-r--r--   0        0        0   153570 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_it.qm
--rw-r--r--   0        0        0   122385 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_ja.qm
--rw-r--r--   0        0        0   120318 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_ko.qm
--rw-r--r--   0        0        0    90502 2023-04-13 13:11:05.729483 prettyqt-1.5.0/prettyqt/localization/language_lt.qm
--rw-r--r--   0        0        0   143558 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_lv.qm
--rw-r--r--   0        0        0   161318 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_pl.qm
--rw-r--r--   0        0        0    50541 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_pt.qm
--rw-r--r--   0        0        0   197476 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_ru.qm
--rw-r--r--   0        0        0   115250 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_sk.qm
--rw-r--r--   0        0        0    96357 2023-04-13 13:11:05.733483 prettyqt-1.5.0/prettyqt/localization/language_sl.qm
--rw-r--r--   0        0        0    47206 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/localization/language_sv.qm
--rw-r--r--   0        0        0   148437 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/localization/language_uk.qm
--rw-r--r--   0        0        0    61089 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/localization/language_zh_CN.qm
--rw-r--r--   0        0        0   125250 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/localization/language_zh_TW.qm
--rw-r--r--   0        0        0     2384 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/__init__.py
--rw-r--r--   0        0        0      387 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/geocodingmanager.py
--rw-r--r--   0        0        0     2867 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/geomaneuver.py
--rw-r--r--   0        0        0     1055 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/georoute.py
--rw-r--r--   0        0        0     5266 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/georouterequest.py
--rw-r--r--   0        0        0      657 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/georoutesegment.py
--rw-r--r--   0        0        0     2021 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/georoutingmanager.py
--rw-r--r--   0        0        0     5880 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/geoserviceprovider.py
--rw-r--r--   0        0        0     2387 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/place.py
--rw-r--r--   0        0        0      864 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeattribute.py
--rw-r--r--   0        0        0      737 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placecategory.py
--rw-r--r--   0        0        0      844 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placecontactdetail.py
--rw-r--r--   0        0        0     1030 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placecontent.py
--rw-r--r--   0        0        0     1275 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placecontentreply.py
--rw-r--r--   0        0        0      947 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placecontentrequest.py
--rw-r--r--   0        0        0      562 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placedetailsreply.py
--rw-r--r--   0        0        0      849 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeicon.py
--rw-r--r--   0        0        0     1185 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeidreply.py
--rw-r--r--   0        0        0     2233 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placemanager.py
--rw-r--r--   0        0        0     1066 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placematchreply.py
--rw-r--r--   0        0        0      726 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placematchrequest.py
--rw-r--r--   0        0        0      223 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeproposedsearchresult.py
--rw-r--r--   0        0        0      316 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeratings.py
--rw-r--r--   0        0        0     1923 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placereply.py
--rw-r--r--   0        0        0      267 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeresult.py
--rw-r--r--   0        0        0     1651 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placesearchreply.py
--rw-r--r--   0        0        0     2230 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placesearchrequest.py
--rw-r--r--   0        0        0      884 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placesearchresult.py
--rw-r--r--   0        0        0      675 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placesupplier.py
--rw-r--r--   0        0        0      215 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/placeuser.py
--rw-r--r--   0        0        0      621 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/location/qlocation.py
--rw-r--r--   0        0        0      167 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/multimediawidgets/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/multimediawidgets/graphicsvideoitem.py
--rw-r--r--   0        0        0      872 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/multimediawidgets/videowidget.py
--rw-r--r--   0        0        0     1172 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/__init__.py
--rw-r--r--   0        0        0     8113 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/abstractsocket.py
--rw-r--r--   0        0        0     1775 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/hostaddress.py
--rw-r--r--   0        0        0     1465 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/httpmultipart.py
--rw-r--r--   0        0        0      823 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/httppart.py
--rw-r--r--   0        0        0     1310 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/localserver.py
--rw-r--r--   0        0        0     2392 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/localsocket.py
--rw-r--r--   0        0        0     2313 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkaccessmanager.py
--rw-r--r--   0        0        0     2000 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkaddressentry.py
--rw-r--r--   0        0        0     1551 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkcookie.py
--rw-r--r--   0        0        0      850 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkcookiejar.py
--rw-r--r--   0        0        0      627 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkdatagram.py
--rw-r--r--   0        0        0     3011 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkinterface.py
--rw-r--r--   0        0        0     3361 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkproxy.py
--rw-r--r--   0        0        0     6462 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/networkrequest.py
--rw-r--r--   0        0        0      779 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/tcpserver.py
--rw-r--r--   0        0        0      178 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/tcpsocket.py
--rw-r--r--   0        0        0      671 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/network/udpsocket.py
--rw-r--r--   0        0        0       26 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/objbrowser/__init__.py
--rw-r--r--   0        0        0     9193 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/objbrowser/attribute_model.py
--rw-r--r--   0        0        0    14897 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/objbrowser/objectbrowser.py
--rw-r--r--   0        0        0    18451 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/objbrowser/objectbrowsertreemodel.py
--rw-r--r--   0        0        0      356 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/paths.py
--rw-r--r--   0        0        0     1169 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/__init__.py
--rw-r--r--   0        0        0      171 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geoaddress.py
--rw-r--r--   0        0        0     1149 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geoareamonitorinfo.py
--rw-r--r--   0        0        0     1260 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geoareamonitorsource.py
--rw-r--r--   0        0        0     1072 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geocircle.py
--rw-r--r--   0        0        0     1172 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geocoordinate.py
--rw-r--r--   0        0        0      558 2023-04-13 13:11:05.737484 prettyqt-1.5.0/prettyqt/positioning/geolocation.py
--rw-r--r--   0        0        0     1021 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geopath.py
--rw-r--r--   0        0        0     1145 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geopolygon.py
--rw-r--r--   0        0        0     1687 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geopositioninfo.py
--rw-r--r--   0        0        0     2960 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geopositioninfosource.py
--rw-r--r--   0        0        0      769 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/georectangle.py
--rw-r--r--   0        0        0     1861 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geosatelliteinfo.py
--rw-r--r--   0        0        0     1110 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geosatelliteinfosource.py
--rw-r--r--   0        0        0      755 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/geoshape.py
--rw-r--r--   0        0        0     1196 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/positioning/nmeapositioninginfosource.py
--rw-r--r--   0        0        0        0 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/py.typed
--rw-r--r--   0        0        0      943 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/jsengine.py
--rw-r--r--   0        0        0     2397 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/jsvalue.py
--rw-r--r--   0        0        0      295 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/jsvalueiterator.py
--rw-r--r--   0        0        0      955 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/qmlapplicationengine.py
--rw-r--r--   0        0        0      907 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/qmlcomponent.py
--rw-r--r--   0        0        0     2020 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/qmlengine.py
--rw-r--r--   0        0        0      536 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/qmlimageproviderbase.py
--rw-r--r--   0        0        0      185 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qml/qmlparserstatus.py
--rw-r--r--   0        0        0      203 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/Qsci/__init__.py
--rw-r--r--   0        0        0      213 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtBluetooth/__init__.py
--rw-r--r--   0        0        0      446 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtCharts/__init__.py
--rw-r--r--   0        0        0     2281 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtCore/__init__.py
--rw-r--r--   0        0        0      690 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtGui/__init__.py
--rw-r--r--   0        0        0      253 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtHelp/__init__.py
--rw-r--r--   0        0        0      281 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtLocation/__init__.py
--rw-r--r--   0        0        0      271 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtMultimedia/__init__.py
--rw-r--r--   0        0        0      292 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtMultimediaWidgets/__init__.py
--rw-r--r--   0        0        0      278 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtNetwork/__init__.py
--rw-r--r--   0        0        0      274 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtPositioning/__init__.py
--rw-r--r--   0        0        0      266 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtQml/__init__.py
--rw-r--r--   0        0        0      272 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtQuick/__init__.py
--rw-r--r--   0        0        0      256 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtScxml/__init__.py
--rw-r--r--   0        0        0      274 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtStateMachine/__init__.py
--rw-r--r--   0        0        0      332 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtSvg/__init__.py
--rw-r--r--   0        0        0      269 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtTest/__init__.py
--rw-r--r--   0        0        0      277 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtTextToSpeech/__init__.py
--rw-r--r--   0        0        0      368 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtUiTools/__init__.py
--rw-r--r--   0        0        0      274 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtWebChannel/__init__.py
--rw-r--r--   0        0        0      280 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtWebEngineCore/__init__.py
--rw-r--r--   0        0        0      289 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtWebEngineWidgets/__init__.py
--rw-r--r--   0        0        0     1548 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/QtWidgets/__init__.py
--rw-r--r--   0        0        0     1200 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qt/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/__init__.py
--rw-r--r--   0        0        0      399 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpcontentitem.py
--rw-r--r--   0        0        0      443 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpcontentmodel.py
--rw-r--r--   0        0        0      460 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpcontentwidget.py
--rw-r--r--   0        0        0      371 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpengine.py
--rw-r--r--   0        0        0     1107 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpenginecore.py
--rw-r--r--   0        0        0      661 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpfilterdata.py
--rw-r--r--   0        0        0      739 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpfilterengine.py
--rw-r--r--   0        0        0      177 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpindexmodel.py
--rw-r--r--   0        0        0      178 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpindexwidget.py
--rw-r--r--   0        0        0      729 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpsearchengine.py
--rw-r--r--   0        0        0      188 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpsearchquerywidget.py
--rw-r--r--   0        0        0      216 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpsearchresult.py
--rw-r--r--   0        0        0      832 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qthelp/helpsearchresultwidget.py
--rw-r--r--   0        0        0     8336 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/qtre.py
--rw-r--r--   0        0        0      868 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/__init__.py
--rw-r--r--   0        0        0      208 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickasyncimageprovider.py
--rw-r--r--   0        0        0      257 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickimageprovider.py
--rw-r--r--   0        0        0      239 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickimageresponse.py
--rw-r--r--   0        0        0     3753 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickitem.py
--rw-r--r--   0        0        0      519 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickitemgrabresult.py
--rw-r--r--   0        0        0     1495 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickpainteditem.py
--rw-r--r--   0        0        0      239 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickrendercontrol.py
--rw-r--r--   0        0        0      271 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quicktextdocument.py
--rw-r--r--   0        0        0     1204 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickview.py
--rw-r--r--   0        0        0     3624 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/quick/quickwindow.py
--rw-r--r--   0        0        0      123 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/scintilla/__init__.py
--rw-r--r--   0        0        0     9347 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/scintilla/sciscintilla.py
--rw-r--r--   0        0        0      193 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/scxml/__init__.py
--rw-r--r--   0        0        0      362 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/scxml/scxmlcompiler.py
--rw-r--r--   0        0        0      176 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/scxml/scxmlstatemachine.py
--rw-r--r--   0        0        0      785 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/__init__.py
--rw-r--r--   0        0        0      361 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/abstractstate.py
--rw-r--r--   0        0        0     1159 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/abstracttransition.py
--rw-r--r--   0        0        0      220 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/eventtransition.py
--rw-r--r--   0        0        0      199 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/finalstate.py
--rw-r--r--   0        0        0     1104 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/historystate.py
--rw-r--r--   0        0        0      223 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/keyeventtransition.py
--rw-r--r--   0        0        0      227 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/mouseeventtransition.py
--rw-r--r--   0        0        0      222 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/signaltransition.py
--rw-r--r--   0        0        0     1276 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/state.py
--rw-r--r--   0        0        0     2222 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/statemachine/statemachine.py
--rw-r--r--   0        0        0      170 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/svg/__init__.py
--rw-r--r--   0        0        0      182 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/svg/graphicssvgitem.py
--rw-r--r--   0        0        0      405 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/svg/svggenerator.py
--rw-r--r--   0        0        0     1080 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/svg/svgrenderer.py
--rw-r--r--   0        0        0      279 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/svg/svgwidget.py
--rw-r--r--   0        0        0      675 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/highlightrule.py
--rw-r--r--   0        0        0     1271 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/jsonhighlighter.py
--rw-r--r--   0        0        0     3178 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/markdownhighlighter.py
--rw-r--r--   0        0        0      872 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
--rw-r--r--   0        0        0     8585 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py
--rw-r--r--   0        0        0     4836 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/pythonhighlighter.py
--rw-r--r--   0        0        0     2079 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
--rw-r--r--   0        0        0     2192 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/xmlhighlighter.py
--rw-r--r--   0        0        0     2106 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/syntaxhighlighters/yamlhighlighter.py
--rw-r--r--   0        0        0      180 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/texttospeech/__init__.py
--rw-r--r--   0        0        0     1328 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/texttospeech/texttospeech.py
--rw-r--r--   0        0        0      944 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/texttospeech/voice.py
--rw-r--r--   0        0        0    15547 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/themes/darktheme.qss
--rw-r--r--   0        0        0      845 2023-04-13 13:11:05.741484 prettyqt-1.5.0/prettyqt/utils/__init__.py
--rw-r--r--   0        0        0     3561 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/autoslot.py
--rw-r--r--   0        0        0     3307 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/colors.py
--rw-r--r--   0        0        0     2161 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/debugging.py
--rw-r--r--   0        0        0     3598 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/helpers.py
--rw-r--r--   0        0        0      894 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/mappers.py
--rw-r--r--   0        0        0     1054 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/prettyprinter.py
--rw-r--r--   0        0        0     5546 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/searchandreplacemixin.py
--rw-r--r--   0        0        0      629 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/signallogger.py
--rw-r--r--   0        0        0     2306 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/singleapplication.py
--rw-r--r--   0        0        0      493 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/singleton.py
--rw-r--r--   0        0        0     2110 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/syncedproperty.py
--rw-r--r--   0        0        0     1887 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/treeitem.py
--rw-r--r--   0        0        0     4119 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/utils/types.py
--rw-r--r--   0        0        0      303 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webchannel/__init__.py
--rw-r--r--   0        0        0      228 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webchannel/webchannel.py
--rw-r--r--   0        0        0     1337 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/__init__.py
--rw-r--r--   0        0        0     3315 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginecontextmenurequest.py
--rw-r--r--   0        0        0     4498 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginedownloadrequest.py
--rw-r--r--   0        0        0     1299 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginehistory.py
--rw-r--r--   0        0        0      422 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginehistoryitem.py
--rw-r--r--   0        0        0     1776 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginehttprequest.py
--rw-r--r--   0        0        0    14262 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginepage.py
--rw-r--r--   0        0        0     2461 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webengineprofile.py
--rw-r--r--   0        0        0     1574 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginescript.py
--rw-r--r--   0        0        0     1278 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginescriptcollection.py
--rw-r--r--   0        0        0     7469 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webenginesettings.py
--rw-r--r--   0        0        0     2044 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webengineurlscheme.py
--rw-r--r--   0        0        0      282 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginecore/webengineurlschemehandler.py
--rw-r--r--   0        0        0      330 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginewidgets/__init__.py
--rw-r--r--   0        0        0     4602 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/webenginewidgets/webengineview.py
--rw-r--r--   0        0        0    13448 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/__init__.py
--rw-r--r--   0        0        0     3797 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractbutton.py
--rw-r--r--   0        0        0      406 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractgraphicsshapeitem.py
--rw-r--r--   0        0        0      257 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractitemdelegate.py
--rw-r--r--   0        0        0    11883 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractitemview.py
--rw-r--r--   0        0        0     5361 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractscrollarea.py
--rw-r--r--   0        0        0     5646 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractslider.py
--rw-r--r--   0        0        0     3715 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/abstractspinbox.py
--rw-r--r--   0        0        0     8208 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/action.py
--rw-r--r--   0        0        0     2143 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/actiongroup.py
--rw-r--r--   0        0        0     8020 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/application.py
--rw-r--r--   0        0        0     2754 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/boxlayout.py
--rw-r--r--   0        0        0      342 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/buttongroup.py
--rw-r--r--   0        0        0     2960 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/calendarwidget.py
--rw-r--r--   0        0        0     1647 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/checkbox.py
--rw-r--r--   0        0        0     3856 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/colordialog.py
--rw-r--r--   0        0        0      331 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/columnview.py
--rw-r--r--   0        0        0     7000 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/combobox.py
--rw-r--r--   0        0        0      365 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/commandlinkbutton.py
--rw-r--r--   0        0        0      281 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/commonstyle.py
--rw-r--r--   0        0        0     3501 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/completer.py
--rw-r--r--   0        0        0     2700 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/datawidgetmapper.py
--rw-r--r--   0        0        0     1412 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/dateedit.py
--rw-r--r--   0        0        0     4324 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/datetimeedit.py
--rw-r--r--   0        0        0     1079 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/dial.py
--rw-r--r--   0        0        0     2813 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/dialog.py
--rw-r--r--   0        0        0     5950 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/dialogbuttonbox.py
--rw-r--r--   0        0        0     2356 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/dockwidget.py
--rw-r--r--   0        0        0     1772 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/doublespinbox.py
--rw-r--r--   0        0        0      328 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/errormessage.py
--rw-r--r--   0        0        0     7417 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/filedialog.py
--rw-r--r--   0        0        0      805 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/fileiconprovider.py
--rw-r--r--   0        0        0     3484 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/filesystemmodel.py
--rw-r--r--   0        0        0      289 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/focusframe.py
--rw-r--r--   0        0        0     2477 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/fontcombobox.py
--rw-r--r--   0        0        0      363 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/fontdialog.py
--rw-r--r--   0        0        0     5000 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/formlayout.py
--rw-r--r--   0        0        0     2540 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/frame.py
--rw-r--r--   0        0        0     1822 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/gesture.py
--rw-r--r--   0        0        0     2334 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsanchorlayout.py
--rw-r--r--   0        0        0     1360 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsblureffect.py
--rw-r--r--   0        0        0      469 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicscolorizeeffect.py
--rw-r--r--   0        0        0      435 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsdropshadoweffect.py
--rw-r--r--   0        0        0      416 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicseffect.py
--rw-r--r--   0        0        0      559 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsellipseitem.py
--rw-r--r--   0        0        0     3589 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsgridlayout.py
--rw-r--r--   0        0        0     4923 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsitem.py
--rw-r--r--   0        0        0      192 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicsitemgroup.py
--rw-r--r--   0        0        0     1173 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicslayout.py
--rw-r--r--   0        0        0      262 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicslayoutitem.py
--rw-r--r--   0        0        0     1098 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicslinearlayout.py
--rw-r--r--   0        0        0      651 2023-04-13 13:11:05.745484 prettyqt-1.5.0/prettyqt/widgets/graphicslineitem.py
--rw-r--r--   0        0        0      700 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsobject.py
--rw-r--r--   0        0        0      538 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsopacityeffect.py
--rw-r--r--   0        0        0      209 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicspathitem.py
--rw-r--r--   0        0        0     2241 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicspixmapitem.py
--rw-r--r--   0        0        0      800 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicspolygonitem.py
--rw-r--r--   0        0        0      198 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsproxywidget.py
--rw-r--r--   0        0        0      542 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsrectitem.py
--rw-r--r--   0        0        0      754 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsrotation.py
--rw-r--r--   0        0        0      490 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsscale.py
--rw-r--r--   0        0        0     8525 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsscene.py
--rw-r--r--   0        0        0      293 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicssimpletextitem.py
--rw-r--r--   0        0        0      707 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicstextitem.py
--rw-r--r--   0        0        0      310 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicstransform.py
--rw-r--r--   0        0        0     8619 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicsview.py
--rw-r--r--   0        0        0     2770 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/graphicswidget.py
--rw-r--r--   0        0        0     4159 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/gridlayout.py
--rw-r--r--   0        0        0     1955 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/groupbox.py
--rw-r--r--   0        0        0     5318 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/headerview.py
--rw-r--r--   0        0        0     3755 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/inputdialog.py
--rw-r--r--   0        0        0      190 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/itemdelegate.py
--rw-r--r--   0        0        0      144 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/itemeditorcreatorbase.py
--rw-r--r--   0        0        0     2331 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/itemeditorfactory.py
--rw-r--r--   0        0        0      846 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/keysequenceedit.py
--rw-r--r--   0        0        0     8483 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/label.py
--rw-r--r--   0        0        0     3961 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/layout.py
--rw-r--r--   0        0        0     1272 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/layoutitem.py
--rw-r--r--   0        0        0     2416 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/lcdnumber.py
--rw-r--r--   0        0        0     6546 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/lineedit.py
--rw-r--r--   0        0        0     5606 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/listview.py
--rw-r--r--   0        0        0     5823 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/listwidget.py
--rw-r--r--   0        0        0     3690 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/listwidgetitem.py
--rw-r--r--   0        0        0     6705 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/mainwindow.py
--rw-r--r--   0        0        0     4591 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/mdiarea.py
--rw-r--r--   0        0        0      689 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/mdisubwindow.py
--rw-r--r--   0        0        0     4397 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/menu.py
--rw-r--r--   0        0        0     2145 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/menubar.py
--rw-r--r--   0        0        0     7314 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/messagebox.py
--rw-r--r--   0        0        0      542 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/pangesture.py
--rw-r--r--   0        0        0     1902 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/pinchgesture.py
--rw-r--r--   0        0        0      415 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/plaintextdocumentlayout.py
--rw-r--r--   0        0        0     9079 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/plaintextedit.py
--rw-r--r--   0        0        0     3564 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/progressbar.py
--rw-r--r--   0        0        0     1029 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/progressdialog.py
--rw-r--r--   0        0        0      231 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/proxystyle.py
--rw-r--r--   0        0        0      804 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/pushbutton.py
--rw-r--r--   0        0        0      517 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/radiobutton.py
--rw-r--r--   0        0        0      758 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/rubberband.py
--rw-r--r--   0        0        0      611 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/scrollarea.py
--rw-r--r--   0        0        0      707 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/scrollbar.py
--rw-r--r--   0        0        0     3060 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/scroller.py
--rw-r--r--   0        0        0     3937 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/scrollerproperties.py
--rw-r--r--   0        0        0     1399 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/shortcut.py
--rw-r--r--   0        0        0      309 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/sizegrip.py
--rw-r--r--   0        0        0     5373 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/sizepolicy.py
--rw-r--r--   0        0        0     2654 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/slider.py
--rw-r--r--   0        0        0     1297 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/spaceritem.py
--rw-r--r--   0        0        0     1837 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/spinbox.py
--rw-r--r--   0        0        0     1181 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/splashscreen.py
--rw-r--r--   0        0        0     3920 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/splitter.py
--rw-r--r--   0        0        0     1417 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/splitterhandle.py
--rw-r--r--   0        0        0      983 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/stackedlayout.py
--rw-r--r--   0        0        0     1372 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/stackedwidget.py
--rw-r--r--   0        0        0     1700 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/statusbar.py
--rw-r--r--   0        0        0    19383 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/style.py
--rw-r--r--   0        0        0      208 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleditemdelegate.py
--rw-r--r--   0        0        0      126 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/stylefactory.py
--rw-r--r--   0        0        0      318 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoption.py
--rw-r--r--   0        0        0      686 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionbutton.py
--rw-r--r--   0        0        0      208 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptioncombobox.py
--rw-r--r--   0        0        0      260 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptioncomplex.py
--rw-r--r--   0        0        0      199 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiondockwidget.py
--rw-r--r--   0        0        0      197 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionfocusrect.py
--rw-r--r--   0        0        0      189 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionframe.py
--rw-r--r--   0        0        0      209 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiongraphicsitem.py
--rw-r--r--   0        0        0      197 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiongroupbox.py
--rw-r--r--   0        0        0      911 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionheader.py
--rw-r--r--   0        0        0     1032 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionmenuitem.py
--rw-r--r--   0        0        0      201 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionprogressbar.py
--rw-r--r--   0        0        0      199 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionrubberband.py
--rw-r--r--   0        0        0      208 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionsizegrip.py
--rw-r--r--   0        0        0     1046 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionslider.py
--rw-r--r--   0        0        0      195 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionspinbox.py
--rw-r--r--   0        0        0     1135 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontab.py
--rw-r--r--   0        0        0      199 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontabbarbase.py
--rw-r--r--   0        0        0      213 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontabwidgetframe.py
--rw-r--r--   0        0        0      197 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontitlebar.py
--rw-r--r--   0        0        0      397 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontoolbar.py
--rw-r--r--   0        0        0     1180 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontoolbox.py
--rw-r--r--   0        0        0      201 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptiontoolbutton.py
--rw-r--r--   0        0        0     1344 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/styleoptionviewitem.py
--rw-r--r--   0        0        0      397 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/stylepainter.py
--rw-r--r--   0        0        0     1311 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/swipegesture.py
--rw-r--r--   0        0        0     1732 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/systemtrayicon.py
--rw-r--r--   0        0        0     5232 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tabbar.py
--rw-r--r--   0        0        0     3112 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tableview.py
--rw-r--r--   0        0        0     1085 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tablewidget.py
--rw-r--r--   0        0        0     3334 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tablewidgetitem.py
--rw-r--r--   0        0        0     1920 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tablewidgetselectionrange.py
--rw-r--r--   0        0        0    10591 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tabwidget.py
--rw-r--r--   0        0        0      392 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tapandholdgesture.py
--rw-r--r--   0        0        0      371 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/tapgesture.py
--rw-r--r--   0        0        0     2400 2023-04-13 13:11:05.749484 prettyqt-1.5.0/prettyqt/widgets/textbrowser.py
--rw-r--r--   0        0        0     6089 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/textedit.py
--rw-r--r--   0        0        0     1526 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/timeedit.py
--rw-r--r--   0        0        0     5008 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/toolbar.py
--rw-r--r--   0        0        0     2568 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/toolbox.py
--rw-r--r--   0        0        0     3175 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/toolbutton.py
--rw-r--r--   0        0        0      710 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/tooltip.py
--rw-r--r--   0        0        0     2532 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/treeview.py
--rw-r--r--   0        0        0      630 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/treewidget.py
--rw-r--r--   0        0        0     4841 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/treewidgetitem.py
--rw-r--r--   0        0        0     4142 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/treewidgetitemiterator.py
--rw-r--r--   0        0        0     1003 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/undoview.py
--rw-r--r--   0        0        0      552 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/whatsthis.py
--rw-r--r--   0        0        0    19395 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/widget.py
--rw-r--r--   0        0        0      545 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/widgetaction.py
--rw-r--r--   0        0        0      248 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/widgetitem.py
--rw-r--r--   0        0        0     9052 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/wizard.py
--rw-r--r--   0        0        0     1997 2023-04-13 13:11:05.753484 prettyqt-1.5.0/prettyqt/widgets/wizardpage.py
--rw-r--r--   0        0        0     4492 2023-04-13 13:11:05.753484 prettyqt-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 prettyqt-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-16 21:30:19.293854 prettyqt-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2746 2023-04-16 21:30:19.293854 prettyqt-1.6.0/docs/index.md
+-rw-r--r--   0        0        0      687 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/__pyinstaller/hook-prettyqt.py
+-rw-r--r--   0        0        0      517 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/bluetoothaddress.py
+-rw-r--r--   0        0        0     2635 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
+-rw-r--r--   0        0        0     1421 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
+-rw-r--r--   0        0        0     1872 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/bluetoothserviceinfo.py
+-rw-r--r--   0        0        0    11927 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/bluetooth/bluetoothuuid.py
+-rw-r--r--   0        0        0     1792 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/abstractaxis.py
+-rw-r--r--   0        0        0     1603 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/abstractbarseries.py
+-rw-r--r--   0        0        0      554 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/abstractseries.py
+-rw-r--r--   0        0        0      517 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/barcategoryaxis.py
+-rw-r--r--   0        0        0      177 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/barseries.py
+-rw-r--r--   0        0        0      932 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/barset.py
+-rw-r--r--   0        0        0     1648 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/boxset.py
+-rw-r--r--   0        0        0      609 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/candlestickset.py
+-rw-r--r--   0        0        0     1767 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/categoryaxis.py
+-rw-r--r--   0        0        0     5315 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/chart.py
+-rw-r--r--   0        0        0     5082 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/chartview.py
+-rw-r--r--   0        0        0      381 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/datetimeaxis.py
+-rw-r--r--   0        0        0      197 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/horizontalbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/horizontalpercentbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-16 21:30:19.293854 prettyqt-1.6.0/prettyqt/charts/horizontalstackedbarseries.py
+-rw-r--r--   0        0        0     2742 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/legend.py
+-rw-r--r--   0        0        0      673 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/lineseries.py
+-rw-r--r--   0        0        0      178 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/logvalueaxis.py
+-rw-r--r--   0        0        0      191 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/percentbarseries.py
+-rw-r--r--   0        0        0     2038 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/pieslice.py
+-rw-r--r--   0        0        0      739 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/polarchart.py
+-rw-r--r--   0        0        0      176 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/scatterseries.py
+-rw-r--r--   0        0        0      191 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/stackedbarseries.py
+-rw-r--r--   0        0        0     1044 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/valueaxis.py
+-rw-r--r--   0        0        0     1219 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/charts/xyseries.py
+-rw-r--r--   0        0        0    50840 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/constants/__init__.py
+-rw-r--r--   0        0        0     8699 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/_calendar.py
+-rw-r--r--   0        0        0     2000 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/_datetime.py
+-rw-r--r--   0        0        0    16492 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/_locale.py
+-rw-r--r--   0        0        0      478 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/_time.py
+-rw-r--r--   0        0        0     3286 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstractanimation.py
+-rw-r--r--   0        0        0      186 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstracteventdispatcher.py
+-rw-r--r--   0        0        0     5260 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstractitemmodel.py
+-rw-r--r--   0        0        0      250 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstractlistmodel.py
+-rw-r--r--   0        0        0      146 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstractnativeeventfilter.py
+-rw-r--r--   0        0        0      632 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstractproxymodel.py
+-rw-r--r--   0        0        0      254 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/abstracttablemodel.py
+-rw-r--r--   0        0        0     2060 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/animationgroup.py
+-rw-r--r--   0        0        0      533 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/basictimer.py
+-rw-r--r--   0        0        0      154 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/buffer.py
+-rw-r--r--   0        0        0      173 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/bytearray.py
+-rw-r--r--   0        0        0      369 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/bytearraymatcher.py
+-rw-r--r--   0        0        0      959 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/collator.py
+-rw-r--r--   0        0        0      126 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/collatorsortkey.py
+-rw-r--r--   0        0        0      324 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/commandlineoption.py
+-rw-r--r--   0        0        0     2231 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/commandlineparser.py
+-rw-r--r--   0        0        0      211 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/concatenatetablesproxymodel.py
+-rw-r--r--   0        0        0     3729 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/coreapplication.py
+-rw-r--r--   0        0        0     2038 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/cryptographichash.py
+-rw-r--r--   0        0        0     3426 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/datastream.py
+-rw-r--r--   0        0        0      470 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/date.py
+-rw-r--r--   0        0        0      766 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/deadlinetimer.py
+-rw-r--r--   0        0        0     1153 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/debug.py
+-rw-r--r--   0        0        0     4467 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/dir.py
+-rw-r--r--   0        0        0      949 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/diriterator.py
+-rw-r--r--   0        0        0     4527 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/easingcurve.py
+-rw-r--r--   0        0        0      918 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/elapsedtimer.py
+-rw-r--r--   0        0        0     7128 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/event.py
+-rw-r--r--   0        0        0     1225 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/eventloop.py
+-rw-r--r--   0        0        0      191 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/file.py
+-rw-r--r--   0        0        0     3694 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/filedevice.py
+-rw-r--r--   0        0        0     1492 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/fileinfo.py
+-rw-r--r--   0        0        0      560 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/fileselector.py
+-rw-r--r--   0        0        0      879 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/filesystemwatcher.py
+-rw-r--r--   0        0        0      188 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/identityproxymodel.py
+-rw-r--r--   0        0        0     1379 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/iodevice.py
+-rw-r--r--   0        0        0      122 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/itemselection.py
+-rw-r--r--   0        0        0      176 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/itemselectionmodel.py
+-rw-r--r--   0        0        0      696 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/itemselectionrange.py
+-rw-r--r--   0        0        0     1677 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/jsondocument.py
+-rw-r--r--   0        0        0      538 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/jsonvalue.py
+-rw-r--r--   0        0        0      730 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/keycombination.py
+-rw-r--r--   0        0        0     1248 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/library.py
+-rw-r--r--   0        0        0     1585 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/libraryinfo.py
+-rw-r--r--   0        0        0     1868 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/line.py
+-rw-r--r--   0        0        0     1997 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/linef.py
+-rw-r--r--   0        0        0      810 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/lockfile.py
+-rw-r--r--   0        0        0      708 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/margins.py
+-rw-r--r--   0        0        0      713 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/marginsf.py
+-rw-r--r--   0        0        0     1110 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/metaenum.py
+-rw-r--r--   0        0        0     1423 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/metamethod.py
+-rw-r--r--   0        0        0     3903 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/metaobject.py
+-rw-r--r--   0        0        0      511 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/metaproperty.py
+-rw-r--r--   0        0        0     5404 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/metatype.py
+-rw-r--r--   0        0        0     1802 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/mimedata.py
+-rw-r--r--   0        0        0      948 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/mimedatabase.py
+-rw-r--r--   0        0        0      208 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/mimetype.py
+-rw-r--r--   0        0        0      176 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/modelindex.py
+-rw-r--r--   0        0        0      336 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/mutex.py
+-rw-r--r--   0        0        0     3583 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/object.py
+-rw-r--r--   0        0        0     2562 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/operatingsystemversion.py
+-rw-r--r--   0        0        0      356 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/parallelanimationgroup.py
+-rw-r--r--   0        0        0      253 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/pauseanimation.py
+-rw-r--r--   0        0        0      338 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/persistentmodelindex.py
+-rw-r--r--   0        0        0      811 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/pluginloader.py
+-rw-r--r--   0        0        0      349 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/point.py
+-rw-r--r--   0        0        0      353 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/pointf.py
+-rw-r--r--   0        0        0     4839 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/process.py
+-rw-r--r--   0        0        0     1367 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/processenvironment.py
+-rw-r--r--   0        0        0      774 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/propertyanimation.py
+-rw-r--r--   0        0        0      126 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/randomgenerator.py
+-rw-r--r--   0        0        0      231 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/randomgenerator64.py
+-rw-r--r--   0        0        0      878 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/rect.py
+-rw-r--r--   0        0        0      442 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/rectf.py
+-rw-r--r--   0        0        0     6495 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/regularexpression.py
+-rw-r--r--   0        0        0     2625 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/regularexpressionmatch.py
+-rw-r--r--   0        0        0      613 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/regularexpressionmatchiterator.py
+-rw-r--r--   0        0        0     1702 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/resource.py
+-rw-r--r--   0        0        0      112 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/runnable.py
+-rw-r--r--   0        0        0      160 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/savefile.py
+-rw-r--r--   0        0        0      350 2023-04-16 21:30:19.297854 prettyqt-1.6.0/prettyqt/core/semaphore.py
+-rw-r--r--   0        0        0      202 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/sequentialanimationgroup.py
+-rw-r--r--   0        0        0     6990 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/settings.py
+-rw-r--r--   0        0        0      122 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/signalblocker.py
+-rw-r--r--   0        0        0      451 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/signalmapper.py
+-rw-r--r--   0        0        0     1124 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/size.py
+-rw-r--r--   0        0        0     1142 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/sizef.py
+-rw-r--r--   0        0        0      471 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/slot.py
+-rw-r--r--   0        0        0      930 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/socketnotifier.py
+-rw-r--r--   0        0        0     2681 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/sortfilterproxymodel.py
+-rw-r--r--   0        0        0     2622 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/standardpaths.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/storageinfo.py
+-rw-r--r--   0        0        0      339 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/stringlistmodel.py
+-rw-r--r--   0        0        0      980 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/temporarydir.py
+-rw-r--r--   0        0        0      164 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/temporaryfile.py
+-rw-r--r--   0        0        0     2583 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/textboundaryfinder.py
+-rw-r--r--   0        0        0     3862 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/textstream.py
+-rw-r--r--   0        0        0      108 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/thread.py
+-rw-r--r--   0        0        0      160 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/threadpool.py
+-rw-r--r--   0        0        0     2318 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/timeline.py
+-rw-r--r--   0        0        0     1770 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/timer.py
+-rw-r--r--   0        0        0     2198 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/timezone.py
+-rw-r--r--   0        0        0     1722 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/translator.py
+-rw-r--r--   0        0        0      190 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/transposeproxymodel.py
+-rw-r--r--   0        0        0     4469 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/url.py
+-rw-r--r--   0        0        0      788 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/urlquery.py
+-rw-r--r--   0        0        0     2333 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/uuid.py
+-rw-r--r--   0        0        0     1501 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/variantanimation.py
+-rw-r--r--   0        0        0     2614 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/versionnumber.py
+-rw-r--r--   0        0        0     2614 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/core/xmlstreamreader.py
+-rw-r--r--   0        0        0      253 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_animations/__init__.py
+-rw-r--r--   0        0        0     1579 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_animations/bounceanimation.py
+-rw-r--r--   0        0        0      644 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_animations/fadeinanimation.py
+-rw-r--r--   0        0        0      978 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_animations/slideanimation.py
+-rw-r--r--   0        0        0      535 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/__init__.py
+-rw-r--r--   0        0        0      887 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/buttondelegate.py
+-rw-r--r--   0        0        0     1001 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/checkboxdelegate.py
+-rw-r--r--   0        0        0     2570 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/icondelegate.py
+-rw-r--r--   0        0        0      596 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/nofocusdelegate.py
+-rw-r--r--   0        0        0     1474 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/progressbardelegate.py
+-rw-r--r--   0        0        0     4789 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/radiodelegate.py
+-rw-r--r--   0        0        0     2574 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/renderlinkdelegate.py
+-rw-r--r--   0        0        0     6634 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_delegates/stardelegate.py
+-rw-r--r--   0        0        0      777 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/__init__.py
+-rw-r--r--   0        0        0     6342 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/columnitemmodel.py
+-rw-r--r--   0        0        0     3285 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/importlibdistributionmodel.py
+-rw-r--r--   0        0        0     4175 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/jsonmodel.py
+-rw-r--r--   0        0        0     3083 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/listmixin.py
+-rw-r--r--   0        0        0     2562 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/modelmixin.py
+-rw-r--r--   0        0        0     2356 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/nesteditem.py
+-rw-r--r--   0        0        0     2177 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/nestedmodel.py
+-rw-r--r--   0        0        0     2126 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/regexmatchesmodel.py
+-rw-r--r--   0        0        0     1698 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/selectionmixin.py
+-rw-r--r--   0        0        0     3089 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/storageinfomodel.py
+-rw-r--r--   0        0        0     2858 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py
+-rw-r--r--   0        0        0      635 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/__init__.py
+-rw-r--r--   0        0        0     2060 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/compositevalidator.py
+-rw-r--r--   0        0        0     1114 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/integervalidator.py
+-rw-r--r--   0        0        0      704 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/notemptyvalidator.py
+-rw-r--r--   0        0        0      700 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/notzerovalidator.py
+-rw-r--r--   0        0        0      620 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/pathvalidator.py
+-rw-r--r--   0        0        0     1554 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/regexpatternvalidator.py
+-rw-r--r--   0        0        0     3143 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_validators/regexvalidators.py
+-rw-r--r--   0        0        0     2704 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/booldicttoolbutton.py
+-rw-r--r--   0        0        0     7718 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/borderlayout.py
+-rw-r--r--   0        0        0     3046 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/codeeditor.py
+-rw-r--r--   0        0        0     2588 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/collapsibleframe.py
+-rw-r--r--   0        0        0     2468 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/colorchooserbutton.py
+-rw-r--r--   0        0        0     7462 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/completionwidget.py
+-rw-r--r--   0        0        0    17651 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/dataset.py
+-rw-r--r--   0        0        0     2219 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/elidedlabel.py
+-rw-r--r--   0        0        0     3450 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/expandableline.py
+-rw-r--r--   0        0        0     3194 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/filechooserbutton.py
+-rw-r--r--   0        0        0     2155 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/flagselectionwidget.py
+-rw-r--r--   0        0        0     3847 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/flowlayout.py
+-rw-r--r--   0        0        0     2156 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/fontchooserbutton.py
+-rw-r--r--   0        0        0     9377 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/framelesswindow.py
+-rw-r--r--   0        0        0     5371 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/iconbrowser.py
+-rw-r--r--   0        0        0     1311 2023-04-16 21:30:19.301854 prettyqt-1.6.0/prettyqt/custom_widgets/iconlabel.py
+-rw-r--r--   0        0        0     1661 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/iconwidget.py
+-rw-r--r--   0        0        0     1292 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/image.py
+-rw-r--r--   0        0        0      644 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/imageviewer.py
+-rw-r--r--   0        0        0     1931 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/inputandslider.py
+-rw-r--r--   0        0        0     2106 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/joystickbutton.py
+-rw-r--r--   0        0        0     4165 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/labeledslider.py
+-rw-r--r--   0        0        0     1214 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/listinput.py
+-rw-r--r--   0        0        0     8209 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/logtextedit.py
+-rw-r--r--   0        0        0      738 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/mappedcheckbox.py
+-rw-r--r--   0        0        0     2388 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/markdownwidget.py
+-rw-r--r--   0        0        0     6576 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/menurecentfiles.py
+-rw-r--r--   0        0        0    18898 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/notification.py
+-rw-r--r--   0        0        0     1038 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/optionalwidget.py
+-rw-r--r--   0        0        0     1332 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/popupinfo.py
+-rw-r--r--   0        0        0      145 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/__main__.py
+-rw-r--r--   0        0        0     1039 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/quick_ref.py
+-rw-r--r--   0        0        0    19388 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/ref.html
+-rw-r--r--   0        0        0     6186 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
+-rw-r--r--   0        0        0     3145 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/regexinput.py
+-rw-r--r--   0        0        0    10698 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/roundprogressbar.py
+-rw-r--r--   0        0        0     4284 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/selectionwidget.py
+-rw-r--r--   0        0        0     6345 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/sidebarwidget.py
+-rw-r--r--   0        0        0     1036 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/singlelinetextedit.py
+-rw-r--r--   0        0        0    18739 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/spanslider.py
+-rw-r--r--   0        0        0     1286 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/standardiconswidget.py
+-rw-r--r--   0        0        0     2313 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/stringornumberwidget.py
+-rw-r--r--   0        0        0     1774 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/subsequencecompleter.py
+-rw-r--r--   0        0        0     8034 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/timeline.py
+-rw-r--r--   0        0        0     9009 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/custom_widgets/waitingspinner.py
+-rw-r--r--   0        0        0      255 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/eventfilters/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/eventfilters/animatedtooltipeventfilter.py
+-rw-r--r--   0        0        0      765 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/eventfilters/hovericoneventfilter.py
+-rw-r--r--   0        0        0     7915 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/__init__.py
+-rw-r--r--   0        0        0     1051 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/abstractfileiconprovider.py
+-rw-r--r--   0        0        0     1269 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/abstracttextdocumentlayout.py
+-rw-r--r--   0        0        0      235 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/bitmap.py
+-rw-r--r--   0        0        0     1451 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/brush.py
+-rw-r--r--   0        0        0     2490 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/clipboard.py
+-rw-r--r--   0        0        0     7636 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/color.py
+-rw-r--r--   0        0        0     3045 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/colorspace.py
+-rw-r--r--   0        0        0      485 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/conicalgradient.py
+-rw-r--r--   0        0        0     1255 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/cursor.py
+-rw-r--r--   0        0        0      439 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/desktopservices.py
+-rw-r--r--   0        0        0     1094 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/doublevalidator.py
+-rw-r--r--   0        0        0      973 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/drag.py
+-rw-r--r--   0        0        0     9049 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/font.py
+-rw-r--r--   0        0        0     4694 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/fontdatabase.py
+-rw-r--r--   0        0        0      243 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/fontinfo.py
+-rw-r--r--   0        0        0      889 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/fontmetrics.py
+-rw-r--r--   0        0        0      719 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/fontmetricsf.py
+-rw-r--r--   0        0        0     5331 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/gradient.py
+-rw-r--r--   0        0        0     5027 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/guiapplication.py
+-rw-r--r--   0        0        0     3986 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/icon.py
+-rw-r--r--   0        0        0     4053 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/iconengine.py
+-rw-r--r--   0        0        0     1630 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/image.py
+-rw-r--r--   0        0        0     3778 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/imageiohandler.py
+-rw-r--r--   0        0        0     3838 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/imagereader.py
+-rw-r--r--   0        0        0     2791 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/imagewriter.py
+-rw-r--r--   0        0        0     1315 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/inputmethod.py
+-rw-r--r--   0        0        0      921 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/intvalidator.py
+-rw-r--r--   0        0        0     6154 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/keysequence.py
+-rw-r--r--   0        0        0      636 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/lineargradient.py
+-rw-r--r--   0        0        0      302 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/matrix4x4.py
+-rw-r--r--   0        0        0     1969 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/movie.py
+-rw-r--r--   0        0        0      297 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pagedpaintdevice.py
+-rw-r--r--   0        0        0     2923 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pagelayout.py
+-rw-r--r--   0        0        0     7804 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pagesize.py
+-rw-r--r--   0        0        0     1676 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/paintdevice.py
+-rw-r--r--   0        0        0      319 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/paintdevicewindow.py
+-rw-r--r--   0        0        0     7794 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/painter.py
+-rw-r--r--   0        0        0     2425 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/painterpath.py
+-rw-r--r--   0        0        0     1641 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/painterpathstroker.py
+-rw-r--r--   0        0        0     5907 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/palette.py
+-rw-r--r--   0        0        0     1026 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pdfwriter.py
+-rw-r--r--   0        0        0     2841 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pen.py
+-rw-r--r--   0        0        0      471 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/picture.py
+-rw-r--r--   0        0        0     4827 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pixmap.py
+-rw-r--r--   0        0        0      796 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/pixmapcache.py
+-rw-r--r--   0        0        0     3489 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/polygon.py
+-rw-r--r--   0        0        0     4325 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/polygonf.py
+-rw-r--r--   0        0        0      898 2023-04-16 21:30:19.305854 prettyqt-1.6.0/prettyqt/gui/radialgradient.py
+-rw-r--r--   0        0        0      220 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/rasterwindow.py
+-rw-r--r--   0        0        0     1145 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/region.py
+-rw-r--r--   0        0        0     1290 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/regularexpressionvalidator.py
+-rw-r--r--   0        0        0     2963 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/screen.py
+-rw-r--r--   0        0        0     1291 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/sessionmanager.py
+-rw-r--r--   0        0        0     6203 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/standarditem.py
+-rw-r--r--   0        0        0     4778 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/standarditemmodel.py
+-rw-r--r--   0        0        0     2225 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/statictext.py
+-rw-r--r--   0        0        0     1146 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/stylehints.py
+-rw-r--r--   0        0        0     1303 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/surface.py
+-rw-r--r--   0        0        0     1352 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/syntaxhighlighter.py
+-rw-r--r--   0        0        0     5221 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textblock.py
+-rw-r--r--   0        0        0      623 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textblockgroup.py
+-rw-r--r--   0        0        0      536 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textblockuserdata.py
+-rw-r--r--   0        0        0     4878 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textcharformat.py
+-rw-r--r--   0        0        0     5551 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textcursor.py
+-rw-r--r--   0        0        0     8932 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textdocument.py
+-rw-r--r--   0        0        0      949 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textdocumentfragment.py
+-rw-r--r--   0        0        0     1062 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textdocumentwriter.py
+-rw-r--r--   0        0        0     3262 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textformat.py
+-rw-r--r--   0        0        0      534 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textframe.py
+-rw-r--r--   0        0        0     3627 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textframeformat.py
+-rw-r--r--   0        0        0      297 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textimageformat.py
+-rw-r--r--   0        0        0      517 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textlayout.py
+-rw-r--r--   0        0        0      725 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textlength.py
+-rw-r--r--   0        0        0     1649 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textline.py
+-rw-r--r--   0        0        0     1327 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textlistformat.py
+-rw-r--r--   0        0        0      445 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textobject.py
+-rw-r--r--   0        0        0      199 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textobjectinterface.py
+-rw-r--r--   0        0        0     1560 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/textoption.py
+-rw-r--r--   0        0        0     4104 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/texttablecellformat.py
+-rw-r--r--   0        0        0     2482 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/transform.py
+-rw-r--r--   0        0        0      640 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/undocommand.py
+-rw-r--r--   0        0        0      356 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/undogroup.py
+-rw-r--r--   0        0        0      957 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/undostack.py
+-rw-r--r--   0        0        0      755 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/validator.py
+-rw-r--r--   0        0        0      575 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/vector3d.py
+-rw-r--r--   0        0        0      578 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/vector4d.py
+-rw-r--r--   0        0        0     2338 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/gui/window.py
+-rw-r--r--   0        0        0    10227 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/animation.py
+-rw-r--r--   0        0        0     3079 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/awesomefileiconprovider.py
+-rw-r--r--   0        0        0      539 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/awesomequickimageprovider.py
+-rw-r--r--   0        0        0      832 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/chariconengine.py
+-rw-r--r--   0        0        0    10996 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/codicon-charmap.json
+-rw-r--r--   0        0        0    68076 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/codicon.ttf
+-rw-r--r--   0        0        0     7924 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
+-rw-r--r--   0        0        0    79556 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
+-rw-r--r--   0        0        0    11206 2023-04-16 21:30:19.309854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
+-rw-r--r--   0        0        0   134316 2023-04-16 21:30:19.313854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
+-rw-r--r--   0        0        0     3947 2023-04-16 21:30:19.313854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
+-rw-r--r--   0        0        0    33692 2023-04-16 21:30:19.313854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
+-rw-r--r--   0        0        0    25663 2023-04-16 21:30:19.313854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
+-rw-r--r--   0        0        0   203644 2023-04-16 21:30:19.313854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
+-rw-r--r--   0        0        0   200215 2023-04-16 21:30:19.317855 prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
+-rw-r--r--   0        0        0  1026284 2023-04-16 21:30:19.325854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
+-rw-r--r--   0        0        0   216192 2023-04-16 21:30:19.325854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
+-rw-r--r--   0        0        0  1108672 2023-04-16 21:30:19.325854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
+-rw-r--r--   0        0        0   151941 2023-04-16 21:30:19.325854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/phosphor-charmap.json
+-rw-r--r--   0        0        0  1392088 2023-04-16 21:30:19.337854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/phosphor.ttf
+-rw-r--r--   0        0        0    72655 2023-04-16 21:30:19.337854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/remixicon-charmap.json
+-rw-r--r--   0        0        0   403056 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/iconprovider/fonts/remixicon.ttf
+-rw-r--r--   0        0        0     8417 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/iconprovider/iconic_font.py
+-rw-r--r--   0        0        0     2468 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/iconprovider/svgbuffericonengine.py
+-rw-r--r--   0        0        0   154232 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/localization/language_ar.qm
+-rw-r--r--   0        0        0   155315 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/localization/language_bg.qm
+-rw-r--r--   0        0        0   178552 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/localization/language_ca.qm
+-rw-r--r--   0        0        0   151054 2023-04-16 21:30:19.341854 prettyqt-1.6.0/prettyqt/localization/language_cs.qm
+-rw-r--r--   0        0        0   179910 2023-04-16 21:30:19.345855 prettyqt-1.6.0/prettyqt/localization/language_da.qm
+-rw-r--r--   0        0        0   212675 2023-04-16 21:30:19.345855 prettyqt-1.6.0/prettyqt/localization/language_de.qm
+-rw-r--r--   0        0        0   154543 2023-04-16 21:30:19.345855 prettyqt-1.6.0/prettyqt/localization/language_es.qm
+-rw-r--r--   0        0        0    97872 2023-04-16 21:30:19.345855 prettyqt-1.6.0/prettyqt/localization/language_fa.qm
+-rw-r--r--   0        0        0   174500 2023-04-16 21:30:19.349855 prettyqt-1.6.0/prettyqt/localization/language_fi.qm
+-rw-r--r--   0        0        0   154190 2023-04-16 21:30:19.349855 prettyqt-1.6.0/prettyqt/localization/language_fr.qm
+-rw-r--r--   0        0        0   183091 2023-04-16 21:30:19.349855 prettyqt-1.6.0/prettyqt/localization/language_gd.qm
+-rw-r--r--   0        0        0   108600 2023-04-16 21:30:19.349855 prettyqt-1.6.0/prettyqt/localization/language_gl.qm
+-rw-r--r--   0        0        0   130568 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_he.qm
+-rw-r--r--   0        0        0   150033 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_hu.qm
+-rw-r--r--   0        0        0   153570 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_it.qm
+-rw-r--r--   0        0        0   122385 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_ja.qm
+-rw-r--r--   0        0        0   120318 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_ko.qm
+-rw-r--r--   0        0        0    90502 2023-04-16 21:30:19.353855 prettyqt-1.6.0/prettyqt/localization/language_lt.qm
+-rw-r--r--   0        0        0   143558 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_lv.qm
+-rw-r--r--   0        0        0   161318 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_pl.qm
+-rw-r--r--   0        0        0    50541 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_pt.qm
+-rw-r--r--   0        0        0   197476 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_ru.qm
+-rw-r--r--   0        0        0   115250 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_sk.qm
+-rw-r--r--   0        0        0    96357 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_sl.qm
+-rw-r--r--   0        0        0    47206 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_sv.qm
+-rw-r--r--   0        0        0   148437 2023-04-16 21:30:19.357855 prettyqt-1.6.0/prettyqt/localization/language_uk.qm
+-rw-r--r--   0        0        0    61089 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/localization/language_zh_CN.qm
+-rw-r--r--   0        0        0   125250 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/localization/language_zh_TW.qm
+-rw-r--r--   0        0        0     2384 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/geocodingmanager.py
+-rw-r--r--   0        0        0     2867 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/geomaneuver.py
+-rw-r--r--   0        0        0     1055 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/georoute.py
+-rw-r--r--   0        0        0     5266 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/georouterequest.py
+-rw-r--r--   0        0        0      657 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/georoutesegment.py
+-rw-r--r--   0        0        0     2021 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/georoutingmanager.py
+-rw-r--r--   0        0        0     5880 2023-04-16 21:30:19.361855 prettyqt-1.6.0/prettyqt/location/geoserviceprovider.py
+-rw-r--r--   0        0        0     2387 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/place.py
+-rw-r--r--   0        0        0      864 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeattribute.py
+-rw-r--r--   0        0        0      737 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placecategory.py
+-rw-r--r--   0        0        0      844 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placecontactdetail.py
+-rw-r--r--   0        0        0     1030 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placecontent.py
+-rw-r--r--   0        0        0     1275 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placecontentreply.py
+-rw-r--r--   0        0        0      947 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placecontentrequest.py
+-rw-r--r--   0        0        0      562 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placedetailsreply.py
+-rw-r--r--   0        0        0      849 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeicon.py
+-rw-r--r--   0        0        0     1185 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeidreply.py
+-rw-r--r--   0        0        0     2233 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placemanager.py
+-rw-r--r--   0        0        0     1066 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placematchreply.py
+-rw-r--r--   0        0        0      726 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placematchrequest.py
+-rw-r--r--   0        0        0      223 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeproposedsearchresult.py
+-rw-r--r--   0        0        0      316 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeratings.py
+-rw-r--r--   0        0        0     1923 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placereply.py
+-rw-r--r--   0        0        0      267 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeresult.py
+-rw-r--r--   0        0        0     1651 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placesearchreply.py
+-rw-r--r--   0        0        0     2230 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placesearchrequest.py
+-rw-r--r--   0        0        0      884 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placesearchresult.py
+-rw-r--r--   0        0        0      675 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placesupplier.py
+-rw-r--r--   0        0        0      215 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/placeuser.py
+-rw-r--r--   0        0        0      621 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/location/qlocation.py
+-rw-r--r--   0        0        0      167 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/multimediawidgets/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/multimediawidgets/graphicsvideoitem.py
+-rw-r--r--   0        0        0      872 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/multimediawidgets/videowidget.py
+-rw-r--r--   0        0        0     1172 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/__init__.py
+-rw-r--r--   0        0        0     8113 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/abstractsocket.py
+-rw-r--r--   0        0        0     1775 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/hostaddress.py
+-rw-r--r--   0        0        0     1465 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/httpmultipart.py
+-rw-r--r--   0        0        0      823 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/httppart.py
+-rw-r--r--   0        0        0     1310 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/localserver.py
+-rw-r--r--   0        0        0     2392 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/localsocket.py
+-rw-r--r--   0        0        0     2313 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkaccessmanager.py
+-rw-r--r--   0        0        0     2000 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkaddressentry.py
+-rw-r--r--   0        0        0     1551 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkcookie.py
+-rw-r--r--   0        0        0      850 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkcookiejar.py
+-rw-r--r--   0        0        0      627 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkdatagram.py
+-rw-r--r--   0        0        0     3011 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkinterface.py
+-rw-r--r--   0        0        0     3361 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkproxy.py
+-rw-r--r--   0        0        0     6462 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/networkrequest.py
+-rw-r--r--   0        0        0      779 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/tcpserver.py
+-rw-r--r--   0        0        0      178 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/tcpsocket.py
+-rw-r--r--   0        0        0      671 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/network/udpsocket.py
+-rw-r--r--   0        0        0       26 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/objbrowser/__init__.py
+-rw-r--r--   0        0        0     9193 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/objbrowser/attribute_model.py
+-rw-r--r--   0        0        0    14897 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/objbrowser/objectbrowser.py
+-rw-r--r--   0        0        0    17795 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/objbrowser/objectbrowsertreemodel.py
+-rw-r--r--   0        0        0      356 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/paths.py
+-rw-r--r--   0        0        0     1169 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geoaddress.py
+-rw-r--r--   0        0        0     1149 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geoareamonitorinfo.py
+-rw-r--r--   0        0        0     1260 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geoareamonitorsource.py
+-rw-r--r--   0        0        0     1072 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geocircle.py
+-rw-r--r--   0        0        0     1172 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geocoordinate.py
+-rw-r--r--   0        0        0      558 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geolocation.py
+-rw-r--r--   0        0        0     1021 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geopath.py
+-rw-r--r--   0        0        0     1145 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geopolygon.py
+-rw-r--r--   0        0        0     1687 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geopositioninfo.py
+-rw-r--r--   0        0        0     2960 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geopositioninfosource.py
+-rw-r--r--   0        0        0      769 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/georectangle.py
+-rw-r--r--   0        0        0     1861 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geosatelliteinfo.py
+-rw-r--r--   0        0        0     1110 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geosatelliteinfosource.py
+-rw-r--r--   0        0        0      755 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/geoshape.py
+-rw-r--r--   0        0        0     1196 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/positioning/nmeapositioninginfosource.py
+-rw-r--r--   0        0        0        0 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/py.typed
+-rw-r--r--   0        0        0      943 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/__init__.py
+-rw-r--r--   0        0        0     1213 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/jsengine.py
+-rw-r--r--   0        0        0     2532 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/jsvalue.py
+-rw-r--r--   0        0        0      295 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/jsvalueiterator.py
+-rw-r--r--   0        0        0      955 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/qmlapplicationengine.py
+-rw-r--r--   0        0        0      907 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/qmlcomponent.py
+-rw-r--r--   0        0        0     2020 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/qmlengine.py
+-rw-r--r--   0        0        0      536 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/qmlimageproviderbase.py
+-rw-r--r--   0        0        0      185 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qml/qmlparserstatus.py
+-rw-r--r--   0        0        0      203 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/Qsci/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtBluetooth/__init__.py
+-rw-r--r--   0        0        0      446 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtCharts/__init__.py
+-rw-r--r--   0        0        0     2281 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtCore/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtGui/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtHelp/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtLocation/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtMultimedia/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtMultimediaWidgets/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtNetwork/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtPositioning/__init__.py
+-rw-r--r--   0        0        0      266 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtQml/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtQuick/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtScxml/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtStateMachine/__init__.py
+-rw-r--r--   0        0        0      332 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtSvg/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtTest/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtTextToSpeech/__init__.py
+-rw-r--r--   0        0        0      368 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtUiTools/__init__.py
+-rw-r--r--   0        0        0      274 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtWebChannel/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtWebEngineCore/__init__.py
+-rw-r--r--   0        0        0      289 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtWebEngineWidgets/__init__.py
+-rw-r--r--   0        0        0     1548 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/QtWidgets/__init__.py
+-rw-r--r--   0        0        0     1200 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qt/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpcontentitem.py
+-rw-r--r--   0        0        0      443 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpcontentmodel.py
+-rw-r--r--   0        0        0      460 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpcontentwidget.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpengine.py
+-rw-r--r--   0        0        0     1107 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpenginecore.py
+-rw-r--r--   0        0        0      661 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpfilterdata.py
+-rw-r--r--   0        0        0      739 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpfilterengine.py
+-rw-r--r--   0        0        0      177 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpindexmodel.py
+-rw-r--r--   0        0        0      178 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpindexwidget.py
+-rw-r--r--   0        0        0      729 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpsearchengine.py
+-rw-r--r--   0        0        0      188 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpsearchquerywidget.py
+-rw-r--r--   0        0        0      216 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpsearchresult.py
+-rw-r--r--   0        0        0      832 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qthelp/helpsearchresultwidget.py
+-rw-r--r--   0        0        0     8336 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/qtre.py
+-rw-r--r--   0        0        0      868 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickasyncimageprovider.py
+-rw-r--r--   0        0        0      257 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickimageprovider.py
+-rw-r--r--   0        0        0      239 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickimageresponse.py
+-rw-r--r--   0        0        0     3753 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickitem.py
+-rw-r--r--   0        0        0      519 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickitemgrabresult.py
+-rw-r--r--   0        0        0     1495 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickpainteditem.py
+-rw-r--r--   0        0        0      239 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickrendercontrol.py
+-rw-r--r--   0        0        0      271 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quicktextdocument.py
+-rw-r--r--   0        0        0     1204 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickview.py
+-rw-r--r--   0        0        0     3624 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/quick/quickwindow.py
+-rw-r--r--   0        0        0      123 2023-04-16 21:30:19.369855 prettyqt-1.6.0/prettyqt/scintilla/__init__.py
+-rw-r--r--   0        0        0     9347 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/scintilla/sciscintilla.py
+-rw-r--r--   0        0        0      193 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/scxml/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/scxml/scxmlcompiler.py
+-rw-r--r--   0        0        0      176 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/scxml/scxmlstatemachine.py
+-rw-r--r--   0        0        0      785 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/__init__.py
+-rw-r--r--   0        0        0      361 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/abstractstate.py
+-rw-r--r--   0        0        0     1159 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/abstracttransition.py
+-rw-r--r--   0        0        0      220 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/eventtransition.py
+-rw-r--r--   0        0        0      199 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/finalstate.py
+-rw-r--r--   0        0        0     1104 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/historystate.py
+-rw-r--r--   0        0        0      223 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/keyeventtransition.py
+-rw-r--r--   0        0        0      227 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/mouseeventtransition.py
+-rw-r--r--   0        0        0      222 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/signaltransition.py
+-rw-r--r--   0        0        0     1276 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/state.py
+-rw-r--r--   0        0        0     2222 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/statemachine/statemachine.py
+-rw-r--r--   0        0        0      170 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/svg/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/svg/graphicssvgitem.py
+-rw-r--r--   0        0        0      405 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/svg/svggenerator.py
+-rw-r--r--   0        0        0     1080 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/svg/svgrenderer.py
+-rw-r--r--   0        0        0      279 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/svg/svgwidget.py
+-rw-r--r--   0        0        0      675 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/highlightrule.py
+-rw-r--r--   0        0        0     1271 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/jsonhighlighter.py
+-rw-r--r--   0        0        0     3178 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/markdownhighlighter.py
+-rw-r--r--   0        0        0      872 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
+-rw-r--r--   0        0        0     8585 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py
+-rw-r--r--   0        0        0     4836 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/pythonhighlighter.py
+-rw-r--r--   0        0        0     2079 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
+-rw-r--r--   0        0        0     2192 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/xmlhighlighter.py
+-rw-r--r--   0        0        0     2106 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/syntaxhighlighters/yamlhighlighter.py
+-rw-r--r--   0        0        0      180 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/texttospeech/__init__.py
+-rw-r--r--   0        0        0     1328 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/texttospeech/texttospeech.py
+-rw-r--r--   0        0        0      944 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/texttospeech/voice.py
+-rw-r--r--   0        0        0    15547 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/themes/darktheme.qss
+-rw-r--r--   0        0        0      845 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/__init__.py
+-rw-r--r--   0        0        0     3561 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/autoslot.py
+-rw-r--r--   0        0        0     3307 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/colors.py
+-rw-r--r--   0        0        0     2161 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/debugging.py
+-rw-r--r--   0        0        0     3598 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/helpers.py
+-rw-r--r--   0        0        0      894 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/mappers.py
+-rw-r--r--   0        0        0     1054 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/prettyprinter.py
+-rw-r--r--   0        0        0     5546 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/searchandreplacemixin.py
+-rw-r--r--   0        0        0      629 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/signallogger.py
+-rw-r--r--   0        0        0     2306 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/singleapplication.py
+-rw-r--r--   0        0        0      493 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/singleton.py
+-rw-r--r--   0        0        0     2110 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/syncedproperty.py
+-rw-r--r--   0        0        0     1887 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/treeitem.py
+-rw-r--r--   0        0        0     4119 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/utils/types.py
+-rw-r--r--   0        0        0      303 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webchannel/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webchannel/webchannel.py
+-rw-r--r--   0        0        0     1337 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/__init__.py
+-rw-r--r--   0        0        0     3315 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginecontextmenurequest.py
+-rw-r--r--   0        0        0     4498 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginedownloadrequest.py
+-rw-r--r--   0        0        0     1299 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginehistory.py
+-rw-r--r--   0        0        0      422 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginehistoryitem.py
+-rw-r--r--   0        0        0     1776 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginehttprequest.py
+-rw-r--r--   0        0        0    14262 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginepage.py
+-rw-r--r--   0        0        0     2461 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webengineprofile.py
+-rw-r--r--   0        0        0     1574 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginescript.py
+-rw-r--r--   0        0        0     1362 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginescriptcollection.py
+-rw-r--r--   0        0        0     7469 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webenginesettings.py
+-rw-r--r--   0        0        0     2044 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webengineurlscheme.py
+-rw-r--r--   0        0        0      282 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginecore/webengineurlschemehandler.py
+-rw-r--r--   0        0        0      330 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginewidgets/__init__.py
+-rw-r--r--   0        0        0     4602 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/webenginewidgets/webengineview.py
+-rw-r--r--   0        0        0    13448 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/__init__.py
+-rw-r--r--   0        0        0     3797 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractbutton.py
+-rw-r--r--   0        0        0      406 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractgraphicsshapeitem.py
+-rw-r--r--   0        0        0      257 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractitemdelegate.py
+-rw-r--r--   0        0        0    11883 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractitemview.py
+-rw-r--r--   0        0        0     5361 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractscrollarea.py
+-rw-r--r--   0        0        0     5646 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractslider.py
+-rw-r--r--   0        0        0     3715 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/abstractspinbox.py
+-rw-r--r--   0        0        0     8208 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/action.py
+-rw-r--r--   0        0        0     2143 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/actiongroup.py
+-rw-r--r--   0        0        0     8323 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/application.py
+-rw-r--r--   0        0        0     2754 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/boxlayout.py
+-rw-r--r--   0        0        0      342 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/buttongroup.py
+-rw-r--r--   0        0        0     2960 2023-04-16 21:30:19.373855 prettyqt-1.6.0/prettyqt/widgets/calendarwidget.py
+-rw-r--r--   0        0        0     1647 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/checkbox.py
+-rw-r--r--   0        0        0     3856 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/colordialog.py
+-rw-r--r--   0        0        0      331 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/columnview.py
+-rw-r--r--   0        0        0     7000 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/combobox.py
+-rw-r--r--   0        0        0      365 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/commandlinkbutton.py
+-rw-r--r--   0        0        0      281 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/commonstyle.py
+-rw-r--r--   0        0        0     3501 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/completer.py
+-rw-r--r--   0        0        0     2700 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/datawidgetmapper.py
+-rw-r--r--   0        0        0     1412 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/dateedit.py
+-rw-r--r--   0        0        0     4324 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/datetimeedit.py
+-rw-r--r--   0        0        0     1079 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/dial.py
+-rw-r--r--   0        0        0     2813 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/dialog.py
+-rw-r--r--   0        0        0     5950 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/dialogbuttonbox.py
+-rw-r--r--   0        0        0     2356 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/dockwidget.py
+-rw-r--r--   0        0        0     1772 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/doublespinbox.py
+-rw-r--r--   0        0        0      328 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/errormessage.py
+-rw-r--r--   0        0        0     7417 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/filedialog.py
+-rw-r--r--   0        0        0      805 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/fileiconprovider.py
+-rw-r--r--   0        0        0     3484 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/filesystemmodel.py
+-rw-r--r--   0        0        0      289 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/focusframe.py
+-rw-r--r--   0        0        0     2477 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/fontcombobox.py
+-rw-r--r--   0        0        0      363 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/fontdialog.py
+-rw-r--r--   0        0        0     5088 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/formlayout.py
+-rw-r--r--   0        0        0     2540 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/frame.py
+-rw-r--r--   0        0        0     1822 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/gesture.py
+-rw-r--r--   0        0        0     2334 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsanchorlayout.py
+-rw-r--r--   0        0        0     1360 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsblureffect.py
+-rw-r--r--   0        0        0      469 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicscolorizeeffect.py
+-rw-r--r--   0        0        0      435 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsdropshadoweffect.py
+-rw-r--r--   0        0        0      416 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicseffect.py
+-rw-r--r--   0        0        0      559 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsellipseitem.py
+-rw-r--r--   0        0        0     3650 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsgridlayout.py
+-rw-r--r--   0        0        0     4923 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsitem.py
+-rw-r--r--   0        0        0      192 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsitemgroup.py
+-rw-r--r--   0        0        0     1173 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicslayout.py
+-rw-r--r--   0        0        0      262 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicslayoutitem.py
+-rw-r--r--   0        0        0     1098 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicslinearlayout.py
+-rw-r--r--   0        0        0      651 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicslineitem.py
+-rw-r--r--   0        0        0      700 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsobject.py
+-rw-r--r--   0        0        0      538 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsopacityeffect.py
+-rw-r--r--   0        0        0      209 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicspathitem.py
+-rw-r--r--   0        0        0     2241 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicspixmapitem.py
+-rw-r--r--   0        0        0      800 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicspolygonitem.py
+-rw-r--r--   0        0        0      198 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsproxywidget.py
+-rw-r--r--   0        0        0      542 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsrectitem.py
+-rw-r--r--   0        0        0      754 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsrotation.py
+-rw-r--r--   0        0        0      490 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsscale.py
+-rw-r--r--   0        0        0     8525 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsscene.py
+-rw-r--r--   0        0        0      293 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicssimpletextitem.py
+-rw-r--r--   0        0        0      707 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicstextitem.py
+-rw-r--r--   0        0        0      310 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicstransform.py
+-rw-r--r--   0        0        0     8619 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicsview.py
+-rw-r--r--   0        0        0     2770 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/graphicswidget.py
+-rw-r--r--   0        0        0     4159 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/gridlayout.py
+-rw-r--r--   0        0        0     1955 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/groupbox.py
+-rw-r--r--   0        0        0     5318 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/headerview.py
+-rw-r--r--   0        0        0     3755 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/inputdialog.py
+-rw-r--r--   0        0        0      190 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/itemdelegate.py
+-rw-r--r--   0        0        0      144 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/itemeditorcreatorbase.py
+-rw-r--r--   0        0        0     2331 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/itemeditorfactory.py
+-rw-r--r--   0        0        0      846 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/keysequenceedit.py
+-rw-r--r--   0        0        0     8483 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/label.py
+-rw-r--r--   0        0        0     4064 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/layout.py
+-rw-r--r--   0        0        0     1272 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/layoutitem.py
+-rw-r--r--   0        0        0     2416 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/lcdnumber.py
+-rw-r--r--   0        0        0     6546 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/lineedit.py
+-rw-r--r--   0        0        0     5606 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/listview.py
+-rw-r--r--   0        0        0     5823 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/listwidget.py
+-rw-r--r--   0        0        0     3690 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/listwidgetitem.py
+-rw-r--r--   0        0        0     6705 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/mainwindow.py
+-rw-r--r--   0        0        0     4591 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/mdiarea.py
+-rw-r--r--   0        0        0      689 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/mdisubwindow.py
+-rw-r--r--   0        0        0     4397 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/menu.py
+-rw-r--r--   0        0        0     2145 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/menubar.py
+-rw-r--r--   0        0        0     7314 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/messagebox.py
+-rw-r--r--   0        0        0      542 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/pangesture.py
+-rw-r--r--   0        0        0     1902 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/pinchgesture.py
+-rw-r--r--   0        0        0      415 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/plaintextdocumentlayout.py
+-rw-r--r--   0        0        0     9079 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/plaintextedit.py
+-rw-r--r--   0        0        0     3564 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/progressbar.py
+-rw-r--r--   0        0        0     1029 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/progressdialog.py
+-rw-r--r--   0        0        0      231 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/proxystyle.py
+-rw-r--r--   0        0        0      804 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/pushbutton.py
+-rw-r--r--   0        0        0      517 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/radiobutton.py
+-rw-r--r--   0        0        0      758 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/rubberband.py
+-rw-r--r--   0        0        0      611 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/scrollarea.py
+-rw-r--r--   0        0        0      973 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/scrollbar.py
+-rw-r--r--   0        0        0     3060 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/scroller.py
+-rw-r--r--   0        0        0     3937 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/scrollerproperties.py
+-rw-r--r--   0        0        0     1399 2023-04-16 21:30:19.377855 prettyqt-1.6.0/prettyqt/widgets/shortcut.py
+-rw-r--r--   0        0        0      309 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/sizegrip.py
+-rw-r--r--   0        0        0     5373 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/sizepolicy.py
+-rw-r--r--   0        0        0     2654 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/slider.py
+-rw-r--r--   0        0        0     1297 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/spaceritem.py
+-rw-r--r--   0        0        0     1837 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/spinbox.py
+-rw-r--r--   0        0        0     1181 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/splashscreen.py
+-rw-r--r--   0        0        0     3920 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/splitter.py
+-rw-r--r--   0        0        0     1417 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/splitterhandle.py
+-rw-r--r--   0        0        0      983 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/stackedlayout.py
+-rw-r--r--   0        0        0     1372 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/stackedwidget.py
+-rw-r--r--   0        0        0     1700 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/statusbar.py
+-rw-r--r--   0        0        0    19383 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/style.py
+-rw-r--r--   0        0        0      208 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleditemdelegate.py
+-rw-r--r--   0        0        0      126 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/stylefactory.py
+-rw-r--r--   0        0        0      318 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoption.py
+-rw-r--r--   0        0        0      686 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionbutton.py
+-rw-r--r--   0        0        0      208 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptioncombobox.py
+-rw-r--r--   0        0        0      260 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptioncomplex.py
+-rw-r--r--   0        0        0      199 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiondockwidget.py
+-rw-r--r--   0        0        0      197 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionfocusrect.py
+-rw-r--r--   0        0        0      189 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionframe.py
+-rw-r--r--   0        0        0      209 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiongraphicsitem.py
+-rw-r--r--   0        0        0      197 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiongroupbox.py
+-rw-r--r--   0        0        0      911 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionheader.py
+-rw-r--r--   0        0        0     1032 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionmenuitem.py
+-rw-r--r--   0        0        0      201 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionprogressbar.py
+-rw-r--r--   0        0        0      199 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionrubberband.py
+-rw-r--r--   0        0        0      208 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionsizegrip.py
+-rw-r--r--   0        0        0     1046 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionslider.py
+-rw-r--r--   0        0        0      195 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionspinbox.py
+-rw-r--r--   0        0        0     1135 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontab.py
+-rw-r--r--   0        0        0      199 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontabbarbase.py
+-rw-r--r--   0        0        0      213 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontabwidgetframe.py
+-rw-r--r--   0        0        0      197 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontitlebar.py
+-rw-r--r--   0        0        0      397 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontoolbar.py
+-rw-r--r--   0        0        0     1180 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontoolbox.py
+-rw-r--r--   0        0        0      201 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptiontoolbutton.py
+-rw-r--r--   0        0        0     1344 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/styleoptionviewitem.py
+-rw-r--r--   0        0        0      397 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/stylepainter.py
+-rw-r--r--   0        0        0     1311 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/swipegesture.py
+-rw-r--r--   0        0        0     1732 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/systemtrayicon.py
+-rw-r--r--   0        0        0     5232 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tabbar.py
+-rw-r--r--   0        0        0     3112 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tableview.py
+-rw-r--r--   0        0        0     1085 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tablewidget.py
+-rw-r--r--   0        0        0     3334 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tablewidgetitem.py
+-rw-r--r--   0        0        0     1920 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tablewidgetselectionrange.py
+-rw-r--r--   0        0        0    10591 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tabwidget.py
+-rw-r--r--   0        0        0      392 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tapandholdgesture.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tapgesture.py
+-rw-r--r--   0        0        0     2400 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/textbrowser.py
+-rw-r--r--   0        0        0     6089 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/textedit.py
+-rw-r--r--   0        0        0     1526 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/timeedit.py
+-rw-r--r--   0        0        0     5015 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/toolbar.py
+-rw-r--r--   0        0        0     2568 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/toolbox.py
+-rw-r--r--   0        0        0     3175 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/toolbutton.py
+-rw-r--r--   0        0        0      710 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/tooltip.py
+-rw-r--r--   0        0        0     2532 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/treeview.py
+-rw-r--r--   0        0        0      630 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/treewidget.py
+-rw-r--r--   0        0        0     4841 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/treewidgetitem.py
+-rw-r--r--   0        0        0     4142 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/treewidgetitemiterator.py
+-rw-r--r--   0        0        0     1003 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/undoview.py
+-rw-r--r--   0        0        0      552 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/whatsthis.py
+-rw-r--r--   0        0        0    20219 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/widget.py
+-rw-r--r--   0        0        0      545 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/widgetaction.py
+-rw-r--r--   0        0        0      248 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/widgetitem.py
+-rw-r--r--   0        0        0     9052 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/wizard.py
+-rw-r--r--   0        0        0     1997 2023-04-16 21:30:19.381855 prettyqt-1.6.0/prettyqt/widgets/wizardpage.py
+-rw-r--r--   0        0        0     4495 2023-04-16 21:30:19.381855 prettyqt-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 prettyqt-1.6.0/PKG-INFO
```

### Comparing `prettyqt-1.5.0/LICENSE` & `prettyqt-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/docs/index.md` & `prettyqt-1.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/__init__.py` & `prettyqt-1.6.0/prettyqt/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for PrettyQt."""
 
 __author__ = """Philipp Temminghoff"""
 __email__ = "phil65@kodi.tv"
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 
 def debug():
     """Print the local variables in the caller's frame."""
     import inspect
 
     frame = inspect.currentframe()
```

### Comparing `prettyqt-1.5.0/prettyqt/__pyinstaller/hook-prettyqt.py` & `prettyqt-1.6.0/prettyqt/__pyinstaller/hook-prettyqt.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/bluetooth/__init__.py` & `prettyqt-1.6.0/prettyqt/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py` & `prettyqt-1.6.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py` & `prettyqt-1.6.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/bluetooth/bluetoothserviceinfo.py` & `prettyqt-1.6.0/prettyqt/bluetooth/bluetoothserviceinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/bluetooth/bluetoothuuid.py` & `prettyqt-1.6.0/prettyqt/bluetooth/bluetoothuuid.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/__init__.py` & `prettyqt-1.6.0/prettyqt/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/abstractaxis.py` & `prettyqt-1.6.0/prettyqt/charts/abstractaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/abstractbarseries.py` & `prettyqt-1.6.0/prettyqt/charts/abstractbarseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/abstractseries.py` & `prettyqt-1.6.0/prettyqt/charts/abstractseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/barcategoryaxis.py` & `prettyqt-1.6.0/prettyqt/charts/barcategoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/barset.py` & `prettyqt-1.6.0/prettyqt/charts/barset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/boxset.py` & `prettyqt-1.6.0/prettyqt/charts/boxset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/candlestickset.py` & `prettyqt-1.6.0/prettyqt/charts/candlestickset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/categoryaxis.py` & `prettyqt-1.6.0/prettyqt/charts/categoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/chart.py` & `prettyqt-1.6.0/prettyqt/charts/chart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/chartview.py` & `prettyqt-1.6.0/prettyqt/charts/chartview.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Literal
 
 from prettyqt import charts, core, gui, widgets
-from prettyqt.qt import QtCharts, QtCore, QtGui, QtWidgets
+from prettyqt.qt import QtCharts, QtCore, QtGui
 from prettyqt.utils import InvalidParamError, bidict
 
 
 RUBBER_BAND = bidict(
     none=QtCharts.QChartView.RubberBand.NoRubberBand,
     vertical=QtCharts.QChartView.RubberBand.VerticalRubberBand,
     horizontal=QtCharts.QChartView.RubberBand.HorizontalRubberBand,
@@ -29,16 +29,15 @@
         self.setChart(chart)
         self.setRenderHint(gui.Painter.RenderHint.Antialiasing)
         self.set_rubber_band("rectangle")
         # self.setDragMode(self.RubberBandDrag)
 
     def keyPressEvent(self, event: QtGui.QKeyEvent):
         """Handle keypress events to allow navigation via keyboard."""
-        key = event.key()
-        match key:
+        match event.key():
             case QtCore.Qt.Key.Key_Escape:
                 self.chart().zoomReset()
             case QtCore.Qt.Key.Key_Plus:
                 self.chart().zoom_by_factor(ZOOM_IN_FACTOR)
             case QtCore.Qt.Key.Key_Minus:
                 self.chart().zoom_by_factor(ZOOM_OUT_FACTOR)
             case QtCore.Qt.Key.Key_Left:
@@ -68,16 +67,15 @@
             event.accept()
             return
         super().mouseReleaseEvent(event)
 
     def mousePressEvent(self, event: QtGui.QMouseEvent):
         """Override to allow dragging the chart."""
         if event.button() == QtCore.Qt.MouseButton.RightButton:
-            cursor = gui.Cursor(QtCore.Qt.CursorShape.SizeAllCursor)
-            widgets.Application.setOverrideCursor(cursor)
+            widgets.Application.set_override_cursor("size_all")
             self.last_mouse_pos = event.position()
             event.accept()
 
         super().mousePressEvent(event)
 
     def mouseMoveEvent(self, event: QtGui.QMouseEvent):
         """Override to allow dragging the chart."""
@@ -87,16 +85,14 @@
                 return
             pos_diff = event.position() - self.last_mouse_pos
             self.chart().scroll(-pos_diff.x(), pos_diff.y())
 
             self.last_mouse_pos = event.position()
             event.accept()
 
-            widgets.Application.restoreOverrideCursor()
-
         super().mouseMoveEvent(event)
 
     @core.Slot()
     def save_as_image(self):
         """Let user choose folder and save chart as an image file."""
         dlg = widgets.FileDialog(mode="save", caption="Save image")
         filters = {"Bmp files": [".bmp"], "Jpeg files": [".jpg"], "Png files": [".png"]}
@@ -105,24 +101,14 @@
         if not filename:
             return
         self.chart().show_legend()
         image = self.get_image()
         image.save(str(filename[0]))
         self.chart().hide_legend()
 
-    def get_image(self) -> QtGui.QPixmap:
-        image = self.grab()
-        gl_widget = self.find_child(QtWidgets.QOpenGLWidget)
-        if gl_widget:
-            d = gl_widget.mapToGlobal(core.Point()) - self.mapToGlobal(core.Point())
-            with gui.Painter(image) as painter:
-                painter.set_composition_mode("source_atop")
-                painter.drawImage(d, gl_widget.grabFramebuffer())
-        return image
-
     def set_rubber_band(self, typ: RubberBandStr):
         """Set the rubber band type.
 
         Args:
             typ: rubber band type
 
         Raises:
```

### Comparing `prettyqt-1.5.0/prettyqt/charts/legend.py` & `prettyqt-1.6.0/prettyqt/charts/legend.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/lineseries.py` & `prettyqt-1.6.0/prettyqt/charts/lineseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/pieslice.py` & `prettyqt-1.6.0/prettyqt/charts/pieslice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/polarchart.py` & `prettyqt-1.6.0/prettyqt/charts/polarchart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/valueaxis.py` & `prettyqt-1.6.0/prettyqt/charts/valueaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/charts/xyseries.py` & `prettyqt-1.6.0/prettyqt/charts/xyseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/constants/__init__.py` & `prettyqt-1.6.0/prettyqt/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/__init__.py` & `prettyqt-1.6.0/prettyqt/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,16 +151,15 @@
 from .pluginloader import PluginLoader  # type: ignore
 
 from .concatenatetablesproxymodel import ConcatenateTablesProxyModel
 from .transposeproxymodel import TransposeProxyModel
 
 
 def app(args: list[str] | None = None) -> CoreApplication:
-    instance = CoreApplication.instance()
-    if instance is not None:
+    if instance := CoreApplication.instance() is not None:
         return instance
     return CoreApplication(sys.argv if args is None else args)
 
 
 __all__ = [
     "app",
     "Event",
```

### Comparing `prettyqt-1.5.0/prettyqt/core/_calendar.py` & `prettyqt-1.6.0/prettyqt/core/_calendar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/_datetime.py` & `prettyqt-1.6.0/prettyqt/core/_datetime.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/_locale.py` & `prettyqt-1.6.0/prettyqt/core/_locale.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/abstractanimation.py` & `prettyqt-1.6.0/prettyqt/core/abstractanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/abstractitemmodel.py` & `prettyqt-1.6.0/prettyqt/core/abstractitemmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         self.beginInsertRows(parent, first, last)
         yield None
         self.endInsertRows()
 
     @contextlib.contextmanager
     def append_rows(self, num_rows: int, parent: QtCore.QModelIndex | None = None):
         parent = QtCore.QModelIndex() if parent is None else parent
-        self.beginInsertRows(parent, self.rowCount(), self.rowCount() + num_rows - 1)
+        row_count = self.rowCount()
+        self.beginInsertRows(parent, row_count, row_count + num_rows - 1)
         yield None
         self.endInsertRows()
 
     @contextlib.contextmanager
     def insert_columns(
         self,
         first: int | None = None,
```

### Comparing `prettyqt-1.5.0/prettyqt/core/animationgroup.py` & `prettyqt-1.6.0/prettyqt/core/animationgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/basictimer.py` & `prettyqt-1.6.0/prettyqt/core/basictimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/collator.py` & `prettyqt-1.6.0/prettyqt/core/collator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/commandlineparser.py` & `prettyqt-1.6.0/prettyqt/core/commandlineparser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/coreapplication.py` & `prettyqt-1.6.0/prettyqt/core/coreapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/cryptographichash.py` & `prettyqt-1.6.0/prettyqt/core/cryptographichash.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/datastream.py` & `prettyqt-1.6.0/prettyqt/core/datastream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/deadlinetimer.py` & `prettyqt-1.6.0/prettyqt/core/deadlinetimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/debug.py` & `prettyqt-1.6.0/prettyqt/core/debug.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/dir.py` & `prettyqt-1.6.0/prettyqt/core/dir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/diriterator.py` & `prettyqt-1.6.0/prettyqt/core/diriterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/easingcurve.py` & `prettyqt-1.6.0/prettyqt/core/easingcurve.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/elapsedtimer.py` & `prettyqt-1.6.0/prettyqt/core/elapsedtimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/event.py` & `prettyqt-1.6.0/prettyqt/core/event.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/eventloop.py` & `prettyqt-1.6.0/prettyqt/core/eventloop.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/filedevice.py` & `prettyqt-1.6.0/prettyqt/core/filedevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/fileinfo.py` & `prettyqt-1.6.0/prettyqt/core/fileinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/fileselector.py` & `prettyqt-1.6.0/prettyqt/core/fileselector.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/filesystemwatcher.py` & `prettyqt-1.6.0/prettyqt/core/filesystemwatcher.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/iodevice.py` & `prettyqt-1.6.0/prettyqt/core/iodevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/itemselectionrange.py` & `prettyqt-1.6.0/prettyqt/core/itemselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/jsondocument.py` & `prettyqt-1.6.0/prettyqt/core/jsondocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/jsonvalue.py` & `prettyqt-1.6.0/prettyqt/core/jsonvalue.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/keycombination.py` & `prettyqt-1.6.0/prettyqt/core/keycombination.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/library.py` & `prettyqt-1.6.0/prettyqt/core/library.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/libraryinfo.py` & `prettyqt-1.6.0/prettyqt/core/libraryinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/line.py` & `prettyqt-1.6.0/prettyqt/core/line.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/linef.py` & `prettyqt-1.6.0/prettyqt/core/linef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/lockfile.py` & `prettyqt-1.6.0/prettyqt/core/lockfile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/margins.py` & `prettyqt-1.6.0/prettyqt/core/margins.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/marginsf.py` & `prettyqt-1.6.0/prettyqt/core/marginsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/metaenum.py` & `prettyqt-1.6.0/prettyqt/core/metaenum.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/metamethod.py` & `prettyqt-1.6.0/prettyqt/core/metamethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/metaobject.py` & `prettyqt-1.6.0/prettyqt/core/metaobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/metatype.py` & `prettyqt-1.6.0/prettyqt/core/metatype.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/mimedata.py` & `prettyqt-1.6.0/prettyqt/core/mimedata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/mimedatabase.py` & `prettyqt-1.6.0/prettyqt/core/mimedatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/object.py` & `prettyqt-1.6.0/prettyqt/core/object.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/operatingsystemversion.py` & `prettyqt-1.6.0/prettyqt/core/operatingsystemversion.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/pluginloader.py` & `prettyqt-1.6.0/prettyqt/core/pluginloader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/process.py` & `prettyqt-1.6.0/prettyqt/core/process.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/processenvironment.py` & `prettyqt-1.6.0/prettyqt/core/processenvironment.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __iter__(self) -> Iterator[tuple[str, str]]:
         return iter((k, self.value(k)) for k in self.keys())
 
     def update(self, other: Mapping[str, str]):
         for k, v in other.items():
             self.insert(k, v)
 
-    def items(self):
+    def items(self) -> list[tuple[str, str]]:
         return list(self)
 
     @classmethod
     def get_system_environment(cls) -> ProcessEnvironment:
         return cls(cls.systemEnvironment())
 
     @classmethod
@@ -43,8 +43,8 @@
         for k, v in dictionary.items():
             env.insert(k, v)
         return env
 
 
 if __name__ == "__main__":
     env = ProcessEnvironment.get_system_environment()
-    print(dict(env))
+    print(env.items())
```

### Comparing `prettyqt-1.5.0/prettyqt/core/propertyanimation.py` & `prettyqt-1.6.0/prettyqt/core/propertyanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/rect.py` & `prettyqt-1.6.0/prettyqt/core/rect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/regularexpression.py` & `prettyqt-1.6.0/prettyqt/core/regularexpression.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/regularexpressionmatch.py` & `prettyqt-1.6.0/prettyqt/core/regularexpressionmatch.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/regularexpressionmatchiterator.py` & `prettyqt-1.6.0/prettyqt/core/regularexpressionmatchiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/resource.py` & `prettyqt-1.6.0/prettyqt/core/resource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/settings.py` & `prettyqt-1.6.0/prettyqt/core/settings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/size.py` & `prettyqt-1.6.0/prettyqt/core/size.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/sizef.py` & `prettyqt-1.6.0/prettyqt/core/sizef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/socketnotifier.py` & `prettyqt-1.6.0/prettyqt/core/socketnotifier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/sortfilterproxymodel.py` & `prettyqt-1.6.0/prettyqt/core/sortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/standardpaths.py` & `prettyqt-1.6.0/prettyqt/core/standardpaths.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/storageinfo.py` & `prettyqt-1.6.0/prettyqt/core/storageinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/temporarydir.py` & `prettyqt-1.6.0/prettyqt/core/temporarydir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/textboundaryfinder.py` & `prettyqt-1.6.0/prettyqt/core/textboundaryfinder.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/textstream.py` & `prettyqt-1.6.0/prettyqt/core/textstream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/timeline.py` & `prettyqt-1.6.0/prettyqt/core/timeline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/timer.py` & `prettyqt-1.6.0/prettyqt/core/timer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/timezone.py` & `prettyqt-1.6.0/prettyqt/core/timezone.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/translator.py` & `prettyqt-1.6.0/prettyqt/core/translator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/url.py` & `prettyqt-1.6.0/prettyqt/core/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,11 +120,26 @@
         return cls(cls.fromUserInput(url, working_dir))
 
     @classmethod
     def from_local_file(cls, path: types.PathType) -> Url:
         url = cls.fromLocalFile(os.fspath(path))
         return cls(url)
 
+    def _has_explicit_scheme(self) -> bool:
+        """Check if a url has an explicit scheme given."""
+        return bool(
+            self.isValid()
+            and self.scheme()
+            and (self.host() or self.path())
+            and not self.path().startswith(":")
+        )
+
+    def is_special_url(self) -> bool:
+        """Return True if url is an about:... or other special URL."""
+        if not self.isValid():
+            return False
+        return self.scheme() in ("about", "file")
+
 
 if __name__ == "__main__":
     url = Url()
     str(url)
```

### Comparing `prettyqt-1.5.0/prettyqt/core/urlquery.py` & `prettyqt-1.6.0/prettyqt/core/urlquery.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return self.hasQueryItem(key)
 
     def __add__(self, other: dict) -> UrlQuery:
         for k, v in other.items():
             self.addQueryItem(k, str(v))
         return self
 
-    def serialize_fields(self):
+    def serialize_fields(self) -> dict[str, Any]:
         return dict(path=self.toString())
 
     def serialize(self) -> dict[str, Any]:
         return self.serialize_fields()
 
     # def add_query_items(self, **items: str):
     #     for k, v in items.items():
```

### Comparing `prettyqt-1.5.0/prettyqt/core/uuid.py` & `prettyqt-1.6.0/prettyqt/core/uuid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Literal
 
 from prettyqt.qt import QtCore
-from prettyqt.utils import bidict
+from prettyqt.utils import InvalidParamError, bidict
 
 
 STRING_FORMATS = bidict(
     with_braces=QtCore.QUuid.StringFormat.WithBraces,
     without_braces=QtCore.QUuid.StringFormat.WithoutBraces,
     id_128=QtCore.QUuid.StringFormat.Id128,
 )
@@ -57,14 +57,29 @@
         return VERSION.inverse[self.version()]
 
     @classmethod
     def create_uuid(cls) -> Uuid:
         # workaround for PySide2, not able to clone in ctor
         return cls(cls.createUuid().toString())
 
+    def to_string(self, fmt: StringFormatStr = "with_braces") -> str:
+        """Return string representation of the Uuid.
+
+        Allowed values are "with_braces", "without_braces", "id_128"
+
+        Args:
+            fmt: Uuid format to use
+
+        Raises:
+            InvalidParamError: Uuid format does not exist
+        """
+        if fmt not in STRING_FORMATS:
+            raise InvalidParamError(fmt, STRING_FORMATS)
+        return self.toString(STRING_FORMATS[fmt])
+
 
 class Uuid(UuidMixin, QtCore.QUuid):
     pass
 
 
 if __name__ == "__main__":
     address = Uuid.create_uuid()
```

### Comparing `prettyqt-1.5.0/prettyqt/core/variantanimation.py` & `prettyqt-1.6.0/prettyqt/core/variantanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/versionnumber.py` & `prettyqt-1.6.0/prettyqt/core/versionnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/core/xmlstreamreader.py` & `prettyqt-1.6.0/prettyqt/core/xmlstreamreader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_animations/bounceanimation.py` & `prettyqt-1.6.0/prettyqt/custom_animations/bounceanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_animations/fadeinanimation.py` & `prettyqt-1.6.0/prettyqt/custom_animations/fadeinanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_animations/slideanimation.py` & `prettyqt-1.6.0/prettyqt/custom_animations/slideanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/__init__.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/buttondelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/buttondelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/checkboxdelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/checkboxdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/icondelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/icondelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/nofocusdelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/nofocusdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/progressbardelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/progressbardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/radiodelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/radiodelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/renderlinkdelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/renderlinkdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_delegates/stardelegate.py` & `prettyqt-1.6.0/prettyqt/custom_delegates/stardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/__init__.py` & `prettyqt-1.6.0/prettyqt/custom_models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 Contains custom models
 """
 
 from .selectionmixin import SelectionMixin
 from .importlibdistributionmodel import ImportlibDistributionModel
 from .regexmatchesmodel import RegexMatchesModel
-from .columnitemmodel import ColumnItemModel, ColumnItem
+from .columnitemmodel import ColumnItemModel, ColumnTableModel, ColumnItem
 from .listmixin import ListMixin
 from .modelmixin import ModelMixin
 from .nesteditem import NestedItem
 from .nestedmodel import NestedModel
 from .subsequencesortfilterproxymodel import SubsequenceSortFilterProxyModel
 
 __all__ = [
     "SelectionMixin",
     "ImportlibDistributionModel",
     "RegexMatchesModel",
     "ColumnItemModel",
+    "ColumnTableModel",
     "ListMixin",
     "ModelMixin",
     "ColumnItem",
     "NestedModel",
     "NestedItem",
     "SubsequenceSortFilterProxyModel",
 ]
```

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/columnitemmodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/columnitemmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from collections.abc import Callable
 from dataclasses import dataclass
 import logging
 
 from prettyqt import constants, core, gui
 from prettyqt.qt import QtCore, QtGui
+from prettyqt.utils import treeitem
 
 
 logger = logging.getLogger(__name__)
 
 SMALL_COL_WIDTH = 120
 MEDIUM_COL_WIDTH = 200
 
@@ -110,36 +111,42 @@
         elif self.width == "medium":
             return MEDIUM_COL_WIDTH
         elif isinstance(self.width, int):
             return self.width
         raise ValueError(self.width)
 
 
-class ColumnItemModel(core.AbstractItemModel):
+class ColumnItemModelMixin:
     """Model that provides an interface to an objectree that is build of TreeItems."""
 
     def __init__(
         self,
         attr_cols: list[ColumnItem] | None = None,
         parent: QtCore.QObject | None = None,
     ):
         super().__init__(parent)
         self._attr_cols = attr_cols if attr_cols is not None else []
 
     def columnCount(self, _parent=None):
         """Return the number of columns in the tree."""
         return len(self._attr_cols)
 
+    def tree_item(self, index: core.ModelIndex) -> treeitem.TreeItem:
+        if not index.isValid():
+            return None
+        else:
+            return index.internalPointer()  # type: ignore
+
     def data(self, index, role):
         """Return the tree item at the given index and role."""
         if not index.isValid():
             return None
 
         col = index.column()
-        tree_item = index.internalPointer()
+        tree_item = self.tree_item(index)
 
         match role:
             case constants.DISPLAY_ROLE | constants.EDIT_ROLE:
                 val = self._attr_cols[col].get_label(tree_item)
                 return val.replace("\n", " ")
             case constants.DECORATION_ROLE:
                 return self._attr_cols[col].get_decoration(tree_item)
@@ -165,14 +172,22 @@
     def headerData(self, section, orientation, role):
         if orientation == constants.HORIZONTAL and role == constants.DISPLAY_ROLE:
             return self._attr_cols[section].name
         else:
             return None
 
 
+class ColumnItemModel(ColumnItemModelMixin, core.AbstractItemModel):
+    pass
+
+
+class ColumnTableModel(ColumnItemModelMixin, core.AbstractTableModel):
+    pass
+
+
 if __name__ == "__main__":
     from prettyqt import widgets
 
     class TestModel(ColumnItemModel):
         def rowCount(self, parent=None):
             return 5
```

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/importlibdistributionmodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/importlibdistributionmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/jsonmodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/listmixin.py` & `prettyqt-1.6.0/prettyqt/custom_models/listmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/modelmixin.py` & `prettyqt-1.6.0/prettyqt/custom_models/modelmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/nesteditem.py` & `prettyqt-1.6.0/prettyqt/custom_models/nesteditem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterable
+from collections.abc import Iterable, Iterator
 
 
 class NestedItem:
     item_name = "not_defined"
 
     def __init__(
         self,
@@ -17,23 +17,23 @@
         self.dynamic_name = dynamic_name if dynamic_name else self.item_name
         self.count = count
         # self.timestamp = kwargs.pop("timestamp", time.time())
         self.children: list[NestedItem] = []
         if children:
             self.add_children(children)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[NestedItem]:
         return iter(self.children)
 
-    def add_children(self, children: Iterable):
+    def add_children(self, children: Iterable[NestedItem]):
         for child in children:
             child.parent = self
         self.children.extend(children)
 
-    def append_child(self, item):
+    def append_child(self, item: NestedItem):
         self.children.append(item)
 
     def child(self, row: int) -> NestedItem:
         return self.children[row]
 
     def row(self) -> int:
         """Return row number.
```

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/nestedmodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/nestedmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/regexmatchesmodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/regexmatchesmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/selectionmixin.py` & `prettyqt-1.6.0/prettyqt/custom_models/selectionmixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py` & `prettyqt-1.6.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/__init__.py` & `prettyqt-1.6.0/prettyqt/custom_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/compositevalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/compositevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/integervalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/integervalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/notemptyvalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/notemptyvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/notzerovalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/notzerovalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/pathvalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/pathvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/regexpatternvalidator.py` & `prettyqt-1.6.0/prettyqt/custom_validators/regexpatternvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_validators/regexvalidators.py` & `prettyqt-1.6.0/prettyqt/custom_validators/regexvalidators.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/__init__.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/booldicttoolbutton.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/booldicttoolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/borderlayout.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/borderlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/codeeditor.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/collapsibleframe.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/collapsibleframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/colorchooserbutton.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/colorchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/completionwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/completionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/dataset.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/dataset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/elidedlabel.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/elidedlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/expandableline.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/expandableline.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         # === SIGNALS === #
         self.expand_btn.toggled.connect(expand_view)
         self.toggle_anim.set_duration(0)
         self.toggle_anim.set_duration(self._animation_duration)
 
     def set_layout(
         self,
-        layout: str | QtWidgets.QLayout | None,
+        layout: widgets.widget.LayoutStr | QtWidgets.QLayout | None,
         margin: int | None = None,
         spacing: int | None = None,
     ) -> None:
         self.content_area.destroy()
         self.content_area.set_layout(layout, margin=margin, spacing=spacing)
         collapsed_height = self.sizeHint().height() - self.content_area.maximumHeight()
         content_height = self.content_area.box.sizeHint().height() + 300
```

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/filechooserbutton.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/filechooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/flagselectionwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/flagselectionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/flowlayout.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/flowlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/fontchooserbutton.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/fontchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/framelesswindow.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/framelesswindow.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,57 +81,57 @@
             self.minimize_button,
             self.maximize_button,
             self.exit_button,
         ]:
             self.box.addWidget(widget)
 
         self.setStyleSheet("width: 100%;" "padding: 0;" "margin: 0;")
-        self.setContentsMargins(0, 0, 0, 0)
-        self.box.setContentsMargins(0, 0, 0, 0)
+        self.set_margin(0)
+        self.box.set_margin(0)
         self.box.setSpacing(0)
 
     def mousePressEvent(self, a0: QtGui.QMouseEvent) -> None:
         self.window_widget.windowHandle().startSystemMove()
 
 
 class FramelessWindow(widgets.Widget):
     BORDER_WIDTH = 5
 
     def __init__(self, parent: QtWidgets.QWidget | None = None):
         super().__init__(parent)
 
         # Remove window title bar and frame
         self.setWindowFlags(
-            QtCore.Qt.WindowFlag.Window  # type: ignore
-            | QtCore.Qt.WindowFlag.FramelessWindowHint
+            QtCore.Qt.WindowType.Window  # type: ignore
+            | QtCore.Qt.WindowType.FramelessWindowHint
         )
 
         self.title_bar = CustomTitleBar(self)
         self.main_widget = widgets.MainWindow()
 
         # Set up layout
         self.main_layout = widgets.BoxLayout("vertical")
         self.main_layout.addWidget(self.title_bar)
         self.main_layout.addWidget(self.main_widget)
 
-        self.main_layout.setContentsMargins(0, 0, 0, 0)
+        self.main_layout.set_margin(0)
         self.main_layout.setSpacing(0)
 
         self.grip_layout = widgets.GridLayout()
 
         self.grip_layout.addLayout(self.main_layout, 1, 1)
         self.grip_layout.addWidget(EdgeGrip("top"), 0, 1)
         self.grip_layout.addWidget(EdgeGrip("right"), 1, 2)
         self.grip_layout.addWidget(EdgeGrip("bottom"), 2, 1)
         self.grip_layout.addWidget(EdgeGrip("left"), 1, 0)
         self.grip_layout.addWidget(EdgeGrip("top_left"), 0, 0)
         self.grip_layout.addWidget(EdgeGrip("top_right"), 0, 2)
         self.grip_layout.addWidget(EdgeGrip("bottom_left"), 2, 0)
         self.grip_layout.addWidget(EdgeGrip("bottom_right"), 2, 2)
-        self.grip_layout.setContentsMargins(0, 0, 0, 0)
+        self.grip_layout.set_margin(0)
         self.grip_layout.setSpacing(0)
         self.setLayout(self.grip_layout)
 
         if sys.platform == "win32":
             self.hwnd = self.winId().__int__()
             window_style = win32gui.GetWindowLong(self.hwnd, GWL_STYLE)
             win32gui.SetWindowLong(
@@ -153,20 +153,20 @@
             #     QtWin.resetExtendedFrame(self)
 
     def __getattr__(self, attr: str):
         return getattr(self.main_widget, attr)
 
     def changeEvent(self, event):
         # not sure if this should be done on non-windows
-        if event.type() == event.WindowStateChange:
+        if event.type() == event.Type.WindowStateChange:
             if self.windowState() & QtCore.Qt.WindowState.WindowMaximized:  # type: ignore
                 margin = abs(self.mapToGlobal(self.rect().topLeft()).y())
-                self.setContentsMargins(margin, margin, margin, margin)
+                self.set_margin(margin)
             else:
-                self.setContentsMargins(0, 0, 0, 0)
+                self.set_margin(0)
 
         return super().changeEvent(event)
 
     def nativeEvent(self, event, message):
         return_value, result = super().nativeEvent(event, message)
         if sys.platform != "win32":
             return return_value, result
@@ -233,37 +233,37 @@
     def __init__(self, edges: str, grip_size=6, parent=None):
         super().__init__(parent)
         self.edges = edges
         self.grip_size = grip_size
         # Sides
         match edges:
             case "top":
-                self.setCursor(QtCore.Qt.SizeVerCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
                 self.setFixedHeight(self.grip_size)
             case "right":
-                self.setCursor(QtCore.Qt.SizeHorCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
                 self.setFixedWidth(self.grip_size)
             case "bottom":
-                self.setCursor(QtCore.Qt.SizeVerCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeVerCursor)
                 self.setFixedHeight(self.grip_size)
             case "left":
-                self.setCursor(QtCore.Qt.SizeHorCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeHorCursor)
                 self.setFixedWidth(self.grip_size)
             # Corners
             case "top_left":
-                self.setCursor(QtCore.Qt.SizeFDiagCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeFDiagCursor)
             case "top_right":
-                self.setCursor(QtCore.Qt.SizeBDiagCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeBDiagCursor)
             case "bottom_left":
-                self.setCursor(QtCore.Qt.SizeBDiagCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeBDiagCursor)
             case "bottom_right":
-                self.setCursor(QtCore.Qt.SizeFDiagCursor)
+                self.setCursor(QtCore.Qt.CursorShape.SizeFDiagCursor)
 
     def mousePressEvent(self, event):
-        if event.button() == QtCore.Qt.LeftButton:
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
             self.parent().windowHandle().startSystemResize(self.edges)
 
 
 if __name__ == "__main__":
     app = widgets.app()
     m = FramelessWindow()
     button = widgets.PushButton("test")
```

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/iconbrowser.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/iconbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/iconlabel.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/iconlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/iconwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/iconwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/image.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/image.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/imageviewer.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/imageviewer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/inputandslider.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/inputandslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/joystickbutton.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/joystickbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/labeledslider.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/labeledslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/listinput.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/listinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/logtextedit.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/logtextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/mappedcheckbox.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/mappedcheckbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/markdownwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/markdownwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/menurecentfiles.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/menurecentfiles.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/notification.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/notification.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/optionalwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/optionalwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/popupinfo.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/popupinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/quick_ref.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/quick_ref.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/ref.html` & `prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/ref.html`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/regexinput.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/regexinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/roundprogressbar.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/roundprogressbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/selectionwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/selectionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/sidebarwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/sidebarwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/singlelinetextedit.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/singlelinetextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/spanslider.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/spanslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/standardiconswidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/standardiconswidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/stringornumberwidget.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/stringornumberwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/subsequencecompleter.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/subsequencecompleter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/timeline.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/timeline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/custom_widgets/waitingspinner.py` & `prettyqt-1.6.0/prettyqt/custom_widgets/waitingspinner.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/eventfilters/animatedtooltipeventfilter.py` & `prettyqt-1.6.0/prettyqt/eventfilters/animatedtooltipeventfilter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/eventfilters/hovericoneventfilter.py` & `prettyqt-1.6.0/prettyqt/eventfilters/hovericoneventfilter.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 class HoverIconEventFilter(core.Object):
     def __init__(self, normal, hover, parent=None):
         super().__init__(parent)
         self.normal = normal
         self.hover = hover
 
     def eventFilter(self, obj, event: core.Event):
-        if event.type() == core.Event.Type.Enter:
-            obj.set_icon(self.hover)
-        elif event.type() == core.Event.Type.Leave:
-            obj.set_icon(self.normal)
+        match event.type():
+            case core.Event.Type.Enter:
+                obj.set_icon(self.hover)
+            case core.Event.Type.Leave:
+                obj.set_icon(self.normal)
         return super().eventFilter(obj, event)
 
 
 if __name__ == "__main__":
     app = widgets.app()
     widget = widgets.PushButton()
     test = HoverIconEventFilter("mdi.timer", "mdi.folder")
```

### Comparing `prettyqt-1.5.0/prettyqt/gui/__init__.py` & `prettyqt-1.6.0/prettyqt/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/abstractfileiconprovider.py` & `prettyqt-1.6.0/prettyqt/gui/abstractfileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/abstracttextdocumentlayout.py` & `prettyqt-1.6.0/prettyqt/gui/abstracttextdocumentlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/brush.py` & `prettyqt-1.6.0/prettyqt/gui/brush.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/clipboard.py` & `prettyqt-1.6.0/prettyqt/gui/clipboard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/color.py` & `prettyqt-1.6.0/prettyqt/gui/color.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/colorspace.py` & `prettyqt-1.6.0/prettyqt/gui/colorspace.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/cursor.py` & `prettyqt-1.6.0/prettyqt/gui/cursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/doublevalidator.py` & `prettyqt-1.6.0/prettyqt/gui/doublevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/drag.py` & `prettyqt-1.6.0/prettyqt/gui/drag.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/font.py` & `prettyqt-1.6.0/prettyqt/gui/font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/fontdatabase.py` & `prettyqt-1.6.0/prettyqt/gui/fontdatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/fontmetrics.py` & `prettyqt-1.6.0/prettyqt/gui/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/fontmetricsf.py` & `prettyqt-1.6.0/prettyqt/gui/fontmetricsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/gradient.py` & `prettyqt-1.6.0/prettyqt/gui/gradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/guiapplication.py` & `prettyqt-1.6.0/prettyqt/gui/guiapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/icon.py` & `prettyqt-1.6.0/prettyqt/gui/icon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/iconengine.py` & `prettyqt-1.6.0/prettyqt/gui/iconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/image.py` & `prettyqt-1.6.0/prettyqt/gui/image.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/imageiohandler.py` & `prettyqt-1.6.0/prettyqt/gui/imageiohandler.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/imagereader.py` & `prettyqt-1.6.0/prettyqt/gui/imagereader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/imagewriter.py` & `prettyqt-1.6.0/prettyqt/gui/imagewriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/inputmethod.py` & `prettyqt-1.6.0/prettyqt/gui/inputmethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/intvalidator.py` & `prettyqt-1.6.0/prettyqt/gui/intvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/keysequence.py` & `prettyqt-1.6.0/prettyqt/gui/keysequence.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/lineargradient.py` & `prettyqt-1.6.0/prettyqt/gui/lineargradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/movie.py` & `prettyqt-1.6.0/prettyqt/gui/movie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pagelayout.py` & `prettyqt-1.6.0/prettyqt/gui/pagelayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pagesize.py` & `prettyqt-1.6.0/prettyqt/gui/pagesize.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/paintdevice.py` & `prettyqt-1.6.0/prettyqt/gui/paintdevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/painter.py` & `prettyqt-1.6.0/prettyqt/gui/painter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/painterpath.py` & `prettyqt-1.6.0/prettyqt/gui/painterpath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/painterpathstroker.py` & `prettyqt-1.6.0/prettyqt/gui/painterpathstroker.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/palette.py` & `prettyqt-1.6.0/prettyqt/gui/palette.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pdfwriter.py` & `prettyqt-1.6.0/prettyqt/gui/pdfwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pen.py` & `prettyqt-1.6.0/prettyqt/gui/pen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pixmap.py` & `prettyqt-1.6.0/prettyqt/gui/pixmap.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/pixmapcache.py` & `prettyqt-1.6.0/prettyqt/gui/pixmapcache.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/polygon.py` & `prettyqt-1.6.0/prettyqt/gui/polygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/polygonf.py` & `prettyqt-1.6.0/prettyqt/gui/polygonf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/radialgradient.py` & `prettyqt-1.6.0/prettyqt/gui/radialgradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/region.py` & `prettyqt-1.6.0/prettyqt/gui/region.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/regularexpressionvalidator.py` & `prettyqt-1.6.0/prettyqt/gui/regularexpressionvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/screen.py` & `prettyqt-1.6.0/prettyqt/gui/screen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/sessionmanager.py` & `prettyqt-1.6.0/prettyqt/gui/sessionmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/standarditem.py` & `prettyqt-1.6.0/prettyqt/gui/standarditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/standarditemmodel.py` & `prettyqt-1.6.0/prettyqt/gui/standarditemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/statictext.py` & `prettyqt-1.6.0/prettyqt/gui/statictext.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/stylehints.py` & `prettyqt-1.6.0/prettyqt/gui/stylehints.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/surface.py` & `prettyqt-1.6.0/prettyqt/gui/surface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/syntaxhighlighter.py` & `prettyqt-1.6.0/prettyqt/gui/syntaxhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textblock.py` & `prettyqt-1.6.0/prettyqt/gui/textblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             return None
         user_data = UserData(data)
         self.setUserData(user_data)
 
     def get_user_data(self):
         user_data = self.userData()
         if isinstance(user_data, UserData):
-            print(user_data.data)
             return user_data.data
         return user_data
 
     @contextlib.contextmanager
     def edit_user_state(self):
         state = self.userState()
         yield state
```

### Comparing `prettyqt-1.5.0/prettyqt/gui/textblockgroup.py` & `prettyqt-1.6.0/prettyqt/gui/textblockgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textblockuserdata.py` & `prettyqt-1.6.0/prettyqt/gui/textblockuserdata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textcharformat.py` & `prettyqt-1.6.0/prettyqt/gui/textcharformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textcursor.py` & `prettyqt-1.6.0/prettyqt/gui/textcursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textdocument.py` & `prettyqt-1.6.0/prettyqt/gui/textdocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textdocumentfragment.py` & `prettyqt-1.6.0/prettyqt/gui/textdocumentfragment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textdocumentwriter.py` & `prettyqt-1.6.0/prettyqt/gui/textdocumentwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textformat.py` & `prettyqt-1.6.0/prettyqt/gui/textformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textframe.py` & `prettyqt-1.6.0/prettyqt/gui/textframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textframeformat.py` & `prettyqt-1.6.0/prettyqt/gui/textframeformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textlayout.py` & `prettyqt-1.6.0/prettyqt/gui/textlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textlength.py` & `prettyqt-1.6.0/prettyqt/gui/textlength.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textline.py` & `prettyqt-1.6.0/prettyqt/gui/textline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textlistformat.py` & `prettyqt-1.6.0/prettyqt/gui/textlistformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/textoption.py` & `prettyqt-1.6.0/prettyqt/gui/textoption.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/texttablecellformat.py` & `prettyqt-1.6.0/prettyqt/gui/texttablecellformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/transform.py` & `prettyqt-1.6.0/prettyqt/gui/transform.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/undocommand.py` & `prettyqt-1.6.0/prettyqt/gui/undocommand.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/undostack.py` & `prettyqt-1.6.0/prettyqt/gui/undostack.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/validator.py` & `prettyqt-1.6.0/prettyqt/gui/validator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/vector3d.py` & `prettyqt-1.6.0/prettyqt/gui/vector3d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/vector4d.py` & `prettyqt-1.6.0/prettyqt/gui/vector4d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/gui/window.py` & `prettyqt-1.6.0/prettyqt/gui/window.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/__init__.py` & `prettyqt-1.6.0/prettyqt/iconprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/animation.py` & `prettyqt-1.6.0/prettyqt/iconprovider/animation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/awesomefileiconprovider.py` & `prettyqt-1.6.0/prettyqt/iconprovider/awesomefileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/awesomequickimageprovider.py` & `prettyqt-1.6.0/prettyqt/iconprovider/awesomequickimageprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/chariconengine.py` & `prettyqt-1.6.0/prettyqt/iconprovider/chariconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/codicon-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/codicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/codicon.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/codicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/phosphor-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/phosphor-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/phosphor.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/phosphor.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/remixicon-charmap.json` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/remixicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/fonts/remixicon.ttf` & `prettyqt-1.6.0/prettyqt/iconprovider/fonts/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/iconic_font.py` & `prettyqt-1.6.0/prettyqt/iconprovider/iconic_font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/iconprovider/svgbuffericonengine.py` & `prettyqt-1.6.0/prettyqt/iconprovider/svgbuffericonengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_ar.qm` & `prettyqt-1.6.0/prettyqt/localization/language_ar.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_bg.qm` & `prettyqt-1.6.0/prettyqt/localization/language_bg.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_ca.qm` & `prettyqt-1.6.0/prettyqt/localization/language_ca.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_cs.qm` & `prettyqt-1.6.0/prettyqt/localization/language_cs.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_da.qm` & `prettyqt-1.6.0/prettyqt/localization/language_da.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_de.qm` & `prettyqt-1.6.0/prettyqt/localization/language_de.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_es.qm` & `prettyqt-1.6.0/prettyqt/localization/language_es.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_fa.qm` & `prettyqt-1.6.0/prettyqt/localization/language_fa.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_fi.qm` & `prettyqt-1.6.0/prettyqt/localization/language_fi.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_fr.qm` & `prettyqt-1.6.0/prettyqt/localization/language_fr.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_gd.qm` & `prettyqt-1.6.0/prettyqt/localization/language_gd.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_gl.qm` & `prettyqt-1.6.0/prettyqt/localization/language_gl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_he.qm` & `prettyqt-1.6.0/prettyqt/localization/language_he.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_hu.qm` & `prettyqt-1.6.0/prettyqt/localization/language_hu.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_it.qm` & `prettyqt-1.6.0/prettyqt/localization/language_it.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_ja.qm` & `prettyqt-1.6.0/prettyqt/localization/language_ja.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_ko.qm` & `prettyqt-1.6.0/prettyqt/localization/language_ko.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_lt.qm` & `prettyqt-1.6.0/prettyqt/localization/language_lt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_lv.qm` & `prettyqt-1.6.0/prettyqt/localization/language_lv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_pl.qm` & `prettyqt-1.6.0/prettyqt/localization/language_pl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_pt.qm` & `prettyqt-1.6.0/prettyqt/localization/language_pt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_ru.qm` & `prettyqt-1.6.0/prettyqt/localization/language_ru.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_sk.qm` & `prettyqt-1.6.0/prettyqt/localization/language_sk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_sl.qm` & `prettyqt-1.6.0/prettyqt/localization/language_sl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_sv.qm` & `prettyqt-1.6.0/prettyqt/localization/language_sv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_uk.qm` & `prettyqt-1.6.0/prettyqt/localization/language_uk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_zh_CN.qm` & `prettyqt-1.6.0/prettyqt/localization/language_zh_CN.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/localization/language_zh_TW.qm` & `prettyqt-1.6.0/prettyqt/localization/language_zh_TW.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/__init__.py` & `prettyqt-1.6.0/prettyqt/location/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/geomaneuver.py` & `prettyqt-1.6.0/prettyqt/location/geomaneuver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/georoute.py` & `prettyqt-1.6.0/prettyqt/location/georoute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/georouterequest.py` & `prettyqt-1.6.0/prettyqt/location/georouterequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/georoutesegment.py` & `prettyqt-1.6.0/prettyqt/location/georoutesegment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/georoutingmanager.py` & `prettyqt-1.6.0/prettyqt/location/georoutingmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/geoserviceprovider.py` & `prettyqt-1.6.0/prettyqt/location/geoserviceprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/place.py` & `prettyqt-1.6.0/prettyqt/location/place.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placeattribute.py` & `prettyqt-1.6.0/prettyqt/location/placeattribute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placecategory.py` & `prettyqt-1.6.0/prettyqt/location/placecategory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placecontactdetail.py` & `prettyqt-1.6.0/prettyqt/location/placecontactdetail.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placecontent.py` & `prettyqt-1.6.0/prettyqt/location/placecontent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placecontentreply.py` & `prettyqt-1.6.0/prettyqt/location/placecontentreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placecontentrequest.py` & `prettyqt-1.6.0/prettyqt/location/placecontentrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placedetailsreply.py` & `prettyqt-1.6.0/prettyqt/location/placedetailsreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placeicon.py` & `prettyqt-1.6.0/prettyqt/location/placeicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placeidreply.py` & `prettyqt-1.6.0/prettyqt/location/placeidreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placemanager.py` & `prettyqt-1.6.0/prettyqt/location/placemanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placematchreply.py` & `prettyqt-1.6.0/prettyqt/location/placematchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placematchrequest.py` & `prettyqt-1.6.0/prettyqt/location/placematchrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placereply.py` & `prettyqt-1.6.0/prettyqt/location/placereply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placesearchreply.py` & `prettyqt-1.6.0/prettyqt/location/placesearchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placesearchrequest.py` & `prettyqt-1.6.0/prettyqt/location/placesearchrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placesearchresult.py` & `prettyqt-1.6.0/prettyqt/location/placesearchresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/placesupplier.py` & `prettyqt-1.6.0/prettyqt/location/placesupplier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/location/qlocation.py` & `prettyqt-1.6.0/prettyqt/location/qlocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/multimediawidgets/graphicsvideoitem.py` & `prettyqt-1.6.0/prettyqt/multimediawidgets/graphicsvideoitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/multimediawidgets/videowidget.py` & `prettyqt-1.6.0/prettyqt/multimediawidgets/videowidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/__init__.py` & `prettyqt-1.6.0/prettyqt/network/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/abstractsocket.py` & `prettyqt-1.6.0/prettyqt/network/abstractsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/hostaddress.py` & `prettyqt-1.6.0/prettyqt/network/hostaddress.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/httpmultipart.py` & `prettyqt-1.6.0/prettyqt/network/httpmultipart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/httppart.py` & `prettyqt-1.6.0/prettyqt/network/httppart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/localserver.py` & `prettyqt-1.6.0/prettyqt/network/localserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/localsocket.py` & `prettyqt-1.6.0/prettyqt/network/localsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkaccessmanager.py` & `prettyqt-1.6.0/prettyqt/network/networkaccessmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkaddressentry.py` & `prettyqt-1.6.0/prettyqt/network/networkaddressentry.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkcookie.py` & `prettyqt-1.6.0/prettyqt/network/networkcookie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkcookiejar.py` & `prettyqt-1.6.0/prettyqt/network/networkcookiejar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkdatagram.py` & `prettyqt-1.6.0/prettyqt/network/networkdatagram.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkinterface.py` & `prettyqt-1.6.0/prettyqt/network/networkinterface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkproxy.py` & `prettyqt-1.6.0/prettyqt/network/networkproxy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/networkrequest.py` & `prettyqt-1.6.0/prettyqt/network/networkrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/tcpserver.py` & `prettyqt-1.6.0/prettyqt/network/tcpserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/network/udpsocket.py` & `prettyqt-1.6.0/prettyqt/network/udpsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/objbrowser/attribute_model.py` & `prettyqt-1.6.0/prettyqt/objbrowser/attribute_model.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/objbrowser/objectbrowser.py` & `prettyqt-1.6.0/prettyqt/objbrowser/objectbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/objbrowser/objectbrowsertreemodel.py` & `prettyqt-1.6.0/prettyqt/objbrowser/objectbrowsertreemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from collections import OrderedDict
 from difflib import SequenceMatcher
 import inspect
 import logging
 from typing import Any
 
-from prettyqt import constants, core, custom_models
+from prettyqt import core, custom_models
 from prettyqt.qt import QtCore
 from prettyqt.utils import helpers, treeitem
 
 
 # TODO: a lot of methods (e.g. rowCount) test if parent.column() > 0. This should probably
 # be replaced with an assert.
 
@@ -99,19 +99,14 @@
             )
             self.inspected_item = self._root_item
 
             # Fetch all items of the root so we can select the first row in the ctor.
             root_index = self.index(0, 0)
             self.fetchMore(root_index)
 
-    def flags(self, index: core.ModelIndex):
-        if not index.isValid():
-            return constants.NO_CHILDREN
-        return constants.IS_ENABLED | constants.IS_SELECTABLE  # type: ignore
-
     def index(
         self, row: int, column: int, parent: core.ModelIndex | None = None
     ) -> core.ModelIndex:
         if parent is None:
             logger.debug("parent is None")
             parent = core.ModelIndex()
 
@@ -406,23 +401,14 @@
         self._show_callables = show_callable_attrs
         self._show_special_attrs = show_special_attrs
 
     def tree_item(self, proxy_index: core.ModelIndex) -> ObjectBrowserTreeItem:
         index = self.mapToSource(proxy_index)
         return self.sourceModel().tree_item(index)
 
-    def first_item_index(self) -> core.ModelIndex:
-        """Return the first child of the root item."""
-        # We cannot just call the same function of the source model because the first node
-        # there may be hidden.
-        source_root_index = self.sourceModel().root_index()
-        proxy_root_index = self.mapFromSource(source_root_index)
-        first_item_index = self.index(0, 0, proxy_root_index)
-        return first_item_index
-
     def filterAcceptsRow(self, source_row: int, source_parent_index: core.ModelIndex):
         """Return true if the item should be included in the model."""
         parent_item = self.sourceModel().tree_item(source_parent_index)
         tree_item = parent_item.child(source_row)
 
         accept = (self._show_special_attrs or not tree_item.is_special_attribute) and (
             self._show_callables or not tree_item.is_callable_attribute
```

### Comparing `prettyqt-1.5.0/prettyqt/positioning/__init__.py` & `prettyqt-1.6.0/prettyqt/positioning/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geoareamonitorinfo.py` & `prettyqt-1.6.0/prettyqt/positioning/geoareamonitorinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geoareamonitorsource.py` & `prettyqt-1.6.0/prettyqt/positioning/geoareamonitorsource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geocircle.py` & `prettyqt-1.6.0/prettyqt/positioning/geocircle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geocoordinate.py` & `prettyqt-1.6.0/prettyqt/positioning/geocoordinate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geolocation.py` & `prettyqt-1.6.0/prettyqt/positioning/geolocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geopath.py` & `prettyqt-1.6.0/prettyqt/positioning/geopath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geopolygon.py` & `prettyqt-1.6.0/prettyqt/positioning/geopolygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geopositioninfo.py` & `prettyqt-1.6.0/prettyqt/positioning/geopositioninfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geopositioninfosource.py` & `prettyqt-1.6.0/prettyqt/positioning/geopositioninfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/georectangle.py` & `prettyqt-1.6.0/prettyqt/positioning/georectangle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geosatelliteinfo.py` & `prettyqt-1.6.0/prettyqt/positioning/geosatelliteinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geosatelliteinfosource.py` & `prettyqt-1.6.0/prettyqt/positioning/geosatelliteinfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/geoshape.py` & `prettyqt-1.6.0/prettyqt/positioning/geoshape.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/positioning/nmeapositioninginfosource.py` & `prettyqt-1.6.0/prettyqt/positioning/nmeapositioninginfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qml/__init__.py` & `prettyqt-1.6.0/prettyqt/qml/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qml/jsengine.py` & `prettyqt-1.6.0/prettyqt/qml/jsengine.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if obj is None:
             obj = QtQml.QJSValue()
         self.installExtensions(EXTENSIONS[extension], obj)
 
     def new_array(self, length: int = 0) -> qml.JSValue:
         return qml.JSValue(self.newArray(length))
 
-    def eval(self, program: str):
+    def eval(self, program: str) -> qml.JSValue:
         result = self.evaluate(program)
         return qml.JSValue(result)  # type: ignore
 
 
 class JSEngine(JSEngineMixin, QtQml.QJSEngine):
     pass
```

### Comparing `prettyqt-1.5.0/prettyqt/qml/jsvalue.py` & `prettyqt-1.6.0/prettyqt/qml/jsvalue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import logging
+from typing import Literal
 
 from prettyqt import qml
 from prettyqt.qt import QtQml
 from prettyqt.utils import bidict
 
 
 logger = logging.getLogger()
 
+ErrorTypeStr = Literal["generic", "range", "reference", "syntax", "type", "uri"]
+
 ERROR_TYPES = bidict(
     generic=QtQml.QJSValue.ErrorType.GenericError,
     range=QtQml.QJSValue.ErrorType.RangeError,
     reference=QtQml.QJSValue.ErrorType.ReferenceError,
     syntax=QtQml.QJSValue.ErrorType.SyntaxError,
     type=QtQml.QJSValue.ErrorType.TypeError,
     uri=QtQml.QJSValue.ErrorType.URIError,
@@ -45,20 +48,20 @@
     def __call__(self, *args) -> JSValue:
         result = self.call(args)
         return JSValue(result)
 
     def get_value(self):
         return self.toVariant()
 
-    def get_error_type(self) -> str | None:
+    def get_error_type(self) -> ErrorTypeStr | None:
         error_type = self.errorType()
         return ERROR_TYPES.inverse.get(error_type)
 
     @classmethod
-    def from_object(cls, obj, jsengine) -> JSValue:
+    def from_object(cls, obj, jsengine: QtQml.QJSEngine) -> JSValue:
         """Convert any python object into a QJSValue (must happen in GUI thread)."""
         match obj:
             case None:
                 return cls()
             case list() | tuple():
                 length = len(obj)
                 array = JSValue(jsengine.newArray(length))
```

### Comparing `prettyqt-1.5.0/prettyqt/qml/qmlapplicationengine.py` & `prettyqt-1.6.0/prettyqt/qml/qmlapplicationengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qml/qmlcomponent.py` & `prettyqt-1.6.0/prettyqt/qml/qmlcomponent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qml/qmlengine.py` & `prettyqt-1.6.0/prettyqt/qml/qmlengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qml/qmlimageproviderbase.py` & `prettyqt-1.6.0/prettyqt/qml/qmlimageproviderbase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qt/QtCore/__init__.py` & `prettyqt-1.6.0/prettyqt/qt/QtCore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qt/QtGui/__init__.py` & `prettyqt-1.6.0/prettyqt/qt/QtGui/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qt/QtWidgets/__init__.py` & `prettyqt-1.6.0/prettyqt/qt/QtWidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qt/__init__.py` & `prettyqt-1.6.0/prettyqt/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/__init__.py` & `prettyqt-1.6.0/prettyqt/qthelp/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/helpenginecore.py` & `prettyqt-1.6.0/prettyqt/qthelp/helpenginecore.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/helpfilterdata.py` & `prettyqt-1.6.0/prettyqt/qthelp/helpfilterdata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/helpfilterengine.py` & `prettyqt-1.6.0/prettyqt/qthelp/helpfilterengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/helpsearchengine.py` & `prettyqt-1.6.0/prettyqt/qthelp/helpsearchengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qthelp/helpsearchresultwidget.py` & `prettyqt-1.6.0/prettyqt/qthelp/helpsearchresultwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/qtre.py` & `prettyqt-1.6.0/prettyqt/qtre.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/__init__.py` & `prettyqt-1.6.0/prettyqt/quick/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/quickitem.py` & `prettyqt-1.6.0/prettyqt/quick/quickitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/quickitemgrabresult.py` & `prettyqt-1.6.0/prettyqt/quick/quickitemgrabresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/quickpainteditem.py` & `prettyqt-1.6.0/prettyqt/quick/quickpainteditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/quickview.py` & `prettyqt-1.6.0/prettyqt/quick/quickview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/quick/quickwindow.py` & `prettyqt-1.6.0/prettyqt/quick/quickwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/scintilla/sciscintilla.py` & `prettyqt-1.6.0/prettyqt/scintilla/sciscintilla.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/statemachine/__init__.py` & `prettyqt-1.6.0/prettyqt/statemachine/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/statemachine/abstracttransition.py` & `prettyqt-1.6.0/prettyqt/statemachine/abstracttransition.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/statemachine/historystate.py` & `prettyqt-1.6.0/prettyqt/statemachine/historystate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/statemachine/state.py` & `prettyqt-1.6.0/prettyqt/statemachine/state.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/statemachine/statemachine.py` & `prettyqt-1.6.0/prettyqt/statemachine/statemachine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/svg/svgrenderer.py` & `prettyqt-1.6.0/prettyqt/svg/svgrenderer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/__init__.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/highlightrule.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/highlightrule.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/jsonhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/jsonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/markdownhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/markdownhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/pythonhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/pythonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/xmlhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/xmlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/syntaxhighlighters/yamlhighlighter.py` & `prettyqt-1.6.0/prettyqt/syntaxhighlighters/yamlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/texttospeech/texttospeech.py` & `prettyqt-1.6.0/prettyqt/texttospeech/texttospeech.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/texttospeech/voice.py` & `prettyqt-1.6.0/prettyqt/texttospeech/voice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/themes/darktheme.qss` & `prettyqt-1.6.0/prettyqt/themes/darktheme.qss`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/__init__.py` & `prettyqt-1.6.0/prettyqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/autoslot.py` & `prettyqt-1.6.0/prettyqt/utils/autoslot.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/colors.py` & `prettyqt-1.6.0/prettyqt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/debugging.py` & `prettyqt-1.6.0/prettyqt/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/helpers.py` & `prettyqt-1.6.0/prettyqt/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/mappers.py` & `prettyqt-1.6.0/prettyqt/utils/mappers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/prettyprinter.py` & `prettyqt-1.6.0/prettyqt/utils/prettyprinter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/searchandreplacemixin.py` & `prettyqt-1.6.0/prettyqt/utils/searchandreplacemixin.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/signallogger.py` & `prettyqt-1.6.0/prettyqt/utils/signallogger.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/singleapplication.py` & `prettyqt-1.6.0/prettyqt/utils/singleapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/syncedproperty.py` & `prettyqt-1.6.0/prettyqt/utils/syncedproperty.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/treeitem.py` & `prettyqt-1.6.0/prettyqt/utils/treeitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/utils/types.py` & `prettyqt-1.6.0/prettyqt/utils/types.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/__init__.py` & `prettyqt-1.6.0/prettyqt/webenginecore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginecontextmenurequest.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginecontextmenurequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginedownloadrequest.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginedownloadrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginehistory.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginehistory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginehttprequest.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginehttprequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginepage.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginepage.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webengineprofile.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webengineprofile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginescript.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginescript.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginescriptcollection.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginescriptcollection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from collections.abc import Iterator
+
 from prettyqt.qt import QtWebEngineCore
 
 
 class WebEngineScriptCollection:
     def __init__(self, item: QtWebEngineCore.QWebEngineScriptCollection):
         self.item = item
 
@@ -12,15 +14,15 @@
 
     def __getitem__(self, index: str) -> QtWebEngineCore.QWebEngineScript:
         return self.item.find(index)[0]
 
     def __len__(self):
         return self.item.count()
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[QtWebEngineCore.QWebEngineScript]:
         return iter(self.item.toList())
 
     def __contains__(self, other: QtWebEngineCore.QWebEngineScript):
         return self.item.contains(other)
 
     def __add__(
         self,
```

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webenginesettings.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webenginesettings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginecore/webengineurlscheme.py` & `prettyqt-1.6.0/prettyqt/webenginecore/webengineurlscheme.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/webenginewidgets/webengineview.py` & `prettyqt-1.6.0/prettyqt/webenginewidgets/webengineview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/__init__.py` & `prettyqt-1.6.0/prettyqt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/abstractbutton.py` & `prettyqt-1.6.0/prettyqt/widgets/abstractbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/abstractitemview.py` & `prettyqt-1.6.0/prettyqt/widgets/abstractitemview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/abstractscrollarea.py` & `prettyqt-1.6.0/prettyqt/widgets/abstractscrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/abstractslider.py` & `prettyqt-1.6.0/prettyqt/widgets/abstractslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/abstractspinbox.py` & `prettyqt-1.6.0/prettyqt/widgets/abstractspinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/action.py` & `prettyqt-1.6.0/prettyqt/widgets/action.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/actiongroup.py` & `prettyqt-1.6.0/prettyqt/widgets/actiongroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/application.py` & `prettyqt-1.6.0/prettyqt/widgets/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,26 +124,33 @@
     ):
         if isinstance(ss, os.PathLike):
             ss = pathlib.Path(ss).read_text()
         elif ss is None:
             ss = ""
         self.setStyleSheet(str(ss))
 
+    def set_style(self, style: str):
+        self.setStyle(QtWidgets.QStyleFactory.create(style))
+        icon_color = self.get_palette().get_color("highlighted_text")
+        iconprovider.set_defaults(color=icon_color)
+
     def get_stylesheet(self) -> qstylizer.style.StyleSheet:
         return qstylizer.parser.parse(self.styleSheet())
 
     def set_theme(self, theme: constants.ThemeStr):
         self.set_palette(theme)
-        if theme == "default":
-            self.set_stylesheet("")
-            iconprovider.set_defaults(color="black")
-        elif theme == "dark":
-            ss = (paths.THEMES_PATH / "darktheme.qss").read_text()
-            self.set_stylesheet(ss)
-            iconprovider.set_defaults(color="lightblue")
+        match theme:
+            case "default":
+                self.set_stylesheet("")
+                color = self.get_palette().get_color("highlighted_text")
+            case "dark":
+                ss = (paths.THEMES_PATH / "darktheme.qss").read_text()
+                self.set_stylesheet(ss)
+                color = gui.Color("lightblue")
+        iconprovider.set_defaults(color=color)
 
     @classmethod
     def get_available_themes(cls) -> dict[constants.ThemeStr, str]:
         return dict(default="Default", dark="Dark")
 
     def send_event(self, obj_or_str: str | QtCore.QObject, event: QtCore.QEvent):
         obj = self.get_widget(obj_or_str) if isinstance(obj_or_str, str) else obj_or_str
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/boxlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/boxlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/calendarwidget.py` & `prettyqt-1.6.0/prettyqt/widgets/calendarwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/checkbox.py` & `prettyqt-1.6.0/prettyqt/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/colordialog.py` & `prettyqt-1.6.0/prettyqt/widgets/colordialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/combobox.py` & `prettyqt-1.6.0/prettyqt/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/completer.py` & `prettyqt-1.6.0/prettyqt/widgets/completer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/datawidgetmapper.py` & `prettyqt-1.6.0/prettyqt/widgets/datawidgetmapper.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/dateedit.py` & `prettyqt-1.6.0/prettyqt/widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/datetimeedit.py` & `prettyqt-1.6.0/prettyqt/widgets/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/dial.py` & `prettyqt-1.6.0/prettyqt/widgets/dial.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/dialog.py` & `prettyqt-1.6.0/prettyqt/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/dialogbuttonbox.py` & `prettyqt-1.6.0/prettyqt/widgets/dialogbuttonbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/dockwidget.py` & `prettyqt-1.6.0/prettyqt/widgets/dockwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/doublespinbox.py` & `prettyqt-1.6.0/prettyqt/widgets/doublespinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/filedialog.py` & `prettyqt-1.6.0/prettyqt/widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/fileiconprovider.py` & `prettyqt-1.6.0/prettyqt/widgets/fileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/filesystemmodel.py` & `prettyqt-1.6.0/prettyqt/widgets/filesystemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/fontcombobox.py` & `prettyqt-1.6.0/prettyqt/widgets/fontcombobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/formlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/formlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections.abc import Iterator
 from typing import Literal
 
 from prettyqt import widgets
 from prettyqt.qt import QtWidgets
 from prettyqt.utils import InvalidParamError, bidict
 
 
@@ -52,15 +53,15 @@
             row = index
             role = "both"
         self.set_widget(value, row, role)
 
     def __delitem__(self, index: int):
         self.removeRow(index)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[QtWidgets.QWidget | QtWidgets.QLayout]:
         return iter(self[i] for i in range(self.count()) if self[i] is not None)
 
     def __len__(self) -> int:
         """Needed for PySide2."""
         return self.rowCount()
 
     def __add__(self, other: QtWidgets.QWidget | QtWidgets.QLayout | tuple):
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/frame.py` & `prettyqt-1.6.0/prettyqt/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/gesture.py` & `prettyqt-1.6.0/prettyqt/widgets/gesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsanchorlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsanchorlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsblureffect.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsblureffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsellipseitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsellipseitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsgridlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsgridlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterable
+from collections.abc import Iterable, Iterator
 
 from prettyqt import constants, widgets
 from prettyqt.qt import QtWidgets
 from prettyqt.utils import InvalidParamError
 
 
 class GraphicsGridLayout(widgets.GraphicsLayoutMixin, QtWidgets.QGraphicsGridLayout):
@@ -43,15 +43,15 @@
         return type(self), (), self.__getstate__()
 
     def __setstate__(self, state):
         for i, (item, pos) in enumerate(zip(state["widgets"], state["positions"])):
             x, y, w, h = pos
             self[x : x + w - 1, y : y + h - 1] = item
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[QtWidgets.QWidget | QtWidgets.QLayout]:
         return iter(self[i] for i in range(self.count()) if self[i] is not None)
 
     def __add__(
         self,
         other: (Iterable[QtWidgets.QGraphicsLayoutItem] | QtWidgets.QGraphicsLayoutItem),
     ):
         if isinstance(other, Iterable):
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicslayout.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicslayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicslinearlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicslinearlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicslineitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicslineitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsobject.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsopacityeffect.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsopacityeffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicspixmapitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicspixmapitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicspolygonitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicspolygonitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsrectitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsrectitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsrotation.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsrotation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsscene.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsscene.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicstextitem.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicstextitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicsview.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicsview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/graphicswidget.py` & `prettyqt-1.6.0/prettyqt/widgets/graphicswidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/gridlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/gridlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/groupbox.py` & `prettyqt-1.6.0/prettyqt/widgets/groupbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/headerview.py` & `prettyqt-1.6.0/prettyqt/widgets/headerview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/inputdialog.py` & `prettyqt-1.6.0/prettyqt/widgets/inputdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/itemeditorfactory.py` & `prettyqt-1.6.0/prettyqt/widgets/itemeditorfactory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/keysequenceedit.py` & `prettyqt-1.6.0/prettyqt/widgets/keysequenceedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/label.py` & `prettyqt-1.6.0/prettyqt/widgets/label.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/layout.py` & `prettyqt-1.6.0/prettyqt/widgets/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections.abc import Iterator
 from typing import Literal
 
 from prettyqt import constants, core, widgets
 from prettyqt.qt import QtCore, QtWidgets
 from prettyqt.utils import InvalidParamError, bidict
 
 
@@ -40,15 +41,15 @@
 
     def __len__(self) -> int:
         return self.count()
 
     def __repr__(self):
         return f"{type(self).__name__}()"
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[QtWidgets.QWidget | QtWidgets.QLayout | None]:
         return iter(self[i] for i in range(self.count()))
 
     def __contains__(self, item: QtWidgets.QWidget | QtWidgets.QLayoutItem):
         return self.indexOf(item) >= 0
 
     def serialize_fields(self):
         return dict(
@@ -87,15 +88,15 @@
         """
         return SIZE_CONSTRAINT.inverse[self.sizeConstraint()]
 
     def set_alignment(
         self,
         alignment: constants.AlignmentStr,
         item: QtWidgets.QWidget | QtWidgets.QLayout | None = None,
-    ):
+    ) -> bool:
         """Set the alignment for widget / layout to alignment.
 
         Returns true if w is found in this layout (not including child layouts).
 
         Args:
             alignment: alignment for the layout
             item: set alignment for specific child only
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/layoutitem.py` & `prettyqt-1.6.0/prettyqt/widgets/layoutitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/lcdnumber.py` & `prettyqt-1.6.0/prettyqt/widgets/lcdnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/lineedit.py` & `prettyqt-1.6.0/prettyqt/widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/listview.py` & `prettyqt-1.6.0/prettyqt/widgets/listview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/listwidget.py` & `prettyqt-1.6.0/prettyqt/widgets/listwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/listwidgetitem.py` & `prettyqt-1.6.0/prettyqt/widgets/listwidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/mainwindow.py` & `prettyqt-1.6.0/prettyqt/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/mdiarea.py` & `prettyqt-1.6.0/prettyqt/widgets/mdiarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/mdisubwindow.py` & `prettyqt-1.6.0/prettyqt/widgets/mdisubwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/menu.py` & `prettyqt-1.6.0/prettyqt/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/menubar.py` & `prettyqt-1.6.0/prettyqt/widgets/menubar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/messagebox.py` & `prettyqt-1.6.0/prettyqt/widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/pangesture.py` & `prettyqt-1.6.0/prettyqt/widgets/pangesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/pinchgesture.py` & `prettyqt-1.6.0/prettyqt/widgets/pinchgesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/plaintextedit.py` & `prettyqt-1.6.0/prettyqt/widgets/plaintextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/progressbar.py` & `prettyqt-1.6.0/prettyqt/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/progressdialog.py` & `prettyqt-1.6.0/prettyqt/widgets/progressdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/pushbutton.py` & `prettyqt-1.6.0/prettyqt/widgets/pushbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/radiobutton.py` & `prettyqt-1.6.0/prettyqt/widgets/radiobutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/rubberband.py` & `prettyqt-1.6.0/prettyqt/widgets/rubberband.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/scrollarea.py` & `prettyqt-1.6.0/prettyqt/widgets/scrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/scroller.py` & `prettyqt-1.6.0/prettyqt/widgets/scroller.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/scrollerproperties.py` & `prettyqt-1.6.0/prettyqt/widgets/scrollerproperties.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/shortcut.py` & `prettyqt-1.6.0/prettyqt/widgets/shortcut.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/sizepolicy.py` & `prettyqt-1.6.0/prettyqt/widgets/sizepolicy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/slider.py` & `prettyqt-1.6.0/prettyqt/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/spaceritem.py` & `prettyqt-1.6.0/prettyqt/widgets/spaceritem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/spinbox.py` & `prettyqt-1.6.0/prettyqt/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/splashscreen.py` & `prettyqt-1.6.0/prettyqt/widgets/splashscreen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/splitter.py` & `prettyqt-1.6.0/prettyqt/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/splitterhandle.py` & `prettyqt-1.6.0/prettyqt/widgets/splitterhandle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/stackedlayout.py` & `prettyqt-1.6.0/prettyqt/widgets/stackedlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/stackedwidget.py` & `prettyqt-1.6.0/prettyqt/widgets/stackedwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/statusbar.py` & `prettyqt-1.6.0/prettyqt/widgets/statusbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/style.py` & `prettyqt-1.6.0/prettyqt/widgets/style.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptionbutton.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptionbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptionheader.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptionheader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptionmenuitem.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptionmenuitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptionslider.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptionslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptiontab.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptiontab.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptiontoolbox.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptiontoolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/styleoptionviewitem.py` & `prettyqt-1.6.0/prettyqt/widgets/styleoptionviewitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/swipegesture.py` & `prettyqt-1.6.0/prettyqt/widgets/swipegesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/systemtrayicon.py` & `prettyqt-1.6.0/prettyqt/widgets/systemtrayicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tabbar.py` & `prettyqt-1.6.0/prettyqt/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tableview.py` & `prettyqt-1.6.0/prettyqt/widgets/tableview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tablewidget.py` & `prettyqt-1.6.0/prettyqt/widgets/tablewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tablewidgetitem.py` & `prettyqt-1.6.0/prettyqt/widgets/tablewidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tablewidgetselectionrange.py` & `prettyqt-1.6.0/prettyqt/widgets/tablewidgetselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tabwidget.py` & `prettyqt-1.6.0/prettyqt/widgets/tabwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/textbrowser.py` & `prettyqt-1.6.0/prettyqt/widgets/textbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/textedit.py` & `prettyqt-1.6.0/prettyqt/widgets/textedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/timeedit.py` & `prettyqt-1.6.0/prettyqt/widgets/timeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/toolbar.py` & `prettyqt-1.6.0/prettyqt/widgets/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         btn.setToolButtonStyle(self.toolButtonStyle())
         btn.set_icon(icon)
         self.menu_buttons.append(btn)
         self.addWidget(btn)
         return btn
 
     def add_separator(
-        self, text: str | None = None, before: QtWidgets.QAction = None
+        self, text: str | None = None, before: QtWidgets.QAction | None = None
     ) -> QtWidgets.QAction:
         """Adds a separator showing an optional label.
 
         Args:
             text: Text to show on separator
             before: insert separator before specific action
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/toolbox.py` & `prettyqt-1.6.0/prettyqt/widgets/toolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/toolbutton.py` & `prettyqt-1.6.0/prettyqt/widgets/toolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/tooltip.py` & `prettyqt-1.6.0/prettyqt/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/treeview.py` & `prettyqt-1.6.0/prettyqt/widgets/treeview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/treewidget.py` & `prettyqt-1.6.0/prettyqt/widgets/treewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/treewidgetitem.py` & `prettyqt-1.6.0/prettyqt/widgets/treewidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/treewidgetitemiterator.py` & `prettyqt-1.6.0/prettyqt/widgets/treewidgetitemiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/undoview.py` & `prettyqt-1.6.0/prettyqt/widgets/undoview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/whatsthis.py` & `prettyqt-1.6.0/prettyqt/widgets/whatsthis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/widget.py` & `prettyqt-1.6.0/prettyqt/widgets/widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         icon = iconprovider.get_icon(icon, color=colors.WINDOW_ICON_COLOR)
         self.setWindowIcon(icon)
 
     def get_icon(self) -> gui.Icon | None:
         icon = self.windowIcon()
         if icon.isNull():
             return None
-        return gui.Icon(self.windowIcon())
+        return gui.Icon(icon)
 
     def set_min_size(self, *size) -> None:
         self.setMinimumSize(*size)
 
     def set_max_size(self, *size) -> None:
         self.setMaximumSize(*size)
 
@@ -325,19 +325,22 @@
         ss = self.get_stylesheet()
         yield ss
         self.set_stylesheet(ss)
 
     def set_stylesheet(
         self, ss: None | str | qstylizer.style.StyleSheet | types.PathType
     ):
-        if isinstance(ss, os.PathLike):
-            ss = pathlib.Path(ss).read_text()
-        elif ss is None:
-            ss = ""
-        self.setStyleSheet(str(ss))
+        match ss:
+            case None:
+                ss = ""
+            case os.PathLike():
+                ss = pathlib.Path(ss).read_text()
+            case qstylizer.style.StyleSheet():
+                ss = str(ss)
+        self.setStyleSheet(ss)
 
     def get_stylesheet(self) -> qstylizer.style.StyleSheet:
         try:
             return qstylizer.parser.parse(self.styleSheet())
         except ValueError:
             return qstylizer.style.StyleSheet()
 
@@ -423,33 +426,30 @@
         layout: LayoutStr | QtWidgets.QLayout | None,
         margin: int | None = None,
         spacing: int | None = None,
     ):
         if layout is None:
             return
         match layout:
-            case "horizontal":
-                self.box = widgets.BoxLayout("horizontal")
-            case "vertical":
-                self.box = widgets.BoxLayout("vertical")
+            case "horizontal" | "vertical":
+                self.box = widgets.BoxLayout(layout)
             case "grid":
                 self.box = widgets.GridLayout()
             case "form":
                 self.box = widgets.FormLayout()
             case "stacked":
                 self.box = widgets.StackedLayout()
             case "flow":
                 from prettyqt import custom_widgets
 
                 self.box = custom_widgets.FlowLayout()
+            case QtWidgets.QLayout():
+                self.box = layout
             case _:
-                if isinstance(layout, QtWidgets.QLayout):
-                    self.box = layout
-                else:
-                    raise ValueError("Invalid Layout")
+                raise ValueError("Invalid Layout")
         self.setLayout(self.box)
         if margin is not None:
             self.box.set_margin(margin)
         if spacing is not None:
             self.box.setSpacing(spacing)
 
     def center(self, screen: int = 0) -> None:
@@ -515,38 +515,61 @@
         return True
 
     def set_mask(
         self,
         area: types.RectType | QtGui.QRegion | None,
         typ: gui.region.RegionTypeStr = "rectangle",
     ):
-        if area is None:
-            self.clearMask()
-            return
-        if isinstance(area, tuple):
-            area = QtCore.QRect(*area)
-        if isinstance(area, QtCore.QRect):
-            area = gui.Region(area, gui.region.REGION_TYPE[typ])
+        match area:
+            case None:
+                self.clearMask()
+                return
+            case tuple():
+                area = gui.Region(*area, gui.region.REGION_TYPE[typ])
+            case QtCore.QRect():
+                area = gui.Region(area, gui.region.REGION_TYPE[typ])
         self.setMask(area)
 
     def set_window_file_path(self, path: types.PathType):
         self.setWindowFilePath(os.fspath(path))
 
     def get_window_file_path(self) -> pathlib.Path | None:
         path = self.windowFilePath()
         if not path:
             return None
         return pathlib.Path(path)
 
+    def get_image(self) -> QtGui.QPixmap:
+        image = self.grab()
+        if gl_widget := self.find_child(QtWidgets.QOpenGLWidget):
+            d = gl_widget.mapToGlobal(core.Point()) - self.mapToGlobal(core.Point())
+            with gui.Painter(image) as painter:
+                painter.set_composition_mode("source_atop")
+                painter.drawImage(d, gl_widget.grabFramebuffer())
+        return image
+
     def get_screen(self) -> gui.Screen | None:
         window = self.window().windowHandle()
         if window is None:
             return None
         return gui.Screen(window.screen())
 
+    def delete_children(self):
+        """Delete all children of the specified QObject."""
+        if hasattr(self, "clear"):
+            return self.clear()
+        layout = self.layout()
+        while layout.count():
+            item = layout.takeAt(0)
+            widget = item.widget()
+            if widget:
+                widget.deleteLater()
+            else:
+                self.delete_children(item.layout())
+
 
 class Widget(WidgetMixin, prettyprinter.PrettyPrinter, QtWidgets.QWidget):
     pass
 
 
 if __name__ == "__main__":
     app = widgets.app()
```

### Comparing `prettyqt-1.5.0/prettyqt/widgets/widgetaction.py` & `prettyqt-1.6.0/prettyqt/widgets/widgetaction.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/wizard.py` & `prettyqt-1.6.0/prettyqt/widgets/wizard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/prettyqt/widgets/wizardpage.py` & `prettyqt-1.6.0/prettyqt/widgets/wizardpage.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.5.0/pyproject.toml` & `prettyqt-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PrettyQt"
-version = "1.5.0"
+version = "1.6.0"
 description = "A pythonic layer on top of PyQt6 / PySide6"
 readme = 'docs/index.md'
 repository = "https://github.com/phil65/prettyqt"
 homepage = "https://github.com/phil65/prettyqt"
 authors = ["phil65 <philipptemminghoff@googlemail.com>"]
 packages = [
     { include = "prettyqt" },
@@ -35,25 +35,25 @@
 # PyQtAds = {version = "^3.8", optional=true}
 pyside6 = {version = "^6.5", python = "<3.12", optional=true}
 darkdetect = {version = "^0", markers = "sys_platform == 'darwin'"}
 pywin32 = {version = "*", markers = "sys_platform == 'win32'"}
 pygments = "^2.6"
 qstylizer = "^0.2"
 deprecated = "^1.2"
-types-Deprecated = "^1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pip = "^23"
 pytest-cov = "^4"
 pytest-qt = {version = "^4.1"}
 mypy = "^1"
 types-Deprecated = "^1.2"
 types-docutils = "^0"
 types-orjson = "^3.6"
+types-python-dateutil = "^2"
 pylint = "^2.5"
 pytest-xvfb = {version = "^2", markers = "sys_platform == 'linux'"}
 coverage = "^7"
 mkdocs = "^1"
 mkdocs-material = "^9"
 mkdocstrings = {version = "^0", extras = ["python-legacy"]}
 
@@ -176,15 +176,15 @@
   | build
   | dist
   | tests/.*/setup.py
 )/
 '''
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.5.0"
+version = "1.6.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_start_rev = "v0.100.0"
 changelog_file = "docs/changelog.md"
 version_files = [
     "prettyqt/__init__.py:__version__",
     "pyproject.toml:version",
```

### Comparing `prettyqt-1.5.0/PKG-INFO` & `prettyqt-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyqt
-Version: 1.5.0
+Version: 1.6.0
 Summary: A pythonic layer on top of PyQt6 / PySide6
 Home-page: https://github.com/phil65/prettyqt
 Author: phil65
 Author-email: philipptemminghoff@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +22,14 @@
 Requires-Dist: docutils (>=0.19,<0.20) ; extra == "addons"
 Requires-Dist: orjson (>=3,<4) ; (python_version < "3.12") and (extra == "addons")
 Requires-Dist: pygments (>=2.6,<3.0)
 Requires-Dist: pyside6 (>=6.5,<7.0) ; (python_version < "3.12") and (extra == "pyside6")
 Requires-Dist: pywin32 ; sys_platform == "win32"
 Requires-Dist: qstylizer (>=0.2,<0.3)
 Requires-Dist: regex (>=2023,<2024)
-Requires-Dist: types-Deprecated (>=1.2,<2.0)
 Project-URL: Repository, https://github.com/phil65/prettyqt
 Description-Content-Type: text/markdown
 
 # prettyqt: Pythonic layer on top of PyQt5 / PyQt6 / PySide6
 [![PyPI Latest Release](https://img.shields.io/pypi/v/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![Package Status](https://img.shields.io/pypi/status/prettyqt.svg)](https://pypi.org/project/prettyqt/)
 [![License](https://img.shields.io/pypi/l/prettyqt.svg)](https://github.com/phil65/PrettyQt/blob/master/LICENSE)
```

