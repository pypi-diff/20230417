# Comparing `tmp/ksfctl-0.2.tar.gz` & `tmp/ksfctl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksfctl-0.2.tar", last modified: Fri Apr  7 15:26:54 2023, max compression
+gzip compressed data, was "ksfctl-0.2.1.tar", last modified: Mon Apr 17 17:58:02 2023, max compression
```

## Comparing `ksfctl-0.2.tar` & `ksfctl-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.672675 ksfctl-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 15:26:54.672675 ksfctl-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 15:26:40.000000 ksfctl-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.668675 ksfctl-0.2/ksfctl/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.668675 ksfctl-0.2/ksfctl/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/cmd/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.672675 ksfctl-0.2/ksfctl/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57858 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/generate/cpp_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.672675 ksfctl-0.2/ksfctl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/parser/ksf_lex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/parser/ksf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/parser/ksf_yacc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-07 15:26:40.000000 ksfctl-0.2/ksfctl/parser/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:26:54.668675 ksfctl-0.2/ksfctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 15:26:54.000000 ksfctl-0.2/ksfctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:26:54.672675 ksfctl-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-07 15:26:40.000000 ksfctl-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 17:58:02.471414 ksfctl-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-17 17:57:51.000000 ksfctl-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/cmd/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87289 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/cpp/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_yacc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:58:02.471414 ksfctl-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 17:57:51.000000 ksfctl-0.2.1/setup.py
```

### Comparing `ksfctl-0.2/ksfctl/generate/cpp_generator.py` & `ksfctl-0.2.1/ksfctl/generate/cpp/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,486 +1,232 @@
+from datetime import datetime
 from hashlib import md5
 
+from ksfctl.generate.cpp.parser import CppParser
 from ksfctl.parser.ksf_parser import *
 from ksfctl.parser.ksf_yacc import generate
 
 
-class CppGenerator:
-    def __init__(self, ast, filename, dest, **kwargs):
-        self.__dict__.update(kwargs)
-        self.ast = ast
+class CppGenerator(CppParser):
+    def __init__(self, ast, filename, repl_ns_dict, repl_inc_dir, destination, push_functions,
+                 **kwargs):
+        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, [], **kwargs)
         file = Path(filename)
         real_name = file.name
         self.ast_in_file = ast.files[real_name]
+        self.generated_file = (Path(destination) / (real_name[:-4] + '.h'))
 
-        Path(dest).mkdir(parents=True, exist_ok=True)
-        self.generated_file = (Path(dest) / (real_name[:-4] + '.h'))
-
-        self.inc_ordered = [
-            "<string>",
-            "<vector>",
-            "<set>",
-            "<unordered_set>",
-            "<map>",
-            "<unordered_map>",
-            "<kup/Ksf.h>",
-            "<kup/KsfJson.h>",
-            "<servant/Agent.h>",
-            "<servant/Servant.h>",
-            "<promise/promise.h>",
-        ]
-        self.inc_native = {
-            "<string>": True,
-            "<vector>": False,
-            "<set>": False,
-            "<unordered_set>": False,
-            "<map>": False,
-            "<unordered_map>": False,
-            "<kup/Ksf.h>": False,
-            "<kup/KsfJson.h>": False,
-            "<servant/Agent.h>": False,
-            "<servant/Servant.h>": False,
-            "<promise/promise.h>": False,
-        }
-        self.inc_depends = []
         self.file_str = ''
         self.curr_tab = ''
 
-    def __getattr__(self, name):
-        if name.startswith('with_') and not hasattr(self, 'name'):
-            return False
-        return super().__getattr__(name)
-
-    def add_include(self, header):
-        if header in self.inc_native:
-            self.inc_native[header] = True
-        else:
-            self.inc_depends.append(header)
-
-    def parse_header(self):
-        output = ""
-        for header in self.inc_ordered:
-            if self.inc_native[header]:
-                output += "#include " + header + "\n"
-
-        output += "\n"
-
-        for header in self.inc_depends:
-            output += "#include " + header + "\n"
-        return output
-
-    def inc_tab(self):
-        self.curr_tab += '\t'
-
-    def del_tab(self):
-        self.curr_tab = self.curr_tab[:-1]
-
-    @staticmethod
-    def get_type_id(curr_module, value_type):
-        return f"{curr_module if value_type['module'] is None else value_type['module']}.{value_type['name']}"
-
-    def is_movable_type(self, module, value_type):
-        """判断是否是可以进行std::move的类型"""
-        if value_type['type'] == 'native':
-            return value_type['name'] == 'string'
-        elif value_type['type'] == 'class':
-
-            if hasattr(value_type, 'module'):
-                class_full_name = value_type['module'] + "." + value_type['name']
-            else:
-                class_full_name = module + "." +value_type['name']
-
-            return class_full_name not in self.ast.enums
-        elif value_type['type'] == 'vector':
-            return True
-        elif value_type['type'] == 'map':
-            return True
-        else:
-            return False
-
-    def parse_type(self, module, value_type):
-        if value_type['type'] == 'native':
-            if value_type['name'] == 'string':
-                self.add_include(f"<string>")
-                return 'std::string'
-            elif value_type['name'] == 'int':
-                if value_type['bit'] == 8:
-                    return f'{"unsigned char" if value_type["unsigned"] else "char"}'
-                return f'{"u" if value_type["unsigned"] else ""}int{value_type["bit"]}_t'
-            elif value_type['name'] == 'float':
-                return value_type['name']
-            elif value_type['name'] == 'double':
-                return value_type['name']
-            elif value_type['name'] == 'bool':
-                return value_type['name']
-            else:
-                raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-        elif value_type['type'] == 'class':
-            if hasattr(value_type, 'module') and module != value_type['module']:
-                return value_type['module'] + "::" + value_type['name']
-            else:
-                return value_type['name']
-        elif value_type['type'] == 'vector':
-            if value_type['is_ordered'] and not value_type['is_hashed'] and not value_type['is_unique_member']:
-                true_type = 'std::vector'
-                self.add_include('<vector>')
-            elif value_type['is_ordered'] and not value_type['is_hashed'] and value_type['is_unique_member']:
-                true_type = 'std::set'
-                self.add_include('<set>')
-            elif not value_type['is_ordered'] and value_type['is_hashed'] and value_type['is_unique_member']:
-                true_type = 'std::unordered_set'
-                self.add_include('<unordered_set>')
-            else:
-                raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-
-            return f"{true_type}<{self.parse_type(module, value_type['value_type'])}>"
-        elif value_type['type'] == 'map':
-            if not value_type['is_ordered'] and value_type['is_hashed'] and value_type['is_unique_member']:
-                true_type = 'std::unordered_map'
-                self.add_include('<unordered_map>')
-            elif value_type['is_ordered'] and not value_type['is_hashed'] and value_type['is_unique_member']:
-                true_type = 'std::map'
-                self.add_include('<map>')
-            else:
-                raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-            return f"{true_type}<{self.parse_type(module, value_type['key_type'])}, {self.parse_type(module, value_type['value_type'])}>"
-
-    def parse_comment_above(self, comment, tab=None):
-        if comment is None or comment == '':
-            return ''
-
-        if tab is None:
-            tab = self.curr_tab
-
-        comment_lines = comment.split('\n')
-        if len(comment_lines) == 1:
-            return f"{tab}//{comment}\n"
-        else:
-            import re
-            matches = re.findall(r"\s+\*\s+(.*)\n", f"/*{comment}*/")
-            comment_str = f'{tab}/**\n'
-
-            # 将每行注释内容拼接为Python风格的注释
-            for match in matches:
-                comment_str += f"{tab} * {match}\n"
-            comment_str += f'{tab} */\n'
-            return comment_str
-
-    def parse_comment_line(self, comment):
-        if comment is None or comment == '':
-            return ''
-
-        comment_lines = comment.split('\n')
-        if len(comment_lines) == 1:
-            return f" //{comment}"
-        else:
-            raise SyntaxError("不支持的注释方式")
-
-    def parse_value(self, value):
-        return value['value'] if value['is_number'] else f'"{value["value"]}"'
-
-    def parse_const(self, curr_module, ksf_const: KsfConst):
-        if ksf_const.value_type['name'] == 'string':
-            return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
-        return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr {self.parse_type(curr_module, ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
-
-    def parse_enum_member(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}{ksf_enum_member.name} = {ksf_enum_member.value}"
-
-    def parse_enum_to_str(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}    case {ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
-
-    def parse_str_to_enum(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}if (s == \"{ksf_enum_member.name}\") {{ e = {ksf_enum_member.name}; return 0; }}"
-
-    def parse_default_var(self, name, value_type, default):
-        if default is None:
-            if value_type['name'] == 'int':
-                return f'''if ({name} == 0) '''
-            elif value_type['name'] == 'float':
-                return f'if (ksf::KS_Common::equal(0.0f, {name})) '
-            elif value_type['name'] == 'double':
-                return f'if (ksf::KS_Common::equal(0.0, {name})) '
-            elif value_type['name'] == 'bool':
-                return f'if ({name})'
-            elif value_type['name'] == 'string':
-                return f'if ({name}.empty())'
-            else:
-                return ''
-
-        # 特殊处理一下bool型
-        if default['is_bool']:
-            return f'if ({"" if default["value"] else "!"}{name})'
-        elif default['is_number']:
-            if value_type['name'] == 'float':
-                return f'if (ksf::KS_Common::equal({name}f, {default["value"]})) '
-            elif value_type['name'] == 'double':
-                return f'if (ksf::KS_Common::equal({name}, {default["value"]})) '
-            return f'if ({name} == {default["value"]}) '
-        elif default['is_enum']:
-            return f'if ({name} == {default["value"]}) '
-        else:
-            return f'if ({name} == "{default["value"]}") '
+        self.to_file()
 
     def parse_enum(self, curr_module, ksf_enum: KsfEnum):
         enum_str = f"{self.parse_comment_above(ksf_enum.comment)}{self.curr_tab}enum {ksf_enum.name} \n{{\n"
-        self.inc_tab()
         enum_member_str_list = []
         enum_member_tostr = []
         enum_member_strto = []
         for m in ksf_enum.member:
             enum_member_str_list.append(self.parse_enum_member(m))
-            enum_member_tostr.append(self.parse_enum_to_str(m))
-            enum_member_strto.append(self.parse_str_to_enum(m))
-
-        self.del_tab()
+            enum_member_tostr.append(self.parse_enum_to_str(curr_module, m))
+            enum_member_strto.append(self.parse_str_to_enum(curr_module, m))
 
-        enum_str += ',\n'.join(enum_member_str_list)
+        enum_str += self.add_lines(',\n'.join(enum_member_str_list), 1)
 
         enum_str += f"\n}};\n\n"
 
         etos_member = '\n'.join(enum_member_tostr)
         enum_str += f"""\
 inline std::string etos(const {ksf_enum.name} &e) {{
     switch (e) {{
-{etos_member}
+{self.add_lines(etos_member, 2)}
         default: return "";
     }}
 }}
 
 """
 
-        stoe_member = '\n'.join(enum_member_strto)
+        stoe_member = self.endl().join(enum_member_strto)
         enum_str += f"""\
 inline int stoe(const std::string &s, {ksf_enum.name} &e) {{
-{stoe_member}
+{self.add_lines(stoe_member, 1)}
     return -1;
 }}
 
 """
         return enum_str
 
-    def parse_variable(self, curr_module, ksf_var: KsfField):
-        def parse_default_var(value_type, default):
-            if default is None:
-                if value_type['name'] == 'int':
-                    return '0'
-                elif value_type['name'] == 'float':
-                    return '0.0f'
-                elif value_type['name'] == 'double':
-                    return '0.0'
-                elif value_type['name'] == 'bool':
-                    return 'true'
-                elif value_type['name'] == 'string':
-                    return '""'
-                else:
-                    return None
-
-            # 特殊处理一下bool型
-            if default['is_bool']:
-                return f'{"true" if default["value"] else "false"}'
-            elif default['is_number'] or default['is_enum']:
-                return f'{default["value"]}'
-            else:
-                return f'"{default["value"]}"'
-        default_var = parse_default_var(ksf_var.value_type, ksf_var.default)
-        return f"{self.parse_type(curr_module, ksf_var.value_type)} \n{ksf_var.name}" \
-               f"{' = ' + default_var if default_var is not None else ''}; " \
-               f"{self.parse_comment_line(ksf_var.comment)}\n\n"
-        pass
-
-    def add_lines(self, lines, tab=None):
-        if tab is None:
-            tab = self.curr_tab
-
-        return f"\n".join(tab + line for line in lines.split("\n")[:-1]) + '\n'
-
     def parse_resetDefault(self, curr_module, ksf_struct: KsfStruct):
         return self.add_lines(f'''\
-/**
- * 重新赋值为初始构造的结构
- */
-void resetDefault() {{
-    *this = {ksf_struct.name}{{}}; 
-}}\n''')
+    ///重新赋值为初始构造的结构
+    void resetDefault() {{
+        *this = {ksf_struct.name}{{}}; 
+    }}\n''')
 
     def parse_variable_writeTo(self, ksf_field: KsfField):
         value_type = ksf_field.value_type
         if self.with_check_default:
-            if value_type['type'] == 'native':
-                if value_type['name'] != 'bool':
+            if isinstance(value_type, KsfBuildInType):
+                if value_type.name != 'bool':
                     return f"""{self.parse_default_var(ksf_field.name, value_type, ksf_field.default)} {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
                 else:
                     if ksf_field.default is None or ksf_field.default['value']:
                         return f"""if (!{ksf_field.name}) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
                     else:
                         return f"""if ({ksf_field.name}) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
-            elif value_type['type'] == 'class':
+            elif isinstance(value_type, KsfStructType):
                 # 如果是枚举类型
-                if value_type['name'] in self.ast.enums:
+                if value_type.name in self.ast.enums:
                     return f"_os.write((int32_t){ksf_field.name}, {ksf_field.tag});"
                 else:
                     return f"_os.write({ksf_field.name}, {ksf_field.tag});"
-            elif value_type['type'] == 'vector':
+            elif isinstance(value_type, KsfVectorType):
                 return f"""if (!{ksf_field.name}.empty()) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
-            elif value_type['type'] == 'map':
+            elif isinstance(value_type, KsfMapType):
                 return f"""if (!{ksf_field.name}.empty()) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
             else:
                 raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
         else:
             return f"_os.write({ksf_field.name}, {ksf_field.tag});"
 
     def parse_writeTo(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             var_list += self.parse_variable_writeTo(ksf_struct.variable[var]) + '\n'
 
         return self.add_lines(f'''\
-/**
- * 序列化为二进制流
- */
-template<typename WriterT>
-void writeTo(ksf::KsfOutputStream<WriterT>& _os) const {{
-{self.add_lines(var_list, '    ')}
-}}\n''')
+    ///序列化为二进制流
+    template<typename WriterT>
+    void writeTo(ksf::KsfOutputStream<WriterT>& _os) const {{
+{self.add_lines(var_list, 2)}
+    }}\n''')
 
     def parse_variable_writeToJson(self, curr_module, ksf_field: KsfField):
         return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson({ksf_field.name});"""
 
     def parse_writeToJson(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             var_list += self.parse_variable_writeToJson(curr_module, ksf_struct.variable[var]) + '\n'
 
         return self.add_lines(f'''\
-/**
- * 序列化为Json
- */
-ksf::JsonValueObjPtr writeToJson() const {{
-    ksf::JsonValueObjPtr p = new ksf::JsonValueObj();
-{self.add_lines(var_list, '    ')}
-    return p;
-}}
-
-/**
- * 序列化为Json字符串
- */
-std::string writeToJsonString() const {{
-    return ksf::KS_Json::writeValue(writeToJson());
-}}\n''')
+    ///序列化为Json
+    ksf::JsonValueObjPtr writeToJson() const {{
+        ksf::JsonValueObjPtr p = new ksf::JsonValueObj();
+{self.add_lines(var_list, 2)}
+        return p;
+    }}
+    
+    ///序列化为Json字符串
+    std::string writeToJsonString() const {{
+        return ksf::KS_Json::writeValue(writeToJson());
+    }}\n''')
 
     def parse_variable_readFrom(self, curr_module, ksf_field: KsfField):
         value_type = ksf_field.value_type
-        if value_type['type'] == 'native':
+        if isinstance(value_type, KsfBuildInType):
             return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif value_type['type'] == 'class':
+        elif isinstance(value_type, KsfStructType):
             return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif value_type['type'] == 'vector':
+        elif isinstance(value_type, KsfVectorType):
             return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif value_type['type'] == 'map':
+        elif isinstance(value_type, KsfMapType):
             return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
         else:
             raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
 
     def parse_readFrom(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             var_list += self.parse_variable_readFrom(curr_module, ksf_struct.variable[var]) + '\n'
 
         return self.add_lines(f'''\
-/**
-  * 二进制反序列化为结构体
-  */
-template<typename ReaderT>
-void readFrom(ksf::KsfInputStream<ReaderT>& _is)
-{{
-    resetDefault();
-{self.add_lines(var_list, '    ')}
-}}\n''')
+    ///二进制反序列化为结构体
+    template<typename ReaderT>
+    void readFrom(ksf::KsfInputStream<ReaderT>& _is)
+    {{
+        resetDefault();
+{self.add_lines(var_list, 2)}
+    }}
+
+''')
 
     def parse_variable_readFromJson(self, curr_module, ksf_field: KsfField):
         return f"""ksf::JsonInput::readJson({ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
 
     def parse_readFromJson(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             var_list += self.parse_variable_readFromJson(curr_module, ksf_struct.variable[var]) + '\n'
 
         return self.add_lines(f'''\
-/**
- * Json反序列化为结构体
- */
-void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
-    resetDefault();
-    if(NULL == p.get() || p->getType() != ksf::eJsonTypeObj)
-    {{
-        char s[128];
-        snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p.get() ? p->getType() : 0));
-        throw ksf::KS_Json_Exception(s);
+    ///Json反序列化为结构体
+    void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
+        resetDefault();
+        if(NULL == p.get() || p->getType() != ksf::eJsonTypeObj)
+        {{
+            char s[128];
+            snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p.get() ? p->getType() : 0));
+            throw ksf::KS_Json_Exception(s);
+        }}
+    
+        ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
+{self.add_lines(var_list, 2)}
     }}
 
-    ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
-{self.add_lines(var_list, '    ')}
-}}
+    ///Json字符串反序列化为结构体
+    void readFromJsonString(const std::string &str) {{
+        readFromJson(ksf::KS_Json::getValue(str));
+    }}
 
-/**
- * Json字符串反序列化为结构体
- */
-void readFromJsonString(const std::string &str) {{
-    readFromJson(ksf::KS_Json::getValue(str));
-}}
-\n''')
+''')
 
     def parse_display(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
             if field.value_type['type'] == "class" and self.get_type_id(curr_module,
                                                                         field.value_type) in self.ast.enums:
                 var_list += f'_ds.display(static_cast<int32_t>({ksf_struct.variable[var].name}),"{ksf_struct.variable[var].name}");\n'
             else:
                 var_list += f'_ds.display({ksf_struct.variable[var].name},"{ksf_struct.variable[var].name}");\n'
 
         return self.add_lines(f'''\
-/**
- * 打印
- */
-std::ostream& display(std::ostream& _os, int _level=0) const
-{{
-    ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, '    ')}
-    return _os;
-}}\n''')
+    ///打印
+    std::ostream& display(std::ostream& _os, int _level=0) const
+    {{
+        ksf::KsfDisplayer _ds(_os, _level);
+{self.add_lines(var_list, 2)}
+        return _os;
+    }}\n''')
 
     def parse_displaySimple(self, curr_module, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
             if field.value_type['type'] == "class" and self.get_type_id(curr_module,
                                                                         field.value_type) in self.ast.enums:
                 var_list += f'_ds.displaySimple(static_cast<int32_t>({ksf_struct.variable[var].name}), true);\n'
             else:
                 var_list += f'_ds.displaySimple({ksf_struct.variable[var].name}, true);\n'
 
         return self.add_lines(f'''\
-/**
- * 简单打印
- */
-std::ostream& displaySimple(std::ostream& _os, int _level=0) const
-{{
-    ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, '    ')}
-    return _os;
-}}\n''')
+    ///简单打印
+    std::ostream& displaySimple(std::ostream& _os, int _level=0) const
+    {{
+        ksf::KsfDisplayer _ds(_os, _level);
+{self.add_lines(var_list, 2)}
+        return _os;
+    }}\n''')
 
     def parse_equal(self, curr_module, ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if field.value_type['type'] == "native" and field.value_type['name'] in {'float', 'double'}:
+            if field.value_type['type'] == "native" and field.value_type.name in {'float', 'double'}:
                 var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
             else:
                 var_list.append(f'l.{field.name} == r.{field.name}')
 
         in_list = ' && '
         var_eq = in_list.join(var_list)
         return self.add_lines(f'''\
@@ -493,59 +239,49 @@
 
         struct_str = f"{self.parse_comment_above(ksf_struct.comment)}"  # 注释(可能没有)
 
         # struct XXX : public ksf::KsfStructBase
         # {
         struct_str += self.add_lines(f"struct {ksf_struct.name} : public ksf::KsfStructBase\n{{\n")
 
+        # 解析字段
+        var_list = []
+        for var in ksf_struct.variable:
+            var_list.append(self.parse_variable(curr_module, ksf_struct.variable[var]))
+
+        var_widths = self.get_column_widths(var_list)
+        for comment, var_type, var_name, var_value in var_list:
+            if comment:
+                struct_str += self.add_lines(f"{comment:<{var_widths[0]}}", 1) + self.endl()
+            struct_str += self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}",
+                                         1) + self.endl()
+
         # public:
+        struct_str += '\n'
         struct_str += self.add_lines(f"public:\n")
-        self.inc_tab()
         #     static std::string className()
         #     {
         #         return "xx.xxx";
         #     }
         #     static std::string MD5()
         #     {
         #         return "a123123123213";
         #     }
         struct_str += self.add_lines(f'''\
-static std::string className() {{
-    return "{ksf_struct.module}.{ksf_struct.name}";
-}}
-
-static std::string MD5() {{
-    return "{md5(ksf_struct.id.encode('utf-8')).hexdigest()}";
-}}\n''')
-        self.del_tab()
-        # public:
-        struct_str += '\n'
-        struct_str += self.add_lines(f"public:\n")
-
-        self.inc_tab()
-        # 解析字段
-        #     std::string appname;
-        #     std::string servername;
-        #     std::string sFilename;
-        #     std::string sFormat;
-        #     std::string setdivision;
-        #     ksf::Bool bHasSufix;
-        #     ksf::Bool bHasAppNamePrefix;
-        #     ksf::Bool bHasSquareBracket;
-        #     std::string sConcatStr;
-        #     std::string sSepar;
-        #     std::string sLogType;
-        for var in ksf_struct.variable:
-            struct_str += self.add_lines(self.parse_variable(curr_module, ksf_struct.variable[var]))
+    static std::string className() {{
+        return "{ksf_struct.module}.{ksf_struct.name}";
+    }}
+    
+    static std::string MD5() {{
+        return "{md5(ksf_struct.id.encode('utf-8')).hexdigest()}";
+    }}
 
-        self.del_tab()
+''')
         # public:
-        struct_str += '\n'
         struct_str += self.add_lines(f"public:\n")
-        self.inc_tab()
         struct_str += self.parse_resetDefault(curr_module, ksf_struct)  # resetDefault
 
         struct_str += '\n'
         struct_str += self.parse_writeTo(curr_module, ksf_struct)  # writeTo
 
         struct_str += '\n'
         struct_str += self.parse_readFrom(curr_module, ksf_struct)  # readFrom
@@ -560,29 +296,30 @@
 
         struct_str += '\n'
         struct_str += self.parse_display(curr_module, ksf_struct)  # display
 
         struct_str += '\n'
         struct_str += self.parse_displaySimple(curr_module, ksf_struct)  # displaySimple
 
-        self.del_tab()
         # };
-        struct_str += f"{self.curr_tab}}};\n"
+        struct_str += f"}};\n"
 
         # inline bool operator==(const {ksf_struct.name}&l, const {ksf_struct.name}&r)
         struct_str += '\n'
         # operator==
         struct_str += self.parse_equal(curr_module, ksf_struct)
 
         struct_str += '\n'
         # operator!=
         struct_str += f"""\
 inline bool operator!=(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
     return !(l == r);
-}}\n"""
+}}
+
+"""
         if len(ksf_struct.key_fields) != 0:
             struct_str += f"""\
 inline bool operator<(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{\n"""
             for key_field in ksf_struct.key_fields:
                 struct_str += f"""\
     if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});\n"""
             struct_str += f"""\
@@ -595,35 +332,34 @@
 
 inline bool operator>(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
     return r < l;
 }}
 
 inline bool operator>=(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
     return !(l < r);
-}}\n\n"""
+}}
 
-        if self.with_json:
+"""
 
-            struct_str += '\n'
+        if self.with_json:
             # operator<<
             struct_str += f"""\
 inline std::ostream &operator<<(std::ostream &os, const {ksf_struct.name} &r) {{
     os << r.writeToJsonString();
     return os;
-}}"""
+}}
 
-            struct_str += '\n'
-            # operator>>
-            struct_str += f"""\
 inline std::istream &operator>>(std::istream &is, {ksf_struct.name} &l) {{
     std::istreambuf_iterator<char> eos;
     std::string s(std::istreambuf_iterator<char>(is), eos);
     l.readFromJsonString(s);
     return is;
-}}\n"""
+}}
+
+"""
         return struct_str
 
     def parse_InterfacePrxCallBack(self, curr_module, ksf_interface: KsfInterface):
         prx_str = f"""\
 class {ksf_interface.name}PrxCallback : public ksf::AgentCallback
 {{
 public:
@@ -635,27 +371,29 @@
         index = 0
         func_case_str = ""
         for item in ksf_interface.operator:
             operator = ksf_interface.operator[item]
 
             def parse_output_vars(with_type=True):
                 def parse_output_var(value_type, name, with_type):
-                    if value_type['name'] != 'void':
+                    if value_type.name != 'void':
                         if not self.is_movable_type(curr_module, value_type):
                             return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
                         elif self.with_param_rvalue_ref:
                             return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
                         else:
                             return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
+
                 vars_list = []
                 if operator.return_type['name'] != 'void':
                     vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
 
                 for i in operator.output:
-                    vars_list.append(parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type))
+                    vars_list.append(
+                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type))
 
                 return ', '.join(vars_list)
 
             prx_str += f"""\
     virtual void callback_{operator.name}({parse_output_vars(True)}) \
 {{ throw std::runtime_error("callback_{operator.name} override incorrect."); }}
     
@@ -757,32 +495,31 @@
 
         dispatch_case_str = ""
         case_index = 0
         for item in ksf_interface.operator:
             operator = ksf_interface.operator[item]
             parsed_str += f"""\
 public:
-    struct Promise{operator.name}: virtual public KS_HandleBase {{
-    public:
+    struct Promise{operator.name}: virtual public KS_HandleBase 
+    {{
         std::map<std::string, std::string> _mRspContext;\n"""
 
             if operator.return_type['name'] != 'void':
                 parsed_str += f"        {self.parse_type(curr_module, operator.return_type)} _ret;\n"
 
             for item in operator.output:
                 var = operator.output[item]
                 parsed_str += f"        {self.parse_type(curr_module, var.value_type)} {var.name};\n"
 
             parsed_str += f"""\
     }};
         
     using Promise{operator.name}Ptr = ksf::KS_AutoPtr<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}>;
     
-    {ksf_interface.name}PrxCallbackPromise(const ksf::Promise<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr> &promise)
-    : _promise_{operator.name}(promise) {{}}
+    {ksf_interface.name}PrxCallbackPromise(const ksf::Promise<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr> &promise): _promise_{operator.name}(promise) {{}}
     
     virtual void callback_{operator.name}(const {ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr &ptr) {{
         _promise_{operator.name}.setValue(ptr);
     }}
     
     virtual void callback_{operator.name}_exception(ksf::Int32 ret) {{
         std::stringstream oss;
@@ -823,14 +560,15 @@
 
                 for item2 in operator.output:
                     var2 = operator.output[item2]
                     func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
 
                 func_case_str += ''.join(func_case_list)
                 return func_case_str
+
             case_index += 1
             dispatch_case_str += parse_func_dispatch()
             dispatch_case_str += f"""\
                 }} catch (std::exception &ex) {{
                     callback_{operator.name}_exception(ksf::KSFCLIENTDECODEERR);
                     return ksf::KSFCLIENTDECODEERR;
                 }} catch (...) {{
@@ -882,24 +620,24 @@
             func_case_str = ""
             index = 0
             for item in ksf_interface.operator:
                 operator = ksf_interface.operator[item]
 
                 def parse_output_vars(with_type=True):
                     def parse_output_var(value_type, name, with_type):
-                        if value_type['name'] != 'void':
+                        if value_type.name != 'void':
                             if not self.is_movable_type(curr_module, value_type):
                                 return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
                             elif self.with_param_rvalue_ref:
                                 return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
                             else:
                                 return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
 
                     vars_list = []
-                    if operator.return_type['name'] != 'void':
+                    if operator.return_type.name != 'void':
                         vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
 
                     for item in operator.output:
                         vars_list.append(
                             parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type))
 
                     return ', '.join(vars_list)
@@ -1060,15 +798,15 @@
         return promise.getFuture();
     }}
     
     void coro_{operator.name}({ksf_interface.name}CoroPrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = KSF_CONTEXT())
     {{
         ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
 {''.join(parse_input_vars())}
-        std::map<std::string, std::string>            _mStatus;
+        std::map<std::string, std::string> _mStatus;
         ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback, true);
     }}\n\n"""
             return parsed_oper_str
 
         parsed_str = f"""\
 class {ksf_interface.name}Proxy : public ksf::Agent
 {{
@@ -1194,51 +932,58 @@
                                     f"const {self.parse_type(curr_module, operator.input[var_name].value_type)} &{var_name}, ")
                         else:
                             parsed_list.append(
                                 f"{self.parse_type(curr_module, operator.input[var_name].value_type)} {var_name}, ")
 
                 return parsed_list
 
-            parsed_str += f"""\
+            if self.enable_async_rsp(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
+                parsed_str += f"""\
 {self.parse_comment_above(operator.comment, tab='    ')}\
     virtual {self.parse_type(curr_module, operator.return_type) if has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}ksf::KsfCurrentPtr _current_) = 0;\n\n"""
 
-            parsed_async_str += f"""\
+                parsed_async_str += f"""\
     static void async_response_{operator.name}(ksf::KsfCurrentPtr _current_{''.join(parse_all_vars())})
     {{
         switch (_current_->getRequestVersion()) {{
             case ksf::KUPVERSION: {{
                 ksf::kup::UniAttribute<ksf::BufferWriterVector, ksf::BufferReader> _ksfAttr_;
                 _ksfAttr_.setVersion(_current_->getRequestVersion());
 {parse_output_vars(mode='kup', tab=4)}
                 std::vector<char> sKupResponseBuffer;
                 _ksfAttr_.encode(sKupResponseBuffer);
                 _current_->sendResponse(ksf::KSFSERVERSUCCESS, sKupResponseBuffer);
                 break;
             }}\n"""
-            if self.with_json:
-                parsed_async_str += f"""\
+
+                # 增加json支持
+                if self.with_json:
+                    parsed_async_str += f"""\
             case ksf::JSONVERSION: {{
                 ksf::JsonValueObjPtr _p = new ksf::JsonValueObj();
 {parse_output_vars(mode='json', tab=4)}
                 std::vector<char> sJsonResponseBuffer;
                 ksf::KS_Json::writeValue(_p, sJsonResponseBuffer);
                 _current_->sendResponse(ksf::KSFSERVERSUCCESS, sJsonResponseBuffer);
                 break;
-        }}\n"""
-            parsed_async_str += f"""\
+            }}\n"""
+
+                parsed_async_str += f"""\
             case ksf::KSFVERSION: {{
                 ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
 {parse_output_vars(mode='ksf', tab=4)}
                 _current_->sendResponse(ksf::KSFSERVERSUCCESS, _os);
                 break;
             }}
             default: {{std::runtime_error("unsupport ksf packet version");}}
-        }} // end switch\n\n"""
+        }} // end switch\n"""
+                parsed_async_str += f"""\
+    }}
 
+"""
             # 链路追踪
             if self.with_trace:
                 if not self.with_json:
                     raise SyntaxError("如果需要链路追踪，需要打开生成Json序列化支持(--json)")
 
                 parsed_async_str += f"""\
         if (_current_->isTraced()) {{
@@ -1250,15 +995,20 @@
                 _trace_param_ = ksf::KS_Json::writeValue(_p_);
             }} else if(ksf::ServantProxyThreadData::TraceContext::ENP_OVERMAXLEN == _trace_param_flag_) {{
                 _trace_param_ = "{{\"trace_param_over_max_len\":true}}";
             }}
             
             KSF_TRACE(_current_->getTraceKey(), TRACE_ANNOTATION_SS, "", ksf::ServerConfig::Application + "." + ksf::ServerConfig::ServerName, "test", 0, _trace_param_, "");
         }}\n"""
-            dispatch_case_str += f"""\
+
+            if self.enable_push(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
+                dispatch_case_str += f"""\
+            case {index}: return ksf::KSFSERVERNOFUNCERR;\n"""
+            else:
+                dispatch_case_str += f"""\
             case {index}: {{
                 ksf::KsfInputStream<ksf::BufferReader> _is;
                 _is.setBuffer(_current->getRequestBuffer());
 {parse_vars_list(tab=4)}
                 switch (_current->getRequestVersion()) {{
                     case ksf::KUPVERSION: {{
                         ksf::kup::UniAttribute<ksf::BufferWriterVector, ksf::BufferReader>  _ksfAttr_;
@@ -1299,18 +1049,16 @@
                     }}
                 }}
                 return ksf::KSFSERVERSUCCESS;
 
             }}\n"""
             index += 1
 
-            parsed_async_str += f"""\
-    }}
-\n"""
-            parsed_push_str += f"""\
+            if self.with_push and self.enable_push(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
+                parsed_push_str += f"""\
     static void async_response_push_{operator.name}(ksf::KsfCurrentPtr _current_{''.join(parse_all_vars())}, const std::map<std::string, std::string> &_context = ksf::Current::KSF_STATUS())
     {{
         {{
             ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
 {parse_output_vars(mode='ksf', tab=3)}
             _current_->sendPushResponse(ksf::KSFSERVERSUCCESS, "{operator.name}", _os, _context);
         }}
@@ -1368,69 +1116,1037 @@
 
     def to_file(self):
         # 生成头文件（需要判断是否忽略路径)
         for inc, inc_file_name in self.ast_in_file.includes:
             if self.with_ignore_relative_path:
                 self.add_include(f'"{inc.name[:-4]}.h"')
             else:
-                self.add_include(f'"{inc_file_name[:-4]}.h"')
+                self.add_include(self.get_repl_headfile(f'"{inc_file_name[:-4]}.h"'))
 
         curr_module = None
         for ele in self.ast_in_file.elements:
             # 生成命名空间
             if curr_module is None:
                 curr_module = ele.module
-                self.file_str += self.curr_tab + f"namespace {ele.module} {{\n\n"
+                self.file_str += self.curr_tab + f"{self.get_ns_begin(ele.module)}\n\n"
             elif curr_module != ele.module:
-                curr_module = ele.module
                 self.file_str += self.curr_tab + f"}} //end {curr_module}\n\n\nnamespace {ele.module} {{\n\n"
+                self.file_str += self.curr_tab + f"{self.get_ns_end(curr_module)}\n\n\nnamespace {ele.module} {{\n\n"
+                curr_module = ele.module
 
             if isinstance(ele, KsfConst):
                 self.file_str += self.parse_const(curr_module, ele)
                 pass
             elif isinstance(ele, KsfEnum):
                 self.file_str += self.parse_enum(curr_module, ele)
                 pass
             elif isinstance(ele, KsfStruct):
                 self.file_str += self.parse_struct(curr_module, ele)
                 pass
             elif isinstance(ele, KsfInterface) and self.with_rpc:
                 self.file_str += self.parse_interface(curr_module, ele)
 
-        self.file_str += f"}} //end {curr_module}\n\n"
+        self.file_str += f"{self.get_ns_end(curr_module)}\n\n"
 
-        self.file_str = "#pragma once\n\n" + self.parse_header() + "\n\n" + self.file_str
+        self.file_str = f"""\
+/**
+ * @brief {self.generated_file.name} generated by ksf2cpp
+ * @date {datetime.now().strftime("%Y-%m-%d %H:%M:%S")}
+ * @version 1.0.0
+ * @copyright kingstar
+ */
+#pragma once
+
+{self.parse_header(with_ksf=True)}
+        
+{self.file_str}
+"""
         # print(self.file_str)
 
         with self.generated_file.open("w") as f:
             f.write(self.file_str)
 
 
-def cpp_gen(files, include_dirs, destination_dir, flags=None):
-    # 读取文件
+################### sdk 模式 ####################
+class CppSdkGenerator(CppParser):
+    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, sdk_invoke,
+                 sdk_export, **kwargs):
+        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, **kwargs)
+        self.sdk_invoke = Path(destination) / sdk_invoke  # 生成的纯rpc头文件
+        self.sdk_export = Path(destination) / sdk_export  # 生成的纯结构体头文件
+
+        self.to_file()
+
+    def parse_enum_pure(self, curr_module, ksf_enum: KsfEnum):
+        enum_str = f"{self.parse_comment_above(ksf_enum.comment)}{self.curr_tab}enum {ksf_enum.name} \n{{\n"
+        enum_member_str_list = []
+        for m in ksf_enum.member:
+            enum_member_str_list.append(self.parse_enum_member(m))
+
+        enum_str += self.add_lines(',\n'.join(enum_member_str_list), 1)
+
+        enum_str += f"}};\n\n"
+        return enum_str
+
+    def parse_enum_func(self, curr_module, ksf_enum: KsfEnum):
+        enum_member_tostr = []
+        enum_member_strto = []
+        for m in ksf_enum.member:
+            enum_member_tostr.append(self.parse_enum_to_str(curr_module, m, True))
+            enum_member_strto.append(self.parse_str_to_enum(curr_module, m, True))
+
+        etos_member = '\n'.join(enum_member_tostr)
+        enum_str = f"""\
+inline std::string etos(const {self.get_full_name(curr_module, ksf_enum.name)} &e) {{
+    switch (e) {{
+{self.add_lines(etos_member, 2)}
+        default: return "";
+    }}
+}}
+
+"""
+
+        stoe_member = '\n'.join(enum_member_strto)
+        enum_str += f"""\
+inline int stoe(const std::string &s, {self.get_full_name(curr_module, ksf_enum.name)} &e) {{
+{self.add_lines(stoe_member, 1)}
+    return -1;
+}}
+
+"""
+        return enum_str
+
+    def parse_resetDefault(self, curr_module, ksf_struct: KsfStruct):
+        return f'''\
+///重新赋值为初始构造的结构
+void resetDefault() {{
+    *this = {ksf_struct.name}{{}}; 
+}}'''
+
+    def parse_variable_writeTo(self, ksf_field: KsfField):
+        value_type = ksf_field.value_type
+        if self.with_check_default:
+            if isinstance(value_type, KsfBuildInType):
+                if value_type.name != 'bool':
+                    return f"""{self.parse_default_var(f'obj.{ksf_field.name}', value_type, ksf_field.default)} {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                else:
+                    if ksf_field.default is None or ksf_field.default['value']:
+                        return f"""if (!obj.{ksf_field.name}) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                    else:
+                        return f"""if (obj.{ksf_field.name}) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+            elif isinstance(value_type, KsfStructType):
+                # 如果是枚举类型
+                if value_type.name in self.ast.enums:
+                    return f"_os.write((int32_t)obj.{ksf_field.name}, {ksf_field.tag});"
+                else:
+                    return f"_os.write(obj.{ksf_field.name}, {ksf_field.tag});"
+            elif isinstance(value_type, KsfVectorType):
+                return f"""if (!obj.{ksf_field.name}.empty()) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+            elif isinstance(value_type, KsfMapType):
+                return f"""if (!obj.{ksf_field.name}.empty()) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+            else:
+                raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+        else:
+            return f"_os.write(obj.{ksf_field.name}, {ksf_field.tag});"
+
+    def parse_writeTo(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            var_list += self.parse_variable_writeTo(ksf_struct.variable[var]) + '\n'
+
+        return self.add_lines(f'''\
+    ///序列化为二进制流
+    template<typename WriterT>
+    void writeTo(ksf::KsfOutputStream<WriterT>& _os) const {{
+{self.add_lines(var_list, 2)}\
+    }}\n''')
+
+    def parse_variable_writeToJson(self, curr_module, ksf_field: KsfField):
+        return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson(obj.{ksf_field.name});"""
+
+    def parse_writeToJson(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            var_list += self.parse_variable_writeToJson(curr_module, ksf_struct.variable[var]) + '\n'
+
+        return self.add_lines(f'''\
+    ///序列化为Json
+    ksf::JsonValueObjPtr writeToJson() const {{
+        ksf::JsonValueObjPtr p = new ksf::JsonValueObj();
+{self.add_lines(var_list, 2)}\
+        return p;
+    }}
+
+    ///序列化为Json字符串
+    std::string writeToJsonString() const {{
+        return ksf::KS_Json::writeValue(writeToJson());
+    }}\n''')
+
+    def parse_variable_readFrom(self, curr_module, ksf_field: KsfField):
+        value_type = ksf_field.value_type
+        if isinstance(value_type, KsfBuildInType):
+            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
+        elif isinstance(value_type, KsfStructType):
+            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
+        elif isinstance(value_type, KsfVectorType):
+            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
+        elif isinstance(value_type, KsfMapType):
+            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
+        else:
+            raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+
+    def parse_readFrom(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            var_list += self.parse_variable_readFrom(curr_module, ksf_struct.variable[var]) + '\n'
+
+        return self.add_lines(f'''\
+    ///二进制反序列化为结构体
+    template<typename ReaderT>
+    void readFrom(ksf::KsfInputStream<ReaderT>& _is) {{
+        obj.resetDefault();
+{self.add_lines(var_list, 2)}\
+    }}\n''')
+
+    def parse_variable_readFromJson(self, curr_module, ksf_field: KsfField):
+        return f"""ksf::JsonInput::readJson(obj.{ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
+
+    def parse_readFromJson(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            var_list += self.parse_variable_readFromJson(curr_module, ksf_struct.variable[var]) + '\n'
+
+        return self.add_lines(f'''\
+    ///Json反序列化为结构体
+    void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
+        obj.resetDefault();
+        if(NULL == p.get() || p->getType() != ksf::eJsonTypeObj) {{
+            char s[128];
+            snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p.get() ? p->getType() : 0));
+            throw ksf::KS_Json_Exception(s);
+        }}
+
+        ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
+{self.add_lines(var_list, 2)}\
+    }}
+
+    ///Json字符串反序列化为结构体
+    void readFromJsonString(const std::string &str) {{
+        readFromJson(ksf::KS_Json::getValue(str));
+    }}\n''')
+
+    def parse_display(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            field = ksf_struct.variable[var]
+            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
+                                                                        field.value_type) in self.ast.enums:
+                var_list += f'_ds.display(static_cast<int32_t>(obj.{ksf_struct.variable[var].name}),"{ksf_struct.variable[var].name}");\n'
+            else:
+                var_list += f'_ds.display(obj.{ksf_struct.variable[var].name}, "{ksf_struct.variable[var].name}");\n'
+
+        return self.add_lines(f'''\
+    ///打印
+    std::ostream& display(std::ostream& _os, int _level=0) const
+    {{
+        ksf::KsfDisplayer _ds(_os, _level);
+{self.add_lines(var_list, 2)}
+        return _os;
+    }}\n''')
+
+    def parse_displaySimple(self, curr_module, ksf_struct: KsfStruct):
+        var_list = ""
+        for var in ksf_struct.variable:
+            field = ksf_struct.variable[var]
+            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
+                                                                        field.value_type) in self.ast.enums:
+                var_list += f'_ds.displaySimple(static_cast<int32_t>(obj.{ksf_struct.variable[var].name}), true);\n'
+            else:
+                var_list += f'_ds.displaySimple(obj.{ksf_struct.variable[var].name}, true);\n'
+
+        return self.add_lines(f'''\
+    ///简单打印
+    std::ostream& displaySimple(std::ostream& _os, int _level=0) const
+    {{
+        ksf::KsfDisplayer _ds(_os, _level);
+{self.add_lines(var_list, 2)}
+        return _os;
+    }}\n''')
+
+    def parse_equal(self, curr_module, ksf_struct: KsfStruct):
+        var_list = []
+        for var in ksf_struct.variable:
+            field = ksf_struct.variable[var]
+            if field.value_type['type'] == "native" and field.value_type.name in {'float', 'double'}:
+                var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
+            else:
+                var_list.append(f'l.{field.name} == r.{field.name}')
+
+        in_list = ' && '
+        var_eq = in_list.join(var_list)
+        return self.add_lines(f'''\
+inline bool operator==(const {self.get_full_name(curr_module, ksf_struct.name)} &l, const {self.get_full_name(curr_module, ksf_struct.name)} &r) {{
+    return {var_eq};
+}}\n''')
+
+    def parse_struct_pure(self, curr_module, ksf_struct: KsfStruct):
+        struct_str = f"{self.parse_comment_above(ksf_struct.comment)}"  # 注释(可能没有)
+
+        struct_str += self.add_lines(f"struct {ksf_struct.name} \n{{")
+
+        # 解析字段
+        var_list = []
+        for var in ksf_struct.variable:
+            var_list.append(self.parse_variable(curr_module, ksf_struct.variable[var]))
+
+        var_widths = self.get_column_widths(var_list)
+        for comment, var_type, var_name, var_value in var_list:
+            if comment:
+                struct_str += self.add_lines(f"{comment:<{var_widths[0]}}", 1)
+            struct_str += self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}", 1)
+
+        struct_str += '\npublic:\n'
+        struct_str += self.add_lines(f"using __self__ = {ksf_struct.name}; //结构体自指标识", 1)
+        struct_str += '\npublic:\n'
+        struct_str += self.add_lines(self.parse_resetDefault(curr_module, ksf_struct), 1)  # resetDefault
+
+        struct_str += '};\n\n'
+        return struct_str
+
+    def parse_struct_warp(self, curr_module, ksf_struct: KsfStruct):
+        full_struct_name = self.get_full_name(ksf_struct.module, ksf_struct.name)
+        struct_str = self.add_lines(f"template<> struct ksf::Wrap<{full_struct_name}> : public ksf::KsfStructBase\n{{")
+        struct_str += f"""\
+public:
+    {full_struct_name} sobj;
+    {full_struct_name} &obj;
+
+public:
+    static std::string className() {{
+        return "{ksf_struct.module}.{ksf_struct.name}";
+    }}
+
+    static std::string MD5() {{
+        return "{md5(ksf_struct.id.encode('utf-8')).hexdigest()}";
+    }}
+
+public:
+    ///构造函数&析构函数
+    Wrap(): obj(sobj) {{obj.resetDefault();}}
+    Wrap(Wrap&& wrap): sobj(std::move(wrap.sobj)), obj(sobj) {{}}
+    Wrap({full_struct_name}& object): obj(object) {{}}
+    Wrap(const {full_struct_name}& object): obj(*(const_cast<{full_struct_name}*>(&object))) {{}}
+    virtual ~Wrap() = default;
+
+public:
+"""
+
+        struct_str += self.parse_writeTo(curr_module, ksf_struct)  # writeTo
+
+        struct_str += '\n'
+        struct_str += self.parse_readFrom(curr_module, ksf_struct)  # readFrom
+
+        if self.with_json:
+            self.add_include("<kup/KsfJson.h>")
+            struct_str += '\n'
+            struct_str += self.parse_writeToJson(curr_module, ksf_struct)  # writeToJson
+
+            struct_str += '\n'
+            struct_str += self.parse_readFromJson(curr_module, ksf_struct)  # readFromJson
+
+        self.add_include("<ostream>")
+        struct_str += '\n'
+        struct_str += self.parse_display(curr_module, ksf_struct)  # display
+
+        struct_str += '\n'
+        struct_str += self.parse_displaySimple(curr_module, ksf_struct)  # displaySimple
+
+        struct_str += f"""\
+    ///转换为字符串
+    std::string toString() const {{
+        std::stringstream ss; 
+        display(ss); 
+        return ss.str(); 
+    }}
+"""
+        # };
+        struct_str += f"}};\n"
+
+        # inline bool operator==(const {ksf_struct.name}&l, const {ksf_struct.name}&r)
+        struct_str += f'\n{self.get_ns_begin(curr_module)}\n'
+
+        # operator==
+        struct_str += self.parse_equal(curr_module, ksf_struct)
+        struct_str += '\n'
+        # operator!=
+        struct_str += f"""\
+inline bool operator!=(const {full_struct_name} &l, const {full_struct_name} &r) {{
+    return !(l == r);
+}}
+"""
+        if len(ksf_struct.key_fields) != 0:
+            struct_str += f"""\
+inline bool operator<(const {full_struct_name} &l, const {full_struct_name} &r) {{\n"""
+            for key_field in ksf_struct.key_fields:
+                struct_str += f"""\
+    if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});
+    return false;
+}}
+
+inline bool operator<=(const {full_struct_name} &l, const {full_struct_name} &r) {{
+    return !(r < l);
+}}
+
+inline bool operator>(const {full_struct_name} &l, const {full_struct_name} &r) {{
+    return r < l;
+}}
+
+inline bool operator>=(const {full_struct_name} &l, const {full_struct_name} &r) {{
+    return !(l < r);
+}}
+"""
+
+        if self.with_json:
+            struct_str += '\n'
+            # operator<<
+            struct_str += f"""\
+inline std::ostream &operator<<(std::ostream &os, const {full_struct_name} &r) {{
+    os << ksf::MakeWrap(r).writeToJsonString();
+    return os;
+}}
+
+inline std::ostream &operator<<(std::ostream &os, const ksf::Wrap<{full_struct_name}> &r) {{
+    os << r.writeToJsonString();
+    return os;
+}}
+"""
+
+            struct_str += '\n'
+            # operator>>
+            struct_str += f"""\
+inline std::istream &operator>>(std::istream &is, {full_struct_name} &l) {{
+    std::istreambuf_iterator<char> eos;
+    std::string s(std::istreambuf_iterator<char>(is), eos);
+    ksf::MakeWrap(l).readFromJsonString(s);
+    return is;
+}}
+
+inline std::istream &operator>>(std::istream &is, ksf::Wrap<{full_struct_name}> &l) {{
+    std::istreambuf_iterator<char> eos;
+    std::string s(std::istreambuf_iterator<char>(is), eos);
+    l.readFromJsonString(s);
+    return is;
+}}
+
+using {ksf_struct.name}Wrap = ksf::Wrap<{full_struct_name}>;
+{self.get_ns_end(curr_module, with_endl=False)}
+
+"""
+
+        return struct_str
+
+    def parse_InterfacePrxCallBack(self, curr_module, ksf_interface: KsfInterface):
+        prx_str = f"""\
+class {ksf_interface.name}WrapPrxCallback : public ksf::AgentCallback
+{{
+public:
+    virtual ~{ksf_interface.name}WrapPrxCallback() = default;
+
+public:
+\n"""
+
+        index = 0
+        func_case_str = ""
+        for item in ksf_interface.operator:
+            operator = ksf_interface.operator[item]
+            if not operator.export:
+                continue
+
+            def parse_output_vars(with_type=True):
+                def parse_output_var(value_type, name, with_type):
+                    if value_type.name != 'void':
+                        if not self.is_movable_type(curr_module, value_type):
+                            return f"{self.parse_type(curr_module, value_type, is_wrap=True)} {name}" if with_type else name
+                        elif self.with_param_rvalue_ref:
+                            return f"{self.parse_type(curr_module, value_type, is_wrap=True)} &&{name}" if with_type else f"std::move({name})"
+                        else:
+                            return f"const {self.parse_type(curr_module, value_type, is_wrap=True)} &{name}" if with_type else name
+
+                vars_list = []
+                if operator.return_type['name'] != 'void':
+                    vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
+
+                for i in operator.output:
+                    vars_list.append(
+                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type))
+
+                return ', '.join(vars_list)
+
+            prx_str += f"""\
+    virtual void callback_{operator.name}Wrap({parse_output_vars(True)}) \
+{{ throw std::runtime_error("callback_{operator.name}Wrap override incorrect."); }}
+
+    virtual void callback_{operator.name}Wrap_exception(int32_t ret) \
+{{ throw std::runtime_error("callback_{operator.name}Wrap_exception override incorrect."); }}
+
+"""
+
+            def parse_var_dispatch(var, name, index):
+                if var['name'] == 'void':
+                    return ""
+
+                return f"""\
+                {self.parse_type(curr_module, var, is_wrap=True)} {name};
+                _is.read({name}, {index}, true);\n\n"""
+
+            def parse_func_dispatch():
+                """处理函数的分发"""
+                func_case_str = f"""
+            case {index}: {{
+                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
+                    callback_{operator.name}Wrap_exception(msg->response->iRet);
+                    return msg->response->iRet;
+                }}
+
+                ksf::KsfInputStream<ksf::BufferReader> _is;
+
+                _is.setBuffer(msg->response->sBuffer);\n\n"""
+
+                func_case_str += parse_var_dispatch(operator.return_type, '_ret', 0)
+
+                for i in operator.output:
+                    var = operator.output[i]
+                    func_case_str += parse_var_dispatch(var.value_type, var.name, var.index)
+
+                func_case_str += f"""\
+
+                ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
+                assert(pCbtd != NULL);
+
+                pCbtd->setResponseContext(msg->response->context);
+
+                callback_{operator.name}Wrap({parse_output_vars(False)});
+
+                pCbtd->delResponseContext();
+
+                return ksf::KSFSERVERSUCCESS;
+            }}"""
+                return func_case_str
+
+            func_case_str += parse_func_dispatch()
+            index += 1
+
+        # 函数列表
+        prx_str += f"""\
+public:
+    virtual const std::map<std::string, std::string> &getResponseContext() const {{
+        ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
+        assert(pCbtd != NULL);
+
+        if (!pCbtd->getContextValid()) {{
+            throw ksf::KS_Exception("cann't get response context");
+        }}
+        return pCbtd->getResponseContext();
+    }}\n\n"""
+
+        prx_str += f"""\
+public:
+    int onDispatch(ksf::ReqMessagePtr msg) override {{
+        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
+
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+
+        if (r.first == r.second) {{
+            return ksf::KSFSERVERNOFUNCERR;
+        }}
+
+        switch (r.first - __{ksf_interface.name}_all) {{
+{func_case_str}
+        }} //end switch
+
+        return ksf::KSFSERVERNOFUNCERR;
+    }} //end onDispatch\n"""
+
+        prx_str += f"""}}; //end {ksf_interface.name}PrxCallback
+
+using {ksf_interface.name}WrapPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallback>;\n\n"""
+
+        return prx_str
+
+    def parse_InterfacePrxCallbackPromise(self, curr_module, ksf_interface: KsfInterface):
+        parsed_str = f"""\
+class {ksf_interface.name}WrapPrxCallbackPromise: public ksf::AgentCallback
+{{
+public:
+    virtual ~{ksf_interface.name}WrapPrxCallbackPromise() = default;
+\n"""
+
+        dispatch_case_str = ""
+        case_index = 0
+        for item in ksf_interface.operator:
+            operator = ksf_interface.operator[item]
+            if not operator.export:
+                continue
+
+            parsed_str += f"""\
+public:
+    struct Promise{operator.name}: virtual public KS_HandleBase 
+    {{
+    public:
+        std::map<std::string, std::string> _mRspContext;\n"""
+
+            if operator.return_type['name'] != 'void':
+                parsed_str += f"\
+        {self.parse_type(curr_module, operator.return_type, is_wrap=True)} _ret;\n"
+
+            for item in operator.output:
+                var = operator.output[item]
+                parsed_str += f"\
+        {self.parse_type(curr_module, var.value_type, is_wrap=True)} {var.name};\n"
+
+            parsed_str += f"""\
+    }};
+
+    using Promise{operator.name}Ptr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}>;
+
+    {ksf_interface.name}WrapPrxCallbackPromise(const ksf::Promise<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr> &promise): _promise_{operator.name}(promise) {{}}
+
+    virtual void callback_{operator.name}Wrap(const {ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr &ptr) {{
+        _promise_{operator.name}.setValue(ptr);
+    }}
+
+    virtual void callback_{operator.name}Wrap_exception(ksf::Int32 ret) {{
+        std::stringstream oss;
+        oss << "Function:{operator.name}Wrap_exception|Ret:";
+        oss << ret;
+        _promise_{operator.name}.setException(ksf::copyException(oss.str(), ret));
+    }}
+
+protected:
+    ksf::Promise<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr > _promise_{operator.name};\n\n"""
+
+            def parse_var_dispatch(var, name, index):
+                if var['name'] == 'void':
+                    return ""
+
+                return f"""\
+                    _is.read(ptr->{name}, {index}, true);\n"""
+
+            def parse_func_dispatch():
+                """处理函数的分发"""
+                func_case_str = f"""\
+            case {case_index}: {{
+                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
+                    callback_{operator.name}Wrap_exception(msg->response->iRet);
+                    return msg->response->iRet;
+                }}
+
+                ksf::KsfInputStream<ksf::BufferReader> _is;
+                _is.setBuffer(msg->response->sBuffer);
+                {ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr ptr = new {ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}();
+
+                try {{\n"""
+
+                func_case_list = []
+                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
+                if ret != "":
+                    func_case_list.append(ret)
+
+                for item2 in operator.output:
+                    var2 = operator.output[item2]
+                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
+
+                func_case_str += ''.join(func_case_list)
+                return func_case_str
+
+            case_index += 1
+            dispatch_case_str += parse_func_dispatch()
+            dispatch_case_str += f"""\
+                }} catch (std::exception &ex) {{
+                    callback_{operator.name}Wrap_exception(ksf::KSFCLIENTDECODEERR);
+                    return ksf::KSFCLIENTDECODEERR;
+                }} catch (...) {{
+                    callback_{operator.name}Wrap_exception(ksf::KSFCLIENTDECODEERR);
+                    return ksf::KSFCLIENTDECODEERR;
+                }}
+
+                ptr->_mRspContext = msg->response->context;
+                callback_{operator.name}Wrap(ptr);
+                return ksf::KSFSERVERSUCCESS;
+            }}\n"""
+
+        parsed_str += f"""\
+public:
+    int onDispatch(ksf::ReqMessagePtr msg) override
+    {{
+        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
+
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+
+        if (r.first == r.second) {{
+            return ksf::KSFSERVERNOFUNCERR;
+        }}
+
+        switch (r.first - __{ksf_interface.name}_all) {{\n"""
+        parsed_str += dispatch_case_str
+        parsed_str += f"""\
+        }} //end switch
+
+        return ksf::KSFSERVERNOFUNCERR;
+    }} //end onDispatch\n"""
+
+        parsed_str += f"\n}}; //end {ksf_interface.name}WrapPrxCallbackPromise\n\n" \
+                      f"using {ksf_interface.name}WrapPrxCallbackPromisePtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallbackPromise>;\n" \
+                      f"\n"
+        return parsed_str
+
+    def parse_InterfaceCoroPrxCallback(self, curr_module, ksf_interface: KsfInterface):
+        def parse_var_dispatch(var, name, index):
+            if var['name'] == 'void':
+                return ""
+
+            return f"""\
+                    {self.parse_type(curr_module, var)} {name};
+                    _is.read({name}, {index}, true);\n\n"""
+
+        def parse_func_dispatch():
+            """处理函数的分发"""
+            func_case_str = ""
+            index = 0
+            for item in ksf_interface.operator:
+                operator = ksf_interface.operator[item]
+                if not operator.export:
+                    index += 1
+                    continue
+
+                def parse_output_vars(with_type=True):
+                    def parse_output_var(value_type, name, with_type):
+                        if value_type.name != 'void':
+                            if not self.is_movable_type(curr_module, value_type):
+                                return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
+                            elif self.with_param_rvalue_ref:
+                                return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
+                            else:
+                                return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
+
+                    vars_list = []
+                    if operator.return_type.name != 'void':
+                        vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
+
+                    for item in operator.output:
+                        vars_list.append(
+                            parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type))
+
+                    return ', '.join(vars_list)
+
+                func_case_str += f"""
+            case {index}: {{
+                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
+                    callback_{operator.name}Wrap_exception(msg->response->iRet);
+                    return msg->response->iRet;
+                }}
+
+                ksf::KsfInputStream<ksf::BufferReader> _is;
+                _is.setBuffer(msg->response->sBuffer);
+
+                try {{\n"""
+                func_case_list = []
+                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
+                if ret != "":
+                    func_case_list.append(ret)
+
+                for item2 in operator.output:
+                    var2 = operator.output[item2]
+                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
+
+                func_case_str += ''.join(func_case_list)
+
+                func_case_str += f"""\
+                    callback_{operator.name}Wrap({parse_output_vars(with_type=False)});
+                }} catch (std::exception &ex) {{
+                    callback_{operator.name}Wrap_exception(ksf::KSFCLIENTDECODEERR);
+                    return ksf::KSFCLIENTDECODEERR;
+                }} catch (...) {{
+                    callback_{operator.name}Wrap_exception(ksf::KSFCLIENTDECODEERR);
+                    return ksf::KSFCLIENTDECODEERR;
+                }}
+
+                return ksf::KSFSERVERSUCCESS;
+            }}\n"""
+
+                index += 1
+
+            return func_case_str
+
+        parsed_str = f"""\
+class {ksf_interface.name}WrapCoroPrxCallback : public {ksf_interface.name}WrapPrxCallback
+{{
+public:
+    virtual ~{ksf_interface.name}WrapCoroPrxCallback() = default;
+
+public:
+    const std::map<std::string, std::string> &getResponseContext() const override {{ return _mRspContext; }}
+
+    virtual void setResponseContext(const std::map<std::string, std::string> &mContext) {{ _mRspContext = mContext; }}
+"""
+        parsed_str += f"""\
+public:
+    int onDispatch(ksf::ReqMessagePtr msg) override
+    {{
+        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
+
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+
+        if (r.first == r.second) {{
+            return ksf::KSFSERVERNOFUNCERR;
+        }}
+
+        switch (r.first - __{ksf_interface.name}_all) {{
+{parse_func_dispatch()}
+        }} //end switch
+
+        return ksf::KSFSERVERNOFUNCERR;
+    }} //end onDispatch
+
+protected:
+    std::map<std::string, std::string> _mRspContext;
+}}; //end {ksf_interface.name}WrapCoroPrxCallback
+
+using {ksf_interface.name}WrapCoroPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapCoroPrxCallback>;\n\n"""
+        return parsed_str
+
+    def parse_InterfaceProxy(self, curr_module, ksf_interface: KsfInterface):
+        def parse_operators():
+            parsed_oper_str = ""
+            for item in ksf_interface.operator:
+                operator = ksf_interface.operator[item]
+                if not operator.export:
+                    continue
+
+                def has_return():
+                    return operator.return_type['name'] != 'void'
+
+                def parse_input_vars():
+                    parsed_list = []
+                    for name in operator.input:
+                        var = operator.input[name]
+                        parsed_list.append(f"""\
+        _os.write({name}, {var.index});\n""")
+                    return parsed_list
+
+                def parse_output_vars():
+                    parsed_list = []
+                    if operator.return_type['name'] != 'void':
+                        parsed_list.append(f"""\
+        {self.parse_type(curr_module, operator.return_type, is_wrap=True)} _ret;
+        _is.read(_ret, 0, true);\n""")
+
+                    for name in operator.output:
+                        var = operator.output[name]
+                        parsed_list.append(f"""\
+        _is.read({name}, {var.index}, true);\n""")
+                    return parsed_list
+
+                def parse_all_vars(with_output=False):
+                    parsed_list = []
+                    for var_name, is_output in operator.ordered_var:
+                        if is_output:
+                            if with_output:
+                                parsed_list.append(
+                                    f"{self.parse_type(curr_module, operator.output[var_name].value_type, is_wrap=True)} &{var_name}, ")
+                        else:
+                            parsed_list.append(
+                                f"const {self.parse_type(curr_module, operator.input[var_name].value_type, is_wrap=True)} &{var_name}, ")
+
+                    return parsed_list
+
+                parsed_oper_str += f"""\
+public:
+{self.parse_comment_above(operator.comment, tab='    ')}\
+    {self.parse_type(curr_module, operator.return_type, is_wrap=True) if has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}const std::map<std::string, std::string> &mapReqContext = {{}}, std::map<std::string, std::string> *pResponseContext = NULL) {{
+        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
+{''.join(parse_input_vars())}
+        std::map<std::string, std::string>   _mStatus;
+        std::shared_ptr<ksf::ResponsePacket> rep = ksf_invoke(ksf::KSFNORMAL, "{operator.name}", _os, mapReqContext, _mStatus);
+        if (pResponseContext) {{
+            pResponseContext->swap(rep->context);
+        }}
+
+        ksf::KsfInputStream<ksf::BufferReader> _is;
+        _is.setBuffer(rep->sBuffer);
+{''.join(parse_output_vars())}
+{f'''        return _ret;
+    }}''' if has_return() else '    }'}
+
+    void async_{operator.name}({ksf_interface.name}WrapPrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = {{}}) {{
+        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
+{''.join(parse_input_vars())}
+        std::map<std::string, std::string> _mStatus;
+        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback);
+    }}
+
+    ksf::Future<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr> promise_async_{operator.name}({''.join(parse_all_vars())}const std::map<std::string, std::string> &context) {{
+        ksf::Promise<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr> promise;
+        {ksf_interface.name}WrapPrxCallbackPromisePtr callback = new {ksf_interface.name}WrapPrxCallbackPromise(promise);
+
+        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
+{''.join(parse_input_vars())}
+        std::map<std::string, std::string> _mStatus;
+        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback);
+
+        return promise.getFuture();
+    }}
+
+    void coro_{operator.name}({ksf_interface.name}WrapCoroPrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = {{}}) {{
+        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
+{''.join(parse_input_vars())}
+        std::map<std::string, std::string>            _mStatus;
+        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback, true);
+    }}\n\n"""
+            return parsed_oper_str
+
+        parsed_str = f"""\
+class {ksf_interface.name}WrapProxy : public ksf::Agent
+{{
+public:
+    {ksf_interface.name}WrapProxy* ksf_hash(uint32_t key) {{
+        return ({ksf_interface.name}WrapProxy*)Agent::ksf_hash(key);
+    }}
+
+    {ksf_interface.name}WrapProxy* ksf_consistent_hash(uint32_t key) {{
+        return ({ksf_interface.name}WrapProxy*)Agent::ksf_consistent_hash(key);
+    }}
+
+    {ksf_interface.name}WrapProxy* ksf_open_trace(bool traceParam = false) {{
+        return ({ksf_interface.name}WrapProxy*)Agent::ksf_open_trace(traceParam);
+    }}
+
+    {ksf_interface.name}WrapProxy* ksf_set_timeout(int32_t ms) {{
+        return ({ksf_interface.name}WrapProxy*)Agent::ksf_set_timeout(ms);
+    }}
+
+    static const char* ksf_prxname() {{ return "{ksf_interface.name}WrapProxy"; }}
+
+{parse_operators()}
+}}; //end {ksf_interface.name}WrapProxy
+
+using {ksf_interface.name}WrapPrx = ksf::KS_AutoPtr<{ksf_interface.name}WrapProxy>;\n\n"""
+
+        return parsed_str
+
+    def parse_interface(self, curr_module, ksf_interface: KsfInterface):
+        interface_str = ''
+
+        self.add_include("<servant/Agent.h>")
+        self.add_include("<servant/Servant.h>")
+
+        interface_str += self.add_lines(self.parse_InterfacePrxCallBack(curr_module, ksf_interface))
+        self.add_include("<promise/promise.h>")
+        interface_str += self.add_lines(self.parse_InterfacePrxCallbackPromise(curr_module, ksf_interface))
+        interface_str += self.parse_InterfaceCoroPrxCallback(curr_module, ksf_interface)
+        interface_str += self.parse_InterfaceProxy(curr_module, ksf_interface)
+
+        return interface_str
+
+    def to_file(self):
+        if len(self.ast.get_all_export_symbol()) == 0:
+            raise RuntimeError("no export symbol")
+
+        curr_module = None
+        const_list = []
+        enum_list = []
+        struct_list = []
+        hidden_str = ''
+        export_str = ''
+
+        for sym in self.ast.get_all_export_symbol():
+            ele = self.ast.all_element.obj[sym]
+            module = ele.module
+
+            if isinstance(ele, KsfConst):
+                const_list.append((ele.module, self.parse_const(module, ele)))
+                pass
+            elif isinstance(ele, KsfEnum):
+                enum_list.append((ele.module, self.parse_enum_pure(module, ele)))
+                hidden_str += self.parse_enum_func(module, ele)
+                pass
+            elif isinstance(ele, KsfStruct):
+                struct_list.append((ele.module, self.parse_struct_pure(module, ele)))
+                hidden_str += self.parse_struct_warp(module, ele)
+                pass
+            elif isinstance(ele, KsfInterface) and self.with_rpc:
+                hidden_str += f"{self.get_ns_begin(ele.module)}"
+                hidden_str += self.parse_interface(module, ele)
+                hidden_str += f"{self.get_ns_end(module)} "
+
+        for module, text in const_list + enum_list + struct_list:
+            if curr_module is None:
+                curr_module = module
+                export_str += f"""\
+{self.get_ns_begin(module)}
+"""
+            elif curr_module != module:
+                export_str += f"""\
+{self.get_ns_end(curr_module)}
+
+{self.get_ns_begin(module)}
+"""
+                curr_module = module
+            export_str += text
+
+        export_str = f"#pragma once\n\n{self.parse_header(with_ksf=False)}{export_str}{self.get_ns_end(curr_module)}\n\n"
+        hidden_str = "#pragma once\n\n" + self.parse_header(
+            with_ksf=True) + "\n\n" + f'#include "{self.sdk_export.name}"\n\n' + hidden_str
+
+        with self.sdk_export.open("w") as f:
+            f.write(export_str)
+
+        with self.sdk_invoke.open("w") as f:
+            f.write(hidden_str)
+
+
+def cpp_gen(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, flags=None):
+    """生成cpp文件"""
     # parser_grammar = {}
     if flags is None:
         flags = defaultdict(bool)
 
     file_path = files
 
     real_inc_dirs = set()
     for inc in include_dirs:
         real_inc_dirs.add(str(Path(inc).resolve()))
-    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'])
+    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], [])
     for file in file_path:
-        CppGenerator(ast, file, destination_dir, **flags).to_file()
+        CppGenerator(ast, file, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, **flags)
+
+
+def cpp_sdk_gen(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, export_symbols,
+                sdk_invoke, sdk_export, flags=None):
+    """生成cpp sdk文件"""
+    if flags is None:
+        flags = defaultdict(bool)
+
+    file_path = files
+
+    real_inc_dirs = set()
+    for inc in include_dirs:
+        real_inc_dirs.add(str(Path(inc).resolve()))
+    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbols)
+    CppSdkGenerator(ast, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, export_symbols,
+                    sdk_invoke, sdk_export, **flags)
 
 
 # 测试用例
 if __name__ == '__main__':
     file_path = [
         'example/enum_simple.ksf',
         'example/const_definition.ksf',
         'example/struct_simple.ksf'
     ]
 
     include_dirs = ['../../']
 
-    destination_dir = '../../gen'
+    destination_dir = '../../../gen'
 
-    cpp_gen(file_path, include_dirs, destination_dir)
+    cpp_gen(file_path, {}, {}, include_dirs, destination_dir)
+    cpp_sdk_gen(file_path, {}, {}, include_dirs, destination_dir)
```

### Comparing `ksfctl-0.2/ksfctl/parser/ksf_lex.py` & `ksfctl-0.2.1/ksfctl/parser/ksf_lex.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
         'INCLUDE',
         'INTERFACE',
         'MODULE',
         'STRUCT',
         'ENUM',
         'CONST',
         'KEY',
+        'USING',
+        'IMPORT',
+        'EXPORT',
 
         # 符号
         'LEFT_PAREN',
         'RIGHT_PAREN',
         'LEFT_BRACE',
         'RIGHT_BRACE',
         "LEFT_SQUARE",
@@ -128,14 +131,17 @@
             "int": "INT",
             "unsigned": "UNSIGNED",
             "key": "KEY",
             "out": "OUTPUT",
             "const": "CONST",
             "false": "FALSE",
             "true": "TRUE",
+            "using": "USING",
+            "import": "IMPORT",
+            "export": "EXPORT",
         }.get(t.value, "IDENTIFIER")
         return t
 
     # 定义字符串
     def t_STRING_CONSTANT(self, t):
         r""""[^"]*\""""
         t.value = t.value[1:-1]
```

### Comparing `ksfctl-0.2/ksfctl/parser/ksf_yacc.py` & `ksfctl-0.2.1/ksfctl/parser/ksf_yacc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import warnings
 
 import ply.yacc as yacc
 
 from ksfctl.parser.ksf_lex import KsfLexer
 from ksfctl.parser.ksf_parser import *
-from ksfctl.parser.tools import Graph
+from ksfctl.parser.tools import *
 
 
 class KsfParser:
     def __init__(self):
         # 解析语法的准备
         self.lexer = KsfLexer()
         self.lexer.build()
@@ -184,14 +184,15 @@
     ####### 结构体进行比较时需要的字段关联 #######
     def p_struct_keyword(self, p):
         """
         struct_keyword : KEY LEFT_SQUARE IDENTIFIER COMMA key_params RIGHT_SQUARE SEMICOLON
         """
         p[0] = {
             'element': 'key',
+            'name': f'key[{p[3]}]',
             'struct': p[3],
             'args': p[5]
         }
 
     ######### 各类list #########
     def p_opt_comma(self, p):
         """
@@ -610,24 +611,24 @@
             SyntaxError("Syntax error at EOF")
 
 
 def pretty_print(jvalue):
     print(json.dumps(jvalue, indent=2, ensure_ascii=False))
 
 
-def generate_ksf_ast(grammar, search_dirs):
+def generate_ksf_ast(grammar, export_symbols=None):
     """
     检查解析出的语法数据是否合法，并生成基础ast树
     :param grammar:
     :return:
     """
-
-    # 1. 生成头文件包含树
     g_files = Graph()  # 文件有向图
     g_files_reverse = Graph()  # 文件逆向有向图
+
+    # 1. 生成头文件包含树
     for file in grammar:
         curr = file
         if len(grammar[file]['include']) != 0:
             for include in grammar[file]['include']:
                 # 在search路径中添加当前文件所在路径
 
                 inc_path = Path(include)
@@ -669,15 +670,16 @@
         if name not in flag_dicts[flag]:
             return False, f"该名称[{name}]不存在"
 
         if filename is None or flag_dicts[flag][name] is None:
             return True, ""
 
         # 如果filename不为None, 则需要递归的判断一下该名称所在的文件是否位于当前文件所能依赖的所有文件中
-        if flag_dicts[flag][name] == filename or flag_dicts[flag][name] in g_files_reverse.get_all_prev(filename, with_self=True):
+        if flag_dicts[flag][name] == filename or flag_dicts[flag][name] in g_files_reverse.get_all_prev(filename,
+                                                                                                        with_self=True):
             return True, ""
         else:
             return False, f"该名称[{name}]不位于被[{filename}]依赖的文件中"
 
     def traverse_all_file(func):
         # 处理单点文件
         for cur_file in grammar:
@@ -685,59 +687,47 @@
                 func(cur_file)
 
         # 按照依赖顺序遍历文件
         g_files.bfs_dag(func)
 
     # traverse_all_file(lambda a:print(a))
     # exit(0)
+
     def check_module_depends(filename):
         for module_desc in grammar[filename]['module']:
             # print(f'检测文件[{filename}]的模块[{module_desc["name"]}]中...')
             module_name = module_desc["name"]
 
-            # 判断类型是否合法
-            def is_valid(etype, default=None):
-                # native 为原生类型，不用解析
-                if etype['type'] == 'native':
-                    return True
+            for element in module_desc['elements']:
+                curr_element_name = module_name + '.' + element['name']
+                if 'name' in element and is_name_collision('element', curr_element_name, filename):
+                    raise SyntaxError(f"不允许有重复的模块元素命名{curr_element_name}")
+
+                # 判断类型是否合法
+                def is_valid(etype, *callback):
+                    # native 为原生类型，不用解析
+                    if etype['type'] == 'native':
+                        return True
+
+                    # vector 需递归解析
+                    if etype['type'] == 'vector':
+                        return is_valid(etype['value_type'])
+
+                    # map 则需要 key_type和value_type双解析
+                    if etype['type'] == 'map':
+                        return is_valid(etype['value_type']) and is_valid(etype['key_type'])
 
-                # vector 需递归解析
-                if etype['type'] == 'vector':
-                    return is_valid(etype['value_type'])
-
-                # map 则需要 key_type和value_type双解析
-                if etype['type'] == 'map':
-                    return is_valid(etype['value_type']) and is_valid(etype['key_type'])
-
-                valid, err_msg = has_name('element',
-                                          (module_name if etype['module'] is None else etype['module']) + '.' + etype[
-                                              'name'], filename)
-                if not valid:
-                    raise SyntaxError(err_msg)
-
-                if default is not None:
-                    if not default['is_enum']:
-                        module_enum = default['value'].split("::")
-                        if len(module_enum) == 1:
-                            valid, err_msg = has_name('enum_member', (module_name if etype['module'] is None else etype['module']) + '.' + etype[
-                                              'name'] + '.' + module_enum[0], filename)
-                            if not valid:
-                                raise SyntaxError(err_msg)
-                        elif len(module_enum) == 2:
-                            if module_enum[0] != (module_name if etype['module'] is None else etype['module']):
-                                raise SyntaxError(f"默认的枚举值[{default['value']}]不属于该类型[{etype['name']}]")
-
-                            valid, err_msg = has_name('enum_member', (module_name if etype['module'] is None else etype['module']) + '.' + etype[
-                                              'name'] + '.' + module_enum[1], filename)
-                            if not valid:
-                                raise SyntaxError(err_msg)
+                    element_name = (module_name if etype['module'] is None else etype['module']) + '.' + etype['name']
+                    valid, err_msg = has_name('element', element_name, filename)
+                    if not valid:
+                        raise SyntaxError(err_msg)
 
-            for element in module_desc['elements']:
-                if 'name' in element and is_name_collision('element', module_name + '.' + element['name'], filename):
-                    raise SyntaxError(f"不允许有重复的模块元素命名{module_name + '.' + element['name']}")
+                    if len(callback) != 0:
+                        for cb in callback:
+                            cb(element_name)
 
                 # pretty_print(element)
                 # 判断是否成立的原则：
                 # 1. 类(结构体or枚举)之前是否有其他类定义，包括在依赖的文件中定义的
                 # 2. 接口中定义的类是否被定义
                 if element['element'] == 'enum':
                     for member in element['member']:
@@ -750,35 +740,62 @@
                     for var in element['variable']:
                         if is_name_collision('struct_variable',
                                              module_name + '.' + element['name'] + '.' + var['name']):
                             raise SyntaxError(
                                 f"结构体[{module_name + '.' + element['name']}]不允许有重名的变量{var['name']}")
 
                         value_type = var['value_type']
-                        is_valid(value_type, var['default'] if 'default' in var else None)
+
+                        def check_default(element_name):
+                            default = var['default'] if 'default' in var else None
+                            if default is not None:
+                                if not default['is_enum']:
+                                    module_enum = default['value'].split("::")
+                                    if len(module_enum) == 1:
+                                        valid, err_msg = has_name('enum_member', (
+                                            module_name if value_type['module'] is None else value_type[
+                                                'module']) + '.' + value_type[
+                                                                      'name'] + '.' + module_enum[0], filename)
+                                        if not valid:
+                                            raise SyntaxError(err_msg)
+                                    elif len(module_enum) == 2:
+                                        if module_enum[0] != (
+                                                module_name if value_type['module'] is None else value_type['module']):
+                                            raise SyntaxError(
+                                                f"默认的枚举值[{default['value']}]不属于该类型[{value_type['name']}]")
+
+                                        valid, err_msg = has_name('enum_member', (
+                                            module_name if value_type['module'] is None else value_type[
+                                                'module']) + '.' + value_type[
+                                                                      'name'] + '.' + module_enum[1], filename)
+                                        if not valid:
+                                            raise SyntaxError(err_msg)
+
+                        is_valid(value_type, check_default)
                 elif element['element'] == 'interface':
                     # 对于所有函数，判断 返回值类型、参数类型是否合法
                     # 对于所有函数，判断 参数名是否重复
                     for operator in element['operator']:
                         if is_name_collision('operator_name',
-                                             module_name + '.' + element['name'] + '.' + operator['name']):
+                                             curr_element_name + '.' + operator['name']):
                             raise SyntaxError(
                                 f"不允许有重名的接口函数{module_name + '.' + element['name'] + '.' + operator['name']}")
 
                         def has_return():
                             return operator['return_type']['name'] != 'void'
 
                         has_return() and is_valid(operator['return_type'])
                         for var in operator['variable']:
                             is_valid(var['value_type'])
-                            if is_name_collision('operator_params',
-                                                 module_name + '.' + element['name'] + '.' + operator['name'] + '.' +
-                                                 var['name']):
+                            operator_name = module_name + '.' + element['name'] + '.' + operator['name'] + '.' + var[
+                                'name']
+                            if is_name_collision('operator_params', operator_name + '.' + var['name']):
                                 raise SyntaxError(f"接口[{module_name + '.' + element['name']}]定义中有重复参数名"
-                                                  f"[{module_name + '.' + element['name'] + '.' + operator['name'] + '.' + var['name']}]")
+                                                  f"[{operator_name + '.' + var['name']}]")
+
                 elif element['element'] == 'key':
                     # 对于所有key值, 保证结构体类型合法，参数名存在于结构体定义中，且Key只能定义在对应的模块中，且每一个结构体只能定义一个key
                     valid, err_msg = has_name('element', module_name + '.' + element['struct'], filename)
                     if not valid:
                         raise SyntaxError(f"定义key时，结构体的{err_msg}")
 
                     if is_name_collision('key', module_name + '.' + element['struct'], filename):
@@ -852,14 +869,22 @@
 
     # 检查模块依赖关系，确定合法
     traverse_all_file(check_module_depends)
 
     # 开始转换文件到结构体
     traverse_all_file(parse_file_to_object)
 
+    # 遍历所有导出的元素
+    # for element in Ksf.all_elements:
+    #     if element.id in Ksf.element_graph:
+    #         print(element.id)
+
+    # Ksf.obj_graph.bfs_dag(lambda x: print(x))
+    Ksf.update_export_symbol(export_symbols)
+
 
 def find_file(file_path, search_dirs, with_curr_dir_first):
     file = Path(file_path)
     if with_curr_dir_first and file.exists():
         return file
 
     if file.is_absolute() and not file.exists():
@@ -869,15 +894,15 @@
         search_file = Path(dir) / file_path
         if search_file.exists():
             return search_file
 
     return None
 
 
-def generate(files, search_dirs: set, with_curr_dir_first: bool):
+def generate(files, search_dirs: set, with_curr_dir_first: bool, export_symbols):
     parser_grammar = {}
 
     def parse_depends(file):
         file = find_file(file, search_dirs, with_curr_dir_first)
         if file is None:
             raise FileNotFoundError(f"文件[{file}]没有找到")
 
@@ -906,15 +931,15 @@
                             parse_depends(inc_path)
 
     for file in files:
         parse_depends(file)
 
     # print(parser_grammar.keys())
 
-    generate_ksf_ast(parser_grammar, search_dirs)
+    generate_ksf_ast(parser_grammar, export_symbols)
     return Ksf
 
 
 # 测试用例
 if __name__ == '__main__':
 
     # 读取文件
```

### Comparing `ksfctl-0.2/ksfctl/parser/tools.py` & `ksfctl-0.2.1/ksfctl/parser/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
         if v not in self.graph[u]:
             self.graph[u].append(v)
             return True
         else:
             return False
 
+    def add_node(self, u):
+        if u not in self.graph:
+            self.graph[u] = []
+
     def find_cycle(self):
         # 初始化所有节点的访问状态
         for node in self.graph:
             self.visited[node] = False
 
         # 从每个节点开始搜索，直到找到第一个环
         for node in self.graph:
@@ -112,7 +116,16 @@
             for neighbor in self.graph[current_node]:
                 if neighbor not in visited_nodes:
                     bfs_queue.append(neighbor)
                     visited_nodes.add(neighbor)
 
     def has_node(self, node):
         return node in self.graph
+
+
+def run_once(func):
+    def wrapper(*args, **kwargs):
+        if not wrapper.has_run:
+            wrapper.has_run = True
+            return func(*args, **kwargs)
+    wrapper.has_run = False
+    return wrapper
```

### Comparing `ksfctl-0.2/setup.py` & `ksfctl-0.2.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ksfctl',
-    version='0.2',
+    version='0.2.1',
     keywords='ksf, client, generator, tool',
     description='a auto generator tools for ksf protocol files, and some useful tools',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'ksfctl': ['parser/parser.out'],
     },
     install_requires=[
         'Click>=8.0.0',
-        'ply>=3.0.0'
+        'ply>=3.0.0',
+        'pyyaml>=5.4.1',
     ],
     entry_points='''
         [console_scripts]
         ksfctl=ksfctl.cmd.cmd:cli
         ksf2cpp=ksfctl.cmd.cmd:parse_cpp
     ''',
 )
```

