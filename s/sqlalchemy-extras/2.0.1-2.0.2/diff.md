# Comparing `tmp/sqlalchemy_extras-2.0.1.tar.gz` & `tmp/sqlalchemy_extras-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_extras-2.0.1.tar", max compression
+gzip compressed data, was "sqlalchemy_extras-2.0.2.tar", max compression
```

## Comparing `sqlalchemy_extras-2.0.1.tar` & `sqlalchemy_extras-2.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/README.md
--rw-r--r--   0        0        0      790 2023-04-11 18:37:54.577136 sqlalchemy_extras-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.1/sqlalchemy_extras/__init__.py
--rw-r--r--   0        0        0     6662 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.1/sqlalchemy_extras/fastapi.py
--rw-r--r--   0        0        0     5402 2023-04-11 18:37:10.574642 sqlalchemy_extras-2.0.1/sqlalchemy_extras/models.py
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/sqlalchemy_extras/py.typed
--rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/sqlalchemy_extras/utils.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.2/README.md
+-rw-r--r--   0        0        0      790 2023-04-17 15:49:47.882722 sqlalchemy_extras-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.2/sqlalchemy_extras/__init__.py
+-rw-r--r--   0        0        0     5876 2023-04-17 15:49:47.882722 sqlalchemy_extras-2.0.2/sqlalchemy_extras/fastapi.py
+-rw-r--r--   0        0        0     5402 2023-04-11 18:37:10.574642 sqlalchemy_extras-2.0.2/sqlalchemy_extras/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.2/sqlalchemy_extras/py.typed
+-rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.2/sqlalchemy_extras/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.2/PKG-INFO
```

### Comparing `sqlalchemy_extras-2.0.1/pyproject.toml` & `sqlalchemy_extras-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = ""
 name = "sqlalchemy-extras"
 readme = "README.md"
-version = "2.0.1"
+version = "2.0.2"
 
 [tool.poetry.dependencies]
 sqlalchemy = "^2.0.9"
 fastapi = { version = ">=0.60.0,<1.0.0", optional = true }
 python = ">=3.10.0, <4"
 
 [tool.poetry.extras]
```

### Comparing `sqlalchemy_extras-2.0.1/sqlalchemy_extras/fastapi.py` & `sqlalchemy_extras-2.0.2/sqlalchemy_extras/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,32 +65,22 @@
         log.debug("Initialicing a session factory.")
         factory = sessionmaker(self.engine)
         log.debug("Session factory initialized.")
         return factory
 
     @contextmanager
     def session(self, *, in_transaction: bool = False) -> Generator[Session, Any, None]:
-        session_contextmanager = None
         if in_transaction:
             log.debug("Starting a transactional session.")
-            session_contextmanager = self.sessionmaker.begin()
+            with self.sessionmaker.begin() as session:
+                yield session
         else:
             log.debug("Starting a non-transactional session.")
-            session_contextmanager = self.sessionmaker()
-        try:
-            log.debug("Connecting to the database.")
-            with session_contextmanager as session:
+            with self.sessionmaker() as session:
                 yield session
-                if session.in_transaction():
-                    log.debug(
-                        "Changes to the session will be committed as the session is in "
-                        "a transaction."
-                    )
-        finally:
-            log.debug("Session terminated.")
 
     @contextmanager
     def connection(
         self, *, in_transaction: bool = False
     ) -> Generator[Connection, Any, None]:
         connection_contextmanager: Optional[ContextManager[Connection]] = None
         if in_transaction:
@@ -146,33 +136,26 @@
     def get_engine(self) -> AsyncEngine:
         return self.engine
 
     @asynccontextmanager
     async def session(
         self, *, in_transaction: bool = False
     ) -> AsyncGenerator[AsyncSession, None]:
-        session_contextmanager: Optional[AsyncContextManager[AsyncSession]] = None
         if in_transaction:
             log.debug("Starting a transactional async session.")
-            session_contextmanager = self.sessionmaker.begin()
+            async with self.sessionmaker.begin() as session:
+                log.debug("Started transaction.")
+                yield session
+                log.debug("Transaction was successful and changes will be committed.")
+
         else:
             log.debug("Starting an async session.")
-            session_contextmanager = self.sessionmaker()
-        try:
-            log.debug("Starting async session.")
-            async with session_contextmanager as session:
-                log.debug("Connected to the database with an async session.")
+            async with self.sessionmaker() as session:
+                log.debug("Non-transactional session started.")
                 yield session
-                if session.in_transaction():
-                    log.debug(
-                        "Changes to the session will be committed because the session "
-                        "is in a transaction."
-                    )
-        finally:
-            log.debug("Async session terminated.")
 
     @asynccontextmanager
     async def connection(
         self, *, in_transaction: bool = False
     ) -> AsyncGenerator[AsyncConnection, None]:
         connection_contextmanager: Optional[AsyncContextManager[AsyncConnection]] = None
         if in_transaction:
```

### Comparing `sqlalchemy_extras-2.0.1/sqlalchemy_extras/models.py` & `sqlalchemy_extras-2.0.2/sqlalchemy_extras/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_extras-2.0.1/sqlalchemy_extras/utils.py` & `sqlalchemy_extras-2.0.2/sqlalchemy_extras/utils.py`

 * *Files identical despite different names*

