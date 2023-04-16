# Comparing `tmp/to-cloud-run-1.1.tar.gz` & `tmp/to-cloud-run-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.1.tar", last modified: Sun Apr 16 15:20:25 2023, max compression
+gzip compressed data, was "to-cloud-run-1.2.tar", last modified: Sun Apr 16 23:25:27 2023, max compression
```

## Comparing `to-cloud-run-1.1.tar` & `to-cloud-run-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:20:25.721536 to-cloud-run-1.1/
--rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:20:25.721269 to-cloud-run-1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2121 2023-04-16 15:20:19.000000 to-cloud-run-1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       38 2023-04-16 15:20:25.721601 to-cloud-run-1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      510 2023-04-16 15:20:19.000000 to-cloud-run-1.1/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:20:25.721019 to-cloud-run-1.1/to_cloud_run.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      252 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       52 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      103 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)     2936 2023-04-16 15:20:18.000000 to-cloud-run-1.1/to_cloud_run.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-16 23:25:27.887461 to-cloud-run-1.2/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-16 23:25:27.887314 to-cloud-run-1.2/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-16 23:25:27.000000 to-cloud-run-1.2/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-16 23:25:27.887506 to-cloud-run-1.2/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-16 23:25:27.000000 to-cloud-run-1.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-16 23:25:27.887114 to-cloud-run-1.2/to_cloud_run.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3127 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.py
```

### Comparing `to-cloud-run-1.1/to_cloud_run.py` & `to-cloud-run-1.2/to_cloud_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python
 from argparse import ArgumentParser
 from os import getenv, system, path
 
 from dotenv import load_dotenv
 
-load_dotenv()
-
 
 def create_dockerfile():
     if not path.exists('./Dockerfile'):
         dockerfile = """
 FROM python:3.9-slim
 WORKDIR /app
 COPY requirements.txt .
@@ -18,63 +16,66 @@
 EXPOSE 8000
 CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]
 """
         with open('./Dockerfile', 'w') as f:
             f.write(dockerfile)
 
 
-def build_docker_image(platform='linux/amd64', tag='1.9.0'):
+def build_docker_image(service_name, platform='linux/amd64', tag='1.9.0'):
     create_dockerfile()
-    system(f'docker build --platform {platform} -t to-pip .')
-    image_repo = f'gcr.io/{getenv("GCP_PROJECT_ID")}/to-pip:{tag}'
-    system(f'docker tag to-pip {image_repo}')
+    system(f'docker build --platform {platform} -t {service_name} .')
+    image_repo = f'gcr.io/{getenv("GCP_PROJECT_ID")}/{service_name}:{tag}'
+    system(f'docker tag {service_name} {image_repo}')
     system(f'docker push {image_repo}')
     return image_repo
 
 
-def deploy_cloud_run(image_repo, service_account, region='us-central1', cpu=0.08, memory='128Mi',
+def deploy_cloud_run(service_name, image_repo, service_account, region='us-central1', cpu=0.08, memory='128Mi',
                      max_instances=1, port=8000):
     system(f'gcloud config set run/region {region}')
-    system(f'gcloud run deploy to-pip '
+    system(f'gcloud run deploy {service_name} '
            f'--image={image_repo} '
            f'--allow-unauthenticated '
            f'--port={port} '
            f'--service-account={service_account} '
            f'--concurrency=1 '
            f'--cpu={cpu} '
            f'--memory={memory} '
            f'--max-instances={max_instances} '
            f'--region={region} '
            f'--project={getenv("GCP_PROJECT_ID")}')
 
 
 def main():
+    load_dotenv()
     if not getenv('GCP_PROJECT_ID'):
         print('Error: GCP_PROJECT_ID is not set in the environment or .env file.')
         return
     if not getenv('GCP_SERVICE_ACCOUNT'):
         print('Error: GCP_SERVICE_ACCOUNT is not set in the environment or .env file.')
         return
 
-    parser = ArgumentParser(description='Deploy to-pip service to GCP Cloud Run')
+    parser = ArgumentParser(description='Deploy a service to GCP Cloud Run')
     arg = parser.add_argument
+    arg('-n', '--service-name', required=True, help='Service name')
     arg('-p', '--platform', default='linux/amd64', help='Docker build platform')
     arg('-t', '--image-tag', required=True, help='Docker image tag')
     arg('-s', '--service-account', default=getenv('GCP_SERVICE_ACCOUNT'),
         help='GCP service account email')
     arg('-c', '--cpu', default=0.08, type=float, help='Cloud Run CPU allocation')
     arg('-m', '--memory', default='128Mi', help='Cloud Run memory allocation')
     arg('-i', '--max-instances', default=1, type=int, help='Cloud Run maximum instance count')
     arg('-r', '--region', default='us-central1', help='Cloud Run region')
     arg('-o', '--port', default=8000, type=int, help='Container port')
 
     args = parser.parse_args()
 
     image_tag = args.image_tag
-    image_repo = build_docker_image(platform=args.platform, tag=image_tag)
-    deploy_cloud_run(image_repo=image_repo, service_account=args.service_account, region=args.region,
+    service_name = args.service_name
+    image_repo = build_docker_image(service_name, platform=args.platform, tag=image_tag)
+    deploy_cloud_run(service_name, image_repo=image_repo, service_account=args.service_account, region=args.region,
                      cpu=args.cpu, memory=args.memory, max_instances=args.max_instances,
                      port=args.port)
 
 
 if __name__ == '__main__':
     main()
```

