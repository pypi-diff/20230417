# Comparing `tmp/mtap-1.2.0.tar.gz` & `tmp/mtap-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtap-1.2.0.tar", last modified: Sat Apr 15 17:37:51 2023, max compression
+gzip compressed data, was "mtap-1.2.1.tar", last modified: Mon Apr 17 14:28:20 2023, max compression
```

## Comparing `mtap-1.2.0.tar` & `mtap-1.2.1.tar`

### file list

```diff
@@ -1,315 +1,327 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/
--rw-r--r--   0 ben       (1000) ben       (1000)       94 2023-03-11 15:03:25.000000 mtap-1.2.0/.dockerignore
--rw-r--r--   0 ben       (1000) ben       (1000)      122 2023-03-11 15:03:25.000000 mtap-1.2.0/.flake8
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/.github/
--rw-r--r--   0 ben       (1000) ben       (1000)      273 2023-03-11 15:03:25.000000 mtap-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/.github/workflows/
--rw-r--r--   0 ben       (1000) ben       (1000)     2820 2023-03-11 15:03:25.000000 mtap-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     5326 2023-03-30 15:59:37.000000 mtap-1.2.0/.gitignore
--rw-r--r--   0 ben       (1000) ben       (1000)      434 2023-03-30 15:59:37.000000 mtap-1.2.0/.readthedocs.yaml
--rw-r--r--   0 ben       (1000) ben       (1000)      708 2023-03-11 15:03:25.000000 mtap-1.2.0/Dockerfile-dev
--rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-11 15:03:25.000000 mtap-1.2.0/LICENSE.txt
--rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-15 17:37:51.555431 mtap-1.2.0/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     2476 2023-04-15 15:21:56.000000 mtap-1.2.0/README.md
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/
--rw-r--r--   0 ben       (1000) ben       (1000)     1343 2023-03-11 15:03:25.000000 mtap-1.2.0/go/Makefile
--rw-r--r--   0 ben       (1000) ben       (1000)     1477 2023-03-30 15:59:37.000000 mtap-1.2.0/go/doc.go
--rw-r--r--   0 ben       (1000) ben       (1000)     1835 2023-03-30 15:59:37.000000 mtap-1.2.0/go/go.mod
--rw-r--r--   0 ben       (1000) ben       (1000)    65077 2023-03-30 15:59:37.000000 mtap-1.2.0/go/go.sum
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/mtap/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/mtap/api/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/api/v1/
--rw-r--r--   0 ben       (1000) ben       (1000)   104710 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events.pb.go
--rw-r--r--   0 ben       (1000) ben       (1000)    71157 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events.pb.gw.go
--rw-r--r--   0 ben       (1000) ben       (1000)    26240 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events_grpc.pb.go
--rw-r--r--   0 ben       (1000) ben       (1000)    33560 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing.pb.go
--rw-r--r--   0 ben       (1000) ben       (1000)    16594 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing.pb.gw.go
--rw-r--r--   0 ben       (1000) ben       (1000)     7483 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing_grpc.pb.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/consul/
--rw-r--r--   0 ben       (1000) ben       (1000)     2981 2023-03-11 15:03:25.000000 mtap-1.2.0/go/mtap/consul/resolver.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/processors/
--rw-r--r--   0 ben       (1000) ben       (1000)     7921 2023-03-30 15:59:37.000000 mtap-1.2.0/go/mtap/processors/processors.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap-gateway/
--rw-r--r--   0 ben       (1000) ben       (1000)     4732 2023-04-14 22:47:09.000000 mtap-1.2.0/go/mtap-gateway/mtap-gateway.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/store-swaggers/
--rw-r--r--   0 ben       (1000) ben       (1000)     1359 2023-03-11 15:03:25.000000 mtap-1.2.0/go/store-swaggers/main.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/googleapis/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/googleapis/google/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/third_party/googleapis/google/api/
--rw-r--r--   0 ben       (1000) ben       (1000)     1045 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/annotations.proto
--rw-r--r--   0 ben       (1000) ben       (1000)     3604 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/field_behavior.proto
--rw-r--r--   0 ben       (1000) ben       (1000)    15140 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/http.proto
--rw-r--r--   0 ben       (1000) ben       (1000)     2693 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/httpbody.proto
--rw-r--r--   0 ben       (1000) ben       (1000)      283 2023-03-30 15:59:37.000000 mtap-1.2.0/go/tools.go
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/
--rw-r--r--   0 ben       (1000) ben       (1000)     7975 2023-04-15 15:21:56.000000 mtap-1.2.0/java/build.gradle
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/gradle/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/gradle/wrapper/
--rw-r--r--   0 ben       (1000) ben       (1000)    61608 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 ben       (1000) ben       (1000)      221 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.properties
--rwxr-xr-x   0 ben       (1000) ben       (1000)     8495 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradlew
--rw-r--r--   0 ben       (1000) ben       (1000)     2868 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradlew.bat
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/log_resources/
--rw-r--r--   0 ben       (1000) ben       (1000)      396 2023-03-11 15:03:25.000000 mtap-1.2.0/java/log_resources/log4j2.xml
--rw-r--r--   0 ben       (1000) ben       (1000)      650 2023-03-11 15:03:25.000000 mtap-1.2.0/java/settings.gradle
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/umn/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/
--rw-r--r--   0 ben       (1000) ben       (1000)    32081 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1042 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1046 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/
--rw-r--r--   0 ben       (1000) ben       (1000)    11652 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3187 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java
--rw-r--r--   0 ben       (1000) ben       (1000)     6838 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2688 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3324 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1745 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1583 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/
--rw-r--r--   0 ben       (1000) ben       (1000)     3269 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java
--rw-r--r--   0 ben       (1000) ben       (1000)     4068 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1192 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1446 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/
--rw-r--r--   0 ben       (1000) ben       (1000)      829 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2282 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java
--rw-r--r--   0 ben       (1000) ben       (1000)     5628 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java
--rw-r--r--   0 ben       (1000) ben       (1000)     4406 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java
--rw-r--r--   0 ben       (1000) ben       (1000)      711 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/
--rw-r--r--   0 ben       (1000) ben       (1000)     1280 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-04-14 01:30:11.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/
--rw-r--r--   0 ben       (1000) ben       (1000)     2110 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java
--rw-r--r--   0 ben       (1000) ben       (1000)      872 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java
--rw-r--r--   0 ben       (1000) ben       (1000)      775 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java
--rw-r--r--   0 ben       (1000) ben       (1000)    14937 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java
--rw-r--r--   0 ben       (1000) ben       (1000)    16528 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java
--rw-r--r--   0 ben       (1000) ben       (1000)    16546 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java
--rw-r--r--   0 ben       (1000) ben       (1000)    13871 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1978 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java
--rw-r--r--   0 ben       (1000) ben       (1000)    13061 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java
--rw-r--r--   0 ben       (1000) ben       (1000)     5777 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java
--rw-r--r--   0 ben       (1000) ben       (1000)     5921 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java
--rw-r--r--   0 ben       (1000) ben       (1000)    10132 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2361 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2030 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2108 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2632 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java
--rw-r--r--   0 ben       (1000) ben       (1000)    19216 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1454 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java
--rw-r--r--   0 ben       (1000) ben       (1000)      864 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/
--rw-r--r--   0 ben       (1000) ben       (1000)     9045 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1404 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2388 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3801 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java
--rw-r--r--   0 ben       (1000) ben       (1000)      803 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java
--rw-r--r--   0 ben       (1000) ben       (1000)      288 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HealthService.java
--rw-r--r--   0 ben       (1000) ben       (1000)      277 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/KeyValue.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1892 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2522 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1542 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2217 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java
--rw-r--r--   0 ben       (1000) ben       (1000)     6864 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1212 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java
--rw-r--r--   0 ben       (1000) ben       (1000)    17320 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java
--rw-r--r--   0 ben       (1000) ben       (1000)      773 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1489 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1877 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2773 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2369 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java
--rw-r--r--   0 ben       (1000) ben       (1000)      381 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/TimingService.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/
--rw-r--r--   0 ben       (1000) ben       (1000)     1132 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3089 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/umn/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/
--rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/
--rw-r--r--   0 ben       (1000) ben       (1000)     2937 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/
--rw-r--r--   0 ben       (1000) ben       (1000)     9334 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     9496 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)    13774 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     9602 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     6141 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)    14423 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3668 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     5091 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)    23583 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)    23618 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)    21240 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/
--rw-r--r--   0 ben       (1000) ben       (1000)     9161 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     1337 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3958 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2514 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     3624 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2471 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java
--rw-r--r--   0 ben       (1000) ben       (1000)     2378 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/
--rw-r--r--   0 ben       (1000) ben       (1000)     1429 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/umn/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/
--rw-r--r--   0 ben       (1000) ben       (1000)      613 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/mtap/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/mtap/api/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/proto/mtap/api/v1/
--rw-r--r--   0 ben       (1000) ben       (1000)    12815 2023-03-30 15:59:37.000000 mtap-1.2.0/proto/mtap/api/v1/events.proto
--rw-r--r--   0 ben       (1000) ben       (1000)     4764 2023-03-30 15:59:37.000000 mtap-1.2.0/proto/mtap/api/v1/processing.proto
--rw-r--r--   0 ben       (1000) ben       (1000)     2356 2023-04-15 15:21:56.000000 mtap-1.2.0/pyproject.toml
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/python/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/docs/
--rw-r--r--   0 ben       (1000) ben       (1000)      582 2023-03-11 15:03:25.000000 mtap-1.2.0/python/docs/Makefile
--rw-r--r--   0 ben       (1000) ben       (1000)     6800 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/conf.py
--rw-r--r--   0 ben       (1000) ben       (1000)      311 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/deployment.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      371 2023-03-30 15:59:37.000000 mtap-1.2.0/python/docs/index.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      787 2023-03-11 15:03:25.000000 mtap-1.2.0/python/docs/make.bat
--rw-r--r--   0 ben       (1000) ben       (1000)     3733 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/mtap.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      549 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/serialization.rst
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/
--rw-r--r--   0 ben       (1000) ben       (1000)     1195 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3578 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/__main__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     5388 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/_config.py
--rw-r--r--   0 ben       (1000) ben       (1000)    15511 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/_events_service.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3229 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/_structs.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/api/
--rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/api/__init__.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/api/v1/
--rw-r--r--   0 ben       (1000) ben       (1000)      646 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/api/v1/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14255 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/events_pb2.py
--rw-r--r--   0 ben       (1000) ben       (1000)    25839 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/events_pb2_grpc.py
--rw-r--r--   0 ben       (1000) ben       (1000)     5283 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/processing_pb2.py
--rw-r--r--   0 ben       (1000) ben       (1000)     6181 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/processing_pb2_grpc.py
--rw-r--r--   0 ben       (1000) ben       (1000)      812 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/constants.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/data/
--rw-r--r--   0 ben       (1000) ben       (1000)     1191 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1565 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_base.py
--rw-r--r--   0 ben       (1000) ben       (1000)    44144 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/_events.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8321 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_label_adapters.py
--rw-r--r--   0 ben       (1000) ben       (1000)    28162 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_label_indices.py
--rw-r--r--   0 ben       (1000) ben       (1000)    16370 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/_labels.py
--rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/defaultConfig.yml
--rw-r--r--   0 ben       (1000) ben       (1000)    23527 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/deployment.py
--rw-r--r--   0 ben       (1000) ben       (1000)     7405 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/discovery.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/
--rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2737 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/exampleDeploymentConfiguration.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     1017 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/examplePipelineConfiguration.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     3617 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/example_pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2514 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/example_processor.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2549 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/example_references_processor.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1829 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/print_processor_meta.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/serialization/
--rw-r--r--   0 ben       (1000) ben       (1000)      603 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/serialization/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3366 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/serialization/brat_converter.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/tutorial/
--rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/tutorial/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1004 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/tutorial/hello.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1278 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/tutorial/pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14203 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/metrics.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/processing/
--rw-r--r--   0 ben       (1000) ben       (1000)     1782 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)    10093 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_base.py
--rw-r--r--   0 ben       (1000) ben       (1000)    17462 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_error_handling.py
--rw-r--r--   0 ben       (1000) ben       (1000)      709 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_exc.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1911 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_mp_config.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8733 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_mp_pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14813 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)     5578 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline_components.py
--rw-r--r--   0 ben       (1000) ben       (1000)     9279 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline_results.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8025 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_runners.py
--rw-r--r--   0 ben       (1000) ben       (1000)    18871 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_service.py
--rw-r--r--   0 ben       (1000) ben       (1000)     6317 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_sources.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8105 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/descriptions.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/processors/
--rw-r--r--   0 ben       (1000) ben       (1000)      615 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/processors/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3426 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/processors/copy_document.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/serialization/
--rw-r--r--   0 ben       (1000) ben       (1000)      987 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/serialization/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)    12775 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/serialization/_serialization.py
--rw-r--r--   0 ben       (1000) ben       (1000)     6748 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/serialization/brat.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2348 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/serialization/event.schema.json
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/utilities/
--rw-r--r--   0 ben       (1000) ben       (1000)     4546 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/utilities/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1231 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/utilities/tokenization.py
--rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap/version.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)    10845 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      334 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        5 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/top_level.txt
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/config/
--rw-r--r--   0 ben       (1000) ben       (1000)       26 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/brokenConfig.yaml
--rw-r--r--   0 ben       (1000) ben       (1000)     2001 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/test_config.py
--rw-r--r--   0 ben       (1000) ben       (1000)       45 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/workingConfig.yaml
--rwxr-xr-x   0 ben       (1000) ben       (1000)     3990 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/conftest.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/consul/
--rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/consul/integrationConfig.yaml
--rw-r--r--   0 ben       (1000) ben       (1000)     5796 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/consul/test_discovery.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/data/
--rw-r--r--   0 ben       (1000) ben       (1000)     4486 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_document.py
--rw-r--r--   0 ben       (1000) ben       (1000)     5570 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_event.py
--rw-r--r--   0 ben       (1000) ben       (1000)     6066 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_events_client.py
--rw-r--r--   0 ben       (1000) ben       (1000)     4611 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_generic_label.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1460 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_labels.py
--rw-r--r--   0 ben       (1000) ben       (1000)    15073 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_standard_ascending_label_index.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14164 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_standard_descending_label_index.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/deployment/
--rw-r--r--   0 ben       (1000) ben       (1000)     3212 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/deployment/test_deployment.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/integration/
--rw-r--r--   0 ben       (1000) ben       (1000)     2386 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/integration/test_hello_world_tutorial.py
--rw-r--r--   0 ben       (1000) ben       (1000)    12156 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/integration/test_integration.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/processing/
--rw-r--r--   0 ben       (1000) ben       (1000)      342 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/pipeline.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     1565 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processing/test_event_processor.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3850 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_pipeline.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1186 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_pipeline_result.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processing/test_processor.py
--rw-r--r--   0 ben       (1000) ben       (1000)     4036 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_processor_service.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/processors/
--rw-r--r--   0 ben       (1000) ben       (1000)     1338 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processors/test_copy_document.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/references/
--rw-r--r--   0 ben       (1000) ben       (1000)     4584 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/references/test_references.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/serialization/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/serialization/brat/
--rw-r--r--   0 ben       (1000) ben       (1000)      452 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/brat/100_1442.ann
--rw-r--r--   0 ben       (1000) ben       (1000)     2583 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/brat/100_1442.txt
--rw-r--r--   0 ben       (1000) ben       (1000)     1484 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_brat.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2292 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_json.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2800 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_pickle.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1796 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_serialization.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2296 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_yml.py
--rw-r--r--   0 ben       (1000) ben       (1000)    14905 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/slf4j-simple-2.0.3.jar
--rwxr-xr-x   0 ben       (1000) ben       (1000)    30744 2023-03-17 16:26:09.000000 mtap-1.2.0/python/tests/test_events_service.py
--rw-r--r--   0 ben       (1000) ben       (1000)     6115 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/test_metrics.py
--rw-r--r--   0 ben       (1000) ben       (1000)     7727 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/test_structs.py
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-15 17:37:51.555431 mtap-1.2.0/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)     1797 2023-03-11 15:03:25.000000 mtap-1.2.0/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/
+-rw-r--r--   0 ben       (1000) ben       (1000)       94 2023-03-11 15:03:25.000000 mtap-1.2.1/.dockerignore
+-rw-r--r--   0 ben       (1000) ben       (1000)      122 2023-03-11 15:03:25.000000 mtap-1.2.1/.flake8
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/.github/
+-rw-r--r--   0 ben       (1000) ben       (1000)      273 2023-03-11 15:03:25.000000 mtap-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/.github/workflows/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2820 2023-04-17 01:08:25.000000 mtap-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     5326 2023-03-30 15:59:37.000000 mtap-1.2.1/.gitignore
+-rw-r--r--   0 ben       (1000) ben       (1000)      434 2023-03-30 15:59:37.000000 mtap-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)      708 2023-03-11 15:03:25.000000 mtap-1.2.1/Dockerfile-dev
+-rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-11 15:03:25.000000 mtap-1.2.1/LICENSE.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-17 14:28:20.207172 mtap-1.2.1/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     2476 2023-04-15 15:21:56.000000 mtap-1.2.1/README.md
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1343 2023-03-11 15:03:25.000000 mtap-1.2.1/go/Makefile
+-rw-r--r--   0 ben       (1000) ben       (1000)     1477 2023-03-30 15:59:37.000000 mtap-1.2.1/go/doc.go
+-rw-r--r--   0 ben       (1000) ben       (1000)     1835 2023-03-30 15:59:37.000000 mtap-1.2.1/go/go.mod
+-rw-r--r--   0 ben       (1000) ben       (1000)    65077 2023-03-30 15:59:37.000000 mtap-1.2.1/go/go.sum
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/go/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/go/mtap/api/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)   104710 2023-04-17 14:22:57.000000 mtap-1.2.1/go/mtap/api/v1/events.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    71157 2023-04-17 14:22:57.000000 mtap-1.2.1/go/mtap/api/v1/events.pb.gw.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    26240 2023-04-17 14:22:57.000000 mtap-1.2.1/go/mtap/api/v1/events_grpc.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    33560 2023-04-17 14:22:58.000000 mtap-1.2.1/go/mtap/api/v1/processing.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    16594 2023-04-17 14:22:58.000000 mtap-1.2.1/go/mtap/api/v1/processing.pb.gw.go
+-rw-r--r--   0 ben       (1000) ben       (1000)     7483 2023-04-17 14:22:58.000000 mtap-1.2.1/go/mtap/api/v1/processing_grpc.pb.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/mtap/consul/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2981 2023-03-11 15:03:25.000000 mtap-1.2.1/go/mtap/consul/resolver.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/mtap/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)     7921 2023-03-30 15:59:37.000000 mtap-1.2.1/go/mtap/processors/processors.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/mtap-gateway/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4732 2023-04-14 22:47:09.000000 mtap-1.2.1/go/mtap-gateway/mtap-gateway.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/store-swaggers/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1359 2023-03-11 15:03:25.000000 mtap-1.2.1/go/store-swaggers/main.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/go/third_party/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/go/third_party/googleapis/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/go/third_party/googleapis/google/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/go/third_party/googleapis/google/api/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1045 2023-03-17 16:24:15.000000 mtap-1.2.1/go/third_party/googleapis/google/api/annotations.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     3604 2023-03-17 16:24:15.000000 mtap-1.2.1/go/third_party/googleapis/google/api/field_behavior.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)    15140 2023-03-17 16:24:15.000000 mtap-1.2.1/go/third_party/googleapis/google/api/http.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     2693 2023-03-17 16:24:15.000000 mtap-1.2.1/go/third_party/googleapis/google/api/httpbody.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)      283 2023-03-30 15:59:37.000000 mtap-1.2.1/go/tools.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/
+-rw-r--r--   0 ben       (1000) ben       (1000)     7975 2023-04-15 15:21:56.000000 mtap-1.2.1/java/build.gradle
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/gradle/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/gradle/wrapper/
+-rw-r--r--   0 ben       (1000) ben       (1000)    61608 2023-04-14 22:47:09.000000 mtap-1.2.1/java/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 ben       (1000) ben       (1000)      221 2023-04-14 22:47:09.000000 mtap-1.2.1/java/gradle/wrapper/gradle-wrapper.properties
+-rwxr-xr-x   0 ben       (1000) ben       (1000)     8495 2023-04-14 22:47:09.000000 mtap-1.2.1/java/gradlew
+-rw-r--r--   0 ben       (1000) ben       (1000)     2868 2023-04-14 22:47:09.000000 mtap-1.2.1/java/gradlew.bat
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/log_resources/
+-rw-r--r--   0 ben       (1000) ben       (1000)      396 2023-03-11 15:03:25.000000 mtap-1.2.1/java/log_resources/log4j2.xml
+-rw-r--r--   0 ben       (1000) ben       (1000)      650 2023-03-11 15:03:25.000000 mtap-1.2.1/java/settings.gradle
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/java/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/java/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/java/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)    32081 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1042 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1046 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/Internal.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.177172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/
+-rw-r--r--   0 ben       (1000) ben       (1000)    11652 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3187 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6838 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2688 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3324 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1745 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1583 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.177172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/
+-rw-r--r--   0 ben       (1000) ben       (1000)     3269 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     4068 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1192 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1446 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.177172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/
+-rw-r--r--   0 ben       (1000) ben       (1000)      829 2023-04-14 22:47:09.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2282 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5628 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     4406 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      711 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.177172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1280 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-04-14 01:30:11.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.177172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2110 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      872 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      775 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    14937 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    16528 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    16546 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13871 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1978 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13061 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5777 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5921 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    10132 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2361 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2030 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2108 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2632 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    19216 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1454 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      864 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/package-info.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.187172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9045 2023-04-14 22:47:09.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1404 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2388 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3801 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      803 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      288 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/HealthService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      277 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/KeyValue.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1892 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2522 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1542 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2217 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6864 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1212 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    17320 2023-04-14 22:47:09.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      773 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1489 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1877 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2773 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2369 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      381 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/TimingService.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.187172 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1132 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3089 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/resources/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/resources/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/resources/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/main/resources/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.187172 mtap-1.2.1/java/src/main/resources/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/test/java/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/test/java/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.157172 mtap-1.2.1/java/src/test/java/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.187172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/common/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2937 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.187172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9334 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     9496 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13774 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     9602 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6141 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    14423 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3668 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5091 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    23583 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    23618 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    21240 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9161 2023-04-14 22:47:09.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1337 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3958 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2514 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3624 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2471 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2378 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1429 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/resources/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/resources/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/resources/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/java/src/test/resources/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/java/src/test/resources/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)      613 2023-03-11 15:03:25.000000 mtap-1.2.1/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/proto/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/proto/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/proto/mtap/api/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/proto/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)    12815 2023-03-30 15:59:37.000000 mtap-1.2.1/proto/mtap/api/v1/events.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     4764 2023-03-30 15:59:37.000000 mtap-1.2.1/proto/mtap/api/v1/processing.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     2356 2023-04-15 15:21:56.000000 mtap-1.2.1/pyproject.toml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.167172 mtap-1.2.1/python/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/docs/
+-rw-r--r--   0 ben       (1000) ben       (1000)      582 2023-03-11 15:03:25.000000 mtap-1.2.1/python/docs/Makefile
+-rw-r--r--   0 ben       (1000) ben       (1000)     6800 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/conf.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      349 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/deployment.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      408 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/index.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      787 2023-03-11 15:03:25.000000 mtap-1.2.1/python/docs/make.bat
+-rw-r--r--   0 ben       (1000) ben       (1000)      153 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/metrics.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     1594 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/mtap.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)     1638 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/pipeline.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      917 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/processing.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      516 2023-04-17 14:21:29.000000 mtap-1.2.1/python/docs/serialization.rst
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1257 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3331 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/__main__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      924 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_common.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5388 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    13992 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_document.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    12731 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_event.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4660 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_events_client.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8839 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_events_client_grpc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2946 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_events_client_pool.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8308 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_label_adapters.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    28446 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_label_indices.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3205 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_labeler.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    16623 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_labels.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3259 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/_structs.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/api/
+-rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/api/__init__.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)      646 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/api/v1/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14255 2023-04-17 07:07:07.000000 mtap-1.2.1/python/mtap/api/v1/events_pb2.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    25839 2023-04-17 07:07:07.000000 mtap-1.2.1/python/mtap/api/v1/events_pb2_grpc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5283 2023-04-17 07:07:07.000000 mtap-1.2.1/python/mtap/api/v1/processing_pb2.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6181 2023-04-17 07:07:07.000000 mtap-1.2.1/python/mtap/api/v1/processing_pb2_grpc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      812 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/constants.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/defaultConfig.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)    23746 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/deployment.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7087 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/descriptors.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7405 2023-04-14 22:47:09.000000 mtap-1.2.1/python/mtap/discovery.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    15478 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/events_server.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/examples/
+-rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2737 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/exampleDeploymentConfiguration.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1017 2023-04-14 22:47:09.000000 mtap-1.2.1/python/mtap/examples/examplePipelineConfiguration.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     3615 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/examples/example_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2502 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/examples/example_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2537 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/examples/example_references_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1829 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/print_processor_meta.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/examples/serialization/
+-rw-r--r--   0 ben       (1000) ben       (1000)      603 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/serialization/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3366 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/serialization/brat_converter.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/examples/tutorial/
+-rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/tutorial/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1004 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/examples/tutorial/hello.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1248 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/examples/tutorial/pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    13416 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/metrics.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/pipeline/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1373 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1091 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_common.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    11219 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_error_handling.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1908 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_mp_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8054 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_mp_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14619 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6296 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_pipeline_components.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5728 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_results.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5865 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/pipeline/_sources.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1074 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5075 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/_exc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1636 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/_processing_component.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     9496 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7855 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/_runners.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    18613 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/_service.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5774 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processing/results.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)      615 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/processors/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3278 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/processors/copy_document.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/serialization/
+-rw-r--r--   0 ben       (1000) ben       (1000)      918 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/serialization/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    12217 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/serialization/_serialization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6587 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/serialization/brat.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2348 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/serialization/event.schema.json
+-rw-r--r--   0 ben       (1000) ben       (1000)      992 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/types.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4535 2023-04-17 14:21:29.000000 mtap-1.2.1/python/mtap/utilities/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1231 2023-03-11 15:03:25.000000 mtap-1.2.1/python/mtap/utilities/tokenization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap/version.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/mtap.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)    11153 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      334 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        5 2023-04-17 14:28:20.000000 mtap-1.2.1/python/mtap.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/tests/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/tests/config/
+-rw-r--r--   0 ben       (1000) ben       (1000)       26 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/config/brokenConfig.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)     2001 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/config/test_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       45 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/config/workingConfig.yaml
+-rwxr-xr-x   0 ben       (1000) ben       (1000)     3976 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/conftest.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/tests/consul/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/consul/integrationConfig.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)     5725 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/consul/test_discovery.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/tests/data/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4975 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_document.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4997 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_event.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6359 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_events_client.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4623 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_generic_label.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1468 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_labels.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    15072 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_standard_ascending_label_index.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14163 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/data/test_standard_descending_label_index.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.197172 mtap-1.2.1/python/tests/deployment/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2977 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/deployment/test_deployment.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/integration/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2376 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/integration/test_hello_world_tutorial.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    12113 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/integration/test_integration.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)      342 2023-04-14 22:47:09.000000 mtap-1.2.1/python/tests/processing/pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1565 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/processing/test_event_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3825 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/processing/test_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1219 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/processing/test_pipeline_result.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/processing/test_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4024 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/processing/test_processor_service.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1338 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/processors/test_copy_document.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/references/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4587 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/references/test_references.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/serialization/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 14:28:20.207172 mtap-1.2.1/python/tests/serialization/brat/
+-rw-r--r--   0 ben       (1000) ben       (1000)      452 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/brat/100_1442.ann
+-rw-r--r--   0 ben       (1000) ben       (1000)     2583 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/brat/100_1442.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)     1484 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/test_brat.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2292 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/test_json.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2800 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/test_pickle.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1796 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/serialization/test_serialization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2176 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/serialization/test_yml.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14905 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/slf4j-simple-2.0.3.jar
+-rwxr-xr-x   0 ben       (1000) ben       (1000)    30740 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/test_events_service.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6435 2023-04-17 14:21:29.000000 mtap-1.2.1/python/tests/test_metrics.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7727 2023-03-11 15:03:25.000000 mtap-1.2.1/python/tests/test_structs.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-17 14:28:20.207172 mtap-1.2.1/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)     1797 2023-03-11 15:03:25.000000 mtap-1.2.1/setup.py
```

### Comparing `mtap-1.2.0/.github/workflows/ci.yml` & `mtap-1.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/.gitignore` & `mtap-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/Dockerfile-dev` & `mtap-1.2.1/Dockerfile-dev`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/LICENSE.txt` & `mtap-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/PKG-INFO` & `mtap-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtap
-Version: 1.2.0
+Version: 1.2.1
 Summary: A framework for distributed text analysis using gRPC and microservices-based architecture.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mtap-1.2.0/README.md` & `mtap-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/Makefile` & `mtap-1.2.1/go/Makefile`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/doc.go` & `mtap-1.2.1/go/doc.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/go.mod` & `mtap-1.2.1/go/go.mod`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/go.sum` & `mtap-1.2.1/go/go.sum`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/events.pb.go` & `mtap-1.2.1/go/mtap/api/v1/events.pb.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/events.pb.gw.go` & `mtap-1.2.1/go/mtap/api/v1/events.pb.gw.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/events_grpc.pb.go` & `mtap-1.2.1/go/mtap/api/v1/events_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/processing.pb.go` & `mtap-1.2.1/go/mtap/api/v1/processing.pb.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/processing.pb.gw.go` & `mtap-1.2.1/go/mtap/api/v1/processing.pb.gw.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/api/v1/processing_grpc.pb.go` & `mtap-1.2.1/go/mtap/api/v1/processing_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/consul/resolver.go` & `mtap-1.2.1/go/mtap/consul/resolver.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap/processors/processors.go` & `mtap-1.2.1/go/mtap/processors/processors.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/mtap-gateway/mtap-gateway.go` & `mtap-1.2.1/go/mtap-gateway/mtap-gateway.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/store-swaggers/main.go` & `mtap-1.2.1/go/store-swaggers/main.go`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/third_party/googleapis/google/api/annotations.proto` & `mtap-1.2.1/go/third_party/googleapis/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/third_party/googleapis/google/api/field_behavior.proto` & `mtap-1.2.1/go/third_party/googleapis/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/third_party/googleapis/google/api/http.proto` & `mtap-1.2.1/go/third_party/googleapis/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/go/third_party/googleapis/google/api/httpbody.proto` & `mtap-1.2.1/go/third_party/googleapis/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/build.gradle` & `mtap-1.2.1/java/build.gradle`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.jar` & `mtap-1.2.1/java/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/gradlew` & `mtap-1.2.1/java/gradlew`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/gradlew.bat` & `mtap-1.2.1/java/gradlew.bat`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/settings.gradle` & `mtap-1.2.1/java/settings.gradle`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/Internal.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/package-info.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java` & `mtap-1.2.1/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml` & `mtap-1.2.1/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java` & `mtap-1.2.1/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml` & `mtap-1.2.1/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/proto/mtap/api/v1/events.proto` & `mtap-1.2.1/proto/mtap/api/v1/events.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/proto/mtap/api/v1/processing.proto` & `mtap-1.2.1/proto/mtap/api/v1/processing.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/pyproject.toml` & `mtap-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/docs/Makefile` & `mtap-1.2.1/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/docs/conf.py` & `mtap-1.2.1/python/docs/conf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 import re
 
-sys.path.insert(0, os.path.abspath('../'))
-
 import mtap
 
+sys.path.insert(0, os.path.abspath('../'))
+
 # -- Project information -----------------------------------------------------
 
 project = 'MTAP'
 copyright = "2019, Regents of the University of Minnesota."
 author = 'NLP-IE Group'
 
 # The short X.Y version
```

### Comparing `mtap-1.2.0/python/docs/make.bat` & `mtap-1.2.1/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/__main__.py` & `mtap-1.2.1/python/mtap/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,52 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
 import logging
-import signal
-import threading
 
 
 def run_events_server(args):
     """Runs the documents service, blocking until keyboard interrupt.
 
     Parameters:
         args: Command line arguments.
     """
     from mtap._config import Config
-    from mtap._events_service import EventsServer
+    from mtap.events_server import EventsServer
     with Config() as c:
         if args.mtap_config is not None:
             c.update_from_yaml(args.mtap_config)
         server = EventsServer(
             args.host,
             sid=args.sid,
             port=args.port,
             register=args.register,
             workers=args.workers,
             write_address=args.write_address
         )
 
-        e = threading.Event()
-
-        def do_stop(*_):
-            e.set()
-
-        signal.signal(signal.SIGINT, do_stop)
-        signal.signal(signal.SIGTERM, do_stop)
-
-        server.start()
-        try:
-            e.wait()
-        except KeyboardInterrupt:
-            pass
-        server.stop()
+        from mtap._common import run_server_forever
+        run_server_forever(server)
 
 
 def main(args=None):
     parser = argparse.ArgumentParser(allow_abbrev=False)
     subparsers = parser.add_subparsers(title='sub-commands',
                                        description='valid sub-commands')
```

### Comparing `mtap-1.2.0/python/mtap/_config.py` & `mtap-1.2.1/python/mtap/_config.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/_events_service.py` & `mtap-1.2.1/python/mtap/events_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,15 @@
     def port(self) -> int:
         """int: The port the processor service is bound to."""
         return self._port
 
     def start(self):
         """Starts the service.
         """
-        logger.info(f'Starting events server (%s) on address: "%s:%d"',
-                    self.sid, self._address, self._port)
+        logger.info(f'Starting events server {self.sid} on address: "{self._address}:{self._port}"')
         self._server.start()
         if self.write_address:
             self._address_file = utilities.write_address_file(
                 '{}:{}'.format(self._address, self.port),
                 self.sid
             )
         if self._register:
@@ -127,14 +126,35 @@
         try:
             self._deregister()
         except AttributeError:
             pass
         return self._server.stop(grace=grace)
 
 
+def _validate_generic_labels(labels, context):
+    for label in labels[1].labels:
+        for key in label.fields:
+            if key in ["document", "location", "text", "id",
+                       "label_index_name"]:
+                _set_error_context(context,
+                                   grpc.StatusCode.INVALID_ARGUMENT,
+                                   "Label included a reserved key: {}".format(
+                                       key))
+                return False
+        for key in label.reference_ids:
+            if key in ["document", "location", "text", "id", "id",
+                       "label_index_name"]:
+                _set_error_context(context,
+                                   grpc.StatusCode.INVALID_ARGUMENT,
+                                   "Label included a reserved key: {}".format(
+                                       key))
+                return False
+    return True
+
+
 class EventsServicer(events_pb2_grpc.EventsServicer):
     def __init__(self, instance_id=None):
         self.lock = threading.RLock()
         self.events = {}
         self.instance_id = instance_id or str(uuid.uuid4())
 
     def _get_event(self, request, context=None):
@@ -324,31 +344,16 @@
             if index_name == '':
                 msg = 'No index_name was set.'
                 _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT,
                                    msg)
                 return empty_pb2.Empty()
             labels = (labels_field, getattr(request, labels_field))
         if labels_field == 'generic_labels' and not request.no_key_validation:
-            for label in labels[1].labels:
-                for key in label.fields:
-                    if key in ["document", "location", "text", "id",
-                               "label_index_name"]:
-                        _set_error_context(context,
-                                           grpc.StatusCode.INVALID_ARGUMENT,
-                                           "Label included a reserved key: {}".format(
-                                               key))
-                        return empty_pb2.Empty()
-                for key in label.reference_ids:
-                    if key in ["document", "location", "text", "id", "id",
-                               "label_index_name"]:
-                        _set_error_context(context,
-                                           grpc.StatusCode.INVALID_ARGUMENT,
-                                           "Label included a reserved key: {}".format(
-                                               key))
-                        return empty_pb2.Empty()
+            if not _validate_generic_labels(labels, context):
+                return None
         document.labels[request.index_name] = labels
         return events_pb2.AddLabelsResponse()
 
     def GetLabels(self, request, context=None):
         try:
             document = self._get_document(request, context)
         except KeyError:
```

### Comparing `mtap-1.2.0/python/mtap/_structs.py` & `mtap-1.2.1/python/mtap/_structs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         else:
             raise TypeError("Unrecognized type:", type(v))
 
 
 def _check_for_reference_cycle(o, parents):
     for parent in parents:
         if o is parent:
-            raise ValueError("Reference cycle while preparing for serialization.")
+            raise ValueError(
+                "Reference cycle while preparing for serialization."
+            )
 
 
 def copy_list_value_to_list(list_value, lst):
     for v in list_value:
         if isinstance(v, (str, float, bool, int)) or v is None:
             lst.append(v)
         elif isinstance(v, struct_pb2.ListValue):
```

### Comparing `mtap-1.2.0/python/mtap/api/__init__.py` & `mtap-1.2.1/python/mtap/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/api/v1/__init__.py` & `mtap-1.2.1/python/mtap/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/api/v1/events_pb2.py` & `mtap-1.2.1/python/mtap/api/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/api/v1/events_pb2_grpc.py` & `mtap-1.2.1/python/mtap/api/v1/events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/api/v1/processing_pb2.py` & `mtap-1.2.1/python/mtap/api/v1/processing_pb2.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/api/v1/processing_pb2_grpc.py` & `mtap-1.2.1/python/mtap/api/v1/processing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/constants.py` & `mtap-1.2.1/python/mtap/constants.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/data/__init__.py` & `mtap-1.2.1/python/mtap/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-#  Copyright 2020 Regents of the University of Minnesota.
+# Copyright 2019 Regents of the University of Minnesota.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-"""Module for MTAP's Data Model
-"""
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Provided for type checking, shouldn't really need to call any of these."""
 
-from mtap.data._base import LabelIndexType, LabelIndexInfo
-from mtap.data._events import (
-    Document,
-    Event,
-    EventsAddressLike,
-    EventsClient,
-    Labeler,
-    LabelAdapters,
-    FailedToConnectToEventsServiceException,
-)
-from mtap.data._label_adapters import (
-    GENERIC_ADAPTER,
-    DISTINCT_GENERIC_ADAPTER,
-    ProtoLabelAdapter,
-)
-from mtap.data._label_indices import (
-    LabelIndex,
-    label_index,
-    presorted_label_index,
-)
-from mtap.data._labels import (
-    GenericLabel,
-    Label,
-    Location,
-    label,
+from mtap._events_client import EventsClient
+from mtap._labels import Label
+from mtap._label_adapters import ProtoLabelAdapter
+from mtap._label_indices import LabelIndex
+from mtap._labeler import Labeler
+
+__all__ = (
+    'EventsClient',
+    'Label',
+    'ProtoLabelAdapter',
+    'LabelIndex',
+    'Labeler',
 )
```

### Comparing `mtap-1.2.0/python/mtap/data/_label_adapters.py` & `mtap-1.2.1/python/mtap/_label_adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,222 +10,242 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from abc import ABC, abstractmethod
 from typing import Generic, Iterable, List, Any, Optional, Sequence, TypeVar
 
-import typing
-
 from mtap import _structs
-from mtap.data import _label_indices, _labels
-
-if typing.TYPE_CHECKING:
-    import mtap
-    from mtap.api.v1 import events_pb2
-    from mtap import data
+from mtap._document import Document
+from mtap._label_indices import presorted_label_index, label_index, LabelIndex
+from mtap._labels import Label, GenericLabel
+from mtap._structs import copy_dict_to_struct
+from mtap.api.v1 import events_pb2
 
-L = TypeVar('L', bound='data.Label')
+L = TypeVar('L', bound=Label)
 
 
 class ProtoLabelAdapter(ABC, Generic[L]):
-    """Responsible for marshalling and unmarshalling of label objects to and from proto messages.
+    """Responsible for marshalling and unmarshalling of label objects to and
+    from proto messages.
     """
     __slots__ = ()
 
     @abstractmethod
     def create_label(self, *args, **kwargs) -> L:
         """Called by labelers to create labels.
 
-        Should include the positional arguments `start_index` and `end_index`, because those are
-        required properties of labels.
+        Should include the positional arguments `start_index` and `end_index`,
+        because those are required properties of labels.
 
         Args:
             args: Arbitrary args used to create the label.
             kwargs: Arbitrary keyword args used to create the label.
 
         Returns:
             Label: An object of the label type.
         """
         ...
 
     @abstractmethod
     def create_index_from_response(
             self,
-            response: 'events_pb2.GetLabelsResponse'
-    ) -> 'data.LabelIndex[L]':
+            response: events_pb2.GetLabelsResponse
+    ) -> LabelIndex[L]:
         """Creates a LabelIndex from the response from an events service.
 
         Args:
-            response (mtap.api.v1.events_pb2.GetLabelsResponse): The response protobuf message from
-                the events service.
+            response: The response protobuf message from the events service.
 
         Returns:
-            LabelIndex[L]: A label index containing all the labels from the events service.
+            A label index containing all the labels from the events service.
         """
         ...
 
     @abstractmethod
     def create_index(self, labels: Iterable[L]):
         """Creates a LabelIndex from an iterable of label objects.
 
         Args:
-            labels (~typing.Iterable[L]): Labels to put in index.
+            labels: Labels to put in index.
 
         Returns:
-            LabelIndex[L]: A label index containing all of the labels in the list.
+            A label index containing all the provided labels.
         """
         ...
 
     @abstractmethod
-    def add_to_message(self, labels: List[L], request: 'events_pb2.AddLabelsRequest'):
-        """Adds a list of labels to a request to the event service to add labels.
+    def add_to_message(self,
+                       labels: Iterable[L],
+                       request: events_pb2.AddLabelsRequest):
+        """Adds labels to an ``AddLabelsRequest``.
 
         Args:
-            labels (Iterable[L]): The list of labels that need to be sent to the server.
-            request (mtap.api.v1.events_pb2.AddLabelsRequest): The request proto message to add the
-                labels to.
+            labels: The labels to add.
+            request: The request.
         """
         ...
 
     @abstractmethod
-    def pack(self, index: 'data.LabelIndex[L]', *, include_label_text: bool = False) -> Any:
-        """Prepares to serialize a label index by transforming the label index into a representation
-        that can be dumped to json, yml, pickle, etc.
+    def pack(self,
+             index: LabelIndex[L], *,
+             include_label_text: bool = False) -> Any:
+        """Prepares to serialize a label index by transforming the label index
+        into a representation that can be dumped to json, yml, pickle, etc.
 
         Args:
             index: The index itself.
-            include_label_text:
-                Whether to include the label's text in the serialized representation
-                (for informative reasons).
+            include_label_text: Whether to include the label's text in the
+                serialized representation (for informative reasons).
 
         Returns:
             A dictionary representation of the label index.
 
         """
         ...
 
     @abstractmethod
-    def unpack(self,
-               packed: Any,
-               label_index_name: str,
-               *, document: Optional['mtap.Document'] = None) -> 'data.LabelIndex[L]':
-        """Takes a packed, serializable object and turns it into a full label index.
+    def unpack(
+            self,
+            packed: Any,
+            label_index_name: str,
+            *, document: Optional[Document] = None
+    ) -> LabelIndex[L]:
+        """Takes a packed, serializable object and turns it into a full label
+        index.
 
         Args:
-            packed (Any): The packed representation.
-            label_index_name (str): The index name of the label index.
-            document (Document): The document this label index occurs on.
+            packed: The packed representation.
+            label_index_name: The index name of the label index.
+            document: The document this label index occurs on.
 
         Returns:
-            LabelIndex[L]: The label index.
+            The label index.
 
         """
         ...
 
     def store_references(self, labels: Sequence[L]):
-        """Take all the references for the labels and turn them into static references.
+        """Take all the references for the labels and turn them into static
+        references.
 
         Args:
-             labels (Sequence[L]): The labels to store the references on.
+             labels: Labels that need their references turned into objects.
         """
         ...
 
 
-class _GenericLabelAdapter(ProtoLabelAdapter['mtap.GenericLabel']):
+class _GenericLabelAdapter(ProtoLabelAdapter[GenericLabel]):
     __slots__ = ('distinct',)
 
     def __init__(self, distinct):
         self.distinct = distinct
 
     def create_label(self, *args, **kwargs):
-        return _labels.GenericLabel(*args, **kwargs)
+        return GenericLabel(*args, **kwargs)
 
     def create_index(self, labels: List[L]):
-        return _label_indices.label_index(labels, self.distinct, adapter=self)
+        return label_index(labels, self.distinct, adapter=self)
 
     def create_index_from_response(self, response):
         generic_labels = response.generic_labels
         labels = []
         for label_message in generic_labels.labels:
             fields = {}
             _structs.copy_struct_to_dict(label_message.fields, fields)
             reference_field_ids = {}
-            _structs.copy_struct_to_dict(label_message.reference_ids, reference_field_ids)
-            generic_label = _labels.GenericLabel(label_message.start_index, label_message.end_index,
-                                                 identifier=label_message.identifier, fields=fields,
-                                                 reference_field_ids=reference_field_ids)
+            _structs.copy_struct_to_dict(label_message.reference_ids,
+                                         reference_field_ids)
+            generic_label = GenericLabel(
+                label_message.start_index,
+                label_message.end_index,
+                identifier=label_message.identifier,
+                fields=fields,
+                reference_field_ids=reference_field_ids
+            )
             labels.append(generic_label)
 
-        return _label_indices.presorted_label_index(labels, generic_labels.is_distinct, adapter=self)
+        return presorted_label_index(labels,
+                                     generic_labels.is_distinct,
+                                     adapter=self)
 
-    def add_to_message(self, labels: List['mtap.GenericLabel'], request):
+    def add_to_message(self, labels: Iterable[GenericLabel], request):
         generic_labels = request.generic_labels
         for label in labels:
             label_message = generic_labels.labels.add()
             label_message.identifier = label.identifier
             label_message.start_index = label.start_index
             label_message.end_index = label.end_index
-            _structs.copy_dict_to_struct(label.fields, label_message.fields, [label])
-            _structs.copy_dict_to_struct(label.reference_field_ids, label_message.reference_ids,
-                                         [label])
+            copy_dict_to_struct(label.fields,
+                                label_message.fields,
+                                [label])
+            copy_dict_to_struct(label.reference_field_ids,
+                                label_message.reference_ids,
+                                [label])
 
     def pack(self,
-             index: 'data.LabelIndex[mtap.GenericLabel]',
+             index: LabelIndex[GenericLabel],
              *, include_label_text: bool = False) -> Any:
         d = {
-            'labels': [_label_to_dict(label, include_label_text) for label in index],
+            'labels': [_label_to_dict(label, include_label_text) for label in
+                       index],
             'distinct': index.distinct
         }
         return d
 
     def unpack(self, packed: Any,
                label_index_name: str,
-               *, document: Optional['mtap.Document'] = None) -> 'data.LabelIndex[L]':
-        return _label_indices.label_index(
-            [_dict_to_label(d, label_index_name, document) for d in packed['labels']],
+               *, document: Optional[
+                Document] = None) -> LabelIndex[GenericLabel]:
+        return label_index(
+            [_dict_to_label(d, label_index_name, document) for d in
+             packed['labels']],
             distinct=packed['distinct'], adapter=self
         )
 
-    def store_references(self, labels: Sequence['mtap.GenericLabel']):
+    def store_references(self, labels: Sequence[GenericLabel]):
         for label in labels:
             for k, v in label.reference_cache.items():
                 if k not in label.reference_field_ids:
                     label.reference_field_ids[k] = _convert_to_references(v)
 
 
 def _convert_to_references(o):
     if o is None:
         return o
-    if isinstance(o, _labels.Label):
+    if isinstance(o, Label):
         ref = '{}:{}'.format(o.label_index_name, o.identifier)
         return ref
-    if isinstance(o, typing.Mapping):
+    if isinstance(o, dict):
         rep = {}
         for k, v in o.items():
             rep[k] = _convert_to_references(v)
         return rep
-    if isinstance(o, Sequence):
+    if isinstance(o, list):
         rep = [_convert_to_references(v) for v in o]
         return rep
+    raise ValueError("")
 
 
 def _label_to_dict(label, include_label_text):
     d = {'start_index': label.start_index,
          'end_index': label.end_index,
          'identifier': label.identifier,
          'fields': label.fields,
          'reference_ids': label.reference_field_ids}
     if include_label_text:
         d['_text'] = label.text
     return d
 
 
 def _dict_to_label(d, label_index_name, document):
-    return _labels.GenericLabel(d['start_index'], d['end_index'], identifier=d['identifier'],
-                                fields=d['fields'], reference_field_ids=d['reference_ids'],
-                                label_index_name=label_index_name, document=document)
+    return GenericLabel(d['start_index'], d['end_index'],
+                        identifier=d['identifier'],
+                        fields=d['fields'],
+                        reference_field_ids=d['reference_ids'],
+                        label_index_name=label_index_name,
+                        document=document)
 
 
 GENERIC_ADAPTER = _GenericLabelAdapter(False)
 
 DISTINCT_GENERIC_ADAPTER = _GenericLabelAdapter(True)
```

### Comparing `mtap-1.2.0/python/mtap/data/_label_indices.py` & `mtap-1.2.1/python/mtap/_label_indices.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,224 +10,278 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Internal implementation of a standard non-distinct label index."""
 from abc import ABCMeta, abstractmethod
 from bisect import bisect_left, bisect_right
+from enum import Enum
 from operator import attrgetter
 from typing import (
     Union,
     Optional,
     Any,
     Iterator,
     List,
     TypeVar,
     Sequence,
     Generic,
     Callable,
     TYPE_CHECKING,
+    NamedTuple, overload,
 )
 
-from mtap.data import _labels
+from mtap._labels import HasStart, LocationLike, HasEnd, Location, Label
 
 if TYPE_CHECKING:
-    from mtap import data
+    from mtap.types import ProtoLabelAdapter
 
-L = TypeVar('L', bound='data.Label')
+L = TypeVar('L', bound=Label)
+
+
+class LabelIndexType(Enum):
+    """The type of serialized labels contained in the label index."""
+    UNKNOWN = 0
+    """Label index not set or type not known."""
+
+    GENERIC = 1
+    """JSON / Generic Label index"""
+
+    CUSTOM = 2
+    """Other / custom protobuf label index"""
+
+
+class LabelIndexInfo(NamedTuple):
+    index_name: str
+    type: LabelIndexType
 
 
 class LabelIndex(Sequence[L], Generic[L]):
-    """An immutable :obj:`~typing.Sequence` of labels ordered by their location in text. By default
-    sorts by ascending `start_index` and then by ascending `end_index`.
+    """An immutable :obj:`~typing.Sequence` of labels ordered by their
+    location in text. By default, sorts by ascending `start_index` and then by
+    ascending `end_index`.
     """
     __slots__ = ()
 
     @property
     @abstractmethod
     def distinct(self) -> bool:
-        """bool: Whether this label index is distinct, i.e. all of the labels in it are
-            non-overlapping.
+        """Whether this label index is distinct, i.e. all the labels in it are
+        non-overlapping.
         """
         ...
 
     @property
     @abstractmethod
-    def adapter(self) -> Optional['data.ProtoLabelAdapter']:
+    def adapter(self) -> Optional['ProtoLabelAdapter']:
         ...
 
     @abstractmethod
-    def filter(self, fn: Callable[['data.Label'], bool]) -> 'data.LabelIndex[L]':
+    def filter(self, fn: Callable[[Label], bool]) -> 'LabelIndex[L]':
         """Filters the label index according to a filter function.
 
         This function is less efficient for filtering based on indices than
-        :func:`~LabelIndex.inside`, :func:`~LabelIndex.covering`, etc., which use a binary search
-        method on the sorted index.
+        :func:`~LabelIndex.inside`, :func:`~LabelIndex.covering`, etc., which
+        use a binary search method on the sorted index.
 
         Args:
-            fn (~typing.Callable[[Label], bool]): A filter function, returns ``true`` if the label
-                should be included, ``false`` if it should not be included
+            fn: A filter function, returns ``true`` if the label should be
+                included, ``false`` if it should not be included
 
         Returns:
             LabelIndex: A view of this label index.
         """
         ...
 
+    @overload
+    def at(self, location: 'LocationLike') -> 'LabelIndex[L]':
+        ...
+
+    @overload
+    def at(self, start: float, end: float) -> 'LabelIndex[L]':
+        ...
+
     @abstractmethod
-    def at(self,
-           x: Union['data.Label', 'data.Location', float],
-           end: Optional[float] = None) -> 'data.LabelIndex[L]':
+    def at(self, x, y=None):
         """Returns the labels at the specified location in text.
 
         Args:
-            x (~typing.Union[Label, Location, float]): A label or location, or start index if `end`
-                is specified.
-            end (~typing.Optional[float]): The exclusive end index of the location in text if it has
-                not been specified by a label.
+            location: A label or location.
+            start: The inclusive start index.
+            end: The inclusive end index of the location in text.
 
         Returns:
-            LabelIndex: A view of this label index.
+            A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 10, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(6, 20, x=3)])
             >>> index.at(0, 10)
-            label_index([GenericLabel(0, 10, x=1), GenericLabel(0, 10, x=2)], distinct=False)
+            label_index([GenericLabel(0, 10, x=1), GenericLabel(0, 10, x=2)],
+            distinct=False)
         """
         ...
 
+    @overload
+    def covering(self, location: 'LocationLike') -> 'LabelIndex[L]':
+        ...
+
+    @overload
+    def covering(self, start: float, end: float) -> 'LabelIndex[L]':
+        ...
+
     @abstractmethod
-    def covering(self,
-                 x: Union['data.Label', 'data.Location', float],
-                 end: Optional[float] = None) -> 'data.LabelIndex[L]':
-        """A label index containing all labels that cover / contain the specified location in text.
+    def covering(self, x, y=None) -> 'LabelIndex[L]':
+        """A label index containing all labels that cover / contain the
+        specified location in text.
 
         Args:
-            x (~typing.Union[~'data.Label', ~'data.Location', float]): A label or location, or start
-                index if `end` is specified.
-            end (~typing.Optional[float]): The exclusive end index of the location in text if it has
-                not been specified by a label.
+            start: The inclusive start of the location.
+            end: The inclusive end of the location.
+            location: A label or location.
 
         Returns:
-            LabelIndex: A view of this label index.
+            A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.covering(5, 10)
-            label_index([GenericLabel(0, 10, x=2), GenericLabel(5, 10, x=3), GenericLabel(5, 15, x=5)], distinct=False)
+            label_index([GenericLabel(0, 10, x=2), GenericLabel(5, 10, x=3),
+            GenericLabel(5, 15, x=5)], distinct=False)
 
         """
         ...
 
+    @overload
+    def inside(self, location: 'LocationLike') -> 'LabelIndex[L]':
+        ...
+
+    @overload
+    def inside(self, start: float, end: float) -> 'LabelIndex[L]':
+        ...
+
     @abstractmethod
-    def inside(self,
-               x: Union['data.Label', 'data.Location', float],
-               end: Optional[float] = None) -> 'data.LabelIndex[L]':
-        """A label index containing all labels that are inside the specified location in text.
+    def inside(self, x: 'HasStart', y: Optional[float] = None):
+        """A label index containing all labels that are inside the specified
+        location in text.
 
         Args:
-            x (~typing.Union[~'data.Label', ~'data.Location', float]): A label or location, or start
-                index if `end` is specified.
-            end (~typing.Optional[float]): The exclusive end index of the location in text if it has
-                not been specified by a label.
+            location: A label or location.
+            start: The inclusive start of the location.
+            end: The inclusive end of the location.
 
         Returns:
-            LabelIndex: A view of this label index.
+            A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.inside(5, 10)
-            label_index([GenericLabel(5, 10, x=3), GenericLabel(7, 10, x=4)], distinct=False)
+            label_index([GenericLabel(5, 10, x=3), GenericLabel(7, 10, x=4)],
+            distinct=False)
         """
         ...
 
+    @overload
+    def beginning_inside(self, location: 'LocationLike') -> 'LabelIndex[L]':
+        ...
+
+    @overload
+    def beginning_inside(self, start: float, end: float) -> 'LabelIndex[L]':
+        ...
+
     @abstractmethod
     def beginning_inside(self,
-                         x: Union['data.Label', 'data.Location', float],
-                         end: Optional[float] = None) -> 'data.LabelIndex[L]':
-        """A label index containing all labels whose begin index is inside the specified location
-        in text.
+                         x: 'HasStart',
+                         end: Optional[float] = None) -> 'LabelIndex[L]':
+        """A label index containing all labels whose begin index is inside the
+        specified location in text.
 
         Args:
-            x (~typing.Union[~'data.Label', ~'data.Location', float]): A label or location, or start
-                index if `end` is specified.
-            end (~typing.Optional[float]): The exclusive end index of the location in text if it has
-                not been specified by a label.
+            location: A label or location.
+            start: The inclusive start of the location.
+            end: The inclusive end of the location.
 
         Returns:
-            LabelIndex: A view of this label index.
+            A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.beginning_inside(6, 11)
-            label_index([GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)], distinct=False)
+            label_index([GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)],
+            distinct=False)
         """
         ...
 
+    @overload
+    def overlapping(self, location: 'LocationLike') -> 'LabelIndex[L]':
+        ...
+
+    @overload
+    def overlapping(self, start: float, end: float) -> 'LabelIndex[L]':
+        ...
+
     @abstractmethod
     def overlapping(self,
-                    x: Union['data.Label', 'data.Location', float],
-                    end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                    x: 'HasStart',
+                    end: Optional[float] = None) -> 'LabelIndex[L]':
         """Returns all labels that overlap the specified location in text.
 
         Args:
-            x (~typing.Union[~'data.Label', ~'data.Location', float]): A label or location, or start
-                index if `end` is specified.
-            end (~typing.Optional[float]): The exclusive end index of the location in text if it has
-                not been specified by a label.
+            location: A label or location.
+            start: The inclusive start of the location.
+            end: The inclusive end of the location.
 
         Returns:
             LabelIndex: A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.overlapping(6, 10)
-            label_index([GenericLabel(0, 10, x=2), GenericLabel(5, 10, x=3), GenericLabel(5, 15, x=5),
-                         GenericLabel(7, 10, x=4)], distinct=False)
-
-
+            label_index([GenericLabel(0, 10, x=2), GenericLabel(5, 10, x=3),
+            GenericLabel(5, 15, x=5), GenericLabel(7, 10, x=4)],
+            distinct=False)
         """
         ...
 
-    def before(self, x: Union['data.Label', 'data.Location', float]) -> 'data.LabelIndex[L]':
-        """A label index containing all labels that are before a label's location in text or
-        an index in text.
+    def before(self, x: 'HasStart') -> 'LabelIndex[L]':
+        """A label index containing all labels that are before a label's
+        location in text or an index in text.
 
         Args:
-            x (~typing.Union[~'data.Label', ~'data.Location', float]): A label or location whose
-                `start_index` will be used, or a float index in text.
+            x: A label or location whose `start_index` will be used, or a
+                float index in text.
 
         Returns:
-            LabelIndex: A view of this label index.
+            A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
@@ -238,45 +292,46 @@
         """
         try:
             index = x.start_index
         except AttributeError:
             index = x
         return self.inside(0, index)
 
-    def after(self, x: Union['data.Label', 'data.Location', float]) -> 'data.LabelIndex[L]':
-        """A label index containing all labels that are after a label's location in text
-        or an index in text.
+    def after(self, x: 'HasEnd') -> 'LabelIndex[L]':
+        """A label index containing all labels that are after a label's
+        location in text or an index in text.
 
         Args:
-            x (~typing.Union[Label, Location, float]): A label or location whose `end_index` will
-                be used, or a float index in text.
+            x: A label or location whose `end_index` will be used, or a float
+                index in text.
 
         Returns:
             LabelIndex: A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.after(6)
-            label_index([GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)], distinct=False)
+            label_index([GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)],
+            distinct=False)
 
         """
         try:
             index = x.end_index
         except AttributeError:
             index = x
         return self.inside(index, float('inf'))
 
     @abstractmethod
-    def ascending(self) -> 'data.LabelIndex[L]':
+    def ascending(self) -> 'LabelIndex[L]':
         """This label index sorted according to ascending start and end index.
 
         Returns:
             LabelIndex: A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
@@ -288,321 +343,350 @@
             ...                      label(10, 15, x=6)])
             >>> index == index.ascending()
             True
         """
         ...
 
     @abstractmethod
-    def descending(self) -> 'data.LabelIndex[L]':
-        """This label index sorted according to descending start index and ascending end index.
+    def descending(self) -> 'LabelIndex[L]':
+        """This label index sorted according to descending start index and
+        ascending end index.
 
         Returns:
             LabelIndex: A view of this label index.
 
         Examples:
             >>> from mtap import label_index, label
             >>> index = label_index([label(0, 5, x=1),
             ...                      label(0, 10, x=2),
             ...                      label(5, 10, x=3),
             ...                      label(7, 10, x=4),
             ...                      label(5, 15, x=5),
             ...                      label(10, 15, x=6)])
             >>> index.descending()
-            label_index([GenericLabel(10, 15, x=6), GenericLabel(7, 10, x=4), GenericLabel(5, 15, x=5),
-                         GenericLabel(5, 10, x=3), GenericLabel(0, 10, x=2), GenericLabel(0, 5, x=1)], distinct=False)
+            label_index([GenericLabel(10, 15, x=6), GenericLabel(7, 10, x=4),
+            GenericLabel(5, 15, x=5), GenericLabel(5, 10, x=3),
+            GenericLabel(0, 10, x=2), GenericLabel(0, 5, x=1)], distinct=False)
         """
         ...
 
 
-def label_index(labels: List[L],
-                distinct: bool = False,
-                adapter: Optional['data.ProtoLabelAdapter'] = None) -> LabelIndex[L]:
+def label_index(
+        labels: List[L],
+        distinct: bool = False,
+        adapter: Optional['ProtoLabelAdapter'] = None
+) -> LabelIndex[L]:
     """Creates a label index from labels.
 
     Args:
-        labels (~typing.List[L]): Zero or more labels to create a label index from.
-        distinct (bool): Whether the label index is distinct or not.
-        adapter (~data.ProtoLabelAdapter): The label adapter for these labels.
+        labels: Zero or more labels to create a label index from.
+        distinct: Whether the label index is distinct or not.
+        adapter: The label adapter for these labels.
 
     Returns:
-        ~data.LabelIndex: The newly created label index.
+        The newly created label index.
 
     Examples:
         >>> from mtap import label_index, label
         >>> index = label_index([label(0, 5, x=1),
         ...                      label(0, 10, x=2),
         ...                      label(5, 10, x=3),
         ...                      label(7, 10, x=4),
         ...                      label(5, 15, x=5),
         ...                      label(10, 15, x=6)])
         >>> index
-        label_index([GenericLabel(0, 5, x=1), GenericLabel(0, 10, x=2), GenericLabel(5, 10, x=3),
-                     GenericLabel(5, 15, x=5), GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)], distinct=False)
+        label_index([GenericLabel(0, 5, x=1), GenericLabel(0, 10, x=2),
+        GenericLabel(5, 10, x=3), GenericLabel(5, 15, x=5),
+        GenericLabel(7, 10, x=4), GenericLabel(10, 15, x=6)], distinct=False)
 
     """
     labels = sorted(labels, key=attrgetter('location'))
     return presorted_label_index(labels, distinct, adapter=adapter)
 
 
-def presorted_label_index(labels: List[L],
-                          distinct: bool = False,
-                          adapter: Optional['data.ProtoLabelAdapter'] = None) -> LabelIndex[L]:
+def presorted_label_index(
+        labels: List[L],
+        distinct: bool = False,
+        adapter: Optional['ProtoLabelAdapter'] = None
+) -> LabelIndex[L]:
     if len(labels) == 0:
         return _Empty(distinct, adapter)
     return _LabelIndex(distinct, _Ascending(labels), adapter=adapter)
 
 
+class _Locations(Sequence[Location]):
+    __slots__ = ('labels', 'indices')
+
+    def __init__(self,
+                 labels: Sequence[Label],
+                 indices: Optional[Sequence[int]]):
+        self.labels = labels
+        self.indices = indices
+
+    def __getitem__(self, item):
+        x = self.indices[item]
+        if isinstance(x, int):
+            return self.labels[x].location
+        return _Locations(self.labels, x)
+
+    def __len__(self) -> int:
+        return len(self.indices)
+
+
 class _View(metaclass=ABCMeta):
-    __slots__ = ('_labels', '_indices', '_locations')
+    __slots__ = ('labels', 'indices', '_locations')
 
-    def __init__(self, labels, indices: Sequence[int] = ...):
-        self._labels = labels
-        self._indices = range(len(labels)) if indices is ... else indices
+    def __init__(self, labels, indices: Optional[Sequence[int]] = None):
+        self.labels = labels
+        self.indices = range(len(labels)) if indices is None else indices
+        self._locations = None
 
     @property
     def locations(self):
-        try:
-            locations = self._locations
-        except AttributeError:
-            locations = [self._labels[i].location for i in self._indices]
-            self._locations = locations
-        return locations
+        if self._locations is None:
+            self._locations = _Locations(self.labels, self.indices)
+        return self._locations
 
     def __len__(self):
-        return len(self._indices)
+        return len(self.indices)
 
     def bound(self,
               min_start: float = 0,
               max_start: float = float('inf'),
               min_end: float = 0,
               max_end: float = float('inf')) -> '_View':
-        filtered_indices = list(self._filter(min_start, max_start, min_end, max_end))
+        filtered_indices = list(
+            self._filter(min_start, max_start, min_end, max_end))
         if len(filtered_indices) == 0:
             raise ValueError
-        return self.__class__(self._labels, filtered_indices)
+        return self.__class__(self.labels, filtered_indices)
 
-    def filter(self, fn: Callable[['data.Label'], bool]) -> '_View':
+    def filter(self, fn: Callable[[Label], bool]) -> '_View':
         filtered_indices = list(self._filter_fn(fn))
         if len(filtered_indices) == 0:
             raise ValueError
-        return self.__class__(self._labels, filtered_indices)
+        return self.__class__(self.labels, filtered_indices)
 
     def _filter(self,
                 min_start: float = 0,
                 max_start: float = float('inf'),
                 min_end: float = 0,
                 max_end: float = float('inf')) -> Iterator[int]:
         try:
-            left = self._index_lt(_labels.Location(min_start, min_end)) + 1
+            left = self._index_lt(Location(min_start, min_end)) + 1
         except ValueError:
             left = 0
 
-        for i in range(left, len(self._indices)):
+        for i in range(left, len(self.indices)):
             location = self.locations[i]
             if location.start_index > max_start:
                 break
             if min_end <= location.end_index <= max_end:
-                yield self._indices[i]
+                yield self.indices[i]
 
-    def _filter_fn(self, fn: Callable[['data.Label'], bool]) -> Iterator[int]:
-        for index in self._indices:
-            label = self._labels[index]
+    def _filter_fn(self, fn: Callable[[Label], bool]) -> Iterator[int]:
+        for index in self.indices:
+            label = self.labels[index]
             if fn(label):
                 yield index
 
     def _first_index_location(self,
-                              location: 'data.Location',
+                              location: Location,
                               from_index: int = 0,
                               to_index: int = ...) -> int:
         if to_index is ...:
             to_index = len(self.locations)
         i = bisect_left(self.locations, location, from_index, to_index)
 
         if i != to_index and self.locations[i] == location:
             return i
         raise ValueError
 
     def _last_index_location(self,
-                             location: 'data.Location',
+                             location: Location,
                              from_index: int = 0,
                              to_index: int = ...):
         if to_index is ...:
             to_index = len(self.locations)
         i = bisect_right(self.locations, location, from_index, to_index)
 
         if i > from_index and self.locations[i - 1] == location:
             return i - 1
         raise ValueError
 
     def _index_lt(self,
-                  location: 'data.Location',
+                  location: Location,
                   from_index: int = 0,
                   to_index: int = ...) -> int:
         if to_index is ...:
             to_index = len(self.locations)
 
         i = bisect_left(self.locations, location, from_index, to_index)
         if i > from_index:
             return i - 1
         raise ValueError
 
     @abstractmethod
-    def __getitem__(self, idx) -> Union['data.Label', '_View']:
+    def __getitem__(self, idx) -> Union[Label, '_View']:
         ...
 
     @abstractmethod
-    def __iter__(self) -> Iterator['data.Label']:
+    def __iter__(self) -> Iterator[Label]:
         ...
 
     @abstractmethod
     def reversed(self):
         ...
 
     @abstractmethod
     def index_location(self,
-                       location: 'data.Location',
+                       location: Location,
                        from_index: int = 0,
                        to_index: int = ...) -> int:
         ...
 
 
 class _Ascending(_View):
     __slots__ = ()
 
-    def __getitem__(self, idx) -> Union['data.Label', '_View']:
+    def __getitem__(self, idx) -> Union[Label, '_View']:
         if isinstance(idx, int):
-            return self._labels[self._indices[idx]]
+            return self.labels[self.indices[idx]]
         elif isinstance(idx, slice):
-            return _Ascending(self._labels, self._indices[idx])
+            return _Ascending(self.labels, self.indices[idx])
 
-    def __iter__(self) -> Iterator['data.Label']:
-        for idx in self._indices:
-            yield self._labels[idx]
+    def __iter__(self) -> Iterator[Label]:
+        for idx in self.indices:
+            yield self.labels[idx]
 
     def reversed(self):
-        return _Descending(self._labels, self._indices)
+        return _Descending(self.labels, self.indices)
 
     def index_location(self,
-                       location: 'data.Location',
+                       location: Location,
                        from_index: int = 0,
                        to_index: int = ...) -> int:
         return self._first_index_location(location, from_index, to_index)
 
 
 class _Descending(_View):
     __slots__ = ()
 
     def _reverse_index(self, i: int = None):
         return -(i + 1)
 
-    def __getitem__(self, idx) -> Union['data.Label', '_View']:
+    def __getitem__(self, idx) -> Union[Label, '_View']:
         if isinstance(idx, int):
-            return self._labels[self._indices[self._reverse_index(idx)]]
+            return self.labels[self.indices[self._reverse_index(idx)]]
         elif isinstance(idx, slice):
             start = idx.stop
             if start is not None:
                 start = self._reverse_index(idx.stop - 1)
             stop = idx.start
             if stop is not None:
                 stop = self._reverse_index(idx.start - 1)
             idx = slice(start, stop, idx.step)
-            return _Descending(self._labels, self._indices[idx])
+            return _Descending(self.labels, self.indices[idx])
 
-    def __iter__(self) -> Iterator['data.Label']:
-        for i in range(len(self._indices)):
-            yield self._labels[self._indices[self._reverse_index(i)]]
+    def __iter__(self) -> Iterator[Label]:
+        for i in range(len(self.indices)):
+            yield self.labels[self.indices[self._reverse_index(i)]]
 
     def reversed(self):
-        return _Ascending(self._labels, self._indices)
+        return _Ascending(self.labels, self.indices)
 
     def index_location(self,
-                       location: 'data.Location',
+                       location: Location,
                        from_index: int = 0,
                        to_index: int = ...) -> int:
-        index_location = self._last_index_location(location, from_index, to_index)
+        index_location = self._last_index_location(location, from_index,
+                                                   to_index)
         return self._reverse_index(index_location)
 
 
-def _start_and_end(x: Union['data.Label', float], end: Optional[float] = None) -> 'data.Location':
+def _start_and_end(x: Union[Label, float],
+                   end: Optional[float] = None) -> Location:
     if end is None:
         x = _location(x)
         start = x.start_index
         end = x.end_index
     else:
         if not isinstance(x, int) and not isinstance(x, float):
             raise TypeError
         if not isinstance(end, int) and not isinstance(end, float):
             raise TypeError
         start = x
         if end is None:
             end = float('inf')
-    return _labels.Location(start, end)
+    return Location(start, end)
 
 
 def _location(x):
-    if isinstance(x, _labels.Label):
+    if isinstance(x, Label):
         x = x.location
-    if not isinstance(x, _labels.Location):
+    if not isinstance(x, Location):
         raise TypeError
     return x
 
 
 class _LabelIndex(LabelIndex[L]):
     __slots__ = ('_distinct', '_view', '_ascending', '_adapter', '__reversed')
 
     def __init__(self, distinct: bool,
                  view: _View,
                  ascending: bool = True,
                  reversed_index: '_LabelIndex[L]' = None,
-                 adapter: Optional['data.ProtoLabelAdapter'] = None):
+                 adapter: Optional['ProtoLabelAdapter'] = None):
         self._distinct = distinct
         self._view = view
         self._ascending = ascending
         self._adapter = adapter
         if reversed_index is not None:
             self.__reversed = reversed_index
 
     @property
     def distinct(self) -> bool:
         return self._distinct
 
     @property
-    def adapter(self) -> 'data.ProtoLabelAdapter[L]':
+    def adapter(self) -> 'ProtoLabelAdapter[L]':
         return self._adapter
 
     @adapter.setter
-    def adapter(self, value: 'data.ProtoLabelAdapter[L]'):
+    def adapter(self, value: 'ProtoLabelAdapter[L]'):
         self._adapter = value
 
-    def filter(self, fn: Callable[['data.Label'], bool]) -> 'data.LabelIndex[L]':
+    def filter(self, fn: Callable[[Label], bool]) -> 'LabelIndex[L]':
         return self._filtered_or_empty(fn)
 
     @property
-    def _reversed(self) -> '_LabelIndex[L]':
+    def _reversed(self) -> 'LabelIndex[L]':
         try:
             reversed_label_index = self.__reversed
         except AttributeError:
             reversed_label_index = _LabelIndex(distinct=self.distinct,
                                                view=self._view.reversed(),
                                                ascending=False,
                                                reversed_index=self)
             self.__reversed = reversed_label_index
         return reversed_label_index
 
-    def __getitem__(self, idx: Union[int, slice]) -> Union[L, 'data.LabelIndex[L]']:
+    def __getitem__(self, idx: Union[int, slice]) -> Union[L, 'LabelIndex[L]']:
         if isinstance(idx, int):
             return self._view[idx]
         elif isinstance(idx, slice):
-            return _LabelIndex(self.distinct, self._view[idx], adapter=self.adapter)
+            return _LabelIndex(self.distinct, self._view[idx],
+                               adapter=self.adapter)
         else:
             raise TypeError("Index must be int or slice.")
 
     def at(self, x, end=None):
         start, end = _start_and_end(x, end)
-        return self._bounded_or_empty(min_start=start, max_start=start, min_end=end, max_end=end)
+        return self._bounded_or_empty(min_start=start, max_start=start,
+                                      min_end=end, max_end=end)
 
     def __contains__(self, item: Any) -> bool:
         try:
             self.index(item)
             return True
         except ValueError:
             return False
@@ -613,67 +697,67 @@
     def __iter__(self) -> Iterator[L]:
         return iter(self._view)
 
     def __reversed__(self) -> Iterator[L]:
         return iter(self._reversed)
 
     def index(self, x: Any, start: int = ..., end: int = ...) -> int:
-        if not isinstance(x, _labels.Label):
+        if not isinstance(x, Label):
             raise ValueError
         for i in range(self._view.index_location(x.location), len(self._view)):
             if self._view[i] == x:
                 return i
         raise ValueError
 
     def count(self, x: Any) -> int:
-        if not isinstance(x, _labels.Label):
+        if not isinstance(x, Label):
             return False
         try:
             i = self._view.index_location(x.location)
         except ValueError:
             return 0
         count = 0
         for label in self._view[i:]:
             if not label.location == x.location:
                 break
             if label == x:
                 count += 1
         return count
 
     def covering(self,
-                 x: Union['data.Label', float],
-                 end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                 x: Union[Label, float],
+                 end: Optional[float] = None) -> 'LabelIndex[L]':
         start, end = _start_and_end(x, end)
         return self._bounded_or_empty(max_start=start, min_end=end)
 
     def overlapping(self,
-                    x: Union['data.Label', float],
-                    end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                    x: Union[Label, float],
+                    end: Optional[float] = None) -> 'LabelIndex[L]':
         start, end = _start_and_end(x, end)
         return self._bounded_or_empty(max_start=end - 1, min_end=start + 1)
 
     def inside(self,
-               x: Union['data.Label', float],
-               end: Optional[float] = None) -> 'data.LabelIndex[L]':
+               x: Union[Label, float],
+               end: Optional[float] = None) -> 'LabelIndex[L]':
         start, end = _start_and_end(x, end)
         return self._bounded_or_empty(start, end - 1, start, end)
 
     def beginning_inside(self,
-                         x: Union['data.Label', float],
-                         end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                         x: Union[Label, float],
+                         end: Optional[float] = None) -> 'LabelIndex[L]':
         start, end = _start_and_end(x, end)
         return self._bounded_or_empty(min_start=start, max_start=end - 1)
 
-    def ascending(self) -> 'data.LabelIndex[L]':
+    def ascending(self) -> 'LabelIndex[L]':
         if self._ascending:
             return self
         else:
             return self._reversed
 
-    def descending(self) -> 'data.LabelIndex[L]':
+    def descending(self) -> 'LabelIndex[L]':
         if not self._ascending:
             return self
         else:
             return self._reversed
 
     def __repr__(self):
         return ("label_index(["
@@ -690,96 +774,97 @@
 
     def _bounded_or_empty(self,
                           min_start: float = 0,
                           max_start: float = float('inf'),
                           min_end: float = 0,
                           max_end: float = float('inf')):
         try:
-            bounded_view = self._view.bound(min_start=min_start, max_start=max_start,
+            bounded_view = self._view.bound(min_start=min_start,
+                                            max_start=max_start,
                                             min_end=min_end, max_end=max_end)
         except ValueError:
             return _Empty(self.distinct, self.adapter)
         return _LabelIndex(self.distinct, bounded_view, adapter=self.adapter)
 
-    def _filtered_or_empty(self, fn: Callable[['data.Label'], bool]):
+    def _filtered_or_empty(self, fn: Callable[[Label], bool]):
         try:
             filtered_view = self._view.filter(fn)
         except ValueError:
             return _Empty(self.distinct, self.adapter)
         return _LabelIndex(self.distinct, filtered_view, adapter=self.adapter)
 
 
 class _Empty(LabelIndex):
     __slots__ = ('_distinct', '_adapter')
 
     @property
-    def adapter(self) -> Optional['data.ProtoLabelAdapter']:
+    def adapter(self) -> Optional['ProtoLabelAdapter']:
         return self._adapter
 
     def __init__(self, distinct, adapter=None):
         self._distinct = distinct
         self._adapter = adapter
 
     @property
     def distinct(self) -> bool:
         return self._distinct
 
     def __getitem__(self, idx):
         raise IndexError
 
-    def filter(self, fn: Callable[['data.Label'], bool]) -> 'data.LabelIndex[L]':
+    def filter(self, fn: Callable[[Label], bool]) -> 'LabelIndex[L]':
         return self
 
     def at(self,
-           x: Union['data.Label', 'data.Location', float],
-           end: Optional[float] = None) -> 'data.LabelIndex[L]':
+           x: Union[Label, 'Location', float],
+           end: Optional[float] = None) -> 'LabelIndex[L]':
         return self
 
     def __len__(self) -> int:
         return 0
 
     def __contains__(self, item: Any) -> bool:
         return False
 
     def __iter__(self) -> Iterator[L]:
         return iter([])
 
-    def __reversed__(self) -> 'data.LabelIndex[L]':
+    def __reversed__(self) -> 'LabelIndex[L]':
         return self
 
     def index(self, x: Any, start: int = ..., end: int = ...) -> int:
         raise ValueError
 
     def count(self, x: Any) -> int:
         return 0
 
     def covering(self,
-                 x: Union['data.Label', float],
-                 end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                 x: Union[Label, float],
+                 end: Optional[float] = None) -> 'LabelIndex[L]':
         return self
 
     def inside(self,
-               x: Union['data.Label', float],
-               end: Optional[float] = None) -> 'data.LabelIndex[L]':
+               x: Union[Label, float],
+               end: Optional[float] = None) -> 'LabelIndex[L]':
         return self
 
     def overlapping(self,
-                    x: Union['data.Label', float],
-                    end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                    x: Union[Label, float],
+                    end: Optional[float] = None) -> 'LabelIndex[L]':
         return self
 
     def beginning_inside(self,
-                         x: Union['data.Label', float],
-                         end: Optional[float] = None) -> 'data.LabelIndex[L]':
+                         x: Union[Label, float],
+                         end: Optional[float] = None) -> 'LabelIndex[L]':
         return self
 
-    def ascending(self) -> 'data.LabelIndex[L]':
+    def ascending(self) -> 'LabelIndex[L]':
         return self
 
-    def descending(self) -> 'data.LabelIndex[L]':
+    def descending(self) -> 'LabelIndex[L]':
         return self
 
     def __eq__(self, other):
         if len(self) != len(other):
             return False
         for s, o in zip(self, other):
             if s != o:
```

### Comparing `mtap-1.2.0/python/mtap/data/_labels.py` & `mtap-1.2.1/python/mtap/_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Labels functionality."""
 import threading
-from abc import ABC, abstractmethod, ABCMeta
+from abc import abstractmethod, ABCMeta
 from queue import Queue
 from typing import (
     TYPE_CHECKING,
     TypeVar,
     NamedTuple,
     Any,
     Mapping,
@@ -27,45 +27,46 @@
 )
 
 if TYPE_CHECKING:
     from mtap import (
         Document
     )
 
-
-LocationLike = 'Union[Location, Label, int]'
+LocationLike = Union['Location', 'Label']
+HasStart = Union['Location', 'Label', float]
+HasEnd = Union['Location', 'Label', float]
 
 
 class Location(NamedTuple):
     """A location in text, a tuple of (`start_index`, `end_index`).
 
     Used to perform comparison of labels based on their locations.
     """
 
     start_index: float
     """The start index inclusive of the location in text."""
 
     end_index: float
     """The end index exclusive of the location in text."""
 
-    def covers(self, other: 'Union[Location, Label]'):
+    def covers(self, other: LocationLike):
         """Whether the span of text covered by this label completely overlaps
         the span of text covered by the ``other`` label or location.
 
         Args:
             other: A location or label to compare against.
 
         Returns:
             ``True`` if `other` is completely overlapped/covered
                 ``False`` otherwise.
         """
         return self.start_index <= other.start_index \
             and self.end_index >= other.end_index
 
-    def relative_to(self, location: LocationLike) -> 'Location':
+    def relative_to(self, location: HasStart) -> 'Location':
         """Creates a location relative to the same origin as ``location``
         and makes it relative to ``location``.
 
         Args:
             location: A location to relativize this
                 location to.
 
@@ -85,15 +86,15 @@
             start_index = location
         if not isinstance(start_index, int):
             raise ValueError(
                 'location must be Label, Location, or an int value')
         return Location(self.start_index - start_index,
                         self.end_index - start_index)
 
-    def offset_by(self, location: LocationLike) -> 'Location':
+    def offset_by(self, location: HasStart) -> 'Location':
         """Creates a location by offsetting this location by an integer or the
         ``start_index`` of a location / label. De-relativizes this location.
 
         Args:
             location: A location to offset this location by.
 
         Returns:
@@ -114,15 +115,15 @@
             raise ValueError(
                 'location must be Label, Location, or an int value'
             )
         return Location(self.start_index + start_index,
                         self.end_index + start_index)
 
 
-class Label(ABC, metaclass=ABCMeta):
+class Label(metaclass=ABCMeta):
     """An abstract base class for a label of attributes on text.
     """
 
     @property
     @abstractmethod
     def document(self) -> 'Document':
         """The parent document this label appears on."""
@@ -176,15 +177,16 @@
     @abstractmethod
     def start_index(self, value: int):
         ...
 
     @property
     @abstractmethod
     def end_index(self) -> int:
-        """The index after the last character of the text covered by this label.
+        """The index after the last character of the text covered by this
+        label.
         """
         ...
 
     @end_index.setter
     @abstractmethod
     def end_index(self, value: int):
         ...
@@ -224,14 +226,28 @@
 
 
 L = TypeVar('L', bound=Label)
 
 _repr_local = threading.local()
 
 
+def _collect_refs_from_item(o, queue, s):
+    if isinstance(o, Label):
+        if o.identifier is None:
+            s.add(id(o))
+    elif isinstance(o, Mapping):
+        for _, v in o.items():
+            if v is not None:
+                queue.put(v)
+    elif isinstance(o, Sequence):
+        for v in o:
+            if v is not None:
+                queue.put(v)
+
+
 class GenericLabel(Label):
     """Default implementation of the Label class which uses a dictionary to
     store attributes.
 
     Will be suitable for the majority of use cases for labels.
 
     Args:
@@ -407,30 +423,23 @@
             if k not in self.reference_cache:
                 attributes.append("{}=ref:{}".format(k, repr(v)))
         stack.remove(id(self))
         return "GenericLabel(".format() + ", ".join(attributes) + ")"
 
     def collect_floating_references(self, s):
         queue = Queue()
+        self._populate_queue(queue)
+        while not queue.empty():
+            o = queue.get_nowait()
+            _collect_refs_from_item(o, queue, s)
+
+    def _populate_queue(self, queue):
         for k, v in self.reference_cache.items():
             if v is not None:
                 queue.put(v)
-        while not queue.empty():
-            o = queue.get_nowait()
-            if isinstance(o, Label):
-                if o.identifier is None:
-                    s.add(id(o))
-            elif isinstance(o, Mapping):
-                for _, v in o.items():
-                    if v is not None:
-                        queue.put(v)
-            elif isinstance(o, Sequence):
-                for v in o:
-                    if v is not None:
-                        queue.put(v)
 
 
 def label(start_index: int,
           end_index: int,
           *, document: 'Optional[Document]' = None,
           **kwargs) -> GenericLabel:
     """An alias for :class:`GenericLabel`.
@@ -453,43 +462,52 @@
     if parents is None:
         parents = [id(o)]
     if isinstance(o, (str, float, bool, int)) or o is None:
         return False
     elif isinstance(o, Label):
         return True
     elif isinstance(o, Mapping):
-        map_is_ref = None
-        for v in o.values():
-            if id(v) in parents:
-                raise ValueError('Recursive loop')
-            x = _is_referential(v, parents + [id(v)])
-            if map_is_ref is None:
-                map_is_ref = x
-            elif x != map_is_ref:
-                raise TypeError(
-                    'Label dictionaries cannot have mixes of references to labels'
-                    'and primitive types.')
-        return map_is_ref
+        return _mapping_is_ref(o, parents)
     elif isinstance(o, Sequence):
-        seq_is_ref = None
-        for v in o:
-            if id(v) in parents:
-                raise ValueError('Recursive loop')
-            x = _is_referential(v, parents + [id(v)])
-            if seq_is_ref is None:
-                seq_is_ref = x
-            elif x != seq_is_ref:
-                raise TypeError(
-                    'Label lists cannot have mixes of references to labels'
-                    'and primitive types.')
-        return seq_is_ref
+        return _sequence_is_ref(o, parents)
     else:
         raise TypeError('Unrecognized type')
 
 
+def _mapping_is_ref(o: Mapping, parents) -> bool:
+    map_is_ref = None
+    for v in o.values():
+        if id(v) in parents:
+            raise ValueError('Recursive loop')
+        x = _is_referential(v, parents + [id(v)])
+        if map_is_ref is None:
+            map_is_ref = x
+        elif x != map_is_ref:
+            raise TypeError(
+                'Label dictionaries cannot have mixes of references to '
+                'labels and primitive types.'
+            )
+    return map_is_ref
+
+
+def _sequence_is_ref(o: Sequence, parents) -> bool:
+    seq_is_ref = None
+    for v in o:
+        if id(v) in parents:
+            raise ValueError('Recursive loop')
+        x = _is_referential(v, parents + [id(v)])
+        if seq_is_ref is None:
+            seq_is_ref = x
+        elif x != seq_is_ref:
+            raise TypeError(
+                'Label lists cannot have mixes of references to labels'
+                'and primitive types.')
+    return seq_is_ref
+
+
 def _dereference(o: Any, document: 'Document') -> Any:
     if o is None:
         return o
     if isinstance(o, str):
         label_index_name, label_id = o.split(':')
         label_index = document.labels[label_index_name]
         label_ = label_index[int(label_id)]
```

### Comparing `mtap-1.2.0/python/mtap/defaultConfig.yml` & `mtap-1.2.1/python/mtap/defaultConfig.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/deployment.py` & `mtap-1.2.1/python/mtap/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 @dataclass
 class GlobalSettings:
     """Settings shared by event service and all processors.
     """
     host: Optional[str] = None
-    """The global host override, forces all services to use a specific host 
+    """The global host override, forces all services to use a specific host
     name."""
 
     mtap_config: Optional[str] = None
     """The path to an MTAP config file to load for all services."""
 
     log_level: Optional[str] = None
     """A python logging level to pass to all services."""
@@ -116,23 +116,23 @@
 
 @dataclass
 class SharedProcessorConfig:
     """Configuration that is shared between multiple processor services.
     """
 
     events_addresses: Optional[List[str]] = None
-    """An optional GRPC-compatible target for the events service to be used by 
+    """An optional GRPC-compatible target for the events service to be used by
     all processors.
     """
 
     workers: Optional[int] = None
     """The default number of worker threads which will perform processing."""
 
     additional_args: Optional[List[str]] = None
-    """A list of additional arguments that should be appended to every 
+    """A list of additional arguments that should be appended to every
     processor.
     """
 
     jvm_args: Optional[List[str]] = None
     """A list of JVM arguments for all Java processors."""
 
     java_classpath: Optional[str] = None
@@ -141,15 +141,15 @@
     java_additional_args: Optional[List[str]] = None
     """A list of additional arguments that is added to only Java processors."""
 
     startup_timeout: Optional[float] = None
     """The default startup timeout for processors."""
 
     mp_spawn_method: Optional[str] = None
-    """A :meth:`multiprocessing.get_context` argument to create the 
+    """A :meth:`multiprocessing.get_context` argument to create the
     multiprocessing context.
     """
 
     @staticmethod
     def from_conf(conf: Optional[Dict[str, Any]]) -> 'SharedProcessorConfig':
         """Builds a configuration from a dictionary representation.
 
@@ -326,35 +326,35 @@
     port: Optional[int] = None
     """The listening port for the processor service."""
 
     workers: Optional[int] = None
     """The number of worker threads per instance."""
 
     register: Optional[bool] = None
-    """Whether the processor should register with the discovery service 
+    """Whether the processor should register with the discovery service
     specified in the MTAP config file.
     """
 
     mtap_config: Optional[str] = None
     """Path to the MTAP configuration file."""
 
     log_level: Optional[str] = None
     """The log level for the processor."""
 
     name: Optional[str] = None
     """An optional service name override to use for registration."""
 
     sid: Union[str, List[str], None] = None
-    """An optional service instance unique identifier. If instances is 1 this 
-    should be a string, if instances is more than 1 this should be a list of 
+    """An optional service instance unique identifier. If instances is 1 this
+    should be a string, if instances is more than 1 this should be a list of
     strings, one for each instance.
     """
 
     pre_args: Optional[List[str]] = None
-    """Arguments that occur prior to the MTAP service arguments (like host, 
+    """Arguments that occur prior to the MTAP service arguments (like host,
     port, etc).
     """
 
     additional_args: Optional[List[str]] = None
     """Arguments that occur after the MTAP service arguments."""
 
     startup_timeout: Optional[float] = None
@@ -390,60 +390,63 @@
     if isinstance(depl.port, list):
         ports = depl.port
     elif depl.port is None:
         ports = [None] * depl.instances
     else:
         ports = list(range(depl.port, depl.port + depl.instances))
     for port in ports:
-        if depl.implementation == 'python':
-            call = [PYTHON_EXE, '-m', depl.entry_point]
-        elif depl.implementation == 'java':
-            call = [str(JAVA_EXE)]
-            if shared_config.jvm_args is not None:
-                call.extend(shared_config.jvm_args)
-            if shared_config.java_classpath is not None:
-                call.extend(['-cp', shared_config.java_classpath])
-            call.append(depl.entry_point)
-        else:
-            raise ValueError(
-                'Unrecognized implementation: ' + depl.implementation)
+        yield from _create_processor_call(depl, global_settings, port,
+                                          service_deployment, shared_config)
 
-        if depl.pre_args is not None:
-            call.extend(depl.pre_args)
 
-        service_args, sid = service_deployment.service_args(
-            host=depl.host,
-            port=port,
-            sid=depl.sid,
-            register_default=global_settings.register,
-            global_host=global_settings.host,
-            mtap_config_default=global_settings.mtap_config,
-            log_level_default=global_settings.log_level,
-            workers_default=shared_config.workers
-        )
-        call.extend(service_args)
-
-        if depl.name is not None:
-            call.extend(['--name', depl.name])
-
-        events_addresses = shared_config.events_addresses
-        if events_addresses is not None:
-            call.extend(['--events', ','.join(events_addresses)])
-
-        if depl.additional_args is not None:
-            call.extend(depl.additional_args)
-
-        if shared_config.additional_args is not None:
-            call.extend(shared_config.additional_args)
-
-        if (depl.implementation == 'java'
-                and shared_config.java_additional_args is not None):
-            call.extend(shared_config.java_additional_args)
-
-        yield call, sid
+def _create_processor_call(depl, global_settings, port, service_deployment,
+                           shared_config):
+    call = _implementation_args(depl, shared_config)
+    if depl.pre_args is not None:
+        call.extend(depl.pre_args)
+    service_args, sid = service_deployment.service_args(
+        host=depl.host,
+        port=port,
+        sid=depl.sid,
+        register_default=global_settings.register,
+        global_host=global_settings.host,
+        mtap_config_default=global_settings.mtap_config,
+        log_level_default=global_settings.log_level,
+        workers_default=shared_config.workers
+    )
+    call.extend(service_args)
+    if depl.name is not None:
+        call.extend(['--name', depl.name])
+    events_addresses = shared_config.events_addresses
+    if events_addresses is not None:
+        call.extend(['--events', ','.join(events_addresses)])
+    if depl.additional_args is not None:
+        call.extend(depl.additional_args)
+    if shared_config.additional_args is not None:
+        call.extend(shared_config.additional_args)
+    if (depl.implementation == 'java'
+            and shared_config.java_additional_args is not None):
+        call.extend(shared_config.java_additional_args)
+    yield call, sid
+
+
+def _implementation_args(depl, shared_config):
+    if depl.implementation == 'python':
+        call = [PYTHON_EXE, '-m', depl.entry_point]
+    elif depl.implementation == 'java':
+        call = [str(JAVA_EXE)]
+        if shared_config.jvm_args is not None:
+            call.extend(shared_config.jvm_args)
+        if shared_config.java_classpath is not None:
+            call.extend(['-cp', shared_config.java_classpath])
+        call.append(depl.entry_point)
+    else:
+        raise ValueError(
+            'Unrecognized implementation: ' + depl.implementation)
+    return call
 
 
 @dataclass
 class Deployment:
     """An automatic deployment configuration which launches a configurable set
     of MTAP services.
     """
```

### Comparing `mtap-1.2.0/python/mtap/discovery.py` & `mtap-1.2.1/python/mtap/discovery.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/__init__.py` & `mtap-1.2.1/python/mtap/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/exampleDeploymentConfiguration.yml` & `mtap-1.2.1/python/mtap/examples/exampleDeploymentConfiguration.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/examplePipelineConfiguration.yml` & `mtap-1.2.1/python/mtap/examples/examplePipelineConfiguration.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/example_pipeline.py` & `mtap-1.2.1/python/mtap/examples/example_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 import shutil
 from argparse import ArgumentParser
 from pathlib import Path
 
 import mtap
 from mtap.serialization import SerializationProcessor, JsonSerializer
-from mtap.processing import (
+from mtap.pipeline import (
     FilesInDirectoryProcessingSource,
     Pipeline,
     LocalProcessor,
 )
 
 
 def print_example(_):
```

### Comparing `mtap-1.2.0/python/mtap/examples/example_processor.py` & `mtap-1.2.1/python/mtap/examples/example_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """An example document processor."""
 
 from mtap import DocumentProcessor, processor, run_processor
-from mtap.processing.descriptions import parameter, labels, label_property
+from mtap.descriptors import parameter, labels, label_property
 
 
 @processor('mtap-example-processor-python',
            human_name="Python Example Processor",
            description="counts the number of times the letters a and b occur "
                        "in a document",
            parameters=[
```

### Comparing `mtap-1.2.0/python/mtap/examples/example_references_processor.py` & `mtap-1.2.1/python/mtap/examples/example_references_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Any
 
 import mtap
-from mtap.processing.descriptions import labels
+from mtap.descriptors import labels
 
 
 @mtap.processor(
     'mtap-python-references-example',
     human_name='Python References Examples',
     description='Shows use of referential fields on labels.',
     outputs=[
```

### Comparing `mtap-1.2.0/python/mtap/examples/print_processor_meta.py` & `mtap-1.2.1/python/mtap/examples/print_processor_meta.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/serialization/__init__.py` & `mtap-1.2.1/python/mtap/examples/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/serialization/brat_converter.py` & `mtap-1.2.1/python/mtap/examples/serialization/brat_converter.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/tutorial/__init__.py` & `mtap-1.2.1/python/mtap/examples/tutorial/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/tutorial/hello.py` & `mtap-1.2.1/python/mtap/examples/tutorial/hello.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/examples/tutorial/pipeline.py` & `mtap-1.2.1/python/mtap/examples/tutorial/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Hello world tutorial pipeline."""
 import sys
 
 if __name__ == '__main__':
-    from mtap import Document, Event, Pipeline, EventsClient
-    from mtap.processing import RemoteProcessor
+    from mtap import Document, Event, Pipeline, events_client
+    from mtap import RemoteProcessor
 
-    with EventsClient(sys.argv[1]) as client:
-        pipeline = Pipeline(
-            RemoteProcessor(processor_name='hello', address=sys.argv[2]),
-        )
+    pipeline = Pipeline(
+        RemoteProcessor(processor_name='hello', address=sys.argv[2]),
+    )
+    with events_client(sys.argv[1]) as client:
         with Event(event_id='1', client=client) as event:
             document = Document(document_name='name', text='YOUR NAME')
             event.add_document(document)
             pipeline.run(document)
-            index = document.get_label_index('hello')
+            index = document.labels['hello']
             for label in index:
                 print(label.response)
```

### Comparing `mtap-1.2.0/python/mtap/metrics.py` & `mtap-1.2.1/python/mtap/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,76 +7,78 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Provides functionality for measuring processor performance against gold standards."""
+"""Provides functionality for measuring processor performance against gold
+standards.
+"""
 import sys
 from abc import ABC, abstractmethod
-from typing import Dict, Any, Optional, Sequence, NamedTuple, Callable, Tuple, TextIO, TYPE_CHECKING
+from typing import Dict, Any, Optional, Sequence, NamedTuple, Callable, Tuple, \
+    TextIO
+
+from mtap._document import Document
+from mtap._label_indices import presorted_label_index
+from mtap.descriptors import processor
+from mtap.processing import DocumentProcessor
+from mtap.types import LabelIndex, Label
+from mtap.utilities import tokenization
 
 __all__ = [
     'Metric',
     'Metrics',
     'print_overlapping',
     'fields_match_test',
     'Accuracy',
     'ConfusionMatrix',
     'FirstTokenConfusion'
 ]
 
-from mtap.data import presorted_label_index
-from mtap.processing import DocumentProcessor, processor
-from mtap.utilities import tokenization
-
-if TYPE_CHECKING:
-    import mtap
-    from mtap import data
-
 
 class Metric(ABC):
     """Base class for metrics.
 
     """
     name = None
 
     @abstractmethod
     def update(self,
-               document: 'mtap.Document',
-               tested_index: 'data.LabelIndex', target_index: 'data.LabelIndex') -> Any:
+               document: Document,
+               tested_index: LabelIndex, target_index: LabelIndex) -> Any:
         ...
 
 
 @processor('mtap-metrics')
 class Metrics(DocumentProcessor):
-    """A document process that computes a set of metrics.
+    """A document processor that computes a set of metrics.
 
-    Args
-    ---
-    tested (str): The name of the index to use as the hypothesis / predictions.
-    target (str): The name of the index to use as the ground truth / gold standard.
-    tested_filter (~typing.Callable[[Label], bool]): A filter to apply to the tested index.
-    target_filter (~typing.Callable[[Label], bool]): A filter to apply to the target index.
+    Args:
+        tested: The name of the index to use as the hypothesis / predictions.
+        target: The name of the index to use as the ground truth / gold
+            standard.
+        tested_filter: A filter to apply to the tested index.
+        target_filter: A filter to apply to the target index.
 
     """
 
     def __init__(self, *metrics: Metric,
                  tested: str,
                  target: str,
-                 tested_filter: Callable[['data.Label'], bool] = None,
-                 target_filter: Callable[['data.Label'], bool] = None):
+                 tested_filter: Callable[[Label], bool] = None,
+                 target_filter: Callable[[Label], bool] = None):
         self.tested = tested
         self.target = target
         self.metrics = metrics
         self.tested_filter = tested_filter
         self.target_filter = target_filter
 
-    def process_document(self, document: 'mtap.Document',
+    def process_document(self, document: Document,
                          params: Dict[str, Any]) -> Optional[Dict[str, Any]]:
         tested = document.labels[self.tested]
         if self.tested_filter is not None:
             tested = tested.filter(self.tested_filter)
         target = document.labels.get(self.target, presorted_label_index([]))
         if self.target_filter is not None:
             target = target.filter(self.target_filter)
@@ -91,64 +93,62 @@
     print('"', target_label.text(document.text), '"')
     overlapping = tested_index.overlapping(target_label)
     print('Overlapping:', overlapping)
     for overlap in overlapping:
         print('"', overlap.text(document.text), '"')
 
 
-def fields_match_test(fields: Optional[Sequence[str]] = ...):
-    """Creates an equivalence test that tests whether the specified fields are equal on both labels.
+def fields_match_test(fields: Optional[Sequence[str]] = None):
+    """Creates an equivalence test that tests whether the specified fields are
+    equal on both labels.
 
-    Parameters
-    ----------
-    fields: Optional[Sequence[str]]
-        The fields to test or ... if all fields should be tested.
+    Args:
+        fields: The fields to test or `None` if all fields should be tested.
 
     """
 
-    def fields_match(tested_label: 'data.Label', target_label: 'data.Label') -> bool:
+    def fields_match(tested_label: Label, target_label: Label) -> bool:
         if fields is not ...:
             return all(
-                getattr(tested_label, field) == getattr(target_label, field) for field in fields)
+                getattr(tested_label, field) == getattr(target_label, field)
+                for field in fields)
         else:
             return tested_label.shallow_fields_equal(target_label)
 
     return fields_match
 
 
 class Accuracy(Metric):
+    """An accuracy metric with several options for equivalence.
+
+    Args:
+        name: An identifier for the metric.
+        mode: 'equals' - counts as a hit if there is one and only one
+            label at the same location in the tested index as the target
+            index, and it has the same values for its fields.
+            'location' - counts as a hit if there is one and only one
+            label at the same location in the tested index as the target
+            index.
+            'any' - counts as a hit if there is one or more labels at the
+            same location with the same values for its fields.
+        print_debug: If true will print debug information about the misses.
+        boundary_fuzz: How different the target label boundaries can be from
+            the tested boundaries before it doesn't count as a match.
+        equivalence_test: callable
+            A function which takes two argument labels, and returns true if
+            the labels are equivalent for the purpose of the test.
+    """
     def __init__(self,
                  name: str = 'accuracy',
                  mode: str = 'equals',
                  print_debug: bool = False,
                  boundary_fuzz: int = 0,
                  fields: Optional[Sequence[str]] = ...,
-                 equivalence_test: Optional[Callable[[Any, Any], bool]] = fields_match_test(...)):
-        """An accuracy metric with several options for equivalence.
-
-        Parameters
-        ----------
-        name: str
-            An identifier for the metric.
-        mode: str
-            'equals' - counts as a hit if there is one and only one label at the same location in
-            the tested index as the target index and it has the same values for its fields
-            'location' - counts as a hit if there is one and only one label at the same location in
-            the tested index as the target index.
-            'any' - counts as a hit if there is one or more labels at the same location with the
-            same values for its fields.
-        print_debug: bool
-            If true will print debug information about the misses.
-        boundary_fuzz: int
-            How different the target label boundaries can be from the tested boundaries before it
-            doesn't count as a match.
-        equivalence_test: callable
-            A function which takes two argument labels, and returns true if the labels are
-            equivalent for the purpose of the test.
-        """
+                 equivalence_test: Optional[
+                     Callable[[Any, Any], bool]] = fields_match_test(...)):
         self.correct = 0
         self.total = 0
         self.name = name
         self.mode = mode
         self.print_debug = print_debug
         self.boundary_fuzz = boundary_fuzz
         if fields is ...:
@@ -157,39 +157,42 @@
             self.equivalence_test = fields_match_test(fields)
 
     @property
     def value(self) -> float:
         return self.correct / self.total if self.total > 0 else 1.
 
     def find_candidates(self,
-                        tested_index: 'data.LabelIndex',
-                        target_label: 'data.Label') -> 'data.LabelIndex':
+                        tested_index: LabelIndex,
+                        target_label: Label) -> LabelIndex:
         if self.boundary_fuzz == 0:
             index = tested_index.at(target_label)
         else:
             index = tested_index.inside(
                 target_label.start_index - 1,
                 target_label.end_index + 1
             ).covering(
                 target_label.start_index + 1,
                 target_label.end_index - 1
             )
         return index
 
-    def has_match(self, candidates: 'data.LabelIndex', target_label: 'data.Label') -> bool:
+    def has_match(self, candidates: LabelIndex, target_label: Label) -> bool:
         if self.mode == 'equals':
-            return len(candidates) == 1 and self.equivalence_test(candidates[0], target_label)
+            return len(candidates) == 1 and self.equivalence_test(
+                candidates[0], target_label)
         elif self.mode == 'location':
             return len(candidates) > 0
         elif self.mode == 'any':
-            return any(self.equivalence_test(candidate, target_label) for candidate in candidates)
-
-    def update(self, document: 'mtap.Document',
-               tested_index: 'data.LabelIndex',
-               target_index: 'data.LabelIndex') -> Any:
+            return any(
+                self.equivalence_test(candidate, target_label) for candidate in
+                candidates)
+
+    def update(self, document: Document,
+               tested_index: LabelIndex,
+               target_index: LabelIndex) -> Any:
         correct = 0
         total = 0
         for target_label in target_index:
             total += 1
             candidates = self.find_candidates(tested_index, target_label)
             if self.has_match(candidates, target_label):
                 correct += 1
@@ -201,52 +204,42 @@
         return correct / total if total != 0 else 1.
 
 
 def _collect_tokens(index, return_insides=True):
     begins = set()
     insides = set()
     for label in index:
-        for i, token in enumerate(tokenization.word_tokenize(label.text, label.start_index)):
+        for i, token in enumerate(
+                tokenization.word_tokenize(label.text, label.start_index)):
             if i == 0:
                 begins.add(token)
                 if not return_insides:
                     break
             else:
                 insides.add(token)
 
     return begins, insides
 
 
-class ConfusionMatrix(NamedTuple('ConfusionMatrix',
-                                 [('true_positives', float),
-                                  ('false_positives', float),
-                                  ('false_negatives', float)])):
+class ConfusionMatrix(NamedTuple):
     """A representation of a confusion matrix.
-
-    Attributes
-    ----------
-    true_positives (float): Count of true positive examples.
-    false_positives (float): Count of false positive examples.
-    false_negatives (float): Count of false negative examples.
-    precision (float): Ratio of true positives to the total number of positive predictions.
-    recall (float): Ratio of true positives to the total number of positive ground truths.
-    f1 (float): The harmonic mean of precision and recall.
-
     """
+    true_positives: float = 0
+    """Count of true positive examples."""
+
+    false_positives: float = 0
+    """Count of false positive examples."""
 
-    def __new__(cls, true_positives: float = 0,
-                false_positives: float = 0,
-                false_negatives: float = 0):
-        self = super().__new__(cls, true_positives, false_positives, false_negatives)
-        return self
+    false_negatives: float = 0
+    """Count of false negative examples."""
 
     def __add__(self, other):
-        return self.__class__(self.true_positives + other.true_positives,
-                              self.false_positives + other.false_positives,
-                              self.false_negatives + other.false_negatives)
+        return ConfusionMatrix(self.true_positives + other.true_positives,
+                               self.false_positives + other.false_positives,
+                               self.false_negatives + other.false_negatives)
 
     @property
     def precision(self):
         predicted_positives = self.true_positives + self.false_positives
         if predicted_positives == 0:
             return 1
         return self.true_positives / predicted_positives
@@ -256,95 +249,98 @@
         ground_truth_positives = self.true_positives + self.false_negatives
         if ground_truth_positives == 0:
             return 1
         return self.true_positives / ground_truth_positives
 
     @property
     def f1(self):
-        divisor = 2 * self.true_positives + self.false_positives + self.false_negatives
+        divisor = (2 * self.true_positives + self.false_positives
+                   + self.false_negatives)
         if divisor == 0:
             return 1
         return 2 * self.true_positives / divisor
 
 
 class FirstTokenConfusion(Metric):
-    """A metric which treats the first word token in every label as an example of the positive
-    class and calculates the precision, recall, and f1 confusion matrix metrics for that
-    positive class. Useful for evaluation of segmentation tasks.
+    """A metric which treats the first word token in every label as an example
+    of the positive class and calculates the precision, recall, and f1
+    confusion matrix metrics for that positive class. Useful for evaluation of
+    segmentation tasks.
 
     precision = true positives / (true positives + false positives)
     recall = true positives / (true positives + false negatives)
     f1 = 2 * true positives / (2 * true positives + false positives + false negatives)
 
-    Args
-    ----
-    name (str): An identifying name for the metric.
-    tested_filter (~typing.Callable[[Label], bool]): A filter to apply to the tested index.
-    target_filter (~typing.Callable[[Label], bool]): A filter to apply to the target index.
-    print_debug (str)
-        An argument to print failing examples. 'fp' prints only false positive
-        errors, 'fn' prints only false negative errors, 'all' prints both false positive and false
-        negative errors
-    debug_range (int): The range before and after the example to print.
-    debug_handle (TextIO): A text io file handle to print the debug information to.
-
-    Attributes
-    ----------
-    precision (float): Ratio of true positives to the total number of positive predictions.
-    recall (float): Ratio of true positives to the total number of positive ground truths.
-    f1 (float): The harmonic mean of precision and recall.
+    Args:
+        name: An identifying name for the metric.
+        tested_filter: A filter to apply to the tested index.
+        target_filter: A filter to apply to the target index.
+        print_debug: An argument to print failing examples. 'fp' prints only
+            false positive errors, 'fn' prints only false negative errors,
+            'all' prints both false positive and false negative errors
+        debug_range: The range before and after the example to print.
+        debug_handle: A text io file handle to print the debug information to.
     """
 
     def __init__(self, name: str = 'first_token_confusion',
-                 tested_filter: Callable[['data.Label'], bool] = None,
-                 target_filter: Callable[['data.Label'], bool] = None,
+                 tested_filter: Callable[[Label], bool] = None,
+                 target_filter: Callable[[Label], bool] = None,
                  print_debug: str = None,
                  debug_range: int = 30,
                  debug_handle: TextIO = sys.stdout):
         self.name = name
         self._matrix = ConfusionMatrix()
         self.tested_filter = tested_filter
         self.target_filter = target_filter
         self.print_debug = print_debug
         self.debug_range = debug_range
         self.debug_handle = debug_handle
 
     @property
     def precision(self) -> float:
+        """Ratio of true positives to the total number of positive
+        predictions.
+        """
         return self._matrix.precision
 
     @property
     def recall(self) -> float:
+        """Ratio of true positives to the total number of positive ground
+        truths.
+        """
         return self._matrix.recall
 
     @property
     def f1(self) -> float:
+        """The harmonic mean of precision and recall."""
         return self._matrix.f1
 
     def update(self,
-               document: 'mtap.Document',
-               tested_index: 'data.LabelIndex',
-               target_index: 'data.LabelIndex') -> Any:
+               document: Document,
+               tested_index: LabelIndex,
+               target_index: LabelIndex) -> Any:
         if self.tested_filter is not None:
             tested_index = tested_index.filter(self.tested_filter)
         if self.target_filter is not None:
             target_index = target_index.filter(self.target_filter)
         tested_tokens, _ = _collect_tokens(tested_index, return_insides=False)
         target_tokens, _ = _collect_tokens(target_index, return_insides=False)
         false_positives = tested_tokens.difference(target_tokens)
         false_negatives = target_tokens.difference(tested_tokens)
         if self.print_debug in ('fp', 'all'):
             self.debug_handle.write('False Positives\n')
             for false_positive in false_positives:
-                _print_example(document.text, false_positive, self.debug_range, self.debug_handle)
+                _print_example(document.text, false_positive, self.debug_range,
+                               self.debug_handle)
             self.debug_handle.write('\n')
         if self.print_debug in ('fn', 'all'):
             self.debug_handle.write('False Negatives\n')
             for false_negative in false_negatives:
-                _print_example(document.text, false_negative, self.debug_range, self.debug_handle)
+                _print_example(document.text, false_negative, self.debug_range,
+                               self.debug_handle)
             self.debug_handle.write('\n')
         local = ConfusionMatrix(
             true_positives=len(tested_tokens.intersection(target_tokens)),
             false_negatives=len(false_negatives),
             false_positives=len(false_positives)
         )
         self._matrix += local
@@ -358,10 +354,11 @@
 def _print_example(text: str,
                    token: Tuple[int, int],
                    debug_range: int,
                    debug_handle: TextIO):
     start, end = token
     print_start = max(0, start - debug_range)
     print_end = min(end + debug_range, len(text))
-    text = text[print_start:start] + '{' + text[start:end] + '}' + text[end:print_end]
+    text = text[print_start:start] + '{' + text[start:end] + '}' + text[
+                                                                   end:print_end]
     text = text.replace('\n', ' ') + '\n'
     debug_handle.write(text)
```

### Comparing `mtap-1.2.0/python/mtap/processing/__init__.py` & `mtap-1.2.1/python/mtap/processing/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,60 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from mtap.processing._base import (
-    DocumentProcessor,
-    EventProcessor,
-    Processor,
-    ProcessorContext,
-    ProcessingComponent,
-    Stopwatch,
-)
-from mtap.processing._exc import ProcessingError
-
-from mtap.processing._error_handling import (
-    StopProcessing,
-    SuppressError,
-    ErrorOrigin,
+from mtap.processing._exc import (
+    ProcessingException,
     ErrorInfo,
-    ProcessingErrorHandler,
-    SimpleErrorHandler,
-    TerminationErrorHandler,
-    LoggingErrorHandler,
-    ErrorsDirectoryErrorHandler,
-    SuppressAllErrorsHandler,
-    ErrorHandlerFactory,
-    ErrorHandlerRegistry,
+    ErrorOrigin,
 )
 
-from mtap.processing.descriptions import processor
-from mtap.processing._pipeline import Pipeline
-from mtap.processing._mp_config import MpConfig
-
-from mtap.processing._pipeline_components import (
-    RemoteProcessor,
-    LocalProcessor,
-    ComponentDescriptor,
+from mtap.processing._processor import (
+    Processor,
+    EventProcessor,
+    DocumentProcessor,
+    Stopwatch,
 )
 
-from mtap.processing._pipeline_results import (
-    AggregateTimingInfo,
-    BatchPipelineResult,
-    PipelineResult,
-    ComponentResult,
-    TimerStats,
+from mtap.processing._processing_component import (
+    ProcessingComponent
 )
 
-from mtap.processing._sources import (
-    FilesInDirectoryProcessingSource,
-    ProcessingSource,
+from mtap.processing._runners import (
+    LocalRunner,
+    RemoteRunner
 )
 
 from mtap.processing._service import (
     processor_parser,
     ProcessorServer,
     run_processor,
 )
```

### Comparing `mtap-1.2.0/python/mtap/processing/_base.py` & `mtap-1.2.1/python/mtap/processing/_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-# Copyright 2022 Regents of the University of Minnesota.
+# Copyright 2019 Regents of the University of Minnesota.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Internal processors and pipelines functionality."""
-import contextlib
 import threading
-from abc import ABCMeta, abstractmethod, ABC
+from abc import abstractmethod, ABCMeta
+from contextlib import contextmanager
+from dataclasses import asdict
 from datetime import datetime, timedelta
-from typing import (
-    ContextManager,
-    Any,
-    Dict,
-    Optional,
-    Mapping,
-    Tuple,
-    TYPE_CHECKING,
-    MutableMapping
-)
-
-from mtap import data
-
-if TYPE_CHECKING:
-    import mtap
-    from mtap import Event, Document
-    from mtap.data import ProtoLabelAdapter
+from typing import ClassVar, Optional, ContextManager, Mapping, Dict, Any, \
+    Callable
+
+from mtap._document import Document
+from mtap._event import Event
+from mtap._label_adapters import ProtoLabelAdapter
+from mtap.descriptors import ProcessorDescriptor
 
 
 class ProcessorContext:
     __slots__ = ('times',)
 
     def __init__(self):
         self.times = {}
@@ -117,17 +107,27 @@
 processor_local = threading.local()
 
 
 class Processor:
     """Mixin used by all processor abstract base classes that provides the
     ability to update serving status and use timers.
     """
-    __slots__ = ('_health_callback')
+    __slots__ = ('_health_callback',)
+
+    descriptor: ClassVar[Optional['ProcessorDescriptor']] = None
+
+    _health_callback: Callable[[str], None]
 
-    metadata = {}
+    @classmethod
+    def metadata(cls) -> Dict[str, Any]:
+        if cls.descriptor is None:
+            return {
+                'name': cls.__name__.casefold()
+            }
+        return asdict(cls.descriptor)
 
     def update_serving_status(self, status: str):
         """Updates the serving status of the processor for health checking.
 
         Args:
             status (str): One of "SERVING", "NOT_SERVING", "UNKNOWN".
         """
@@ -183,18 +183,19 @@
             >>>         # work you do want timed
             >>>         ...
             >>>         stopwatch.stop()
         """
         return Stopwatch(key, getattr(processor_local, 'context', None))
 
     @staticmethod
-    @contextlib.contextmanager
+    @contextmanager
     def enter_context() -> ContextManager[ProcessorContext]:
-        # Used by the MTAP framework to enter a processing context where things like timing
-        # results are stored. Users should not need to call this in normal usage.
+        # Used by the MTAP framework to enter a processing context where
+        # things like timing results are stored. Users should not need to
+        # call this in normal usage.
         try:
             old_context = processor_local.context
         except AttributeError:
             old_context = None
         try:
             processor_local.context = ProcessorContext()
             yield processor_local.context
@@ -212,28 +213,28 @@
         ...     def process(self, event, params):
         ...          # do work on the event
         ...          ...
     """
     __slots__ = ()
 
     @property
-    def custom_label_adapters(self) -> 'Mapping[str, ProtoLabelAdapter]':
+    def custom_label_adapters(self) -> Mapping[str, ProtoLabelAdapter]:
         """Optional method used to provide non-standard proto label adapters
         for specific index names. Default implementation returns an empty
         dictionary.
 
         Returns:
             A mapping from strings to label adapters.
         """
         return {}
 
     @abstractmethod
     def process(
             self,
-            event: 'Event',
+            event: Event,
             params: Dict[str, Any]
     ) -> Optional[Dict[str, Any]]:
         """Performs processing on an event, implemented by the subclass.
 
         Parameters:
             event: The event object to be processed.
             params: Processing parameters. A dictionary of strings mapped to
@@ -294,46 +295,7 @@
         up. Will be called by the framework after it's done with the processor.
         """
         pass
 
     def process(self, event, params):
         document = event.documents[params['document_name']]
         return self.process_document(document, params)
-
-
-class ProcessingComponent(ABC):
-    __slots__ = ()
-
-    metadata = {}
-
-    @property
-    @abstractmethod
-    def processor_name(self) -> str:
-        ...
-
-    @property
-    @abstractmethod
-    def component_id(self) -> str:
-        ...
-
-    @abstractmethod
-    def call_process(
-            self,
-            event_id: str,
-            event_instance_id: str,
-            params: Optional[Dict[str, Any]]
-    ) -> Tuple[Dict, Dict, Dict]:
-        """Calls a processor.
-
-        Parameters
-            event_id: The event to process.
-            event_instance_id: The service instance the event is stored on.
-            params: The processor parameters.
-
-        Returns
-            A tuple of the processing result dictionary, the processor times
-            dictionary, and the "created indices" dictionary.
-        """
-        ...
-
-    def close(self):
-        ...
```

### Comparing `mtap-1.2.0/python/mtap/processing/_error_handling.py` & `mtap-1.2.1/python/mtap/pipeline/_error_handling.py`

 * *Files 21% similar despite different names*

```diff
@@ -54,125 +54,37 @@
     params:
       max_failures: 0
   components:
     ...
 
 New error handlers can be registered to be loaded in this fashion using
 :meth:`~mtap.processing.ErrorHandlerRegistry.register`
-
 """
-import abc
 import dataclasses
 import logging
 import os.path
-import traceback
-from enum import Enum, auto
+from abc import abstractmethod, ABCMeta
 from os import PathLike
 from typing import (
     Any,
-    TYPE_CHECKING,
     Callable,
     Dict,
     Optional,
     Union,
-    List
+    Type,
+    ClassVar
 )
 
-import grpc
-from google.rpc import error_details_pb2, status_pb2
-from grpc_status import rpc_status
-
-if TYPE_CHECKING:
-    import mtap
-    from mtap import Event
-    from mtap.serialization import Serializer
+from mtap._event import Event
+from mtap.processing import ErrorInfo
+from mtap.serialization import Serializer, SerializerRegistry
 
 LOGGER = logging.getLogger('mtap.processing')
 
-
-class ProcessingException(Exception):
-    """An exception that occurred in a processing component.
-
-    Attributes
-        error_info (ErrorInfo): Information about the error.
-
-    """
-
-    def __init__(self, error_info: 'ErrorInfo'):
-        self.error_info = error_info
-
-    def to_rpc_status(self):
-        info = self.error_info
-        status = status_pb2.Status()
-        status.code = grpc.StatusCode.UNKNOWN.value[0]
-
-        error_info = error_details_pb2.ErrorInfo()
-        error_info.reason = "PROCESSING_FAILURE"
-        error_info.domain = "mtap.nlpie.umn.edu"
-        error_info.metadata['lang'] = info.lang
-        error_info.metadata['errorType'] = info.error_type
-        error_info.metadata['errorRepr'] = info.error_repr
-        error_info_any = status.details.add()
-        error_info_any.Pack(error_info)
-
-        debug_info = error_details_pb2.DebugInfo()
-        debug_info.stack_entries.extend(info.stack_trace)
-        debug_info_any = status.details.add()
-        debug_info_any.Pack(debug_info)
-
-        localized_message = error_details_pb2.LocalizedMessage()
-        localized_message.locale = info.locale
-        localized_message.message = info.localized_msg
-        localized_message_any = status.details.add()
-        localized_message_any.Pack(localized_message)
-        return status
-
-    @staticmethod
-    def from_local_exception(exc, component_id, message=None):
-        error_info = ErrorInfo(
-            origin=ErrorOrigin.LOCAL,
-            component_id=component_id,
-            lang='python',
-            error_type=str(type(exc)),
-            error_repr=repr(exc),
-            localized_msg=message or "An internal error occurred while "
-                                     "attempting to process an Event. "
-                                     "This is potentially a bug, contact the "
-                                     "developer of the component.",
-            locale="en-US",
-            stack_trace=list(traceback.format_exception(exc))
-        )
-        return ProcessingException(error_info)
-
-    @staticmethod
-    def from_rpc_error(rpc_error, component_id, address):
-
-        status = rpc_status.from_call(rpc_error)
-        if status is None:
-            return ProcessingException.from_local_exception(rpc_error,
-                                                            component_id)
-        info = error_details_pb2.ErrorInfo()
-        debug_info = error_details_pb2.DebugInfo()
-        localized_message = error_details_pb2.LocalizedMessage()
-        for detail in status.details:
-            for target in [info, debug_info, localized_message]:
-                if detail.Is(target.DESCRIPTOR):
-                    detail.Unpack(target)
-        error_info = ErrorInfo(
-            origin=ErrorOrigin.REMOTE,
-            component_id=component_id,
-            lang=info.metadata['lang'],
-            error_type=info.metadata['errorType'],
-            error_repr=info.metadata['errorRepr'],
-            localized_msg=localized_message.message,
-            locale=localized_message.locale,
-            stack_trace=list(debug_info.stack_entries),
-            address=address,
-        )
-        return ProcessingException(error_info)
+ErrorHandlerFactory = Callable[..., 'ProcessingErrorHandler']
 
 
 class StopProcessing(Exception):
     """Thrown by error handlers when the pipeline should immediately
     terminate."""
     pass
 
@@ -180,60 +92,67 @@
 class SuppressError(Exception):
     """Thrown by error handlers when the error should be suppressed
     and not handled by any downstream error handlers (later in the pipeline's
     list of error handlers) ."""
     pass
 
 
-class ErrorOrigin(Enum):
-    """Where the error occurred.
+class ErrorHandlerRegistry(ABCMeta):
+    """Registry for error handlers so that they can be instantiated from
+    configuration.
+
+    Classes implementing :class:`ProcessingErrorHandler` will automatically
+    be added by their name but can override that by overriding the
+    :meth:`mtap.pipeline.ProcessingErrorHandler.name` method.
     """
-    #: Error occurred locally to this process.
-    LOCAL = auto()
-    #: Error occurred on a remote component.
-    REMOTE = auto()
+    registry: ClassVar[Dict[str, ErrorHandlerFactory]] = {}
+
+    def __init__(cls: Type['ProcessingErrorHandler'], *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        ErrorHandlerRegistry.registry[cls.name()] = cls
 
+    @staticmethod
+    def from_dict(conf: Optional[Dict[str, Any]]) -> 'ProcessingErrorHandler':
+        """Creates an error handler from its dictionary representation.
 
-@dataclasses.dataclass
-class ErrorInfo:
-    """Information about an error.
+        Args:
+            conf: The dictionary representation of the error handler.
 
-    Attributes:
-        origin: The source of the error.
-        component_id: The id of the processing component that
-            the error occurred in.
-        lang: What language did the error occur in?
-        error_type: The type of the error.
-        error_repr: The string representation of the error.
-        localized_msg: A localized, user-friendly message.
-        locale: The locale of the message.
-        stack_trace: The stack trace of the message.
-        address: The remote address.
-    """
-    origin: 'mtap.processing.ErrorOrigin'
-    component_id: str
-    lang: str
-    error_type: str
-    error_repr: str
-    localized_msg: str
-    locale: str
-    stack_trace: List[str]
-    address: Optional[str] = None
+        Returns:
+            The instantiated error handler.
+
+        """
+        return ErrorHandlerRegistry.registry[conf['name']](
+            **conf.get('params', {})
+        )
 
 
-class ProcessingErrorHandler(abc.ABC):
+class ProcessingErrorHandler(metaclass=ErrorHandlerRegistry):
     """Base class for an error handler that is included in a pipeline to
     report and decide action for errors / exceptions that occur during
-    processing."""
+    processing.
 
-    @abc.abstractmethod
+    Note that you should not store any state on the error handler since it may
+    be reused across multiple runs of the same pipeline, instead store stateful
+    information in the state dictionary.
+    """
+
+    @classmethod
+    def name(cls):
+        """Optional method that returns the name the error handler should be
+        loaded into the registry with, by default will just use the full path
+        name.
+        """
+        return '.'.join([cls.__module__, cls.__name__])
+
+    @abstractmethod
     def handle_error(
             self,
-            event: 'Event',
-            error_info: 'ErrorInfo',
+            event: Event,
+            error_info: ErrorInfo,
             state: Dict[Any, Any]
     ):
         """Handles an error that was caught by processing logic and
         transformed into a :class:`~mtap.processing.ProcessingException`.
 
         Args:
             event:
@@ -249,102 +168,33 @@
             StopProcessing: if the pipeline should immediately stop processing.
             SuppressError: if the error should be suppressed and not passed to
                 any downstream error handlers (later in the pipeline's list of
                 error handlers).
         """
         raise NotImplementedError()
 
-    @abc.abstractmethod
-    def handle_exception(
-            self,
-            event: 'Event',
-            exc: 'Exception',
-            state: Dict[Any, Any]
-    ):
-        """Handles an exception that was not caught by the processing logic,
-        for example one that occurred in the MTAP pipeline or component logic.
-
-        Args:
-            event:
-                The event that was being processed when the exception was
-                thrown.
-            exc: The exception thrown.
-            state:
-                A dictionary that is preserved in-between calls to the
-                error handler that the handler can use to store state local
-                to the current run of processing.
-
-        Raises:
-            StopProcessing: The pipeline should immediately stop processing.
-            SuppressError: The error should be suppressed and not passed to
-                any downstream error handlers (later in the pipeline's list of
-                error handlers).
-        """
-        raise NotImplementedError()
-
 
-ErrorHandlerFactory = Callable[[Dict[str, Any]], ProcessingErrorHandler]
-
-registry: Dict[str, ErrorHandlerFactory] = {}
-
-
-class ErrorHandlerRegistry:
-    """Registry for error handlers so that they can be instantiated from
-    configuration.
-    """
-
-    @staticmethod
-    def register(
-            name: str
-    ) -> Callable[[ErrorHandlerFactory], ErrorHandlerFactory]:
-        """Registers an error handler.
-
-        Args:
-            name: The unique identifier
-
-        Returns:
-            A decorator that adds the factory to the registry.
-
-        """
-        def decorate(f: ErrorHandlerFactory) -> ErrorHandlerFactory:
-            if name in registry:
-                raise ValueError('Duplicate name for ErrorHandler: ' + name)
-            registry[name] = f
-            return f
-
-        return decorate
-
-    @staticmethod
-    def from_dict(conf: Optional[Dict[str, Any]]) -> ProcessingErrorHandler:
-        """Creates an error handler from its dictionary representation.
-
-        Args:
-            conf: The dictionary representation of the error handler.
-
-        Returns:
-            The instantiated error handler.
-
-        """
-        return registry[conf['name']](**conf.get('params', {}))
-
-
-@ErrorHandlerRegistry.register('simple')
 class SimpleErrorHandler(ProcessingErrorHandler):
     """Prints a simple helpful explanation of the error info.
     """
 
     def __init__(self, more_help: Optional[str] = None):
         #: Additional help to be printed after every error.
         self.more_help: str = (
                 more_help or
                 "Check the configuration settings to enable enhanced "
                 "debug behavior."
         )
 
+    @classmethod
+    def name(cls):
+        return 'simple'
+
     def handle_error(self, event, error_info, state):
+        from mtap.processing import ErrorOrigin
         if error_info.origin == ErrorOrigin.REMOTE:
             print(
                 f"An error occurred while processing an event with id "
                 f"'{event.event_id}' through the remote component "
                 f"'{error_info.component_id}' at address "
                 f"'{error_info.address}': {error_info.error_repr}\n"
                 f"It had the following message: {error_info.localized_msg}\n"
@@ -353,55 +203,45 @@
             print(
                 f"An error occurred while processing an event with id "
                 f"'{event.event_id}' through the component "
                 f"'{error_info.component_id}': '{error_info.error_repr}'\n"
                 f"It had the following message: {error_info.localized_msg}\n"
                 f"{self.more_help}")
 
-    def handle_exception(self, event, exc, state):
-        print(
-            f"An error occurred while processing an event with id "
-            f"'{event.event_id}': '{repr(exc)}'\n"
-            f"{self.more_help}")
-
 
-@ErrorHandlerRegistry.register('termination')
 class TerminationErrorHandler(ProcessingErrorHandler):
     """Terminates the pipeline after more than :attr:`max_failures`
     number of errors occurs.
 
     Attributes:
         max_failures: The maximum number of errors to allow before
             immediately terminating the pipeline.
 
     """
     max_failures: int
 
     def __init__(self, max_failures: int = 0):
         self.max_failures = max_failures
 
-    def _increment_and_check(self, state):
+    @classmethod
+    def name(cls):
+        return 'termination'
+
+    def handle_error(self, _1, _2, state):
         try:
             state['failures'] += 1
         except KeyError:
             state['failures'] = 1
         if state['failures'] >= self.max_failures:
             print(f"Pipeline exceeded the maximum number "
                   f"of allowed failures ({self.max_failures}) "
                   f"and is terminating.")
             raise StopProcessing()
 
-    def handle_error(self, _1, _2, state):
-        self._increment_and_check(state)
-
-    def handle_exception(self, _1, _2, state):
-        self._increment_and_check(state)
-
 
-@ErrorHandlerRegistry.register('logging')
 class LoggingErrorHandler(ProcessingErrorHandler):
     """Logs errors to a specified :class:`logging.Logger` object.
 
     Args:
         logger: Either the logger itself, the logger name, or none to use
             ``mtap.processing``.
 
@@ -412,93 +252,71 @@
     logger: logging.Logger
 
     def __init__(self, logger: Union[str, logging.Logger, None] = None):
         if isinstance(logger, str):
             logger = logging.getLogger(logger)
         self.logger = (logger or logging.getLogger('mtap.processing'))
 
+    @classmethod
+    def name(cls):
+        return 'logging'
+
     def handle_error(self, event, error_info, state):
         self.logger.error(
             f"An error occurred while processing an event with id "
             f"'{event.event_id}' through the remote component "
             f"'{error_info.component_id}' at address "
             f"'{error_info.address}': {error_info.error_repr}\n"
             f"It had the following message: {error_info.localized_msg}\n"
             + ''.join(error_info.stack_trace)
         )
 
-    def handle_exception(self, event, exc, state):
-        self.logger.error(
-            f"An error occurred while processing an event with id "
-            f"'{event.event_id}': {exc}\n"
-            + ''.join(traceback.format_exception(exc))
-        )
 
-
-@ErrorHandlerRegistry.register('directory')
 class ErrorsDirectoryErrorHandler(ProcessingErrorHandler):
-    """Built-in Error Handler which handles failures in pipeline processing by 
+    """Built-in Error Handler which handles failures in pipeline processing by
     writing files containing the error info, stack trace, and serialized event.
 
     Args:
         serializer: Either a serializer, a configuration dictionary that can
             be used to instantiate a serializer, or ``None`` to use the
             default json serializer.
 
     Attributes:
         output_directory: The directory to write the files to.
         serializer: The serializer to use to serialize the event.
 
     """
     output_directory: Union[str, bytes, PathLike]
-    serializer: 'Serializer'
+    serializer: Serializer
 
     def __init__(self,
-                 output_directory: 'Union[str, bytes, PathLike]',
-                 serializer: 'Union[Serializer, Dict[str, Any], None]' = None):
+                 output_directory: Union[str, bytes, PathLike],
+                 serializer: Union[Serializer, str, None] = None):
         self.output_directory = output_directory
         if serializer is None:
-            from mtap.serialization import SerializerRegistry
-            serializer = SerializerRegistry.create('json')
+            serializer = SerializerRegistry.get('json')
         if not isinstance(serializer, Serializer):
-            from mtap.serialization import SerializerRegistry
-            serializer = SerializerRegistry.from_dict(serializer)
+            serializer = SerializerRegistry.get(serializer)
         self.serializer = serializer
 
-    def _write_out(self, event, error_info):
+    @classmethod
+    def name(cls):
+        return 'to_directory'
+
+    def handle_error(self, event, error_info, _):
         d = os.path.join(self.output_directory, event.event_id)
         os.makedirs(d, exist_ok=True)
         print(f"Writing error information to: "
               f"'{os.path.abspath(os.fspath(d))}'")
         import json
         with open(os.path.join(d, 'info.json'), 'w') as f:
             json.dump(dataclasses.asdict(error_info), f, default=str)
-        ser_path = os.path.join(d, 'event' + self.serializer.extension)
+        ser_path = os.path.join(d, 'event' + self.serializer.extension())
         self.serializer.event_to_file(event, ser_path)
         with open(os.path.join(d, 'trace.txt'), 'w') as f:
             for line in error_info.stack_trace:
                 f.write(line)  # The lines already have builtin line breaks
 
-    def handle_error(self, event, error_info, _):
-        self._write_out(event, error_info)
-
-    def handle_exception(self, event, exc, _):
-        error_info = ErrorInfo(
-            ErrorOrigin.LOCAL,
-            'pipeline',
-            'python',
-            str(type(exc)),
-            repr(exc),
-            'en-US',
-            'An exception occurred in the pipeline.',
-            traceback.format_exception(exc),
-        )
-        self._write_out(event, error_info)
 
-
-@ErrorHandlerRegistry.register('suppress')
 class SuppressAllErrorsHandler(ProcessingErrorHandler):
     def handle_error(self, *_args, **_kwargs):
         raise SuppressError()
-
-    def handle_exception(self, *_args, **_kwargs):
-        raise SuppressError()
```

### Comparing `mtap-1.2.0/python/mtap/processing/_exc.py` & `mtap-1.2.1/python/tests/processing/test_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,29 @@
-# Copyright 2023 Regents of the University of Minnesota.
+#  Copyright 2020 Regents of the University of Minnesota.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
 #
-#     http://www.apache.org/licenses/LICENSE-2.0
+#      http://www.apache.org/licenses/LICENSE-2.0
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+from datetime import timedelta
 
-class ProcessingError(Exception):
-    """Exception for when processing results in a failure."""
-    pass
+from mtap.processing import Processor
+
+
+def test_stopwatch_no_fail_outside_context():
+    with Processor.started_stopwatch('foo'):
+        blah = True
+    assert blah
+
+
+def test_preserves_times():
+    with Processor.enter_context() as context:
+        context.add_time("foo", timedelta(seconds=2))
+        context.add_time("foo", timedelta(seconds=2))
+        assert context.times["foo"] == timedelta(seconds=4)
```

### Comparing `mtap-1.2.0/python/mtap/processing/_mp_config.py` & `mtap-1.2.1/python/mtap/pipeline/_mp_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     show_progress: bool = False
     """Whether progress should be displayed in the console."""
 
     params: Dict[str, Any] = field(default_factory=dict)
 
     workers: int = 10
-    """Number of workers to concurrently process events through the 
+    """Number of workers to concurrently process events through the
     pipeline."""
 
     read_ahead: int = 10
     """The number of documents to read onto the events service(s) to
     queue for processing."""
 
     close_events: bool = False
@@ -42,17 +42,17 @@
     log_level: str = 'INFO'
     """"""
 
     mp_start_method: str = "spawn"
     """The start method for multiprocessing processes see:
     :meth:`multiprocessing.get_context`."""
 
-    mp_context: 'Optional[multiprocessing]' = None
-    """An optional mp_context. If set overrides the ``mp_start_method`` 
-    attribute. If not set will use 
+    mp_context: Optional['multiprocessing'] = None
+    """An optional mp_context. If set overrides the ``mp_start_method``
+    attribute. If not set will use
     ``multiprocessing.get_context(mp_start_method)``
     to create the context.
     """
 
     @staticmethod
     def from_configuration(conf: Dict) -> 'MpConfig':
         return MpConfig(**conf)
```

### Comparing `mtap-1.2.0/python/mtap/processing/_mp_pipeline.py` & `mtap-1.2.1/python/mtap/pipeline/_mp_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,38 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 import logging
 import multiprocessing
 import signal
 import traceback
 from logging.handlers import QueueListener
 from threading import Condition, Lock
 from typing import Optional, TYPE_CHECKING
 
+from grpc import RpcError
 from tqdm import tqdm
 
-from mtap import Config
-from mtap.processing import _pipeline_results
-from mtap.processing._error_handling import (
+from mtap._config import Config
+from mtap.pipeline._common import event_and_params
+from mtap.pipeline._error_handling import StopProcessing, SuppressError
+from mtap.pipeline._sources import ProcessingSource, IterableProcessingSource
+from mtap.processing import (
     ProcessingException,
-    SuppressError,
-    StopProcessing,
-)
-from mtap.processing._pipeline import (
-    event_and_params,
-    ProcessingSourceLike, ActivePipeline
-)
-from mtap.processing._sources import (
-    ProcessingSource,
-    IterableProcessingSource
 )
 
 if TYPE_CHECKING:
-    from mtap import Pipeline
-    from mtap.processing import BatchPipelineResult
+    from mtap.pipeline._pipeline import ActivePipeline
+
 
-_mp_pipeline: Optional[ActivePipeline] = None
+_mp_pipeline: Optional['ActivePipeline'] = None
 
 
 def _mp_process_init(config, pipeline, queue, log_level):
     global _mp_pipeline
 
     # set up multiprocess logging via queue back to listener
     h = logging.handlers.QueueHandler(queue)
@@ -77,32 +69,32 @@
         return event_id, None, e.error_info
     except Exception as e:
         ei = ProcessingException.from_local_exception(e, 'pipeline').error_info
         return event_id, None, ei
     return event_id, result, None
 
 
-class ActiveRun:
+class ActiveMpRun:
     __slots__ = (
         'pipeline',
         'config',
         'targets_cond',
         'active_targets',
         'progress_bar',
         'source',
         'pool',
         'active_events',
         'log_listener',
-        'stop'
+        'stop',
+        'times',
+        'handler_states',
+        'callback'
     )
 
-    def __init__(self,
-                 pipeline: 'Pipeline',
-                 source: 'ProcessingSourceLike',
-                 total: Optional[int] = None):
+    def __init__(self, pipeline, source, total=None, callback=None):
         self.pipeline = pipeline
         self.config = pipeline.mp_config
         self.targets_cond = Condition(Lock())
         total = (source.total if hasattr(source, 'total') else None) or total
         self.progress_bar = tqdm(
             total=total,
             unit='events',
@@ -140,14 +132,17 @@
                 logging_queue,
                 self.config.log_level
             )
         )
         self.active_targets = 0
         self.active_events = {}
         self.stop = False
+        self.times = self.pipeline.create_times()
+        self.handler_states = [{} for _ in self.pipeline.error_handlers]
+        self.callback = callback
 
     @property
     def max_targets(self):
         return self.config.workers + self.config.read_ahead
 
     def increment_active_tasks(self):
         with self.targets_cond:
@@ -174,86 +169,73 @@
         with self.targets_cond:
             self.targets_cond.wait_for(self.read_ready)
 
     def stop_processing(self):
         self.stop = True
         self.pool.terminate()
 
-    def run(self) -> 'BatchPipelineResult':
-        br = _pipeline_results.BatchPipelineResult(
-            self.pipeline.name,
-            [component.component_id for component in self.pipeline]
-        )
-        error_handlers = copy.deepcopy(self.pipeline.error_handlers)
-        handler_states = [{} for _ in error_handlers]
-
-        def result_handler(result):
-            event_id, result, error = result
-            event = self.active_events[event_id]
-            if result is not None:
-                br.add_result_times(result)
-                self.source.receive_result(result, event)
-            else:
-                for handler, state in zip(error_handlers, handler_states):
-                    try:
-                        handler.handle_error(event, error, state)
-                    except StopProcessing:
-                        self.stop_processing()
-                    except SuppressError:
-                        break
-                    except Exception:
-                        print("An error handler raised an exception")
-                        traceback.print_exc()
-
-            self.task_completed()
-            if self.config.close_events:
-                event.release_lease()
-
-        def error_handler(error):
-            for handler, state in zip(error_handlers, handler_states):
+    def handle_result(self, result):
+        event_id, result, error = result
+        event = self.active_events[event_id]
+        if result is not None:
+            self.times.add_result_times(result)
+            if self.callback:
+                self.callback(result, event)
+        else:
+            for handler, state in zip(self.pipeline.error_handlers,
+                                      self.handler_states):
                 try:
-                    handler.handle_exception('unknown', error, state)
+                    handler.handle_error(event, error, state)
                 except StopProcessing:
                     self.stop_processing()
                 except SuppressError:
                     break
-                except Exception:
-                    print("An error handler raised an exception")
+                except Exception as e:
+                    print("An error handler raised an exception: ", e)
                     traceback.print_exc()
 
-        def consume(target):
-            if self.stop:
-                raise StopIteration
-            event, params = event_and_params(target, self.config.params)
+        self.task_completed()
+        if self.config.close_events:
+            event.release_lease()
+        self.active_events.pop(event_id)
+
+    def consume(self, target):
+        if self.stop:
+            raise StopIteration
+        event, params = event_and_params(target, self.config.params)
+        try:
+            event.lease()
+            event_id = event.event_id
+            self.active_events[event_id] = event
+            self.pool.apply_async(_mp_process_event,
+                                  args=(event_id,
+                                        event.event_service_instance_id,
+                                        params),
+                                  callback=self.handle_result)
+            self.increment_active_tasks()
+        except BaseException as e:
+            # here we failed (or exited) sometime between taking a new
+            # lease and adding the done callback to the future,
+            # meaning the lease will never get freed.
             try:
-                event.lease()
-                event_id = event.event_id
-                self.active_events[event_id] = event
-                self.pool.apply_async(_mp_process_event,
-                                      args=(event_id,
-                                            event.event_service_instance_id,
-                                            params),
-                                      callback=result_handler,
-                                      error_callback=error_handler)
-                self.increment_active_tasks()
-            except BaseException as e:
-                # here we failed sometime between taking a new lease and adding
-                # the done callback to the future, meaning the lease will never
-                # get freed.
                 event.release_lease()
-                raise e
-            self.wait_to_read()
+            except RpcError:
+                # Client might already be closed, we tried our best
+                pass
+            raise e
+        self.wait_to_read()
 
+    def run(self):
         try:
             with self.source:
-                self.source.provide(consume)
+                self.source.produce(self.consume)
             self.wait_tasks_completed()
         except KeyboardInterrupt:
             print('Pipeline terminated by user (KeyboardInterrupt).')
-        return br
+        return self.times
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `mtap-1.2.0/python/mtap/processing/_pipeline.py` & `mtap-1.2.1/python/mtap/pipeline/_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,147 +21,119 @@
 from os import PathLike
 from typing import (
     Optional,
     Dict,
     Any,
     Union,
     List,
-    TYPE_CHECKING, MutableSequence,
+    MutableSequence,
+    Iterable,
 )
 
-from mtap.data import Event, EventsAddressLike
-from mtap.processing import _pipeline_components
-from mtap.processing import (
-    _pipeline_results,
-    _mp_config,
-)
-from mtap.processing._error_handling import (
+from mtap._events_client import EventsAddressLike
+from mtap.pipeline._common import EventLike, event_and_params
+from mtap.pipeline._error_handling import (
+    ErrorHandlerRegistry,
+    ProcessingErrorHandler,
     SimpleErrorHandler,
     TerminationErrorHandler,
-    ErrorHandlerRegistry
 )
-
-if TYPE_CHECKING:
-    from mtap import (
-        Document,
-        Event,
-    )
-    from mtap.processing import (
-        MpConfig,
-        ProcessingErrorHandler,
-        PipelineResult,
-        ProcessingComponent,
-        BatchPipelineResult,
-        ComponentDescriptor,
-    )
+from mtap.pipeline._mp_config import MpConfig
+from mtap.pipeline._pipeline_components import (
+    RemoteProcessor,
+    ComponentDescriptor,
+)
+from mtap.pipeline._results import (
+    PipelineResult,
+    PipelineTimes,
+    PipelineCallback,
+)
+from mtap.pipeline._sources import ProcessingSource
+from mtap.processing import ProcessingComponent
+from mtap.processing.results import ComponentResult
 
 logger = logging.getLogger('mtap.processing')
 
-ProcessingSourceLike = "Union[Iterable[Union[Document, Event]], " \
-                       "ProcessingSource]"
-
-
-def event_and_params(target, params):
-    try:
-        document_name = target.document_name
-        params = dict(params or {})
-        params['document_name'] = document_name
-        event = target.event
-    except AttributeError:
-        event = target
-    return event, params
+ProcessingSourceLike = Union[Iterable[EventLike], ProcessingSource]
 
 
 def _cancel_callback(event, read_ahead, cd, close_events):
     def fn(future: Future):
         if close_events:
             event.close()
         read_ahead.task_completed()
         cd.count_down(future.exception() is not None)
 
     return fn
 
 
-def _create_pipeline(name: Optional[str] = None,
-                     mp_config: 'Optional[MpConfig]' = None,
-                     error_handlers: 'Optional[ProcessingErrorHandler]' = None,
-                     *components: 'ComponentDescriptor'):
-    pipeline = Pipeline(*components)
-    pipeline.name = name
-    pipeline.mp_config = mp_config
-    pipeline.error_handlers = error_handlers
-    return pipeline
-
-
 class ActivePipeline:
     __slots__ = (
         'components'
     )
 
-    components: 'List[ProcessingComponent]'
+    components: List[ProcessingComponent]
 
-    def __init__(self, components: 'List[ProcessingComponent]'):
+    def __init__(self, components: List[ProcessingComponent]):
         self.components = components
 
     def run_by_event_id(
             self,
             event_id: str,
             event_service_instance_id: str,
             params: Dict[str, Any]
     ) -> 'PipelineResult':
         start = datetime.now()
         results = []
         for component in self.components:
             d, ti, ci = component.call_process(event_id,
                                                event_service_instance_id,
                                                params)
-            pr = _pipeline_results.ComponentResult(
+            pr = ComponentResult(
                 identifier=component.component_id,
                 result_dict=d,
                 timing_info=ti,
                 created_indices=ci
             )
             results.append(pr)
 
         total = datetime.now() - start
         logger.debug('Finished processing event_id: %s', event_id)
-        return _pipeline_results.PipelineResult(results, total)
+        return PipelineResult(results, total)
 
     def run(
             self,
-            target: 'Union[Event, Document]',
+            target: EventLike,
             *, params: Optional[Dict[str, Any]] = None
-    ) -> 'PipelineResult':
+    ) -> PipelineResult:
         event, params = event_and_params(target, params)
         event_id = event.event_id
 
-        return self.run_by_event_id(event_id,
-                                    event.event_service_instance_id,
-                                    params)
+        return self.run_by_event_id(
+            event_id,
+            event.event_service_instance_id,
+            params
+        )
 
 
-class Pipeline(
-    list,
-    MutableSequence[_pipeline_components.ComponentDescriptor]
-):
+class Pipeline(list, MutableSequence[ComponentDescriptor]):
     """An object which can be used to build and run a pipeline of remote and
     local processors.
 
     Pipelines are a :obj:`~typing.MutableSequence` containing
     one or more :class:`~mtap.processing.ComponentDescriptor`,
     a pipeline can be modified after creation using this functionality.
 
     Args:
         *components: Component descriptors created using
             :class:`RemoteProcessor` or :class:`LocalProcessor`.
-        mp_config: Optional multiprocessing configuration for the pipeline.
 
     Attributes:
         name: The pipeline's name.
-        events_address: The events address.
+        events_address: Optional events address.
         mp_config: The multiprocessing configuration for the pipeline.
         error_handlers: The error handlers to use when running the pipeline.
 
     Examples:
         Remote pipeline with name discovery:
 
         >>> pipeline = Pipeline(RemoteProcessor('processor-1-id'),
@@ -196,40 +168,51 @@
         'mp_config',
         'error_handlers',
         '_provided_events_client',
     )
 
     name: str
     events_address: EventsAddressLike
-    mp_config: 'MpConfig'
-    error_handlers: 'List[ProcessingErrorHandler]'
+    mp_config: MpConfig
+    error_handlers: List[ProcessingErrorHandler]
 
     def __init__(self,
-                 *components: 'ComponentDescriptor',
+                 *components: ComponentDescriptor,
                  name: Optional[str] = None,
                  events_address: EventsAddressLike = None,
-                 mp_config: 'Optional[MpConfig]' = None,
-                 error_handlers: 'List[ProcessingErrorHandler]' = None):
+                 mp_config: Optional[MpConfig] = None,
+                 error_handlers: List[ProcessingErrorHandler] = None):
         super().__init__(components)
         self.name = name or 'pipeline'
         self.events_address = events_address
-        self.mp_config = mp_config or _mp_config.MpConfig()
+        self.mp_config = mp_config or MpConfig()
         self.error_handlers = error_handlers or [
             SimpleErrorHandler(),
             TerminationErrorHandler()
         ]
 
     def __reduce__(self):
         params = (
             self.name,
+            self.events_address,
             self.mp_config,
             self.error_handlers,
         )
-        params += tuple(self)
-        return _create_pipeline, params
+
+        return Pipeline._reconstruct, params, None, iter(self)
+
+    @staticmethod
+    def _reconstruct(name, events_address, mp_config, error_handlers):
+        pipeline = Pipeline(
+            name=name,
+            events_address=events_address,
+            mp_config=mp_config,
+            error_handlers=error_handlers
+        )
+        return pipeline
 
     @staticmethod
     def from_yaml_file(conf_path: Union[str, bytes, PathLike]) -> 'Pipeline':
         """Creates a pipeline from a yaml pipeline configuration file.
 
         Args:
             conf_path: The path to the configuration file.
@@ -288,101 +271,100 @@
                     "The 'processor_id' field has been renamed to 'name' "
                     "in pipeline configurations."
                     "For now it is automatically migrated, but it may fail "
                     "in a future version"
                 )
                 conf_component['name'] = conf_component['processor_id']
             components.append(
-                _pipeline_components.RemoteProcessor(
+                RemoteProcessor(
                     processor_name=conf_component['name'],
                     address=conf_component.get('address', None),
                     component_id=conf_component.get('component_id', None),
                     params=dict(conf_component.get('params', {}))
                 )
             )
         error_handlers = []
         conf_error_handlers = conf.get('error_handlers', [])
         for conf_error_handler in conf_error_handlers:
             handler = ErrorHandlerRegistry.from_dict(conf_error_handler)
             error_handlers.append(handler)
-        mp_config = _mp_config.MpConfig.from_configuration(
-            conf.get('mp_config', {})
+        mp_config = MpConfig.from_configuration(conf.get('mp_config', {}))
+        return Pipeline(
+            *components,
+            name=name,
+            mp_config=mp_config,
+            error_handlers=error_handlers,
+            events_address=events_address
         )
-        return Pipeline(*components, name=name, mp_config=mp_config,
-                        error_handlers=error_handlers)
 
     def run_multithread(
             self,
             source: ProcessingSourceLike,
             *, total: Optional[int] = None,
+            callback: Optional[PipelineCallback] = None,
             **kwargs,
-    ) -> 'BatchPipelineResult':
+    ) -> PipelineTimes:
         """Runs this pipeline on a source which provides multiple
         documents / events.
 
         Concurrency is per-event, with each event being provided a thread
         which runs it through the pipeline.
 
         Args:
             source: The processing source.
             total: Total documents in the processing source.
+            callback: A callback that receives events and their associated
+                results from the finished pipeline.
             kwargs: Override for any of the :class:`MpConfig` attributes.
 
         Examples:
             >>> docs = list(pathlib.Path('abc/').glob('*.txt'))
+            >>>
             >>> def document_source():
             >>>     for path in docs:
             >>>         with path.open('r') as f:
             >>>             txt = f.read()
-            >>>         with Event(event_id=path.name, client=pipeline.events_client) as event:
+            >>>         with Event(event_id=path.name,
+            >>>                    client=pipeline.events_client) as event:
             >>>             doc = event.create_document('plaintext', txt)
             >>>             yield doc
             >>>
             >>> pipeline.run_multithread(document_source(), total=len(docs))
-
         """
-        from mtap.processing._mp_pipeline import ActiveRun
+        from mtap.pipeline._mp_pipeline import ActiveMpRun
         pipeline = copy.deepcopy(self)
         mp = dataclasses.asdict(pipeline.mp_config)
         mp.update(kwargs)
-        pipeline.mp_config = _mp_config.MpConfig(**mp)
-        with ActiveRun(pipeline, source, total) as runner:
+        pipeline.mp_config = MpConfig(**mp)
+        with ActiveMpRun(pipeline, source, total, callback) as runner:
             result = runner.run()
         return result
 
     def run(
             self,
-            target: 'Union[Event, Document]',
+            target: EventLike,
             *, params: Optional[Dict[str, Any]] = None
-    ) -> 'PipelineResult':
+    ) -> PipelineResult:
         """Processes the event/document using all the processors in the
         pipeline.
 
         Args:
-            target (~typing.Union[Event, Document]):
-                Either an event or a document to process.
-            params (dict[str, ~typing.Any]):
-                Json object containing params specific to processing this
+            target: Either an event or a document to process.
+            params: Json object containing params specific to processing this
                 event, the existing params dictionary defined in
                 :func:`~PipelineBuilder.add_processor` will be updated with
                 the contents of this dict.
 
         Returns:
-            list[ProcessingResult]:
-                The results of all the processors in the pipeline.
+            The results of all the processors in the pipeline.
 
         Examples:
             >>> e = mtap.Event()
             >>> document = mtap.Document('plaintext', text="...", event=e)
-            >>> with Pipeline(...) as pipeline:
-            >>>     pipeline.run(document)
-
-            The 'document_name' param is used to indicate to
-            :obj:`~mtap.DocumentProcessor` which document on the event
-            to process.
+            >>> pipeline.run(document)
         """
         with self.activate() as active:
             return active.run(target, params=params)
 
     @contextmanager
     def activate(self) -> ActivePipeline:
         components = []
@@ -416,7 +398,24 @@
         super().append(item)
         self._check_for_duplicates(item)
 
     def extend(self, other):
         super().extend(other)
         for item in other:
             self._check_for_duplicates(item)
+
+    def create_times(self) -> PipelineTimes:
+        """Creates a timing object that can be used to store run times.
+
+        Returns:
+            A timing object.
+
+        Examples:
+
+        >>> times = pipeline.create_times()
+        >>> result = pipeline.run(document)
+        >>> times.add_result_times(result)
+        """
+        return PipelineTimes(
+            self.name,
+            [component.component_id for component in self]
+        )
```

### Comparing `mtap-1.2.0/python/mtap/processing/_pipeline_components.py` & `mtap-1.2.1/python/mtap/pipeline/_pipeline_components.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
-import typing
 from abc import ABC, abstractmethod
 from typing import Optional, Dict, Any
 
-from mtap.data import EventsAddressLike
-from mtap.processing import _runners
-
-if typing.TYPE_CHECKING:
-    from mtap import EventProcessor, processing
+from mtap._events_client import EventsAddressLike
+from mtap.processing import ProcessingComponent, EventProcessor, LocalRunner, \
+    RemoteRunner
 
 
 class ComponentDescriptor(ABC):
     """A configuration which describes either a local or remote pipeline
     component and what the pipeline needs to do to call the component.
     """
     __slots__ = ()
@@ -34,15 +31,15 @@
     def component_id(self) -> str:
         ...
 
     @abstractmethod
     def create_pipeline_component(
             self,
             events_address: EventsAddressLike
-    ) -> 'processing.ProcessingComponent':
+    ) -> ProcessingComponent:
         pass
 
 
 class LocalProcessor(ComponentDescriptor):
     """A configuration of a locally-invoked processor.
 
     Attributes:
@@ -52,42 +49,47 @@
             components in the pipeline.
         params: An optional parameter dictionary that will be passed to the
             processor as parameters with every event or document processed.
             Values should be json-serializable.
     """
     __slots__ = ('processor', 'component_id', 'params')
 
-    processor: 'EventProcessor'
+    processor: EventProcessor
     component_id: str
     params: Dict[str, Any]
 
     def __init__(self,
-                 processor: 'EventProcessor',
+                 processor: EventProcessor,
                  *, component_id: Optional[str] = None,
                  params: Optional[Dict[str, Any]] = None):
         self.processor = processor
-        self.component_id = component_id or self.processor.metadata['name']
+        self.component_id = component_id or self.processor.metadata()['name']
         self.params = params or {}
 
     def __reduce__(self):
         params = (
             self.processor,
             self.component_id,
             self.params
         )
-        return LocalProcessor, params
+        return LocalProcessor._reconstructor, params
+
+    @staticmethod
+    def _reconstructor(processor, component_id, params):
+        return LocalProcessor(processor, component_id=component_id,
+                              params=params)
 
     def create_pipeline_component(
             self,
             events_address: EventsAddressLike
-    ) -> 'processing.ProcessingComponent':
-        runner = _runners.LocalRunner(processor=self.processor,
-                                      events_address=events_address,
-                                      component_id=self.component_id,
-                                      params=copy.deepcopy(self.params))
+    ) -> ProcessingComponent:
+        runner = LocalRunner(processor=self.processor,
+                             events_address=events_address,
+                             component_id=self.component_id,
+                             params=copy.deepcopy(self.params))
         return runner
 
     def __repr__(self):
         return (f"LocalProcessor(proc={self.processor}, "
                 f"component_id={self.component_id}, "
                 f"params={self.params}")
 
@@ -132,23 +134,42 @@
                  enable_proxy: bool = False):
         self.processor_name = processor_name
         self.address = address
         self.component_id = component_id or self.processor_name
         self.params = params or {}
         self.enable_proxy = enable_proxy
 
+    def __reduce__(self):
+        params = (
+            self.processor_name,
+            self.address,
+            self.component_id,
+            self.params,
+            self.enable_proxy
+        )
+        return RemoteProcessor._reconstructor, params
+
+    @staticmethod
+    def _reconstructor(processor_name, address, component_id, params,
+                       enable_proxy):
+        return RemoteProcessor(processor_name=processor_name,
+                               address=address,
+                               component_id=component_id,
+                               params=params,
+                               enable_proxy=enable_proxy)
+
     def create_pipeline_component(
             self,
             events_address: EventsAddressLike
-    ) -> 'processing.ProcessingComponent':
-        runner = _runners.RemoteRunner(processor_name=self.processor_name,
-                                       component_id=self.component_id,
-                                       address=self.address,
-                                       params=copy.deepcopy(self.params),
-                                       enable_proxy=self.enable_proxy)
+    ) -> ProcessingComponent:
+        runner = RemoteRunner(processor_name=self.processor_name,
+                              component_id=self.component_id,
+                              address=self.address,
+                              params=copy.deepcopy(self.params),
+                              enable_proxy=self.enable_proxy)
         return runner
 
     def __repr__(self):
         return (f"RemoteProcessor(processor_name={self.processor_name}, "
                 f"address={self.address}, "
                 f"component_id={self.component_id}, "
                 f"params={self.params})")
```

### Comparing `mtap-1.2.0/python/mtap/processing/_runners.py` & `mtap-1.2.1/python/mtap/processing/_runners.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import logging
-from typing import Optional, Dict, Any, TYPE_CHECKING
+from typing import Optional, Dict, Any
 
 import grpc
+from grpc import insecure_channel
 
-from mtap import _structs, Config
-from mtap import data
-from mtap.api.v1 import processing_pb2, processing_pb2_grpc
-from mtap.data import FailedToConnectToEventsServiceException
-from mtap.processing._base import ProcessingComponent, Processor
-from mtap.processing._error_handling import ProcessingException
-
-if TYPE_CHECKING:
-    from mtap import EventProcessor, EventsClient
-    from mtap.data import EventsAddressLike
+from mtap import Config
+from mtap._event import Event
+from mtap._events_client import events_client, EventsAddressLike, EventsClient
+from mtap._structs import copy_dict_to_struct, copy_struct_to_dict
+from mtap.api.v1 import processing_pb2_grpc, processing_pb2
+from mtap.processing._exc import ProcessingException
+from mtap.processing._processing_component import ProcessingComponent
+from mtap.processing._processor import Processor, EventProcessor
 
 logger = logging.getLogger('mtap.processing')
 
 
 class LocalRunner(ProcessingComponent):
     __slots__ = (
         '_processor',
@@ -39,73 +38,69 @@
         '_component_id',
         '_params',
         'metadata',
         '_client'
     )
 
     def __init__(self,
-                 processor: 'EventProcessor',
-                 events_address: 'EventsAddressLike',
+                 processor: EventProcessor,
+                 events_address: EventsAddressLike,
                  component_id: Optional[str] = None,
                  params: Optional[Dict[str, Any]] = None):
         self._processor = processor
         self._events_address = events_address
-        self._processor_name = processor.metadata['name']
+        self._processor_name = processor.metadata()['name']
         self._component_id = component_id or self.processor_name
         self._params = params or {}
-        self.metadata = processor.metadata
+        self.metadata = processor.metadata()
         self._client = None
 
     @property
     def processor_name(self) -> str:
         return self._processor_name
 
     @property
     def component_id(self) -> str:
         return self._component_id
 
     @property
-    def _events_client(self) -> 'EventsClient':
+    def _events_client(self) -> EventsClient:
         if self._client is None:
-            self._client = data.EventsClient(self._events_address)
+            self._client = events_client(self._events_address)
         return self._client
 
     def call_process(self, event_id, event_instance_id, params):
         p = copy.deepcopy(self._params)
         if params is not None:
             p.update(params)
 
         with Processor.enter_context() as c, \
-                data.Event(
+                Event(
                     event_id=event_id,
                     event_service_instance_id=event_instance_id,
                     client=self._events_client,
                     label_adapters=self._processor.custom_label_adapters
                 ) as event:
             with Processor.started_stopwatch('process_method'):
                 try:
                     result = self._processor.process(event, p)
-                except FailedToConnectToEventsServiceException as e:
-                    raise ProcessingException.from_local_exception(
-                        e, self.component_id, e.msg
-                    )
                 except KeyError as e:
                     if e.args[0] == 'document_name':
                         raise ProcessingException.from_local_exception(
                             e, self.component_id,
                             "This error is likely caused by attempting "
                             "to run an event through a document processor. "
                             "Either call the pipeline with a document or "
                             "set the 'document_name' processor parameter."
-                        )
+                        ) from e
                     raise e
                 except Exception as e:
                     raise ProcessingException.from_local_exception(
                         e, self.component_id
-                    )
+                    ) from e
             return result, c.times, event.created_indices
 
     def close(self):
         if self._client is not None:
             self._client.close()
             self._client = None
 
@@ -139,15 +134,15 @@
                 = enable_proxy
         if address is None:
             from mtap.discovery import DiscoveryMechanism
             discovery = DiscoveryMechanism()
             address = discovery.discover_processor_service(processor_name,
                                                            'v1')
         channel_options = config.get('grpc.processor_options', {})
-        self._channel = grpc.insecure_channel(address, options=list(
+        self._channel = insecure_channel(address, options=list(
             channel_options.items()))
         self._stub = processing_pb2_grpc.ProcessorStub(self._channel)
 
     @property
     def processor_name(self) -> str:
         return self._processor_name
 
@@ -165,15 +160,15 @@
 
         with Processor.enter_context() as context:
             request = processing_pb2.ProcessRequest(
                 processor_id=self.processor_name,
                 event_id=event_id,
                 event_service_instance_id=event_instance_id
             )
-            _structs.copy_dict_to_struct(p, request.params, [p])
+            copy_dict_to_struct(p, request.params, [p])
             with Processor.started_stopwatch('remote_call'):
                 try:
                     response = self._stub.Process(
                         request,
                         metadata=[('service-name', self.processor_name)])
                 except grpc.RpcError as e:
                     if e.code() == grpc.StatusCode.UNAVAILABLE:
@@ -182,22 +177,22 @@
                             self.component_id,
                             "Failed to connect to processor service, check "
                             "that the service is running and the address is "
                             "correctly configured."
                         )
                     raise ProcessingException.from_rpc_error(
                         e, self.component_id, self._address
-                    )
+                    ) from e
                 except Exception as e:
                     raise ProcessingException.from_local_exception(
                         e, self.component_id
-                    )
+                    ) from e
 
             r = {}
-            _structs.copy_struct_to_dict(response.result, r)
+            copy_struct_to_dict(response.result, r)
 
             timing_info = response.timing_info
             for k, v in timing_info.items():
                 context.add_time(k, v.ToTimedelta())
 
             created_indices = {}
             for created_index in response.created_indices:
```

### Comparing `mtap-1.2.0/python/mtap/processing/_service.py` & `mtap-1.2.1/python/mtap/processing/_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,70 +9,68 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
 import logging
-import signal
 import threading
 import traceback
-import typing
 import uuid
 from concurrent.futures import thread
 from logging.handlers import QueueListener
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import grpc
 from grpc_health.v1 import health, health_pb2_grpc
 from grpc_status import rpc_status
 
-from mtap import _config, _structs, data, utilities
+from mtap import _config, _structs, utilities
+from mtap._common import run_server_forever
+from mtap._event import Event
 from mtap.api.v1 import processing_pb2, processing_pb2_grpc
-from mtap.processing import _base, _runners, _pipeline_results
-from mtap.processing._error_handling import ProcessingException
-
-if typing.TYPE_CHECKING:
-    import mtap
+from mtap.processing import _runners, Processor, EventProcessor
+from mtap.processing._exc import ProcessingException
+from mtap.processing._processing_component import ProcessingComponent
+from mtap.processing.results import add_times, create_timer_stats
 
 logger = logging.getLogger('mtap.processing')
 
 
-def run_processor(proc: 'mtap.EventProcessor',
+def run_processor(proc: EventProcessor,
                   *,
                   mp: bool = False,
                   options: Optional[argparse.Namespace] = None,
                   args: Optional[Sequence[str]] = None,
                   mp_context=None):
-    """Runs the processor as a GRPC service, blocking until an interrupt signal 
+    """Runs the processor as a GRPC service, blocking until an interrupt signal
     is received.
 
     Args:
         proc: The processor to host.
         mp: If true, will create instances of ``proc`` on multiple
-            forked processes to process events. This is useful if the processor 
-            is computationally intensive and would run into Python GIL issues 
+            forked processes to process events. This is useful if the processor
+            is computationally intensive and would run into Python GIL issues
             on a single process.
         options: The parsed arguments
             from the parser returned by :func:`processor_parser`.
         args: Arguments to parse
             server settings from if ``namespace`` was not supplied.
-        mp_context: A multiprocessing context that gets passed to the process 
+        mp_context: A multiprocessing context that gets passed to the process
             pool executor in the case of mp = True.
 
     Examples:
         Will automatically parse arguments:
 
         >>> run_processor(MyProcessor())
 
         Manual arguments:
 
         >>> run_processor(MyProcessor(), args=['-p', '8080'])
     """
-    from mtap import EventProcessor
     if not isinstance(proc, EventProcessor):
         print("Processor must be instance of EventProcessor class.")
         exit(1)
 
     if options is None:
         processors_parser = argparse.ArgumentParser(
             parents=[processor_parser()]
@@ -87,15 +85,15 @@
     if options.events_addresses is not None:
         events_addresses.extend(options.events_addresses.split(','))
 
     with _config.Config() as c:
         if options.mtap_config is not None:
             c.update_from_yaml(options.mtap_config)
         # instantiate runner
-        name = options.name or proc.metadata['name']
+        name = options.name or proc.metadata()['name']
         sid = options.sid
 
         enable_http_proxy = options.grpc_enable_http_proxy
         if enable_http_proxy is not None:
             c['grpc.events_channel_options.grpc.enable_http_proxy'] \
                 = enable_http_proxy
         if mp:
@@ -112,78 +110,68 @@
                                  sid=sid,
                                  host=options.host,
                                  port=options.port,
                                  register=options.register,
                                  workers=options.workers,
                                  write_address=options.write_address)
 
-        e = threading.Event()
-
-        def do_stop(*_):
-            e.set()
-
-        signal.signal(signal.SIGINT, do_stop)
-        signal.signal(signal.SIGTERM, do_stop)
-
-        server.start()
-        try:
-            e.wait()
-        except KeyboardInterrupt:
-            pass
-        server.stop()
+        run_server_forever(server)
 
 
 _mp_processor = ...  # EventProcessor
 _mp_client = ...  # EventClient
 
 
-def _mp_initialize(proc: 'mtap.EventProcessor',
+def _mp_initialize(proc: EventProcessor,
                    events_address,
                    config,
                    log_queue):
     global _mp_processor
     global _mp_client
 
     h = logging.handlers.QueueHandler(log_queue)
     root = logging.getLogger()
     root.addHandler(h)
     root.setLevel(logging.DEBUG)
 
     _config.Config(config)
     _mp_processor = proc
-    _mp_client = data.EventsClient(address=events_address)
+    from mtap import events_client
+    _mp_client = events_client(address=events_address)
 
 
 def _mp_call_process(event_id, event_service_instance_id, params):
     global _mp_processor
     global _mp_client
-    with _base.Processor.enter_context() as c, \
-            data.Event(event_id=event_id,
-                       event_service_instance_id=event_service_instance_id,
-                       client=_mp_client) as event:
-        with _base.Processor.started_stopwatch('process_method'):
+    with Processor.enter_context() as c, \
+            Event(
+                event_id=event_id,
+                event_service_instance_id=event_service_instance_id,
+                client=_mp_client
+            ) as event:
+        with Processor.started_stopwatch('process_method'):
             result = _mp_processor.process(event, params)
         return result, c.times, event.created_indices
 
 
 class MpProcessorRunner:
     __slots__ = (
         'pool',
         'metadata',
         'processor_name',
         'component_id',
         'log_listener',
     )
 
     def __init__(self,
-                 proc: 'mtap.EventProcessor',
+                 proc: EventProcessor,
                  processor_name: str,
-                 component_id: 'Optional[str]' = None,
-                 workers: 'Optional[int]' = 8,
-                 events_address: 'Optional[Union[str, Sequence[str]]]' = None,
+                 component_id: Optional[str] = None,
+                 workers: Optional[int] = 8,
+                 events_address: Optional[Union[str, Sequence[str]]] = None,
                  mp_context=None,
                  log_level=None):
         if mp_context is None:
             import multiprocessing as mp
             mp_context = mp.get_context('spawn')
         config = _config.Config()
         log_queue = mp_context.Queue(-1)
@@ -218,15 +206,15 @@
     def close(self):
         self.pool.terminate()
         self.pool.join()
         self.log_listener.stop()
 
 
 def processor_parser() -> argparse.ArgumentParser:
-    """An :class:`~argparse.ArgumentParser` that can be used to parse the 
+    """An :class:`~argparse.ArgumentParser` that can be used to parse the
     settings for :func:`run_processor`.
 
     Returns:
         A parser containing server settings.
 
     Examples:
         Using this as a parent parser:
@@ -320,15 +308,15 @@
         p.nullable = property_meta['nullable']
 
 
 class _ProcessorServicer(processing_pb2_grpc.ProcessorServicer):
     def __init__(self,
                  address: str,
                  sid: str,
-                 runner: '_base.ProcessingComponent',
+                 runner: ProcessingComponent,
                  health_servicer: health.HealthServicer,
                  register: bool = False):
         self.config = _config.Config()
         self.address = address
         self.sid = sid
         self._runner = runner
         self.register = register
@@ -374,15 +362,15 @@
                 event_id,
                 event_service_instance_id,
                 params
             )
             if result is not None:
                 _structs.copy_dict_to_struct(result, response.result, [])
 
-            _pipeline_results.add_times(self._times_map, times)
+            add_times(self._times_map, times)
             for k, l in times.items():
                 response.timing_info[k].FromTimedelta(l)
             for document_name, l in added_indices.items():
                 for index_name in l:
                     created_index = response.created_indices.add()
                     created_index.document_name = document_name
                     created_index.index_name = index_name
@@ -391,16 +379,16 @@
             logger.error(str(e))
             logger.error(traceback.format_exc())
             context.abort_with_status(rpc_status.to_status(e.to_rpc_status()))
 
     def GetStats(self, request, context):
         r = processing_pb2.GetStatsResponse(processed=self.processed,
                                             failures=self.failure_count)
-        tsd = _pipeline_results.create_timer_stats(self._times_map,
-                                                   self._runner.component_id)
+        tsd = create_timer_stats(self._times_map,
+                                 self._runner.component_id)
         for k, v in tsd.items():
             ts = r.timing_stats[k]
             ts.mean.FromTimedelta(v.mean)
             ts.std.FromTimedelta(v.std)
             ts.max.FromTimedelta(v.max)
             ts.min.FromTimedelta(v.min)
             ts.sum.FromTimedelta(v.sum)
@@ -437,15 +425,15 @@
     """
     host: str
     processor_name: str
     sid: str
     write_address: bool
 
     def __init__(self,
-                 runner: 'mtap.processing.ProcessingComponent',
+                 runner: ProcessingComponent,
                  host: str,
                  port: int = 0,
                  *,
                  sid: Optional[str] = None,
                  register: bool = False,
                  workers: Optional[int] = None,
                  write_address: bool = False):
```

### Comparing `mtap-1.2.0/python/mtap/processing/_sources.py` & `mtap-1.2.1/python/mtap/pipeline/_sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,89 +11,71 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 from abc import ABC, abstractmethod
 from os import PathLike
 from pathlib import Path
-from typing import Union, Optional, ContextManager, Callable, TYPE_CHECKING
+from typing import Union, Optional, ContextManager, Callable
 
-if TYPE_CHECKING:
-    import mtap
-    from mtap import Event, Document, processing
+from mtap._document import Document
+from mtap._event import Event
+from mtap._events_client import EventsClient
 
 
 class ProcessingSource(ContextManager, ABC):
     """Provides events or documents for the multithreaded pipeline runner.
     Also has functionality for receiving results.
 
     """
-    __slots__ = ('_total')
+    __slots__ = ()
+
+    _total: Optional[int] = None
 
     @property
     def total(self) -> Optional[int]:
         """The total number of documents this source will provide.
 
         Returns:
             Total number of events this source will provide or ``None`` if not
             known.
 
         """
-        try:
-            return self._total
-        except AttributeError:
-            return None
+        return self._total
 
     @total.setter
     def total(self, count: Optional[int]):
         self._total = count
 
     @abstractmethod
-    def provide(
+    def produce(
             self,
-            consume: 'Callable[[Union[Document, Event]], None]'
+            consume: Callable[[Union[Document, Event]], None]
     ):
-        """The method which provides documents for the multithreaded runner.
-        This method provides documents or events to the pipeline.
+        """The method which provides documents or events to the pipeline
+        to batch process.
 
         Args:
             consume: The consumer method to pass documents or events to
                 process.
 
         Examples:
             Example implementation for processing text documents:
 
             >>> ...
-            >>> def provide(self, consume):
+            >>> def produce(self, consume):
             >>>     for file in Path(".").glob("*.txt"):
             >>>         with file.open('r') as fio:
             >>>             txt = fio.read()
-            >>>         event = Event()
-            >>>         doc = event.create_document('plaintext', txt)
-            >>>         consume(doc)
+            >>>         with Event(client=client) as e:
+            >>>             doc = event.create_document('plaintext', txt)
+            >>>             consume(doc)
         """
         ...
 
-    def receive_result(self,
-                       result: 'processing.PipelineResult',
-                       event: 'mtap.Event'):
-        """Optional method: Asynchronous callback which returns the results of
-        processing.
-
-        This method is called on a processing worker thread.
-        Default behavior is to do nothing.
-
-        Args:
-            result: The result of processing using the
-                pipeline.
-            event: The event processed.
-
-        """
-        pass
-
     def close(self):
         """Optional method: called to clean up after processing is complete.
 
         Default behavior is to do nothing.
         """
         pass
 
@@ -114,16 +96,20 @@
     def __init__(self, source):
         # We use an iterator here to can ensure that it gets closed on
         # unexpected / early termination and any caller context managers are
         # exited before their client gets shut down.
         # Using a for-in loop we're not guaranteed, which can cause zombie
         # unclosed events on the event service.
         self.it = iter(source)
+        try:
+            self.total = len(source)
+        except (AttributeError, TypeError):
+            pass
 
-    def provide(self, consume):
+    def produce(self, consume):
         while True:
             try:
                 target = next(self.it)
             except StopIteration:
                 break
             consume(target)
 
@@ -163,15 +149,15 @@
         'directory',
         'document_name',
         'extension_glob',
         'errors',
         'total'
     )
 
-    def __init__(self, client: 'mtap.EventsClient',
+    def __init__(self, client: EventsClient,
                  directory: Union[str, bytes, PathLike],
                  *, document_name: str = 'plaintext',
                  extension_glob: str = '*.txt',
                  count_total: bool = True,
                  errors: Optional[str] = None):
         self.client = client
         if not os.path.isdir(directory):
@@ -182,15 +168,15 @@
         self.document_name = document_name
         self.extension_glob = extension_glob
         self.errors = errors
         if count_total:
             self.total = sum(1 for _
                              in Path(directory).rglob(self.extension_glob))
 
-    def provide(self, consume):
+    def produce(self, consume):
         for path in Path(self.directory).rglob(self.extension_glob):
             with path.open('r', errors=self.errors) as f:
                 txt = f.read()
             relative = str(path.relative_to(self.directory))
             with Event(event_id=relative, client=self.client,
                        only_create_new=True) as e:
                 doc = e.create_document(self.document_name, txt)
```

### Comparing `mtap-1.2.0/python/mtap/processing/descriptions.py` & `mtap-1.2.1/python/mtap/descriptors.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,56 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Descriptors for processor functionality."""
-import typing
-from typing import NamedTuple, Optional, List, Dict, Any
+from dataclasses import dataclass
+from typing import Optional, List, Dict, Any, TYPE_CHECKING, Type, Callable
 
-if typing.TYPE_CHECKING:
-    from mtap import EventProcessor
+if TYPE_CHECKING:
+    from mtap.processing import EventProcessor
 
 __all__ = [
     'label_property',
+    'LabelPropertyDescriptor',
     'labels',
+    'LabelIndexDescriptor',
     'parameter',
+    'ParameterDescriptor',
     'processor',
+    'ProcessorDescriptor'
 ]
 
 
-def processor(name: str,
-              *,
-              human_name: Optional[str] = None,
-              description: Optional[str] = None,
-              parameters: 'Optional[List[parameter]]' = None,
-              inputs: 'Optional[List[labels]]' = None,
-              outputs: 'Optional[List[labels]]' = None,
-              **additional_metadata: Any):
+def processor(
+        name: str,
+        *args,
+        **kwargs
+) -> Callable[[Type['EventProcessor']], Type['EventProcessor']]:
     """Decorator which attaches a service name and metadata to a processor.
     Which then can be used for runtime reflection of how the processor works.
 
     Args:
-        name: Identifying service name both for launching via command line and
-            for service registration.
-            Should be a mix of alphanumeric characters and dashes so that it
-            plays nice with the DNS name requirements of service discovery
-            tools like Consul.
-        human_name: An optional human name for the processor.
-        description: A short description of the processor and what it does.
-        parameters: The processor's parameters.
-        inputs: String identifiers for the label output from a previously-run
-            processor that this processor requires as an input.
-
-            Takes the format ``"[processor-name]/[output]"``. Examples would be
-            ``"tagger/pos_tags"`` or ``"sentence-detector/sentences"``.
-        outputs: The label indices this processor outputs.
-        **additional_metadata: Any other data that should be added to the
-            processor's metadata, should be serializable to yaml and json.
+        name: The required arg of
+        *args: Arbitrary args accepted by
+            :class:`~mtap.descriptors.ProcessorDescriptor`.
+        **kwargs: Arbitrary args accepted by
+            :class:`~mtap.descriptors.ProcessorDescriptor`.
 
     Returns:
         A decorator to be applied to instances of EventProcessor or
         DocumentProcessor. This decorator attaches the metadata, so it can be
         reflected at runtime.
 
     Examples:
@@ -94,136 +84,128 @@
         >>>                       properties=[label_property('letter',
         >>>                                                  data_type='str'),
         >>>                                   label_property('count',
         >>>                                                  data_type='int')])
         >>>            ])
         >>> class ExampleProcessor(DocumentProcessor):
         >>>     ...
+    """
+
+    def decorator(cls: 'Type[EventProcessor]'):
+        cls.descriptor = ProcessorDescriptor(name, *args, **kwargs)
+        return cls
+
+    return decorator
 
 
+@dataclass
+class ProcessorDescriptor:
+    name: str
+    """Identifying service name both for launching via command line and
+    for service registration.
+
+    Should be a mix of alphanumeric characters and dashes so that it
+    plays nice with the DNS name requirements of service discovery
+    tools like Consul.
     """
 
-    def decorator(cls):
-        cls.metadata = {
-            'name': name,
-            'human_name': human_name,
-            'description': description
-        }
-        if parameters is not None:
-            cls.metadata['parameters'] = [_parameter_to_map(p)
-                                          for p in parameters]
-        if inputs is not None:
-            cls.metadata['inputs'] = [_desc_to_dict(desc) for desc in inputs]
-        if outputs is not None:
-            cls.metadata['outputs'] = [_desc_to_dict(desc) for desc in outputs]
-        if additional_metadata is not None:
-            cls.metadata.update(additional_metadata)
-        if 'implementation_lang' not in cls.metadata:
-            cls.metadata['implementation_lang'] = 'Python'
+    human_name: Optional[str] = None
+    """An optional human name for the processor."""
 
-        return cls
+    description: Optional[str] = None
+    """A short description of the processor and what it does."""
 
-    return decorator
+    parameters: Optional[List['ParameterDescriptor']] = None
+    """The processor's parameters."""
 
+    inputs: Optional[List['LabelIndexDescriptor']] = None
+    """String identifiers for the label output from a previously-run
+    processor that this processor requires as an input.
 
-class parameter(NamedTuple):
+    Takes the format ``"[processor-name]/[output]"``. Examples would be
+    ``"tagger/pos_tags"`` or ``"sentence-detector/sentences"``.
+    """
+
+    outputs: Optional[List['LabelIndexDescriptor']] = None
+    """The label indices this processor outputs."""
+
+    additional_data: Optional[Dict[str, Any]] = None
+    """Any other data that should be added to the
+    processor's metadata, should be serializable to yaml and json.
+    """
+
+
+@dataclass
+class ParameterDescriptor:
     """A description of one of the processor's parameters.
     """
     name: str
     """The parameter name / key."""
 
     description: Optional[str] = None
     """A short description of the property and what it does."""
 
     data_type: Optional[str] = None
-    """The data type of the parameter. str, float, or bool; List[T] 
+    """The data type of the parameter. str, float, or bool; List[T]
     or Mapping[T1, T2] of those."""
 
     required: bool = False
     """Whether the processor parameter is required."""
 
 
-class labels(NamedTuple):
+parameter: Callable[..., ParameterDescriptor] = ParameterDescriptor
+"""Alias for :class:`~mtap.descriptors.ParameterDescriptor`."""
+
+
+@dataclass
+class LabelIndexDescriptor:
     """A description for a label type.
     """
     name: str
     """The label index name."""
 
     reference: Optional[str] = None
     """If this is an output of another processor, that processor's
     name followed by a slash and the default output name of the index
     go here.
     Example: "sentence-detector/sentences"."""
 
     name_from_parameter: Optional[str] = None
-    """If the label index gets its name from a parameter of the processor, 
+    """If the label index gets its name from a parameter of the processor,
     specify that name here."""
 
     optional: bool = False
     """Whether this label index is an optional input or  output."""
 
     description: Optional[str] = None
     """A short description of the label index."""
 
-    properties: 'Optional[List[label_property]]' = None
+    properties: Optional[List['LabelPropertyDescriptor']] = None
     """The properties of the labels in the label index."""
 
 
-class label_property(NamedTuple):
+labels: Callable[..., 'LabelIndexDescriptor'] = LabelIndexDescriptor
+"""Alias for :class:`~mtap.descriptors.ParameterDescriptor`"""
+
+
+@dataclass
+class LabelPropertyDescriptor:
     """Creates a description for a property on a label.
     """
     name: str
     """The property's name."""
 
     description: Optional[str] = None
     """A short description of the property."""
 
     data_type: Optional[str] = None
-    """The data type of the property. Options are ``"str"``, ``"float"``, or 
-    ``"bool"``; ``"List[T]"`` or ``"Mapping[str, T]"`` where ``T`` is 
+    """The data type of the property. Options are ``"str"``, ``"float"``, or
+    ``"bool"``; ``"List[T]"`` or ``"Mapping[str, T]"`` where ``T`` is
     one of those types."""
 
     nullable: bool = False
     """Whether the property can have a valid value of null."""
 
 
-def _desc_to_dict(description: labels) -> dict:
-    m = {
-        'name': description.name
-    }
-    if description.name_from_parameter is not None:
-        m['name_from_parameter'] = description.name_from_parameter
-    if description.reference is not None:
-        m['reference'] = description.reference
-    if description.optional is not None:
-        m['optional'] = description.optional
-    if description.description is not None:
-        m['description'] = description.description
-    if description.properties is not None:
-        m['properties'] = [_prop_to_dict(p) for p in description.properties]
-    return m
-
-
-def _prop_to_dict(p: label_property) -> Dict[str, Any]:
-    m = {
-        'name': p.name
-    }
-    if p.description is not None:
-        m['description'] = p.description
-    if p.data_type is not None:
-        m['data_type'] = p.data_type
-    if p.nullable is not None:
-        m['nullable'] = p.nullable
-    return m
-
-
-def _parameter_to_map(p: parameter) -> Dict[str, Any]:
-    m = {
-        'name': p.name
-    }
-    if p.description is not None:
-        m['description'] = p.description
-    if p.data_type is not None:
-        m['data_type'] = p.data_type
-    if p.required is not None:
-        m['required'] = p.required
-    return m
+label_property: Callable[..., 'LabelPropertyDescriptor'] \
+    = LabelPropertyDescriptor
+"""Alias for :class:`~mtap.descriptors.LabelPropertyDescriptor`."""
```

### Comparing `mtap-1.2.0/python/mtap/processors/__init__.py` & `mtap-1.2.1/python/mtap/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/processors/copy_document.py` & `mtap-1.2.1/python/mtap/processors/copy_document.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,88 +10,85 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
 import typing
 
-import mtap
-
-
 __all__ = [
     'copy_document', 'CopyDocument', 'main'
 ]
 
+from mtap import Event, Document, processor, EventProcessor, processor_parser, \
+    run_processor
+
 
-def copy_document(event: mtap.Event,
+def copy_document(event: Event,
                   source_document_name: str,
                   target_document_name: str,
                   index_names: typing.Sequence[str] = ...):
     """Copies one document to another on the same event.
 
     Parameters
     ----------
     event: Event
         The event.
     source_document_name: str
         The source document name.
     target_document_name: str
         The target document name.
     index_names: Sequence[str]
-        If specified will only copy the specified label indices, by default all indices will be
-        copied.
+        If specified will only copy the specified label indices, by default all
+        indices will be copied.
     """
     source_document = event.documents[source_document_name]
-    target_document = mtap.Document(target_document_name, text=source_document.text)
+    target_document = Document(target_document_name, text=source_document.text)
     event.add_document(target_document)
     if index_names is ...:
         index_names = list(source_document.labels)
     for index_name in index_names:
         index = source_document.labels[index_name]
         target_document.add_labels(index_name, index, distinct=index.distinct)
 
 
-@mtap.processor('mtap-copy-processor')
-class CopyDocument(mtap.EventProcessor):
+@processor('mtap-copy-processor')
+class CopyDocument(EventProcessor):
     """Copies one document to another.
-
-    Parameters
-    ----------
-    source_document_name: str
-        The source document name.
-    target_document_name: str
-        The target document name.
-    index_names: Sequence[str]
-        If specified will only copy the specified label indices, by default all indices will be
-        copied.
     """
 
     def __init__(self,
                  source_document_name: str,
                  target_document_name: str,
                  index_names: typing.Sequence[str] = ...):
         self.source_document_name = source_document_name
         self.target_document_name = target_document_name
         self.index_names = index_names
 
-    def process(self, event: mtap.Event, params: typing.Dict[str, typing.Any]):
-        copy_document(event, self.source_document_name, self.target_document_name, self.index_names)
+    def process(self, event: Event, params: typing.Dict[str, typing.Any]):
+        copy_document(
+            event,
+            self.source_document_name,
+            self.target_document_name,
+            self.index_names
+        )
 
 
 def main(args=None):
     parser = argparse.ArgumentParser(
         description='Deploys a processor that copies one document to another.',
-        parents=[mtap.processor_parser()]
+        parents=[processor_parser()]
     )
-    parser.add_argument('--index-names', nargs='*', metavar='INDEX_NAME', default=...,
+    parser.add_argument('--index-names', nargs='*', metavar='INDEX_NAME',
+                        default=...,
                         help='')
     parser.add_argument('source_document_name', metavar='SOURCE_NAME',
                         help='Name of source document.')
     parser.add_argument('target_document_name', metavar='TARGET_NAME',
                         help='Name of target document.')
     ns = parser.parse_args(args)
-    p = CopyDocument(ns.source_document_name, ns.target_document_name, ns.index_names)
-    mtap.run_processor(p, options=ns)
+    p = CopyDocument(ns.source_document_name, ns.target_document_name,
+                     ns.index_names)
+    run_processor(p, options=ns)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mtap-1.2.0/python/mtap/serialization/__init__.py` & `mtap-1.2.1/python/mtap/serialization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,9 @@
     dict_to_event,
     dict_to_document,
     Serializer,
     SerializationProcessor,
     JsonSerializer,
     YamlSerializer,
     PickleSerializer,
-    standard_serializers,
-    get_serializer,
     SerializerRegistry,
-    SerializerFactory,
 )
```

### Comparing `mtap-1.2.0/python/mtap/serialization/_serialization.py` & `mtap-1.2.1/python/mtap/serialization/_serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,31 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Serialization, serializers, and helper methods for going to and from
 flattened python dictionary representations of events.
 """
 import io
 import logging
-from abc import ABC, abstractmethod
+import os
+from abc import abstractmethod, ABCMeta
 from os import PathLike
-from pathlib import Path
-from typing import Union, Dict, Any, Optional, TextIO, Callable
+from typing import Union, Dict, Any, Optional, TextIO, Type, ClassVar, IO, \
+    BinaryIO
 
-import mtap
-from mtap import data, processing
-from mtap.processing.descriptions import *
+from mtap._document import Document
+from mtap._event import Event
+from mtap._events_client import EventsClient
+from mtap._label_adapters import GENERIC_ADAPTER
+from mtap.descriptors import processor, parameter
+from mtap.processing import EventProcessor, Processor
 
 logger = logging.getLogger('mtap.serialization')
 
 
-def event_to_dict(event: mtap.Event, *,
+def event_to_dict(event: Event, *,
                   include_label_text: bool = False) -> Dict:
     """A helper method that turns an event into a python dictionary.
 
     Args:
         event: The event object.
         include_label_text: Whether to include the text labels cover with the
             labels.
@@ -52,15 +56,15 @@
         d['documents'][doc.document_name] = document_to_dict(
             doc,
             include_label_text=include_label_text
         )
     return d
 
 
-def document_to_dict(document: mtap.Document, *,
+def document_to_dict(document: Document, *,
                      include_label_text: bool = False) -> Dict:
     """A helper method that turns a document into a python dictionary.
 
     Args:
         document: The document object.
         include_label_text: Whether to include the text labels cover with the
             labels.
@@ -72,160 +76,147 @@
         'text': document.text,
         'label_indices': {}
     }
 
     for index_name, index in document.labels.items():
         adapter = index.adapter
         if adapter is None:
-            adapter = data.GENERIC_ADAPTER
+            adapter = GENERIC_ADAPTER
         d['label_indices'][index_name] = adapter.pack(
             index,
             include_label_text=include_label_text
         )
     return d
 
 
 def dict_to_event(d: Dict, *,
-                  client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+                  client: Optional[EventsClient] = None) -> Event:
     """Turns a serialized dictionary into an Event.
 
     Args:
         d: A json-like (only ``str`` keys) dictionary representation of the
             event.
         client: If specified, will upload the event to this events service.
             Otherwise, creates a local event.
 
     Returns:
         The deserialized event object.
     """
-    event = mtap.Event(event_id=d['event_id'], client=client)
+    event = Event(event_id=d['event_id'], client=client)
     for k, v in d['metadata'].items():
         event.metadata[k] = v
     for k, v in d['documents'].items():
         dict_to_document(k, v, event=event)
     return event
 
 
 def dict_to_document(document_name: str,
                      d: Dict,
-                     *, event: Optional[mtap.Event] = None) -> mtap.Document:
+                     *, event: Optional[Event] = None) -> Document:
     """Turns a serialized dictionary into a Document.
 
     Args:
         document_name: The name identifier of the document.
         d: A json-like (only ``str`` keys) dictionary representation of the
             document.
         event: If specified, the function will add the document to this
             event. Otherwise, it will create a stand-alone document.
 
     Returns:
         The deserialized Document object.
 
     """
-    document = mtap.Document(document_name=document_name, text=d['text'])
+    document = Document(document_name=document_name, text=d['text'])
     if event is not None:
         event.add_document(document)
     for k, v in d['label_indices'].items():
-        adapter = document.get_default_adapter(k)
+        adapter = document.default_adapter(k)
         index = adapter.unpack(v, k, document=document)
         document.add_labels(k, index, distinct=index.distinct)
 
     return document
 
 
-class Serializer(ABC):
+class SerializerRegistry(ABCMeta):
+    REGISTRY: ClassVar[Dict[str, Type['Serializer']]] = {}
+
+    def __init__(cls: Type['Serializer'], *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        SerializerRegistry.REGISTRY[cls.name()] = cls
+
+    @staticmethod
+    def get(name: str) -> Type['Serializer']:
+        return SerializerRegistry.REGISTRY[name]
+
+
+class Serializer(metaclass=SerializerRegistry):
     """Abstract base class for a serializer of MTAP events.
     """
 
-    @property
-    @abstractmethod
-    def extension(self) -> str:
+    @classmethod
+    def name(cls) -> str:
+        return cls.__name__.casefold()
+
+    @classmethod
+    def extension(cls) -> str:
         """str: Filename extension, including period. Ex: ``'.json'``."""
         ...
 
+    @classmethod
     @abstractmethod
     def event_to_file(
-            self,
-            event: mtap.Event,
-            f: Union[str, bytes, PathLike, TextIO],
+            cls,
+            event: Event,
+            f: Union[str, bytes, PathLike, IO],
             *, include_label_text: bool = False
     ):
         """Writes the event to a file.
 
         Args:
-            event (Event): The event object to serialize.
-            f (~typing.Union[~pathlib.Path, str, ~io.IOBase]):
-                A file or a path to a file to write the event to.
-            include_label_text (bool):
-                Whether, when serializing, to include the text that each label
-                covers with the rest of the label.
+            event: The event object to serialize.
+            f: A file or a path to a file to write the event to.
+            include_label_text: Whether, when serializing, to include the text
+            that each label covers with the rest of the label.
         """
         ...
 
+    @classmethod
     @abstractmethod
     def file_to_event(
-            self,
-            f: Union[str, bytes, PathLike, TextIO], *,
-            client: Optional[mtap.EventsClient] = None
-    ) -> mtap.Event:
+            cls,
+            f: Union[str, bytes, PathLike, IO],
+            *, client: Optional[EventsClient] = None
+    ) -> Event:
         """Loads an event from a serialized file.
 
         Args:
             f (~typing.Union[~pathlib.Path, str, ~io.IOBase]):
                 The file to load from.
             client (~typing.Optional[EventsClient]):
                 The events service to load the event into.
 
         Returns:
             Event: The loaded event object.
         """
         ...
 
 
-SerializerFactory = Callable[[Dict[str, Any]], Serializer]
-
-registry: Dict[str, SerializerFactory] = {}
-
-
-class SerializerRegistry:
-    @staticmethod
-    def register(
-            name: str
-    ) -> Callable[[SerializerFactory], SerializerFactory]:
-        def decorate(f: SerializerFactory) -> SerializerFactory:
-            registry[name] = f
-            return f
-
-        return decorate
-
-    @staticmethod
-    def create(name: str,
-               params: Optional[Dict[str, Any]] = None) -> Serializer:
-        return registry[name](**params)
-
-    @staticmethod
-    def from_dict(conf: Dict[str, Any]):
-        name = conf['name']
-        params = conf.get('params', {})
-        return SerializerRegistry.create(name, params)
-
-
-@mtap.processing.processor(
+@processor(
     'mtap-serializer',
     description='Serializes events to a specific directory',
     parameters=[
         parameter(
             'filename',
             data_type='str',
             description='Optional override for the filename '
                         'to write the document to.'
         )
     ]
 )
-class SerializationProcessor(mtap.EventProcessor):
+class SerializationProcessor(EventProcessor):
     """An MTAP :obj:`EventProcessor` that serializes events to a specific
     directory.
 
     Attributes:
         serializer: The serializer to use.
         output_dir: The output directory.
         include_label_text: Whether to attach the covered text to labels.
@@ -238,159 +229,158 @@
     def __init__(
             self,
             serializer: Serializer,
             output_dir: Union[str, bytes, PathLike],
             include_label_text: bool = False
     ):
         self.serializer = serializer
-        self.output_dir = output_dir
+        self.output_dir = os.path.abspath(output_dir)
         self.include_label_text = include_label_text
-        Path(self.output_dir).mkdir(parents=True, exist_ok=True)
+        os.makedirs(self.output_dir, exist_ok=True)
 
-    def process(self, event: mtap.Event, params: Dict[str, Any]):
+    def process(self, event: Event, params: Dict[str, Any]):
         name = params.get('filename',
-                          event.event_id + self.serializer.extension)
-        path = Path(self.output_dir, name)
+                          event.event_id + self.serializer.extension())
+        path = os.path.join(self.output_dir, name)
         self.serializer.event_to_file(
-            event, path, include_label_text=self.include_label_text)
+            event,
+            path,
+            include_label_text=self.include_label_text
+        )
 
 
-@SerializerRegistry.register('json')
-class _JsonSerializer(Serializer):
+class JsonSerializer(Serializer):
     """Serializer implementation that performs serialization to JSON.
     """
-    @property
-    def extension(self) -> str:
+
+    @classmethod
+    def name(cls) -> str:
+        return 'json'
+
+    @classmethod
+    def extension(cls) -> str:
         return '.json'
 
-    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
+    @classmethod
+    def event_to_file(cls,
+                      event: Event,
+                      f: Union[str, bytes, PathLike, IO], *,
                       include_label_text: bool = False):
         import json
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             d = event_to_dict(event, include_label_text=include_label_text)
-        with processing.Processor.started_stopwatch('io'):
+        with Processor.started_stopwatch('io'):
             try:
                 json.dump(d, f)
-            except AttributeError:
-                f = Path(f)
-                f.parent.mkdir(parents=True, exist_ok=True)
-                with f.open('w') as f:
+            except (AttributeError, TypeError):
+                os.makedirs(os.path.dirname(f), exist_ok=True)
+                with open(f, 'w') as f:
                     json.dump(d, f)
 
-    def file_to_event(self, f: Union[Path, str, TextIO],
-                      client: Optional[
-                          mtap.EventsClient] = None) -> mtap.Event:
+    @classmethod
+    def file_to_event(cls,
+                      f: Union[str, bytes, PathLike, IO],
+                      client: Optional[EventsClient] = None) -> Event:
         import json
-        with processing.Processor.started_stopwatch('io'):
+        with Processor.started_stopwatch('io'):
             try:
                 d = json.load(f)
-            except AttributeError:
-                if isinstance(f, str):
-                    f = Path(f)
-                with f.open('r') as f:
+            except (AttributeError, TypeError):
+                with open(f, 'r') as f:
                     d = json.load(f)
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
 
 
-@SerializerRegistry.register('yaml')
-class _YamlSerializer(Serializer):
+class YamlSerializer(Serializer):
     """Serializer implementation that performs serialization to YAML.
     """
-    @property
-    def extension(self) -> str:
+
+    @classmethod
+    def name(cls) -> str:
+        return 'yaml'
+
+    @classmethod
+    def extension(cls) -> str:
         return '.yml'
 
-    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
+    @classmethod
+    def event_to_file(cls, event: Event,
+                      f: Union[str, bytes, PathLike, IO], *,
                       include_label_text: bool = False):
         import yaml
         try:
             from yaml import CDumper as Dumper
         except ImportError:
             from yaml import Dumper
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             d = event_to_dict(event, include_label_text=include_label_text)
-        with processing.Processor.started_stopwatch('io'):
-            if isinstance(f, io.IOBase):
+        with Processor.started_stopwatch('io'):
+            try:
                 yaml.dump(d, f, Dumper=Dumper)
-            else:
-                f = Path(f)
-                with f.open('w') as f:
+            except (AttributeError, TypeError):
+                os.makedirs(os.path.dirname(f), exist_ok=True)
+                with open(f, 'w') as f:
                     yaml.dump(d, f, Dumper=Dumper)
 
-    def file_to_event(self, f: Union[Path, str, TextIO], *,
-                      client: Optional[
-                          mtap.EventsClient] = None) -> mtap.Event:
+    @classmethod
+    def file_to_event(cls,
+                      f: Union[str, bytes, PathLike, TextIO],
+                      *, client: Optional[EventsClient] = None) -> Event:
         import yaml
         try:
             from yaml import CLoader as Loader
         except ImportError:
             from yaml import Loader
-        with processing.Processor.started_stopwatch('io'):
-            if isinstance(f, io.IOBase):
+        with Processor.started_stopwatch('io'):
+            try:
                 d = yaml.load(f, Loader=Loader)
-            else:
-                with Path(f).open() as f:
+            except (AttributeError, TypeError):
+                with open(f) as f:
                     d = yaml.load(f, Loader=Loader)
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
 
 
-@SerializerRegistry.register('pickle')
-class _PickleSerializer(Serializer):
+class PickleSerializer(Serializer):
     """Serializer implementation that performs serialization to .pickle.
     """
-    @property
-    def extension(self) -> str:
+
+    @classmethod
+    def name(cls) -> str:
+        return 'pickle'
+
+    @classmethod
+    def extension(cls) -> str:
         return '.pickle'
 
-    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
+    @classmethod
+    def event_to_file(cls,
+                      event: Event,
+                      f: Union[str, bytes, PathLike, BinaryIO], *,
                       include_label_text: bool = False):
         import pickle
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             d = event_to_dict(event, include_label_text=include_label_text)
-        with processing.Processor.started_stopwatch('io'):
+        with Processor.started_stopwatch('io'):
             try:
                 pickle.dump(d, f)
-            except TypeError:
-                with Path(f).open('wb') as f:
+            except (AttributeError, TypeError):
+                os.makedirs(os.path.dirname(f), exist_ok=True)
+                with open(f, 'wb') as f:
                     pickle.dump(d, f)
 
-    def file_to_event(self, f: Union[Path, str, TextIO], *,
-                      client: Optional[
-                          mtap.EventsClient] = None) -> mtap.Event:
+    @classmethod
+    def file_to_event(
+            cls,
+            f: Union[str, bytes, PathLike, BinaryIO], *,
+            client: Optional[EventsClient] = None
+    ) -> Event:
         import pickle
-        with processing.Processor.started_stopwatch('io'):
+        with Processor.started_stopwatch('io'):
             try:
                 d = pickle.load(f)
-            except TypeError:
-                with Path(f).open('rb') as f:
+            except (AttributeError, TypeError):
+                with open(f, 'rb') as f:
                     d = pickle.load(f)
-        with processing.Processor.started_stopwatch('transform'):
+        with Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
-
-
-JsonSerializer: Serializer = _JsonSerializer()
-
-YamlSerializer: Serializer = _YamlSerializer()
-
-PickleSerializer: Serializer = _PickleSerializer()
-
-standard_serializers = {
-    'json': JsonSerializer,
-    'yml': YamlSerializer,
-    'pickle': PickleSerializer
-}
-
-
-def get_serializer(identifier: str) -> Serializer:
-    """Returns a serializer by its identifier.
-
-    Options are: ``json``, ``yml``, and ``pickle``.
-
-    Parameters:
-        identifier: The serializer identifier.
-
-    Returns:
-        The specified serializer.
-    """
-    return standard_serializers[identifier]
```

### Comparing `mtap-1.2.0/python/mtap/serialization/brat.py` & `mtap-1.2.1/python/mtap/serialization/brat.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,120 +11,132 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tools for reading in files annotated using BRAT (https://brat.nlplab.org/)."""
 
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Union, Iterable, Optional, TYPE_CHECKING
+from typing import Union, Iterable, Optional
 
-from mtap import data
-
-if TYPE_CHECKING:
-    import mtap
+from mtap._document import Document
+from mtap._event import Event
+from mtap._events_client import EventsClient
 
 __all__ = [
     'ann_to_labels',
     'read_brat_document',
     'read_brat_documents',
 ]
 
 
-def read_brat_documents(directory: Union[Path, str],
-                        client: Optional['mtap.EventsClient'] = None,
-                        document_name: str = 'plaintext',
-                        label_index_name_prefix: str = '',
-                        encoding: Optional[str] = None,
-                        create_indices: Optional[Iterable[str]] = None) -> Iterable['mtap.Event']:
-    """Reads a directory full of BRAT-annotated ".txt" and ".ann" files, creating events for each
-    .txt containing labels created from the annotations in its ".ann" counterpart.
+def read_brat_documents(
+        directory: Union[Path, str],
+        client: Optional[EventsClient] = None,
+        document_name: str = 'plaintext',
+        label_index_name_prefix: str = '',
+        encoding: Optional[str] = None,
+        create_indices: Optional[Iterable[str]] = None
+) -> Iterable[Event]:
+    """Reads a directory full of BRAT-annotated ".txt" and ".ann" files,
+    creating events for each .txt containing labels created from the
+    annotations in its ".ann" counterpart.
 
     Args:
-        directory (str, Path): The directory containing the files or sub-directories containing the
-            files.
-        client (EventsClient): The client to the events server to add the documents to.
-        document_name (str): The document name to create on each event containing the brat data.
-        label_index_name_prefix  (str): A prefix to append to the brat annotation names.
-        encoding (optional str): The encoding to use when reading the files.
-        create_indices (optional iterable of str): These indices will be created no matter what,
+        directory: The directory containing the files or subdirectories
+            containing the files.
+        client: The client to the events server to add the documents to.
+        document_name: The document name to create on each event containing
+            the brat data.
+        label_index_name_prefix: A prefix to append to the brat annotation
+            names.
+        encoding: The encoding to use when reading the files.
+        create_indices: These indices will be created no matter what,
             even if empty.
 
     Returns:
-        Iterable of Event: Iterable of all the events from the directory of brat documents.
+        Iterable of all the events from the directory of brat documents.
 
     Examples:
         >>> client = mtap.EventsClient()
         >>> for event in read_brat_documents('docs', client=client):
         >>>   with event:
         >>>      # use event
 
     """
     directory = Path(directory)
     for txt_file in directory.glob('**/*.txt'):
-        with read_brat_document(txt_file, client=client, document_name=document_name,
-                                label_index_name_prefix=label_index_name_prefix, encoding=encoding,
-                                relative_to=directory, create_indices=create_indices) as event:
+        with read_brat_document(txt_file, client=client,
+                                document_name=document_name,
+                                label_index_name_prefix=label_index_name_prefix,
+                                encoding=encoding,
+                                relative_to=directory,
+                                create_indices=create_indices) as event:
             yield event
 
 
 @contextmanager
 def read_brat_document(txt_file: Union[Path, str],
-                       client: Optional['mtap.EventsClient'] = None,
+                       client: Optional[EventsClient] = None,
                        document_name: str = 'plaintext',
                        label_index_name_prefix: str = '',
                        encoding: Optional[str] = None,
                        relative_to: Optional[Union[Path, str]] = None,
-                       create_indices: Optional[Iterable[str]] = None) -> 'mtap.Event':
+                       create_indices: Optional[
+                           Iterable[str]] = None) -> Event:
     """Reads a BRAT .txt and .ann file pair into an Event.
 
     Args:
-        txt_file (Path or str): The path to the .txt file.
-        client (optional EventsClient): The client to the events server to add the documents to.
-        document_name (str): The document name to create on the event to hold the brat data.
-        label_index_name_prefix (str): A prefix to append to the brat annotation names.
-        encoding (optional str): The encoding to use when reading the files.
-        relative_to (optional str or Path): A str of a path or a Path object for which the event_id
-            will be relative to, if this is omitted then the file's name without extension will be
-            used.
-        create_indices (optional iterable of str): These indices will be created no matter what,
+        txt_file: The path to the .txt file.
+        client: The client to the events server to add the documents to.
+        document_name: The document name to create on the event to hold the
+            brat data.
+        label_index_name_prefix: A prefix to append to the brat annotation
+            names.
+        encoding: The encoding to use when reading the files.
+        relative_to: A str of a path or a Path object for which the event_id
+            will be relative to, if this is omitted then the file's name
+            without extension will be used.
+        create_indices: These indices will be created no matter what,
             even if empty.
 
     Returns:
-        Event: An event containing the text and annotations as labels.
+        An event containing the text and annotations as labels.
 
     """
     txt_file = Path(txt_file)
     ann_file = txt_file.with_suffix('.ann')
     if relative_to is not None:
         relative_to = Path(relative_to)
         event_id = str(txt_file.with_suffix('').relative_to(relative_to))
     else:
         event_id = txt_file.stem
-    with data.Event(event_id=event_id, client=client) as event:
+    with Event(event_id=event_id, client=client) as event:
         with txt_file.open('r', encoding=encoding) as f:
             txt = f.read()
         document = event.create_document(document_name=document_name, text=txt)
-        ann_to_labels(ann_file, document, label_index_name_prefix=label_index_name_prefix,
+        ann_to_labels(ann_file, document,
+                      label_index_name_prefix=label_index_name_prefix,
                       encoding=encoding, create_indices=create_indices)
         yield event
 
 
 def ann_to_labels(ann_file: Union[str, Path],
-                  document: 'mtap.Document',
+                  document: Document,
                   label_index_name_prefix: str,
                   encoding: Optional[str],
                   create_indices: Optional[Iterable[str]] = None):
-    """Reads all of the annotations in a brat annotations file into a document.
+    """Reads all the annotations in a brat annotations file into a document.
 
     Args:
-        ann_file (str or Path): A BRAT .ann file to load annotations from.
-        document (Document): The document to add labels to.
-        label_index_name_prefix (str): A prefix to append to the brat annotation names.
-        encoding (optional str): The encoding to use when reading the ann file.
-        create_indices (optional iterable of str): These indices will be created no matter what,
+        ann_file: A BRAT .ann file to load annotations from.
+        document: The document to add labels to.
+        label_index_name_prefix: A prefix to append to the brat annotation
+            names.
+        encoding: The encoding to use when reading the ann file.
+        create_indices: These indices will be created no matter what,
             even if empty.
     """
     labelers = {}
     if create_indices is not None:
         for index in create_indices:
             labelers[index] = document.get_labeler(index)
     ann_file = Path(ann_file)
```

### Comparing `mtap-1.2.0/python/mtap/serialization/event.schema.json` & `mtap-1.2.1/python/mtap/serialization/event.schema.json`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap/utilities/__init__.py` & `mtap-1.2.1/python/mtap/utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import contextlib
 import os
 import pathlib
-import signal
 import subprocess
 import sys
 import typing
 
-import grpc
-
-
 __all__ = [
     'find_free_port',
     'subprocess_events_server',
     'read_address',
     'write_address_file',
     'tokenization'
 ]
@@ -67,14 +63,16 @@
 
     Returns
     -------
     str
         The address that the events server us running on.
 
     """
+    import grpc
+
     if cwd is None:
         cwd = pathlib.Path.cwd()
     env = dict(os.environ)
     if config_path is not None:
         env['MTAP_CONFIG'] = str(config_path)
     if port is None:
         port = find_free_port()
```

### Comparing `mtap-1.2.0/python/mtap/utilities/tokenization.py` & `mtap-1.2.1/python/mtap/utilities/tokenization.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/mtap.egg-info/PKG-INFO` & `mtap-1.2.1/python/mtap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtap
-Version: 1.2.0
+Version: 1.2.1
 Summary: A framework for distributed text analysis using gRPC and microservices-based architecture.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mtap-1.2.0/python/mtap.egg-info/SOURCES.txt` & `mtap-1.2.1/python/mtap.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -127,69 +127,81 @@
 proto/mtap/api/v1/events.proto
 proto/mtap/api/v1/processing.proto
 python/docs/Makefile
 python/docs/conf.py
 python/docs/deployment.rst
 python/docs/index.rst
 python/docs/make.bat
+python/docs/metrics.rst
 python/docs/mtap.rst
+python/docs/pipeline.rst
+python/docs/processing.rst
 python/docs/serialization.rst
 python/mtap/__init__.py
 python/mtap/__main__.py
+python/mtap/_common.py
 python/mtap/_config.py
-python/mtap/_events_service.py
+python/mtap/_document.py
+python/mtap/_event.py
+python/mtap/_events_client.py
+python/mtap/_events_client_grpc.py
+python/mtap/_events_client_pool.py
+python/mtap/_label_adapters.py
+python/mtap/_label_indices.py
+python/mtap/_labeler.py
+python/mtap/_labels.py
 python/mtap/_structs.py
 python/mtap/constants.py
 python/mtap/defaultConfig.yml
 python/mtap/deployment.py
+python/mtap/descriptors.py
 python/mtap/discovery.py
+python/mtap/events_server.py
 python/mtap/metrics.py
+python/mtap/types.py
 python/mtap/version.py
 python/mtap.egg-info/PKG-INFO
 python/mtap.egg-info/SOURCES.txt
 python/mtap.egg-info/dependency_links.txt
 python/mtap.egg-info/requires.txt
 python/mtap.egg-info/top_level.txt
 python/mtap/api/__init__.py
 python/mtap/api/v1/__init__.py
 python/mtap/api/v1/events_pb2.py
 python/mtap/api/v1/events_pb2_grpc.py
 python/mtap/api/v1/processing_pb2.py
 python/mtap/api/v1/processing_pb2_grpc.py
-python/mtap/data/__init__.py
-python/mtap/data/_base.py
-python/mtap/data/_events.py
-python/mtap/data/_label_adapters.py
-python/mtap/data/_label_indices.py
-python/mtap/data/_labels.py
 python/mtap/examples/__init__.py
 python/mtap/examples/exampleDeploymentConfiguration.yml
 python/mtap/examples/examplePipelineConfiguration.yml
 python/mtap/examples/example_pipeline.py
 python/mtap/examples/example_processor.py
 python/mtap/examples/example_references_processor.py
 python/mtap/examples/print_processor_meta.py
 python/mtap/examples/serialization/__init__.py
 python/mtap/examples/serialization/brat_converter.py
 python/mtap/examples/tutorial/__init__.py
 python/mtap/examples/tutorial/hello.py
 python/mtap/examples/tutorial/pipeline.py
+python/mtap/pipeline/__init__.py
+python/mtap/pipeline/_common.py
+python/mtap/pipeline/_error_handling.py
+python/mtap/pipeline/_mp_config.py
+python/mtap/pipeline/_mp_pipeline.py
+python/mtap/pipeline/_pipeline.py
+python/mtap/pipeline/_pipeline_components.py
+python/mtap/pipeline/_results.py
+python/mtap/pipeline/_sources.py
 python/mtap/processing/__init__.py
-python/mtap/processing/_base.py
-python/mtap/processing/_error_handling.py
 python/mtap/processing/_exc.py
-python/mtap/processing/_mp_config.py
-python/mtap/processing/_mp_pipeline.py
-python/mtap/processing/_pipeline.py
-python/mtap/processing/_pipeline_components.py
-python/mtap/processing/_pipeline_results.py
+python/mtap/processing/_processing_component.py
+python/mtap/processing/_processor.py
 python/mtap/processing/_runners.py
 python/mtap/processing/_service.py
-python/mtap/processing/_sources.py
-python/mtap/processing/descriptions.py
+python/mtap/processing/results.py
 python/mtap/processors/__init__.py
 python/mtap/processors/copy_document.py
 python/mtap/serialization/__init__.py
 python/mtap/serialization/_serialization.py
 python/mtap/serialization/brat.py
 python/mtap/serialization/event.schema.json
 python/mtap/utilities/__init__.py
```

### Comparing `mtap-1.2.0/python/tests/config/test_config.py` & `mtap-1.2.1/python/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/conftest.py` & `mtap-1.2.1/python/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
 import os
-import signal
 import subprocess
 from threading import Thread
 
 import grpc
 import pytest
 
 logging.basicConfig(level=logging.DEBUG)
```

### Comparing `mtap-1.2.0/python/tests/consul/integrationConfig.yaml` & `mtap-1.2.1/python/tests/consul/integrationConfig.yaml`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/consul/test_discovery.py` & `mtap-1.2.1/python/tests/consul/test_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from subprocess import Popen, TimeoutExpired, PIPE, STDOUT
 
 import pytest
 import requests
 from requests import RequestException
 
 import mtap
-from mtap import EventsClient, Event, RemoteProcessor, utilities
+from mtap import events_client, Event, RemoteProcessor, utilities
 from mtap.utilities import subprocess_events_server
 
 
 @pytest.fixture(name='disc_python_events', scope='module')
 def fixture_disc_python_events():
     with subprocess_events_server(cwd=Path(__file__).parents[2],
                                   register=True) as address:
@@ -90,47 +90,47 @@
             p.kill()
             stdout, _ = p.communicate()
             print("api gateway exited with code: ", p.returncode)
             print(stdout.decode('utf-8'))
 
 
 PHASERS = """
-Maybe if we felt any human loss as keenly as we feel one of those close to us, human history would 
-be far less bloody. The Enterprise computer system is controlled by three primary main processor 
-cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface modules. Our 
-neural pathways have become accustomed to your sensory input patterns. Mr. Worf, you do remember 
-how to fire phasers?"""
+Maybe if we felt any human loss as keenly as we feel one of those close to us,
+human history would be far less bloody. The Enterprise computer system is
+controlled by three primary main processor cores, cross-linked with a redundant
+melacortz ramistat, fourteen kiloquad interface modules. Our
+neural pathways have become accustomed to your sensory input patterns. Mr.
+Worf, you do remember how to fire phasers?"""
 
 
 @pytest.mark.consul
 def test_disc_pipeline(disc_python_events, disc_python_processor,
                        disc_java_processor):
     pipeline = mtap.Pipeline(
         RemoteProcessor('mtap-example-processor-python',
                         address='localhost:50501',
                         params={'do_work': True}),
         RemoteProcessor('mtap-example-processor-java',
                         address='localhost:50502',
                         params={'do_work': True})
     )
-    with EventsClient(address=disc_python_events) as client:
+    with events_client() as client:
         with Event(event_id='1', client=client) as event:
             event.metadata['a'] = 'b'
             document = event.create_document('plaintext', PHASERS)
-            result = pipeline.run_multithread([document])
-            letter_counts = document.get_label_index(
-                'mtap.examples.letter_counts')
+            times = pipeline.run_multithread([document])
+            letter_counts = document.labels['mtap.examples.letter_counts']
             a_counts = letter_counts[0]
             assert a_counts.count == 23
             b_counts = letter_counts[1]
             assert b_counts.count == 6
-            result.print_times()
-            thes = document.get_label_index("mtap.examples.word_occurrences")
-            assert thes[0].start_index == 121
-            assert thes[0].end_index == 124
+            times.print()
+            thes = document.labels["mtap.examples.word_occurrences"]
+            assert thes[0].start_index == 120
+            assert thes[0].end_index == 123
 
 
 @pytest.mark.consul
 def test_disc_api_gateway(disc_api_gateway):
     session = requests.Session()
     session.trust_env = False
     resp = session.get(f"http://{disc_api_gateway}/v1/processors", timeout=10)
```

### Comparing `mtap-1.2.0/python/tests/data/test_document.py` & `mtap-1.2.1/python/tests/data/test_document.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,113 +8,110 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from mtap import Event, EventsClient, Document, GenericLabel
-from mtap.data import DISTINCT_GENERIC_ADAPTER, GENERIC_ADAPTER
+from mtap import Event, Document, GenericLabel
+from mtap._label_adapters import GENERIC_ADAPTER, DISTINCT_GENERIC_ADAPTER
+from mtap.types import EventsClient
 
 
 def test_add_labels_not_distinct(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_label_index_info.return_value = []
     event = Event(event_id='1', client=client)
     document = Document(document_name='plaintext',
-                        text='The quick brown fox jumped over the lazy dog.', event=event)
+                        text='The quick brown fox jumped over the lazy dog.',
+                        event=event)
     labels = [
         GenericLabel(0, 10, document=document, x=1),
         GenericLabel(11, 15, document=document, x=2),
         GenericLabel(16, 20, document=document, x=3)
     ]
     document.add_labels('index', labels)
-    client.add_labels.assert_called_with(
-        event_id='1',
-        document_name='plaintext',
-        index_name='index',
-        labels=labels,
-        adapter=mocker.ANY
-    )
+    client.add_labels.assert_called_with('0', '1', 'plaintext',
+                                         index_name='index',
+                                         labels=labels,
+                                         adapter=mocker.ANY
+                                         )
     l2 = document.labels['index']
     assert l2 == labels
     assert not l2.distinct
 
 
 def test_add_labels_distinct(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_label_index_info.return_value = []
     event = Event(event_id='1', client=client)
     document = Document(document_name='plaintext',
-                        text='The quick brown fox jumped over the lazy dog.', event=event)
+                        text='The quick brown fox jumped over the lazy dog.',
+                        event=event)
     labels = [
         GenericLabel(0, 10, document=document, x=1),
         GenericLabel(11, 15, document=document, x=2),
         GenericLabel(16, 20, document=document, x=3)
     ]
     document.add_labels('index', labels, distinct=True)
-    client.add_labels.assert_called_with(
-        event_id='1',
-        document_name='plaintext',
-        index_name='index',
-        labels=labels,
-        adapter=mocker.ANY
-    )
+    client.add_labels.assert_called_with('0', '1', 'plaintext',
+                                         index_name='index',
+                                         labels=labels,
+                                         adapter=mocker.ANY
+                                         )
     l2 = document.labels['index']
     assert l2 == labels
     assert l2.distinct
 
 
 def test_labeler_not_distinct_default(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_label_index_info.return_value = []
     event = Event(event_id='1', client=client)
     document = Document(document_name='plaintext',
-                        text='The quick brown fox jumped over the lazy dog.', event=event)
+                        text='The quick brown fox jumped over the lazy dog.',
+                        event=event)
     with document.get_labeler('index') as add_generic_label:
         add_generic_label(0, 10, x=1)
         add_generic_label(11, 15, x=2)
         add_generic_label(16, 20, x=3)
     labels = [
         GenericLabel(0, 10, document=document, x=1),
         GenericLabel(11, 15, document=document, x=2),
         GenericLabel(16, 20, document=document, x=3)
     ]
     label_adapter = GENERIC_ADAPTER
-    client.add_labels.assert_called_with(
-        event_id='1',
-        document_name='plaintext',
-        index_name='index',
-        labels=labels,
-        adapter=label_adapter
-    )
+    client.add_labels.assert_called_with('0', '1', 'plaintext',
+                                         index_name='index',
+                                         labels=labels,
+                                         adapter=label_adapter
+                                         )
     assert document.labels['index'] == labels
 
 
 def test_labeler_distinct(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_label_index_info.return_value = []
     event = Event(event_id='1', client=client)
     document = Document(document_name='plaintext',
-                        text='The quick brown fox jumped over the lazy dog.', event=event)
+                        text='The quick brown fox jumped over the lazy dog.',
+                        event=event)
     with document.get_labeler('index', distinct=True) as add_generic_label:
         add_generic_label(0, 10, x=1)
         add_generic_label(11, 15, x=2)
         add_generic_label(16, 20, x=3)
     labels = [
         GenericLabel(0, 10, document=document, x=1),
         GenericLabel(11, 15, document=document, x=2),
         GenericLabel(16, 20, document=document, x=3)
     ]
     label_adapter = DISTINCT_GENERIC_ADAPTER
-    client.add_labels.assert_called_with(
-        event_id='1',
-        document_name='plaintext',
-        index_name='index',
-        labels=labels,
-        adapter=label_adapter
-    )
+    client.add_labels.assert_called_with('0', '1', 'plaintext',
+                                         index_name='index',
+                                         labels=labels,
+                                         adapter=label_adapter
+                                         )
     assert document.labels['index'] == labels
```

### Comparing `mtap-1.2.0/python/tests/data/test_event.py` & `mtap-1.2.1/python/tests/data/test_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,33 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pytest
 
-from mtap.data._events import EventsClient, Event, Document
+from mtap import Event, Document
+from mtap.types import EventsClient
 
 
 def test_add_document(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     event = Event(event_id='1', client=client)
     document = Document('plaintext',
                         text="“You're no help,” he told the lime. "
                              "This was unfair. It was only a lime; "
                              "there was nothing special about it at all. "
                              "It was doing the best it could.")
     event.add_document(document)
     assert event.documents['plaintext'] == document
-    client.add_document.assert_called_once_with('1', 'plaintext',
-                                                "“You're no help,” he told the lime. "
-                                                "This was unfair. It was only a lime; "
-                                                "there was nothing special about it at all. "
-                                                "It was doing the best it could.")
+    client.add_document.assert_called_once_with(
+        '0', '1', 'plaintext',
+        "“You're no help,” he told the lime. "
+        "This was unfair. It was only a lime; "
+        "there was nothing special about it at all. "
+        "It was doing the best it could."
+    )
 
 
 def test_add_document_no_client():
     event = Event(event_id='1')
     document = Document('plaintext',
                         text="“You're no help,” he told the lime. "
                              "This was unfair. It was only a lime; "
@@ -43,83 +46,88 @@
                              "It was doing the best it could.")
     event.add_document(document)
     assert event.documents['plaintext'] == document
 
 
 def test_create_document(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     event = Event(event_id='1', client=client)
-    document = event.create_document('plaintext', "“You're no help,” he told the lime. "
-                                                  "This was unfair. It was only a lime; "
-                                                  "there was nothing special about it at all. "
-                                                  "It was doing the best it could.")
+    document = event.create_document(
+        'plaintext',
+        "“You're no help,” he told the lime. "
+        "This was unfair. It was only a lime; "
+        "there was nothing special about it at all. "
+        "It was doing the best it could.")
     assert event.documents['plaintext'] == document
-    client.add_document.assert_called_once_with('1', 'plaintext',
-                                                "“You're no help,” he told the lime. "
-                                                "This was unfair. It was only a lime; "
-                                                "there was nothing special about it at all. "
-                                                "It was doing the best it could.")
+    client.add_document.assert_called_once_with(
+        '0', '1', 'plaintext',
+        "“You're no help,” he told the lime. "
+        "This was unfair. It was only a lime; "
+        "there was nothing special about it at all. "
+        "It was doing the best it could.")
 
 
 def test_create_document_no_client():
     event = Event(event_id='1')
-    document = event.create_document('plaintext', "“You're no help,” he told the lime. "
-                                                  "This was unfair. It was only a lime; "
-                                                  "there was nothing special about it at all. "
-                                                  "It was doing the best it could.")
+    document = event.create_document(
+        'plaintext',
+        "“You're no help,” he told the lime. "
+        "This was unfair. It was only a lime; "
+        "there was nothing special about it at all. "
+        "It was doing the best it could.")
     assert event.documents['plaintext'] == document
 
 
 def test_get_document(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_all_document_names.return_value = ['plaintext']
     event = Event(event_id='1', client=client)
     document = event.documents['plaintext']
     assert document.document_name == 'plaintext'
 
 
 def test_get_document_missing(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_all_document_names.return_value = ['plaintext']
     event = Event(event_id='1', client=client)
     with pytest.raises(KeyError):
         _ = event.documents['foo']
 
 
 def test_get_document_missing_no_client():
     event = Event(event_id='1')
     with pytest.raises(KeyError):
         _ = event.documents['foo']
 
 
 def test_iter_documents(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_all_document_names.return_value = ['plaintext', 'two', 'three']
     event = Event(event_id='1', client=client)
     documents = {document for document in event.documents}
     assert documents == {'plaintext', 'two', 'three'}
 
 
 def test_contains_documents(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_all_document_names.return_value = ['plaintext', 'two', 'three']
     event = Event(event_id='1', client=client)
     assert 'plaintext' in event.documents
     assert 'two' in event.documents
     assert 'four' not in event.documents
 
 
 def test_documents_len(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
+    client.open_event.return_value = '0'
     client.get_all_document_names.return_value = ['plaintext', 'two', 'three']
     event = Event(event_id='1', client=client)
     assert len(event.documents) == 3
 
 
 def test_created_indices_no_documents():
     event = Event(event_id='1')
```

### Comparing `mtap-1.2.0/python/tests/data/test_events_client.py` & `mtap-1.2.1/python/tests/data/test_events_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 from concurrent.futures.thread import ThreadPoolExecutor
 
 import grpc_testing
 import pytest
 from grpc import StatusCode
 
-from mtap import EventsClient
-from mtap.api.v1 import events_pb2, events_pb2_grpc
-from mtap.data import LabelIndexType, LabelIndexInfo
+from mtap._events_client_grpc import GrpcEventsClient
+from mtap._label_indices import LabelIndexType
+from mtap.api.v1 import events_pb2
 
 
 @pytest.fixture(name='events_channel')
 def fixture_events_channel():
     yield grpc_testing.channel(
         [
             events_pb2.DESCRIPTOR.services_by_name['Events']
@@ -37,30 +37,33 @@
     executor = ThreadPoolExecutor(max_workers=1)
     yield executor
     executor.shutdown(wait=True)
 
 
 def test_get_label_index_info(events_channel, events_client_executor):
     def call():
-        client = EventsClient(address='a', _pool=object(), _channel=events_channel)
-        result = client.get_label_index_info(event_id='1', document_name='plaintext')
+        client = GrpcEventsClient(address='a', channel=events_channel)
+        result = client.get_label_index_info(instance_id='0', event_id='1',
+                                             document_name='plaintext')
         return result
 
     future = events_client_executor.submit(call)
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetEventsInstanceId']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetEventsInstanceId']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.GetEventsInstanceIdResponse()
     response.instance_id = '0'
     rpc.terminate(response, None, StatusCode.OK, '')
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetLabelIndicesInfo']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetLabelIndicesInfo']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.GetLabelIndicesInfoResponse()
     first = response.label_index_infos.add()
     first.index_name = 'foo'
     first.type = events_pb2.GetLabelIndicesInfoResponse.LabelIndexInfo.GENERIC
     second = response.label_index_infos.add()
@@ -80,81 +83,91 @@
     assert infos[1].type == LabelIndexType.CUSTOM
     assert infos[2].index_name == 'baz'
     assert infos[2].type == LabelIndexType.UNKNOWN
 
 
 def test_get_binary_data_names(events_channel, events_client_executor):
     def call():
-        client = EventsClient(address='a', _pool=object(), _channel=events_channel)
-        result = client.get_all_binary_data_names(event_id='1')
+        client = GrpcEventsClient(address='a', channel=events_channel)
+        result = client.get_all_binary_data_names(instance_id='0',
+                                                  event_id='1')
         return result
 
     future = events_client_executor.submit(call)
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetEventsInstanceId']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetEventsInstanceId']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.GetEventsInstanceIdResponse()
     response.instance_id = '0'
     rpc.terminate(response, None, StatusCode.OK, '')
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetAllBinaryDataNames']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetAllBinaryDataNames']
     )
     rpc.send_initial_metadata(())
-    response = events_pb2.GetAllBinaryDataNamesResponse(binary_data_names=['a', 'b', 'c'])
+    response = events_pb2.GetAllBinaryDataNamesResponse(
+        binary_data_names=['a', 'b', 'c'])
     rpc.terminate(response, None, StatusCode.OK, '')
 
     assert future.result(5) == ['a', 'b', 'c']
 
 
 def test_add_binary_data(events_channel, events_client_executor):
     def call():
-        client = EventsClient(address='a', _pool=object(), _channel=events_channel)
-        result = client.add_binary_data(event_id='1', binary_data_name='foo', binary_data=b'\xFF')
+        client = GrpcEventsClient(address='a', channel=events_channel)
+        result = client.add_binary_data(instance_id='0', event_id='1',
+                                        binary_data_name='foo',
+                                        binary_data=b'\xFF')
         return result
 
     events_client_executor.submit(call)
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetEventsInstanceId']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetEventsInstanceId']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.GetEventsInstanceIdResponse()
     response.instance_id = '0'
     rpc.terminate(response, None, StatusCode.OK, '')
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['AddBinaryData']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'AddBinaryData']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.AddBinaryDataResponse()
     rpc.terminate(response, None, StatusCode.OK, '')
     assert req.binary_data == b'\xFF'
 
 
 def test_get_binary_data(events_channel, events_client_executor):
     def call():
-        client = EventsClient(address='a', _pool=object(), _channel=events_channel)
-        result = client.get_binary_data(event_id='1', binary_data_name='foo')
+        client = GrpcEventsClient(address='a', channel=events_channel)
+        result = client.get_binary_data('0', event_id='1', binary_data_name='foo')
         return result
 
     future = events_client_executor.submit(call)
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetEventsInstanceId']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetEventsInstanceId']
     )
     rpc.send_initial_metadata(())
     response = events_pb2.GetEventsInstanceIdResponse()
     response.instance_id = '0'
     rpc.terminate(response, None, StatusCode.OK, '')
 
     _, req, rpc = events_channel.take_unary_unary(
-        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name['GetBinaryData']
+        events_pb2.DESCRIPTOR.services_by_name['Events'].methods_by_name[
+            'GetBinaryData']
     )
     assert req.event_id == '1'
     assert req.binary_data_name == 'foo'
     rpc.send_initial_metadata(())
     response = events_pb2.GetBinaryDataResponse(binary_data=b'\xFF')
     rpc.terminate(response, None, StatusCode.OK, '')
```

### Comparing `mtap-1.2.0/python/tests/data/test_generic_label.py` & `mtap-1.2.1/python/tests/data/test_generic_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,19 @@
 def test_set_document():
     label = GenericLabel(0, 4)
     label.document = document
     assert label.document == document
 
 
 def test_try_assign_reserved():
-    l = GenericLabel(0, 0)
+    label = GenericLabel(0, 0)
     with pytest.raises(ValueError):
-        l.location = 10
+        label.location = 10
     with pytest.raises(ValueError):
-        l.text = 'blah'
+        label.text = 'blah'
 
 
 def test_construct_with_reserved():
     with pytest.raises(ValueError):
         GenericLabel(0, 0, location=1)
     with pytest.raises(ValueError):
         GenericLabel(0, 0, text='some text')
```

### Comparing `mtap-1.2.0/python/tests/data/test_labels.py` & `mtap-1.2.1/python/tests/data/test_labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 def test_text_from_document():
     d = Document('plaintext', text='This is text.')
     assert GenericLabel(5, 7, document=d).text == 'is'
 
 
 def test_label_location():
-    l = GenericLabel(0, 10)
-    assert l.location == Location(0, 10)
+    label = GenericLabel(0, 10)
+    assert label.location == Location(0, 10)
 
 
 def test_location_relative_to():
     first = Location(10, 20)
     assert first.relative_to(5) == Location(5, 15)
     assert first.relative_to(GenericLabel(5, 25)) == Location(5, 15)
     assert first.relative_to(Location(5, 25)) == Location(5, 15)
```

### Comparing `mtap-1.2.0/python/tests/data/test_standard_ascending_label_index.py` & `mtap-1.2.1/python/tests/data/test_standard_ascending_label_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
 from mtap import GenericLabel, Location, Document
-from mtap.data._label_indices import presorted_label_index, label_index
+from mtap._label_indices import presorted_label_index, label_index
 
 
 document = Document('plaintext', text='blah')
 
 
 @pytest.fixture
 def tested():
@@ -378,16 +378,16 @@
 
 
 def test_contains_false_not_label(tested):
     assert "blub" not in tested
 
 
 def test_reversed(tested):
-    l = list(reversed(tested))
-    assert l == [
+    rev = list(reversed(tested))
+    assert rev == [
         GenericLabel(9, 13, document=document, i=7),
         GenericLabel(9, 13, document=document, i=6),
         GenericLabel(9, 10, document=document, i=5),
         GenericLabel(6, 8, document=document, i=4),
         GenericLabel(6, 7, document=document, i=3),
         GenericLabel(2, 6, document=document, i=2),
         GenericLabel(0, 7, document=document, i=1),
```

### Comparing `mtap-1.2.0/python/tests/data/test_standard_descending_label_index.py` & `mtap-1.2.1/python/tests/data/test_standard_descending_label_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 import pytest
 
 from mtap import GenericLabel, Location, Document
-from mtap.data._label_indices import presorted_label_index
+from mtap._label_indices import presorted_label_index
 
 
 document = Document('plaintext', text='blah')
 
 
 @pytest.fixture
 def tested():
@@ -369,16 +369,16 @@
 
 
 def test_contains_false_not_label(tested):
     assert "blub" not in tested
 
 
 def test_reversed(tested):
-    l = list(reversed(tested))
-    assert l == [
+    rev = list(reversed(tested))
+    assert rev == [
         GenericLabel(0, 5, document=document, i=7),
         GenericLabel(0, 7, document=document, i=6),
         GenericLabel(2, 6, document=document, i=5),
         GenericLabel(6, 7, document=document, i=4),
         GenericLabel(6, 8, document=document, i=3),
         GenericLabel(9, 10, document=document, i=2),
         GenericLabel(9, 13, document=document, i=1),
```

### Comparing `mtap-1.2.0/python/tests/deployment/test_deployment.py` & `mtap-1.2.1/python/tests/deployment/test_deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import pytest
 
-import mtap
-from mtap import RemoteProcessor, EventsClient
+from mtap import RemoteProcessor, Pipeline, events_client, Event
 from mtap.deployment import Deployment, ProcessorDeployment
 
 text = """
 Why, friends, you go to do you know not what:
 Wherein hath Caesar thus deserved your loves?
 Alas, you know not: I must tell you then:
 You have forgot the will I told you of.
@@ -41,35 +40,32 @@
     from importlib_resources import files, as_file
     deployment_config = files('mtap.examples').joinpath('exampleDeploymentConfiguration.yml')
     run_config = files('mtap.examples').joinpath('examplePipelineConfiguration.yml')
     with as_file(deployment_config) as deployment_f, as_file(run_config) as run_f:
         deployment = Deployment.from_yaml_file(deployment_f)
         deployment.global_settings.log_level = 'DEBUG'
         deployment.shared_processor_config.java_classpath = java_exe[-1]
-        deployment.shared_processor_config.jvm_args = ["-Dorg.slf4j.simpleLogger.log.edu.umn.nlpie.mtap=debug"]
+        deployment.shared_processor_config.jvm_args = [
+            "-Dorg.slf4j.simpleLogger.log.edu.umn.nlpie.mtap=debug"
+        ]
         deployment.processors.append(ProcessorDeployment(
             implementation='python',
             entry_point='mtap.examples.tutorial.hello',
             port=10103
         ))
         with deployment.run_servers():
-            pipeline = mtap.Pipeline.from_yaml_file(run_f)
+            pipeline = Pipeline.from_yaml_file(run_f)
             pipeline.append(
                 RemoteProcessor(
                     processor_name='hello',
                     address='127.0.0.1:10103'
                 )
             )
-            pipeline.mp_config.close_events = False
-            with EventsClient(deployment.events_deployment.address) as c:
-                with mtap.Event(client=c) as e:
-                    d = e.create_document('plaintext', text)
-                    results = pipeline.run(d)
-                    assert results is not None
-                with mtap.Event(client=c) as e:
+            with events_client(deployment.events_deployment.address) as c:
+                with Event(client=c) as e:
                     d = e.create_document('plaintext', text)
 
                     def source():
                         yield d
 
                     pipeline.run_multithread(source(), total=1, log_level='DEBUG')
                     assert len(d.labels['mtap.examples.letter_counts']) > 0
```

### Comparing `mtap-1.2.0/python/tests/integration/test_hello_world_tutorial.py` & `mtap-1.2.1/python/tests/integration/test_hello_world_tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 import sys
 from subprocess import PIPE, STDOUT, Popen, run
 
 import pytest
 
 from mtap.utilities import find_free_port, subprocess_events_server
```

### Comparing `mtap-1.2.0/python/tests/integration/test_integration.py` & `mtap-1.2.1/python/tests/integration/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 try:
     from yaml import CDumper as Dumper
 except ImportError:
     from yaml import Dumper
 from requests import RequestException
 
 import mtap
-from mtap import EventsClient, Event, RemoteProcessor
+from mtap import events_client, Event, RemoteProcessor
 from mtap.utilities import subprocess_events_server, find_free_port
 
 os.environ['no_proxy'] = '127.0.0.1,localhost'
 
 
 @pytest.fixture(name='python_events')
 def fixture_python_events():
@@ -132,46 +132,46 @@
                 p.kill()
                 stdout, _ = p.communicate()
                 print("api gateway exited with code: ", p.returncode)
                 print(stdout.decode('utf-8'))
 
 
 PHASERS = """
-Maybe if we felt any human loss as keenly as we feel one of those close to us, human history would 
-be far less bloody. The Enterprise computer system is controlled by three primary main processor 
-cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface modules. Our 
-neural pathways have become accustomed to your sensory input patterns. Mr. Worf, you do remember 
-how to fire phasers?"""
+Maybe if we felt any human loss as keenly as we feel one of those close to us,
+human history would be far less bloody. The Enterprise computer system is
+controlled by three primary main processor cores, cross-linked with a redundant
+melacortz ramistat, fourteen kiloquad interface modules. Our
+neural pathways have become accustomed to your sensory input patterns. Mr.
+Worf, you do remember how to fire phasers?"""
 
 
 @pytest.mark.integration
 def test_pipeline(python_events, python_processor, java_processor):
     pipeline = mtap.Pipeline(
         RemoteProcessor('mtap-example-processor-python',
                         address=python_processor,
                         params={'do_work': True}),
         RemoteProcessor('mtap-example-processor-java',
                         address=java_processor,
                         params={'do_work': True})
     )
-    with EventsClient(address=python_events) as client:
+    with events_client(address=python_events) as client:
         with Event(event_id='1', client=client) as event:
             event.metadata['a'] = 'b'
             document = event.create_document('plaintext', PHASERS)
             result = pipeline.run_multithread([document])
-            letter_counts = document.get_label_index(
-                'mtap.examples.letter_counts')
+            letter_counts = document.labels['mtap.examples.letter_counts']
             a_counts = letter_counts[0]
             assert a_counts.count == 23
             b_counts = letter_counts[1]
             assert b_counts.count == 6
-            result.print_times()
-            thes = document.get_label_index("mtap.examples.word_occurrences")
-            assert thes[0].start_index == 121
-            assert thes[0].end_index == 124
+            result.print()
+            thes = document.labels["mtap.examples.word_occurrences"]
+            assert thes[0].start_index == 120
+            assert thes[0].end_index == 123
 
 
 @pytest.mark.integration
 @pytest.mark.gateway
 def test_api_gateway(python_events, python_processor, java_processor,
                      api_gateway):
     session = requests.Session()
@@ -334,16 +334,16 @@
         timeout=1
     )
     assert resp.status_code == 200
     labels = resp.json()['generic_labels']['labels']
     assert labels == [
         {
             'identifier': 0,
-            'start_index': 121,
-            'end_index': 124,
+            'start_index': 120,
+            'end_index': 123,
             'fields': {},
             'reference_ids': {}
         }
     ]
 
     resp = session.get(
         base_url + "/v1/events/1/documents/plaintext/labels",
```

### Comparing `mtap-1.2.0/python/tests/processing/test_event_processor.py` & `mtap-1.2.1/python/tests/processing/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/processing/test_pipeline.py` & `mtap-1.2.1/python/tests/processing/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
+
+
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import pickle
@@ -18,20 +20,20 @@
 from pathlib import Path
 from typing import Dict, Any
 
 from mtap import (
     Pipeline,
     EventProcessor,
     Event,
-    EventsClient,
     processor,
     RemoteProcessor,
     LocalProcessor
 )
-from mtap.processing import MpConfig, SimpleErrorHandler, \
+from mtap._events_client import EventsClient
+from mtap.pipeline import MpConfig, SimpleErrorHandler, \
     TerminationErrorHandler
 
 
 @processor('test-processor')
 class Processor(EventProcessor):
     def __init__(self, identifier='1'):
         self.identifier = identifier
@@ -46,15 +48,14 @@
         event.metadata[self.identifier] = 'True'
         event.metadata['processor'] = self.identifier
         self.processed += 1
 
 
 def test_time_result(mocker):
     client = mocker.Mock(EventsClient)
-    client.get_local_instance.return_value = client
     client.get_all_document_names.return_value = ['plaintext']
     client.get_all_metadata.return_value = {}
     client.instance_id = 0
     pipeline = Pipeline(
         LocalProcessor(Processor(),
                        component_id='test_processor')
     )
```

### Comparing `mtap-1.2.0/python/tests/processing/test_pipeline_result.py` & `mtap-1.2.1/python/tests/processing/test_pipeline_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from datetime import timedelta
 
 import pytest
 
-from mtap.processing import PipelineResult, ComponentResult
+from mtap.processing.results import ComponentResult
+from mtap.pipeline import PipelineResult
 
 
 def test_component_result():
     result = PipelineResult(
         component_results=[
             ComponentResult(
                 identifier='a',
```

### Comparing `mtap-1.2.0/python/tests/processing/test_processor_service.py` & `mtap-1.2.1/python/tests/processing/test_processor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import grpc
 import grpc_testing
 import pytest
 
 from mtap import processor, Document, DocumentProcessor
 from mtap.api.v1 import processing_pb2
 from mtap.processing import _runners
-from mtap.processing.descriptions import parameter, labels, label_property
+from mtap.descriptors import parameter, labels, label_property
 from mtap.processing._service import _ProcessorServicer
 
 
 @processor('mtap-test-processor',
            description='Processor desc.',
            parameters=[
                parameter('a_param', required=True, data_type='bool',
```

### Comparing `mtap-1.2.0/python/tests/processors/test_copy_document.py` & `mtap-1.2.1/python/tests/processors/test_copy_document.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/references/test_references.py` & `mtap-1.2.1/python/tests/references/test_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import sys
 from pathlib import Path
 from subprocess import Popen, PIPE, STDOUT
 
 import pytest
 
-from mtap import EventsClient, Pipeline, Event, GenericLabel, RemoteProcessor
+from mtap import events_client, Pipeline, Event, GenericLabel, RemoteProcessor
 from mtap.utilities import subprocess_events_server, find_free_port
 
 
 @pytest.fixture(name='python_events')
 def fixture_python_events():
     with subprocess_events_server(cwd=Path(__file__).parents[2]) as address:
         yield address
@@ -54,15 +54,15 @@
 
 @pytest.mark.integration
 def test_java_references(python_events, java_references_processor):
     pipeline = Pipeline(
         RemoteProcessor('mtap-java-reference-labels-example-processor',
                         address=java_references_processor)
     )
-    with EventsClient(python_events) as c, \
+    with events_client(python_events) as c, \
             Event(event_id='1', client=c) as event:
         document = event.create_document('plaintext', 'abcd')
         pipeline.run(document)
         references = document.labels['references']
         assert references[0].a == GenericLabel(0, 1)
         assert references[0].b == GenericLabel(1, 2)
         assert references[1].a == GenericLabel(2, 3)
@@ -85,15 +85,15 @@
 
 @pytest.mark.integration
 def test_python_references(python_events, python_references_processor):
     pipeline = Pipeline(
         RemoteProcessor('mtap-python-references-example',
                         address=python_references_processor)
     )
-    with EventsClient(python_events) as client, \
+    with events_client(python_events) as client, \
             Event(event_id='1', client=client) as event:
         document = event.create_document('plaintext', 'abcd')
         pipeline.run(document)
         references = document.labels['references']
         assert references[0].a == GenericLabel(0, 1)
         assert references[0].b == GenericLabel(1, 2)
         assert references[1].a == GenericLabel(2, 3)
```

### Comparing `mtap-1.2.0/python/tests/serialization/brat/100_1442.txt` & `mtap-1.2.1/python/tests/serialization/brat/100_1442.txt`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/serialization/test_brat.py` & `mtap-1.2.1/python/tests/serialization/test_brat.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/serialization/test_json.py` & `mtap-1.2.1/python/tests/serialization/test_json.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/serialization/test_pickle.py` & `mtap-1.2.1/python/tests/serialization/test_pickle.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/serialization/test_serialization.py` & `mtap-1.2.1/python/tests/serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/serialization/test_yml.py` & `mtap-1.2.1/python/tests/serialization/test_yml.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from tempfile import TemporaryFile
 
-try:
-    from yaml import CLoader as Loader, CDumper as Dumper
-except ImportError:
-    from yaml import Loader, Dumper
-
 from mtap import Event, Document, label
 from mtap.serialization import YamlSerializer
 
 
 def test_yml_serializer():
     event = Event(event_id='1')
     event.metadata['foo'] = "bar"
```

### Comparing `mtap-1.2.0/python/tests/slf4j-simple-2.0.3.jar` & `mtap-1.2.1/python/tests/slf4j-simple-2.0.3.jar`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/python/tests/test_events_service.py` & `mtap-1.2.1/python/tests/test_events_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import grpc
 import grpc_testing
 import pytest
 
-from mtap._events_service import EventsServicer
+from mtap.events_server import EventsServicer
 from mtap.api.v1 import events_pb2
 
-PHASERS = """Maybe if we felt any human loss as keenly as we feel one of those close to us, human 
-history would be far less bloody. The Enterprise computer system is controlled by three primary 
-main processor cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface 
-modules. Our neural pathways have become accustomed to your sensory input patterns. Mr. Worf, you 
-do remember how to fire phasers?"""
+
+PHASERS = """
+Maybe if we felt any human loss as keenly as we feel one of those close to us,
+human history would be far less bloody. The Enterprise computer system is
+controlled by three primary main processor cores, cross-linked with a redundant
+melacortz ramistat, fourteen kiloquad interface modules. Our
+neural pathways have become accustomed to your sensory input patterns. Mr.
+Worf, you do remember how to fire phasers?"""
 
 
 @pytest.fixture(name='events_server')
 def fixture_events_server():
     events_service = EventsServicer()
     yield grpc_testing.server_from_dictionary(
         {
```

### Comparing `mtap-1.2.0/python/tests/test_metrics.py` & `mtap-1.2.1/python/tests/test_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 
-import serialization
-
 from mtap import Event
-from mtap.metrics import Accuracy, Metrics, FirstTokenConfusion, ConfusionMatrix
+from mtap.metrics import Accuracy, Metrics, FirstTokenConfusion, \
+    ConfusionMatrix
 
 
 def test_accuracy():
     with Event(event_id='1') as event:
         doc = event.create_document('test', 'This is some text.')
         with doc.get_labeler('tested') as tested:
             tested(0, 5)
@@ -95,15 +94,18 @@
         metrics = Metrics(acc, tested='tested', target='target')
         metrics.process_document(doc, params={})
         assert abs(acc.value - 0.8) < 1e-6
 
 
 def test_begin_token_precision_recall_f1():
     with Event() as event:
-        doc = event.create_document('test', 'The quick brown fox jumps over the lazy dog.')
+        doc = event.create_document(
+            'test',
+            'The quick brown fox jumps over the lazy dog.'
+        )
         with doc.get_labeler('tested') as label_tested:
             label_tested(0, 9)
             label_tested(10, 19)
             label_tested(20, 44)
         with doc.get_labeler('target') as label_target:
             label_target(0, 19)
             label_target(20, 30)
@@ -131,45 +133,54 @@
     assert first.true_positives == 5
     assert first.false_positives == 3
     assert first.false_negatives == 6
 
 
 def test_print_debug_fn():
     event = Event()
-    doc = event.create_document('test', 'The quick brown fox jumps over the lazy dog.')
+    doc = event.create_document('test',
+                                'The quick brown fox jumps over the lazy dog.')
     with doc.get_labeler('target') as label_target:
         label_target(16, 19)
     with doc.get_labeler('tested') as label_tested:
         label_tested(10, 15)
 
     string_io = io.StringIO()
     metric = FirstTokenConfusion(print_debug='fn', debug_handle=string_io)
     metric.update(doc, doc.labels['tested'], doc.labels['target'])
-    assert string_io.getvalue() == 'False Negatives\nThe quick brown {fox} jumps over the lazy dog.\n\n'
+    expected = 'False Negatives\nThe quick brown {fox} jumps over the lazy ' \
+               'dog.\n\n'
+    assert (string_io.getvalue() == expected)
 
 
 def test_print_debug_fp():
     event = Event()
-    doc = event.create_document('test', 'The quick brown fox jumps over the lazy dog.')
+    doc = event.create_document('test',
+                                'The quick brown fox jumps over the lazy dog.')
     with doc.get_labeler('target') as label_target:
         label_target(16, 19)
     with doc.get_labeler('tested') as label_tested:
         label_tested(10, 15)
 
     string_io = io.StringIO()
     metric = FirstTokenConfusion(print_debug='fp', debug_handle=string_io)
     metric.update(doc, doc.labels['tested'], doc.labels['target'])
-    assert string_io.getvalue() == 'False Positives\nThe quick {brown} fox jumps over the lazy dog.\n\n'
+    assert string_io.getvalue() == 'False Positives\nThe quick {brown} fox ' \
+                                   'jumps over the lazy dog.\n\n'
 
 
 def test_print_debug_all():
     event = Event()
-    doc = event.create_document('test', 'The quick brown fox jumps over the lazy dog.')
+    doc = event.create_document('test',
+                                'The quick brown fox jumps over the lazy dog.')
     with doc.get_labeler('target') as label_target:
         label_target(16, 19)
     with doc.get_labeler('tested') as label_tested:
         label_tested(10, 15)
 
     string_io = io.StringIO()
     metric = FirstTokenConfusion(print_debug='all', debug_handle=string_io)
     metric.update(doc, doc.labels['tested'], doc.labels['target'])
-    assert string_io.getvalue() == 'False Positives\nThe quick {brown} fox jumps over the lazy dog.\n\nFalse Negatives\nThe quick brown {fox} jumps over the lazy dog.\n\n'
+    assert string_io.getvalue() == 'False Positives\nThe quick {brown} fox ' \
+                                   'jumps over the lazy dog.\n\nFalse ' \
+                                   'Negatives\nThe quick brown {fox} jumps ' \
+                                   'over the lazy dog.\n\n'
```

### Comparing `mtap-1.2.0/python/tests/test_structs.py` & `mtap-1.2.1/python/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `mtap-1.2.0/setup.py` & `mtap-1.2.1/setup.py`

 * *Files identical despite different names*

