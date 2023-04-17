# Comparing `tmp/hqdragondownload-1.1.0.tar.gz` & `tmp/hqdragondownload-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqdragondownload-1.1.0.tar", last modified: Thu Jul  7 19:55:25 2022, max compression
+gzip compressed data, was "hqdragondownload-1.1.1.tar", last modified: Mon Apr 17 20:05:23 2023, max compression
```

## Comparing `hqdragondownload-1.1.0.tar` & `hqdragondownload-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-07-07 19:55:25.346177 hqdragondownload-1.1.0/
--rw-rw-rw-   0        0        0     1114 2022-03-23 05:45:04.000000 hqdragondownload-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      789 2022-07-07 19:55:25.346177 hqdragondownload-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      899 2022-04-20 19:12:53.000000 hqdragondownload-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-07 19:55:25.302178 hqdragondownload-1.1.0/hqdragon/
--rw-rw-rw-   0        0        0       97 2022-07-07 19:52:51.000000 hqdragondownload-1.1.0/hqdragon/__init__.py
--rw-rw-rw-   0        0        0     6371 2022-07-07 19:48:36.000000 hqdragondownload-1.1.0/hqdragon/__main__.py
-drwxrwxrwx   0        0        0        0 2022-07-07 19:55:25.344181 hqdragondownload-1.1.0/hqdragondownload.egg-info/
--rw-rw-rw-   0        0        0      789 2022-07-07 19:55:22.000000 hqdragondownload-1.1.0/hqdragondownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2022-07-07 19:55:23.000000 hqdragondownload-1.1.0/hqdragondownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-07 19:55:22.000000 hqdragondownload-1.1.0/hqdragondownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-07-07 19:55:22.000000 hqdragondownload-1.1.0/hqdragondownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-07 19:55:22.000000 hqdragondownload-1.1.0/hqdragondownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2022-07-07 19:55:25.350178 hqdragondownload-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1015 2022-07-07 19:52:21.000000 hqdragondownload-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.161341 hqdragondownload-1.1.1/
+-rw-rw-rw-   0        0        0     1114 2022-04-21 03:01:14.000000 hqdragondownload-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      786 2023-04-17 20:05:23.162338 hqdragondownload-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2022-04-21 03:01:14.000000 hqdragondownload-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.124356 hqdragondownload-1.1.1/hqdragon/
+-rw-rw-rw-   0        0        0       97 2023-04-17 20:05:03.000000 hqdragondownload-1.1.1/hqdragon/__init__.py
+-rw-rw-rw-   0        0        0     6502 2023-04-16 09:56:44.000000 hqdragondownload-1.1.1/hqdragon/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:23.159334 hqdragondownload-1.1.1/hqdragondownload.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 20:05:21.000000 hqdragondownload-1.1.1/hqdragondownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-04-17 20:05:23.170345 hqdragondownload-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-04-17 20:04:48.000000 hqdragondownload-1.1.1/setup.py
```

### Comparing `hqdragondownload-1.1.0/LICENSE.txt` & `hqdragondownload-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hqdragondownload-1.1.0/README.md` & `hqdragondownload-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hqdragondownload-1.1.0/hqdragon/__main__.py` & `hqdragondownload-1.1.1/hqdragon/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 my_parse = argparse.ArgumentParser(description="CLI para baixar hq's.")
 
 my_parse.add_argument("--search", action="store", type=str, help="Pesquisar.")
 my_parse.add_argument("--url", action="store", type=str, help="Url da hq.")
 my_parse.add_argument("--output", action="store", type=str, help="Nome de saida do pdf.")
 my_parse.add_argument("--option", action="store", type=int, help="Opção da pesquisa.")
 my_parse.add_argument("--no-pdf", action="store", type=bool, help="Salva apenas as imagens.", default=False)
-my_parse.add_argument("--cap", action="store", type=list, help="Define os capitulos.")
+my_parse.add_argument("--cap", action="store", type=str, help="Define os capitulos.")
 
 args = my_parse.parse_args()
 
+args.cap = args.cap.split(',')
+
 if args.search:
     page = requests.get(headers=headers, url=url+query_search+args.search)
     tree = html.fromstring(page.content)
     titles = tree.xpath("//div[@class='col-sm-6 col-md-3 lista-hqs']/a/text()")
     links = tree.xpath("//div[@class='col-sm-6 col-md-3 lista-hqs']/a/@href")[::2]
     if len(links) == 0:
         print('Nenhum resultado encontrado.')
@@ -49,14 +51,15 @@
         if args.output != None:
             if '//' in args.output or '/' in args.output:
                 print('output recebe apenas o nome do arquivo.')
                 exit()
         file_name = args.output if args.output != None else datetime.datetime.now().strftime('%d_%m_%Y__%H_%M_%S')
         print("[+]Downloading...[+]")
         for idx,cap in enumerate(caps):
+            cap_n = cap.split('/')[-1]
             if args.cap != None:
                 if int(cap.split('/')[-1]) not in [int(x) for x in args.cap if x != ',']:
                     continue
             page=requests.get(cap, headers=headers)
             tree=html.fromstring(page.content)
             pags=[x.replace('Pag. ','') for x in tree.xpath('//*[@id="paginas"]/option/text()')]
             path_name =file_name+'_'+cap.split('/')[-1]
@@ -81,28 +84,29 @@
                     pdf.output(f'{path}.pdf',"F")
                 for path in paths:
                     imgs = os.listdir(path)
                     for img in imgs:
                         os.remove(path+'/'+img)
                     os.rmdir(path)
 
-                print("[+]Finished...[+]")
+                print(f"[+]Finished Cap. {cap_n}[+]")
 
 elif args.url:
     page = requests.get(headers=headers, url=args.url)
     tree = html.fromstring(page.content)
     caps = tree.xpath("//table[@class='table table-bordered']/tbody/tr/td/a/@href")[::-1]
 
     if args.output != None:
         if '//' in args.output or '/' in args.output:
             print('output recebe apenas o nome do arquivo.')
             exit()
     file_name = args.output if args.output != None else datetime.datetime.now().strftime('%d_%m_%Y__%H_%M_%S')
     print("[+]Downloading...[+]")
     for idx,cap in enumerate(caps):
+        cap_n = cap.split('/')[-1]
         if args.cap != None:
             if int(cap.split('/')[-1]) not in [int(x) for x in args.cap if x != ',']:
                 continue
         page=requests.get(cap, headers=headers)
         tree=html.fromstring(page.content)
         pags=[x.replace('Pag. ','') for x in tree.xpath('//*[@id="paginas"]/option/text()')]
         path_name =file_name+'_'+cap.split('/')[-1]
@@ -127,15 +131,15 @@
                 pdf.output(f'{path}.pdf',"F")
             for path in paths:
                 imgs = os.listdir(path)
                 for img in imgs:
                     os.remove(path+'/'+img)
                 os.rmdir(path)
 
-            print("[+]Finished...[+]")
+            print(f"[+]Finished Cap. {cap_n}[+]")
 
 else:
     template ="""
     Exemplos:
     1. $python .\main.py --search "superman" --option 1 --no-pdf True
     2. $python .\main.py --search "superman" --option 1 --cap 2 --output "superman"
     3. $python .\main.py --search "superman" --option 1 --cap 1,2 --no-pdf True
```

### Comparing `hqdragondownload-1.1.0/setup.py` & `hqdragondownload-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name = 'hqdragondownload',
-    version = '1.1.0',
+    version = '1.1.1',
     author = 'MrPowerUp',
     author_email = 'gustavohenrique8282@hotmail.com',
     packages = ['hqdragon'],
     description = 'CLI para baixar hqs no site.',
     long_description = 'CLI para baixar hqs no site.',
     url = 'https://github.com/MrPowerUp82/hqdragondownload',
     project_urls = {
```

