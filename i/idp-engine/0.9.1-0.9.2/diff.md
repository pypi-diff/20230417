# Comparing `tmp/idp-engine-0.9.1.tar.gz` & `tmp/idp-engine-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idp-engine-0.9.1.tar", max compression
+gzip compressed data, was "idp-engine-0.9.2.tar", max compression
```

## Comparing `idp-engine-0.9.1.tar` & `idp-engine-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    40127 2021-02-22 11:24:27.786697 idp-engine-0.9.1/LICENSE.md
--rw-r--r--   0        0        0     1218 2022-01-18 14:46:21.268113 idp-engine-0.9.1/README-pypi.md
--rw-r--r--   0        0        0    28517 2022-01-25 10:50:39.073231 idp-engine-0.9.1/idp_engine/Annotate.py
--rw-r--r--   0        0        0     9803 2022-01-25 08:43:12.508380 idp-engine-0.9.1/idp_engine/Assignments.py
--rw-r--r--   0        0        0    43884 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Expression.py
--rw-r--r--   0        0        0     2577 2021-11-09 08:55:16.752782 idp-engine-0.9.1/idp_engine/IDP_Z3.py
--rw-r--r--   0        0        0     7002 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Idp.tx
--rw-r--r--   0        0        0    15275 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Idp_to_Z3.py
--rw-r--r--   0        0        0    21822 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Interpret.py
--rw-r--r--   0        0        0    44135 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Parse.py
--rw-r--r--   0        0        0    45458 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Problem.py
--rw-r--r--   0        0        0    18253 2022-01-25 11:03:35.223508 idp-engine-0.9.1/idp_engine/Propagate.py
--rw-r--r--   0        0        0     6656 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Relevance.py
--rw-r--r--   0        0        0     9175 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/Run.py
--rw-r--r--   0        0        0    19629 2022-01-25 08:43:12.516379 idp-engine-0.9.1/idp_engine/Simplify.py
--rw-r--r--   0        0        0      398 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/__init__.py
--rw-r--r--   0        0        0     5049 2022-01-25 10:50:39.077231 idp-engine-0.9.1/idp_engine/utils.py
--rw-r--r--   0        0        0     1191 2022-01-25 11:11:23.246881 idp-engine-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2123 2022-01-25 11:13:32.522309 idp-engine-0.9.1/setup.py
--rw-r--r--   0        0        0     2036 2022-01-25 11:13:32.522559 idp-engine-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    40127 2021-02-22 11:24:27.786697 idp-engine-0.9.2/LICENSE.md
+-rw-r--r--   0        0        0     1218 2022-02-07 16:21:06.451629 idp-engine-0.9.2/README-pypi.md
+-rw-r--r--   0        0        0    28954 2022-02-10 15:32:47.787854 idp-engine-0.9.2/idp_engine/Annotate.py
+-rw-r--r--   0        0        0     9808 2022-02-07 16:21:06.487629 idp-engine-0.9.2/idp_engine/Assignments.py
+-rw-r--r--   0        0        0    45719 2022-02-10 15:32:47.787854 idp-engine-0.9.2/idp_engine/Expression.py
+-rw-r--r--   0        0        0     2577 2021-11-09 08:55:16.752782 idp-engine-0.9.2/idp_engine/IDP_Z3.py
+-rw-r--r--   0        0        0     7009 2022-02-10 15:32:47.787854 idp-engine-0.9.2/idp_engine/Idp.tx
+-rw-r--r--   0        0        0    15275 2022-02-09 17:26:12.238752 idp-engine-0.9.2/idp_engine/Idp_to_Z3.py
+-rw-r--r--   0        0        0    22552 2022-02-10 15:32:47.787854 idp-engine-0.9.2/idp_engine/Interpret.py
+-rw-r--r--   0        0        0    45046 2022-02-10 15:32:47.791854 idp-engine-0.9.2/idp_engine/Parse.py
+-rw-r--r--   0        0        0    18252 2022-02-07 16:21:06.491629 idp-engine-0.9.2/idp_engine/Propagate.py
+-rw-r--r--   0        0        0     6656 2022-02-07 16:21:06.491629 idp-engine-0.9.2/idp_engine/Relevance.py
+-rw-r--r--   0        0        0     9175 2022-02-07 16:21:06.491629 idp-engine-0.9.2/idp_engine/Run.py
+-rw-r--r--   0        0        0    17338 2022-02-10 15:32:47.791854 idp-engine-0.9.2/idp_engine/Simplify.py
+-rw-r--r--   0        0        0    45531 2022-02-09 11:52:30.589396 idp-engine-0.9.2/idp_engine/Theory.py
+-rw-r--r--   0        0        0      397 2022-02-07 16:21:06.491629 idp-engine-0.9.2/idp_engine/__init__.py
+-rw-r--r--   0        0        0     4287 2022-02-10 15:32:47.791854 idp-engine-0.9.2/idp_engine/utils.py
+-rw-r--r--   0        0        0     1215 2022-02-10 15:56:11.178658 idp-engine-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2123 2022-02-10 16:36:27.556126 idp-engine-0.9.2/setup.py
+-rw-r--r--   0        0        0     2036 2022-02-10 16:36:27.556382 idp-engine-0.9.2/PKG-INFO
```

### Comparing `idp-engine-0.9.1/LICENSE.md` & `idp-engine-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idp-engine-0.9.1/README-pypi.md` & `idp-engine-0.9.2/README-pypi.md`

 * *Files identical despite different names*

### Comparing `idp-engine-0.9.1/idp_engine/Annotate.py` & `idp-engine-0.9.2/idp_engine/Annotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 """
 
 Methods to annotate the Abstract Syntax Tree (AST) of an IDP-Z3 program.
 
 """
 
 from copy import copy
+from itertools import chain
 
-from .Parse import (Vocabulary, Extern, TypeDeclaration, Type, Domain,
+from .Parse import (Vocabulary, Import, TypeDeclaration, Type, Subtype,
                     SymbolDeclaration, Symbol,
                     TheoryBlock, Definition, Rule,
                     Structure, SymbolInterpretation, Enumeration, FunctionEnum,
                     Tuple, ConstructedFrom, Display)
 from .Expression import (Expression, Constructor, AIfExpr, AQuantification, Quantee,
                          ARImplication, AImplication, AEquivalence,
                          Operator, AComparison, AUnary, AAggregate,
@@ -39,18 +40,18 @@
 
 
 # Class Vocabulary  #######################################################
 
 def annotate(self, idp):
     self.idp = idp
 
-    # process extern vocabulary and determine the constructors of CONCEPT
+    # process Import and determine the constructors of CONCEPT
     temp = {}  # contains the new self.declarations
     for s in self.declarations:
-        if isinstance(s, Extern):
+        if isinstance(s, Import):
             other = self.idp.vocabularies[s.name]
             for s1 in other.declarations:
                 if s1.name in temp:
                     s.check(str(temp[s1.name]) == str(s1),
                             f"Inconsistent declaration for {s1.name}")
                 temp[s1.name] = s1
         else:
@@ -110,14 +111,18 @@
     self.check(self.name not in voc.symbol_decls,
                 f"duplicate declaration in vocabulary: {self.name}")
     voc.symbol_decls[self.name] = self
     for s in self.sorts:
         s.annotate(voc, {})
     self.out.annotate(voc, {})
     self.type = self.out.name
+
+    for s in chain(self.sorts, [self.out]):
+        self.check(s.name != CONCEPT or s == s, # use equality to check nested concepts
+                   f"`Concept` must be qualified with a type signature in {self}")
     return self
 SymbolDeclaration.annotate = annotate
 
 
 # Class Symbol  #######################################################
 
 def annotate(self, voc, q_vars):
@@ -125,23 +130,23 @@
         return q_vars[self.name]
     self.decl = voc.symbol_decls[self.name]
     self.type = self.decl.type
     return self
 Symbol.annotate = annotate
 
 
-# Class Domain  #######################################################
+# Class Subtype  #######################################################
 
 def annotate(self, voc, q_vars={}):
     Symbol.annotate(self, voc, q_vars)
-    if self.ins:
+    if self.out:
         self.ins = [s.annotate(voc, q_vars) for s in self.ins]
         self.out = self.out.annotate(voc, q_vars)
     return self
-Domain.annotate = annotate
+Subtype.annotate = annotate
 
 
 # Class TheoryBlock  #######################################################
 
 def annotate(self, idp):
     self.check(self.vocab_name in idp.vocabularies,
                 f"Unknown vocabulary: {self.vocab_name}")
@@ -406,21 +411,21 @@
 # Class Constructor  #######################################################
 
 def annotate(self, voc):
     for a in self.sorts:
         self.check(a.type in voc.symbol_decls,
                    f"Unknown type: {a.type}" )
         a.decl = SymbolDeclaration(annotations='', name=a.accessor,
-                                   sorts=[Domain(name=self.type)],
-                                   out=Domain(name=a.type))
+                                   sorts=[Subtype(name=self.type)],
+                                   out=Subtype(name=a.type))
         a.decl.annotate(voc)
     self.tester = SymbolDeclaration(annotations='',
                                     name=Symbol(name=f"is_{self.name}"),
-                                    sorts=[Domain(name=self.type)],
-                                    out=Domain(name=BOOL))
+                                    sorts=[Subtype(name=self.type)],
+                                    out=Subtype(name=BOOL))
     self.tester.annotate(voc)
 Constructor.annotate = annotate
 
 
 # Class Display  #######################################################
 
 def annotate(self, idp):
@@ -639,16 +644,16 @@
                 if name in voc.symbol_decls:
                     symbol_decl = voc.symbol_decls[name]
                     to_create = False
                 else:
                     symbol_decl = SymbolDeclaration.make(
                         "_"+self.str, # name `_ *`
                         len(q_vars),  # arity
-                        [Domain(name=v.sort.code) for v in q_vars.values()],
-                        Domain(name=self.type)).annotate(voc)    # output_domain
+                        [Subtype(name=v.sort.code) for v in q_vars.values()],
+                        Subtype(name=self.type)).annotate(voc)    # output_domain
                     to_create = True
                 symbol = Symbol(name=symbol_decl.name)
                 applied = AppliedSymbol.make(symbol, q_vars.values())
                 applied = applied.annotate(voc, q_vars)
 
                 if to_create:
                     coc1 = EXISTS(self.quantees,
@@ -712,14 +717,22 @@
 
 def annotate(self, voc, q_vars):
     self.type = self.sort.decl.name if self.sort and self.sort.decl else ''
     return self
 Variable.annotate = annotate
 
 
+# Class Number  #######################################################
+
+def annotate(self, voc, q_vars):
+    self.decl = voc.symbol_decls[self.type]
+    return self
+Number.annotate = annotate
+
+
 # Class UnappliedSymbol  #######################################################
 
 def annotate(self, voc, q_vars):
     if self.name in voc.symbol_decls:
         self.decl = voc.symbol_decls[self.name]
         self.variables = {}
         self.check(type(self.decl) == Constructor,
```

### Comparing `idp-engine-0.9.1/idp_engine/Assignments.py` & `idp-engine-0.9.2/idp_engine/Assignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,18 +225,18 @@
             self[sentence.code] = out
             self.symbols[out.symbol_decl.name] = out.symbol_decl
         return out
 
     def __str__(self) -> str:
         """ Print the assignments in the same format as a model.
 
-        Most symbols are printed as `name := {(val1, ..., val} -> valx, ...}`
+        Most symbols are printed as `name := {(val1, ..., val} -> valx, ...}.`
         with two exceptions:
-            1. Nullary symbols are printed as `name := value`
-            2. Predicates without True atoms are printed as `name := {}`
+            1. Nullary symbols are printed as `name := value.`
+            2. Predicates without True atoms are printed as `name := {}.`
         """
         out = {}
         nullary = set()
         for a in self.values():
             if (a.value is not None and not a.sentence.is_reified()):
                 # If an atom is false, add an empty list to the dict to take
                 # into account exception 2.
@@ -258,11 +258,11 @@
                     # Symbol is a function.
                     c = f"{c}->{str(a.value)}"
                 out[a.symbol_decl.name] = out.get(a.symbol_decl.name, []) + [c]
 
         model_str = ""
         for k, a in out.items():
             if k in nullary:  # Exception 1.
-                model_str += f"{k} := {a[0][2:]}{NEWL}"
+                model_str += f"{k} := {a[0][2:]}.{NEWL}"
             else:
-                model_str += f"{k} := {{{ ', '.join(s for s in a) }}}{NEWL}"
+                model_str += f"{k} := {{{ ', '.join(s for s in a) }}}.{NEWL}"
         return model_str
```

### Comparing `idp-engine-0.9.1/idp_engine/Expression.py` & `idp-engine-0.9.2/idp_engine/Expression.py`

 * *Files 3% similar despite different names*

```diff
@@ -527,38 +527,75 @@
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return str(self)
 
+    def has_element(self, term: Expression) -> Expression:
+        """Returns an expression that says whether `term` is in the type denoted by `self`.
 
-class Domain(Symbol):
+        Args:
+            term (Expression): the argument to be checked
+
+        Returns:
+            Expression: whether `term` is in the type denoted by `self`.
+        """
+        return self.decl.check_bounds(term)
+
+
+class Subtype(Symbol):
     """ASTNode representing `aType` or `Concept[aSignature]`, e.g., `Concept[T*T->Bool]`
 
+    Inherits from Symbol
+
     Args:
         name (Symbol): name of the concept
 
-        ins (List[Symbol], Optional): domain of the signature, e.g., `[T, T]`
+        ins (List[Symbol], Optional): domain of the Concept signature, e.g., `[T, T]`
 
-        out (Symbol, Optional): range of the signature, e.g., `Bool`
+        out (Symbol, Optional): range of the Concept signature, e.g., `Bool`
     """
 
     def __init__(self, **kwargs):
         self.ins = kwargs.pop('ins', None)
         self.out = kwargs.pop('out', None)
         super().__init__(**kwargs)
 
     def __str__(self):
-        return self.name + ("" if not self.ins else
+        return self.name + ("" if not self.out else
                             f"[{'*'.join(str(s) for s in self.ins)}->{self.out}]")
 
+    def __eq__(self, other):
+        self.check(self.name != CONCEPT or self.out,
+                   f"`Concept` must be qualified with a type signature")
+        return (self.name == other.name and
+                (not self.out or (
+                    self.out == other.out and
+                    len(self.ins) == len(other.ins) and
+                    all(s==o for s, o in zip(self.ins, other.ins)))))
+
     def range():
         pass  # monkey-patched
 
+    def has_element(self, term: Expression) -> Expression:
+        """Returns an Expression that says whether `term` is in the type denoted by `self`.
+
+        Args:
+            term (Expression): the argument to be checked
+
+        Returns:
+            Expression: whether `term` `term` is in the type denoted by `self`.
+        """
+        if self.name == CONCEPT:
+            comparisons = [EQUALS([term, c]) for c in self.range()]
+            return OR(comparisons)
+        else:
+            return self.decl.check_bounds(term)
+
 
 class AIfExpr(Expression):
     PRECEDENCE = 10
     IF = 0
     THEN = 1
     ELSE = 2
 
@@ -585,38 +622,38 @@
 
 
 class Quantee(Expression):
     """represents the description of quantification, e.g., `x in T` or `(x,y) in P`
     The `Concept` type may be qualified, e.g. `Concept[Color->Bool]`
 
     Attributes:
-        vars (List[List[Variable]): the (tuples of) variables being quantified
+        vars (List[List[Variable]]): the (tuples of) variables being quantified
 
-        domain (Domain, Optional): a literal Domain to quantify over, e.g., `Color` or `Concept[Color->Bool]`.
+        subtype (Subtype, Optional): a literal Subtype to quantify over, e.g., `Color` or `Concept[Color->Bool]`.
 
         sort (SymbolExpr, Optional): a dereferencing expression, e.g.,. `$(i)`.
 
         sub_exprs (List[SymbolExpr], Optional): the (unqualified) type or predicate to quantify over,
         e.g., `[Color], [Concept] or [$(i)]`.
 
         arity (int): the length of the tuple of variables
 
         decl (SymbolDeclaration, Optional): the (unqualified) Declaration to quantify over, after resolution of `$(i)`.
         e.g., the declaration of `Color`
     """
     def __init__(self, **kwargs):
         self.vars = kwargs.pop('vars')
-        self.domain = kwargs.pop('domain') if 'domain' in kwargs else None
+        self.subtype = kwargs.pop('subtype') if 'subtype' in kwargs else None
         sort = kwargs.pop('sort') if 'sort' in kwargs else None
-        if self.domain:
-            self.check(not (self.domain.name != CONCEPT and 0 <len(self.domain.ins)),
-                   f"Can't use signature after predicate {self.domain.name}")
+        if self.subtype:
+            self.check(self.subtype.name == CONCEPT or self.subtype.out is None,
+                   f"Can't use signature after predicate {self.subtype.name}")
 
         self.sub_exprs = ([sort] if sort else
-                          [self.domain] if self.domain else
+                          [self.subtype] if self.subtype else
                           [])
         self.arity = None
         for i, v in enumerate(self.vars):
             if hasattr(v, 'vars'):  # varTuple
                 self.vars[i] = v.vars
                 self.arity = len(v.vars) if self.arity == None else self.arity
             else:
@@ -640,14 +677,29 @@
         )
         return (f"{','.join(str(v) for vs in self.vars for v in vs)} "
                 f"∈ {self.sub_exprs[0] if self.sub_exprs else None}"
                 f"{signature}")
 
 
 class AQuantification(Expression):
+    """ASTNode representing a quantified formula
+
+    Args:
+        annotations (Dict[str, str]):
+            The set of annotations given by the expert in the IDP-Z3 program.
+
+            ``annotations['reading']`` is the annotation
+            giving the intended meaning of the expression (in English).
+
+        q (str): either '∀' or '∃'
+
+        quantees (List[Quantee]): list of variable declarations
+
+        f (Expression): the formula being quantified
+    """
     PRECEDENCE = 20
 
     def __init__(self, **kwargs):
         self.annotations = kwargs.pop('annotations')
         self.q = kwargs.pop('q')
         self.quantees = kwargs.pop('quantees')
         self.f = kwargs.pop('f')
@@ -1157,15 +1209,15 @@
     """
     PRECEDENCE = 200
 
     def __init__(self, **kwargs):
         self.name = kwargs.pop('name')
         sort = kwargs.pop('sort') if 'sort' in kwargs else None
         self.sort = sort
-        assert sort is None or isinstance(sort, Domain) or isinstance(sort, Symbol)
+        assert sort is None or isinstance(sort, Subtype) or isinstance(sort, Symbol)
 
         super().__init__()
 
         self.type = sort.decl.name if sort and sort.decl else ''
         self.sub_exprs = []
         self.variables = set([self.name])
```

### Comparing `idp-engine-0.9.1/idp_engine/IDP_Z3.py` & `idp-engine-0.9.2/idp_engine/IDP_Z3.py`

 * *Files identical despite different names*

### Comparing `idp-engine-0.9.1/idp_engine/Idp.tx` & `idp-engine-0.9.2/idp_engine/Idp.tx`

 * *Files 4% similar despite different names*

```diff
@@ -10,56 +10,56 @@
 Comment:
   /\/\/.*$/
 ;
 
 Shebang: '#!' /.*$/;
 
 Vocabulary: 'vocabulary' name=ID? '{' (declarations=Declaration)* '}';
-  Declaration: Extern | TypeDeclaration | SymbolDeclaration;
+  Declaration: TypeDeclaration | SymbolDeclaration | Import;
 
-    Extern: 'extern' 'vocabulary' (name=ID);
+    Import: 'import' (name=ID);
 
     TypeDeclaration:
       /type[ \t]/
       name=ID
       (':=' ( enumeration=Ranges
             | enumeration=Enumeration
             | enumeration=ConstructedFrom))?;
 
     SymbolDeclaration: annotations=Annotations symbols+=Symbol[','] ':'
-          ( '(' sorts*=Domain[/[*⨯]/] ')' | sorts*=Domain[/[*⨯]/] )
-          ('->' | '→') out=Domain;
+          ( '(' sorts*=Subtype[/[*⨯]/] ')' | sorts*=Subtype[/[*⨯]/] )
+          ('->' | '→') out=Subtype;
       Symbol: name=/`?[^\d\W]\w*\b|𝔹|ℤ|ℝ|'(\.|[^'])*'/;
 
   Annotations: ('[' annotations*=/[^\]]*/ ']')*;
 
 TheoryBlock: 'theory' (name=ID ':' vocab_name=ID)? '{'
              ( definitions=Definition*
-               constraints=Constraint*
+               constraints=Axiom*
                interpretations=SymbolInterpretation*
              )* '}';
 
   Definition: annotations=Annotations '{' rules*=Rule '}';
   Rule: annotations=Annotations
         (('!'|'∀') quantees+=Quantee[','] ':' )*
         definiendum=AppliedSymbol
         ('=' out=SumMinus)?
         (('<-'|'←') body=Expression)? '.' ;
-      Quantee: ( vars+=Variable[','] ( ('in' | '∈') (domain=Domain | sort=SymbolExpr) )?
-               | vars+=VarTuple[','] ( ('in' | '∈') (domain=Domain | sort=SymbolExpr) )?);
+      Quantee: ( vars+=Variable[','] ( ('in' | '∈') (subtype=Subtype | sort=SymbolExpr) )?
+               | vars+=VarTuple[','] ( ('in' | '∈') (subtype=Subtype | sort=SymbolExpr) )?);
           Variable: name=/`?[^\d\W]\w*\b/;
           VarTuple: '(' vars+=Variable[','] ')';
-          Domain: name=/[^\d\W]\w*\b|𝔹|ℤ|ℝ|'(\.|[^'])*'/
+          Subtype: name=/[^\d\W]\w*\b|𝔹|ℤ|ℝ|'(\.|[^'])*'/
             ( '['
-              ( '(' ins*=Symbol[/[*⨯]/] ')' | ins*=Symbol[/[*⨯]/] )
-              ('->' | '→') out=Symbol
+              ( '(' ins*=Subtype[/[*⨯]/] ')' | ins*=Subtype[/[*⨯]/] )
+              ('->' | '→') out=Subtype
               ']'
             )?;
 
-  Constraint: annotations=Annotations expr=Expression '.';
+  Axiom: annotations=Annotations expr=Expression '.';
 
     Expression:     AQuantification | RImplication;
     RImplication:   ARImplication   | Equivalence;
     Equivalence:    AEquivalence    | Implication;
     Implication:    AImplication    | Disjunction;
     Disjunction:    ADisjunction    | Conjunction;
     Conjunction:    AConjunction    | Comparison;
@@ -119,15 +119,16 @@
            '{' interpretations*=SymbolInterpretation '}';
   SymbolInterpretation: name=UnappliedSymbol ':='
                         ( enumeration=FunctionEnum ('else' default=Identifier)?
                         | enumeration=Ranges
                         | enumeration=Enumeration
                         | enumeration=CSVEnumeration
                         | enumeration=ConstructedFrom
-                        | default=Identifier '.'?);
+                        | default=Identifier
+                        ) '.';
   FunctionEnum: '{' tuples+=FunctionTuple[','] '}';
   FunctionTuple: ( args=Identifier | '(' args*=Identifier[','] ')' )?
                   ('->' | '→') value=Identifier;
   Ranges: '{' elements+=RangeElement[','] '}';
       RangeElement:   (fromI=Number ('..' toI=Number)?)
                     | (fromI=Date   ('..' toI=Date  )?) ;
   Enumeration: '{' tuples*=Tuple[','] '}';
@@ -143,15 +144,15 @@
   Identifier: AppliedSymbol | UnappliedSymbol | Number | Date;
 
 Goal: 'goal' name=ID;
 
 View: 'view' viewType=ViewType;
   ViewType: 'normal' | 'expanded';
 
-Display: 'display' '{' (constraints=Expression '.' | interpretations=SymbolInterpretation '.'?)* '}';
+Display: 'display' '{' (constraints=Expression '.' | interpretations=SymbolInterpretation)* '}';
 
 Procedure: 'procedure' name=ID '(' args=ID*')' '{' pystatements=PyStatement* '}';
 
   PyStatement: PyAssignment | Call1 ;
   PyAssignment: var=ID '=' val=PyExpr;
   PyExpr: !PyAssignment (String | Call1 | Number | PyList);
```

### Comparing `idp-engine-0.9.1/idp_engine/Idp_to_Z3.py` & `idp-engine-0.9.2/idp_engine/Idp_to_Z3.py`

 * *Files identical despite different names*

### Comparing `idp-engine-0.9.1/idp_engine/Interpret.py` & `idp-engine-0.9.2/idp_engine/Interpret.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,52 +15,51 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 
-Methods to interpret a theory in a data structure
+Methods to ground / interpret a theory in a data structure
 
-* substitute a constant by its value in an expression
-* replace symbols interpreted in a structure by their interpretation
 * expand quantifiers
+* replace symbols interpreted in the structure by their interpretation
 
 This module also includes methods to:
 
-* substitute an node by another in an AST tree
+* substitute a node by another in an AST tree
 * instantiate an expresion, i.e. replace a variable by a value
 
 This module monkey-patches the ASTNode class and sub-classes.
 
 ( see docs/zettlr/Substitute.md )
 
 """
 
 import copy
 from itertools import product
 
 from .Assignments import Status as S
-from .Parse import (Extern, TypeDeclaration,
+from .Parse import (Import, TypeDeclaration,
                     SymbolDeclaration, Symbol, SymbolInterpretation,
                     FunctionEnum, Enumeration, Tuple, ConstructedFrom,
                     Definition)
 from .Expression import (AIfExpr, SymbolExpr, Expression, Constructor,
-                    AQuantification, Domain, FORALL, IMPLIES, AND, AAggregate,
+                    AQuantification, Subtype, FORALL, IMPLIES, AND, AAggregate,
                     NOT, AppliedSymbol, UnappliedSymbol,
                     Variable, TRUE, Number)
 from .utils import (BOOL, RESERVED_SYMBOLS, CONCEPT, OrderedSet, DEFAULT,
                     GOAL_SYMBOL, EXPAND)
 
 
-# class Extern  ###########################################################
+# class Import  ###########################################################
 
 def interpret(self, problem):
     pass
-Extern.interpret = interpret
+Import.interpret = interpret
 
 
 # class TypeDeclaration  ###########################################################
 
 def interpret(self, problem):
     if self.name in problem.interpretations:
         problem.interpretations[self.name].interpret(problem)
@@ -74,15 +73,15 @@
 
 TypeDeclaration.interpret = interpret
 
 
 # class SymbolDeclaration  ###########################################################
 
 def interpret(self, problem):
-    assert all(isinstance(s, Domain) for s in self.sorts), 'internal error'
+    assert all(isinstance(s, Subtype) for s in self.sorts), 'internal error'
     self.in_domain = list(product(*[s.range() for s in self.sorts]))
     self.range = self.out.range()
 
     # create instances
     if self.name not in RESERVED_SYMBOLS:
         self.instances = {}
         for arg in self.in_domain:
@@ -146,18 +145,31 @@
     status = S.DEFAULT if self.block.name == DEFAULT else S.STRUCTURE
     if self.is_type_enumeration:
         self.enumeration.interpret(problem)
         self.symbol.decl.interpretation = self
     elif not self.name in [GOAL_SYMBOL, EXPAND]:
         # update problem.assignments with data from enumeration
         for t in self.enumeration.tuples:
+
             if type(self.enumeration) == FunctionEnum:
                 args, value = t.args[:-1], t.args[-1]
+                self.check(self.symbol.decl.has_in_range(value).same_as(TRUE),
+                           f"{value} is not in the range of {self.symbol.name}")
             else:
                 args, value = t.args, TRUE
+
+            # check that the arguments are in the domain
+            a = (str(args) if 1<len(args) else
+                    str(args[0]) if len(args)==1 else
+                    "()")
+            self.check(len(self.symbol.decl.sorts) == len(args),
+                f"Incorrect arity of {a} for {self.name}")
+            self.check(self.symbol.decl.has_in_domain(args).same_as(TRUE),
+                        f"{a} is not in the domain of {self.symbol.name}")
+
             expr = AppliedSymbol.make(self.symbol, args)
             self.check(expr.code not in problem.assignments
                 or problem.assignments[expr.code].status == S.UNKNOWN,
                 f"Duplicate entry in structure for '{self.name}': {str(expr)}")
             e = problem.assignments.assert__(expr, value, status)
             if (status == S.DEFAULT  # for proper display in IC
                 and type(self.enumeration) == FunctionEnum):
@@ -279,14 +291,16 @@
     # instantiate expressions, with simplification
     out = self.update_exprs(e.instantiate(e0, e1, problem)
                             for e in self.sub_exprs)
 
     if out.value is not None:  # replace by new value
         out = out.value
     else:
+        self.check(len(e0) == len(e1),
+                   f"Incorrect arity: {e0}, {e1}")
         for o, n in zip(e0, e1):
             if o.name in out.variables:
                 out.variables.discard(o.name)
                 if type(n) == Variable:
                     out.variables.add(n.name)
             out.code = str(out)
     out.annotations['reading'] = out.code
@@ -297,28 +311,29 @@
 # class Symbol ###########################################################
 
 def instantiate(self, e0, e1, problem=None):
     return self
 Symbol.instantiate = instantiate
 
 
-# class Domain ###########################################################
+# class Subtype ###########################################################
 
 def range(self):
     range = [t for t in self.decl.range]
-    if self.ins:  # x in Concept[T->T]
+    if self.out:  # x in Concept[T->T]
         range = [v for v in range
                  if v.decl.symbol.decl.arity == len(self.ins)
                  and isinstance(v.decl.symbol.decl, SymbolDeclaration)
                  and v.decl.symbol.decl.out.name == self.out.name
-                 and all(s.name == q.name
+                 and len(v.decl.symbol.decl.sorts) == len(self.ins)
+                 and all(s == q
                          for s, q in zip(v.decl.symbol.decl.sorts,
                                          self.ins))]
     return range
-Domain.range = range
+Subtype.range = range
 
 
 # Class AQuantification  ######################################################
 
 def interpret(self, problem):
     """apply information in the problem and its vocabulary
 
@@ -357,15 +372,15 @@
             if domain.code in problem.interpretations:
                 enumeration = problem.interpretations[domain.code].enumeration
                 range = [t.args for t in enumeration.tuples.values()]
                 guard = None
             elif type(domain.decl) == SymbolDeclaration:
                 range = domain.decl.in_domain
                 guard = domain
-            elif isinstance(domain, Domain):
+            elif isinstance(domain, Subtype):
                 range = [[t] for t in domain.range()]
                 guard = None
             else:  # SymbolExpr (e.g. $(`Color))
                 range = [[t] for t in domain.decl.range] #TODO1 decl.enumeration.tuples
                 guard = None
 
 
@@ -457,17 +472,15 @@
             if interpretation.block.name != DEFAULT:
                 f = interpretation.interpret_application
                 value = f(problem, 0, self, sub_exprs)
         if (not self.in_head and not self.variables):
             inst = [defin.instantiate_definition(self.decl, sub_exprs, problem)
                               for defin in problem.definitions]
             inst = [x for x in inst if x]
-            if len(inst) == 1:
-                co_constraint = inst[0]
-            elif len(inst) > 1:
+            if inst:
                 co_constraint = AND(inst)
         out = (value if value else
                self._change(sub_exprs=sub_exprs, simpler=simpler,
                         co_constraint=co_constraint))
         return out
     else:
         return self
@@ -533,14 +546,16 @@
         self.sort = self.sort.substitute(e0,e1, assignments, tag)
     return e1 if self.code == e0.code else self
 Variable.substitute = substitute
 
 def instantiate1(self, e0, e1, problem=None):
     if self.sort:
         self.sort = self.sort.instantiate(e0, e1, problem)
+    self.check(len(e0) == len(e1),
+               f"Incorrect arity: {e0}, {e1}")
     for o, n in zip(e0, e1):
         if self.code == o.code:
             return n
     return self
 Variable.instantiate1 = instantiate1
```

### Comparing `idp-engine-0.9.1/idp_engine/Parse.py` & `idp-engine-0.9.2/idp_engine/Parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 
 Classes to parse an IDP-Z3 theory.
 
 """
-__all__ = ["IDP", "Vocabulary", "Annotations", "Extern",
+__all__ = ["IDP", "Vocabulary", "Annotations", "Import",
            "TypeDeclaration",
            "SymbolDeclaration", "Symbol", "TheoryBlock", "Definition",
            "Rule", "Structure", "Enumeration", "Tuple",
            "Display", "Procedure", ]
 
 from copy import copy
 from datetime import date
@@ -35,23 +35,23 @@
 from sys import intern
 from textx import metamodel_from_file
 from typing import Dict, List, Union, Optional
 
 
 from .Assignments import Assignments
 from .Expression import (Annotations, ASTNode, Constructor, Accessor, Symbol, SymbolExpr,
-                         AIfExpr, AQuantification, Domain, Quantee,
+                         Expression, AIfExpr, AQuantification, Subtype, Quantee,
                          ARImplication, AEquivalence,
                          AImplication, ADisjunction, AConjunction,
                          AComparison, ASumMinus, AMultDiv, APower, AUnary,
                          AAggregate, AppliedSymbol, UnappliedSymbol,
                          Number, Brackets, Date,
-                         Variable, TRUEC, FALSEC, TRUE, FALSE, EQUALS, OR, EQUIV)
+                         Variable, TRUEC, FALSEC, TRUE, FALSE, EQUALS, AND, OR, EQUIV)
 from .utils import (RESERVED_SYMBOLS, OrderedSet, NEWL, BOOL, INT, REAL, DATE, CONCEPT,
-                    GOAL_SYMBOL, EXPAND, RELEVANT, ABS, ARITY, INPUT_DOMAIN, OUTPUT_DOMAIN, IDPZ3Error,
+                    GOAL_SYMBOL, EXPAND, RELEVANT, ABS, IDPZ3Error,
                     CO_CONSTR_RECURSION_DEPTH, MAX_QUANTIFIER_EXPANSION)
 
 
 def str_to_IDP(atom, val_string):
     """cast a string value for 'atom into an Expr object, or None
 
     used to convert Z3 models or json data from GUI
@@ -258,29 +258,24 @@
             TypeDeclaration(name=INT, enumeration=IntRange()),
             TypeDeclaration(name=REAL, enumeration=RealRange()),
             TypeDeclaration(name=DATE, enumeration=DateRange()),
             TypeDeclaration(
                 name=CONCEPT,
                 constructors=[]),
             SymbolDeclaration(annotations='', name=Symbol(name=GOAL_SYMBOL),
-                                sorts=[Domain(name=CONCEPT)], out=Domain(name=BOOL)),
+                              sorts=[Subtype(name=CONCEPT, ins=[],
+                                             out=Subtype(name=BOOL))],
+                              out=Subtype(name=BOOL)),
             SymbolDeclaration(annotations='', name=Symbol(name=RELEVANT),
-                                sorts=[Domain(name=CONCEPT)], out=Domain(name=BOOL)),
-            SymbolDeclaration(annotations='', name=Symbol(name=ARITY),
-                                sorts=[Domain(name=CONCEPT)],
-                                out=Domain(name=INT)),
+                              sorts=[Subtype(name=CONCEPT, ins=[],
+                                             out=Subtype(name=BOOL))],
+                              out=Subtype(name=BOOL)),
             SymbolDeclaration(annotations='', name=Symbol(name=ABS),
-                                sorts=[Domain(name=INT)],
-                                out=Domain(name=INT)),
-            SymbolDeclaration(annotations='', name=Symbol(name=INPUT_DOMAIN),
-                                sorts=[Domain(name=CONCEPT), Domain(name=INT)],
-                                out=Domain(name=CONCEPT)),
-            SymbolDeclaration(annotations='', name=Symbol(name=OUTPUT_DOMAIN),
-                                sorts=[Domain(name=CONCEPT)],
-                                out=Domain(name=CONCEPT))
+                                sorts=[Subtype(name=INT)],
+                                out=Subtype(name=INT)),
             ] + self.declarations
 
     def __str__(self):
         return (f"vocabulary {{{NEWL}"
                 f"{NEWL.join(str(i) for i in self.declarations)}"
                 f"{NEWL}}}{NEWL}")
 
@@ -300,20 +295,20 @@
                 and self.name != BOOL):
                 block.check(s.name not in block.interpretations,
                             f"Duplicate enumeration of {self.name} "
                             f"in vocabulary and block {block.name}")
                 block.interpretations[s.name] = s.interpretation
 
 
-class Extern(ASTNode):
+class Import(ASTNode):
     def __init__(self, **kwargs):
         self.name = kwargs.pop('name')
 
     def __str__(self):
-        return f"extern vocabulary {self.name}"
+        return f"Import {self.name}"
 
 
 class TypeDeclaration(ASTNode):
     """AST node to represent `type <symbol> := <enumeration>`
 
     Args:
         name (string): name of the type
@@ -388,17 +383,17 @@
 
         symbols ([Symbol]): the symbols being defined, before expansion
 
         name (string): the identifier of the symbol, after expansion of the node
 
         arity (int): the number of arguments
 
-        sorts (List[Symbol]): the types of the arguments
+        sorts (List[Subtype]): the types of the arguments
 
-        out (Symbol): the type of the symbol
+        out (Subtype): the type of the symbol
 
         type (string): name of the Z3 type of an instance of the symbol
 
         in_domain (List): the list of possible tuples of arguments
 
         instances (Dict[string, Expression]):
             a mapping from the code of a symbol applied to a tuple of
@@ -444,14 +439,19 @@
         self.type = None  # a string
         self.in_domain = None  # all possible arguments
         self.range = None  # all possible values
         self.instances = None  # {string: AppliedSymbol} not starting with '_'
         self.block: Optional[Block] = None  # vocabulary where it is declared
         self.view = ViewType.NORMAL  # "hidden" | "normal" | "expanded" whether the symbol box should show atoms that contain that symbol, by default
 
+    @classmethod
+    def make(cls, strname, arity, sorts, out):
+        o = cls(strname=strname, arity=arity, sorts=sorts, out=out, annotations={})
+        return o
+
     def __str__(self):
         if self.name in RESERVED_SYMBOLS:
             return ''
         args = '⨯'.join(map(str, self.sorts)) if 0 < len(self.sorts) else ''
         return (f"{self.name}: "
                 f"{ '('+args+')' if args else '()'}"
                 f" -> {self.out.name}")
@@ -459,19 +459,33 @@
     def __repr__(self):
         return str(self)
 
     def is_subset_of(self, other):
         return (self.arity == 1 and self.type == BOOL
                 and self.sorts[0].decl == other)
 
-    @classmethod
-    def make(cls, strname, arity, sorts, out):
-        o = cls(strname=strname, arity=arity, sorts=sorts, out=out, annotations={})
-        return o
+    def has_in_domain(self, args: List[Expression]) -> Expression:
+        """Returns an expression that says whether the `args` are in the domain of the symbol.
+
+        Arguments:
+            args (List[Expression]): the list of arguments to be checked, e.g. `[1, 2]`
+
+        Returns:
+            Expression: whether `(1,2)` is in the domain of the symbol
+        """
+        assert len(self.sorts) == len(args), \
+            f"Incorrect arity of {str(args)} for {self.name}"
+        return AND([typ.has_element(term)
+                   for typ, term in zip(self.sorts, args)])
+
 
+    def has_in_range(self, value: Expression) -> Expression:
+        """Returns an expression that says whether `value` is in the range of the symbol.
+        """
+        return self.out.has_element(value)
 
 Type = Union[TypeDeclaration, SymbolDeclaration]
 
 
 ################################ TheoryBlock  ###############################
 
 
@@ -609,15 +623,15 @@
         symbs = {s for (s, ss) in dependencies if s == ss}
         for r in self.rules:
             key = r.definiendum.symbol.decl
             if key not in symbs or key in self.level_symbols:
                 continue
             symbdec = SymbolDeclaration.make(
                 "_"+str(self.id)+"lvl_"+key.name,
-                key.arity, key.sorts, Domain(name=REAL))
+                key.arity, key.sorts, Subtype(name=REAL))
             self.level_symbols[key] = Symbol(name=symbdec.name)
             self.level_symbols[key].decl = symbdec
 
         for decl in self.level_symbols.keys():
             self.check(decl.out.name == BOOL,
                        f"Inductively defined functions are not supported yet: "
                        f"{decl.name}.")
@@ -709,15 +723,15 @@
 
     def __str__(self):
         return self.name
 
 
 class SymbolInterpretation(ASTNode):
     """
-    AST node representing `<symbol> := { <identifiers*> } else <default>`
+    AST node representing `<symbol> := { <identifiers*> } else <default>.`
 
     Attributes:
         name (string): name of the symbol being enumerated.
 
         symbol (Symbol): symbol being enumerated
 
         enumeration ([Enumeration]): enumeration.
@@ -854,14 +868,22 @@
         self.constructors = kwargs.pop('constructors')
         self.tuples = None
         self.accessors = dict()
 
     def contains(self, args, function, arity=None, rank=0, tuples=None):
         """returns True if args belong to the type enumeration"""
         # args must satisfy the tester of one of the constructors
+        assert len(args) == 1, f"Incorrect arity in {self.parent.name}{args}"
+        if type(args[0].decl) == Constructor:  # try to simplify it
+            self.check(self.parent.name == args[0].decl.type,
+                       f"Incorrect type of {args[0]} for {self.parent.name}")
+            self.check(len(args[0].sub_exprs) == len(args[0].decl.sorts),
+                       f"Incorrect arity")
+            return AND([t.decl.out.has_element(e)
+                        for e,t in zip(args[0].sub_exprs, args[0].decl.sorts)])
         out = [AppliedSymbol.construct(constructor.tester, args)
                 for constructor in self.constructors]
         return OR(out)
 
 class Tuple(ASTNode):
     def __init__(self, **kwargs):
         self.args = kwargs.pop('args')
@@ -920,15 +942,15 @@
                 else:
                     self.check(False, f"Incorrect value {x.toI} for {self.type}")
         Enumeration.__init__(self, tuples=tuples)
 
     def contains(self, args, function, arity=None, rank=0, tuples=None):
         var = args[0]
         if not self.elements:
-            return None
+            return TRUE
         if self.tuples and len(self.tuples) < MAX_QUANTIFIER_EXPANSION:
             es = [EQUALS([var, c.args[0]]) for c in self.tuples]
             e = OR(es)
             return e
         sub_exprs = []
         for x in self.elements:
             if x.toI is None:
@@ -1106,16 +1128,16 @@
 Block = Union[Vocabulary, TheoryBlock, Structure, Display]
 
 dslFile = path.join(path.dirname(__file__), 'Idp.tx')
 
 idpparser = metamodel_from_file(dslFile, memoization=True,
                                 classes=[IDP, Annotations,
 
-                                         Vocabulary, Extern,
-                                         TypeDeclaration, Accessor, Domain,
+                                         Vocabulary, Import,
+                                         TypeDeclaration, Accessor, Subtype,
                                          SymbolDeclaration, Symbol,
                                          SymbolExpr,
 
                                          TheoryBlock, Definition, Rule, AIfExpr,
                                          AQuantification, Quantee, ARImplication,
                                          AEquivalence, AImplication,
                                          ADisjunction, AConjunction,
```

### Comparing `idp-engine-0.9.1/idp_engine/Problem.py` & `idp-engine-0.9.2/idp_engine/Theory.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
         declarations (Dict[str, Type]): the list of type and symbol declarations
 
         constraints (OrderedSet): a set of assertions.
 
         definitions ([Definition]): a list of definitions in this problem
 
+        interpretations (Dict[string, SymbolInterpretation]):
+            A mapping of enumerated symbols to their interpretation.
+
         def_constraints (Dict[SymbolDeclaration, Definition], list[Expression]):
             A mapping of defined symbol to the whole-domain constraints
             equivalent to its definition.
 
-        interpretations (Dict[string, SymbolInterpretation]):
-            A mapping of enumerated symbols to their interpretation.
-
         _constraintz (List(ExprRef), Optional): a list of assertions, co_constraints and definitions in Z3 form
 
         _symbols (Set[str]): set of symbol name occurring in self._constraintz
 
         _formula (ExprRef, optional): the Z3 formula that represents
             the problem (assertions, co_constraints, definitions and assignments).
 
@@ -343,15 +343,15 @@
             val = str_to_IDP(atom, str(value))
             self.assignments.assert__(atom, val, status)
         self._formula = None
 
     def enable_law(self, code: str) -> "Theory":
         """Enables a law, represented as a code string taken from the output of explain(...).
 
-        The law should not result from a structure (e.g., from ``p:=true``)
+        The law should not result from a structure (e.g., from ``p:=true.``)
         or from a types (e.g., from ``T:={1..10}`` and ``c: () -> T``).
 
         Args:
             code (str): the code of the law to be enabled
 
         Raises:
             AssertionError: if code is unknown
@@ -361,15 +361,15 @@
                    for _, e in self.expl_reifs.values()), \
                 f"Cannot enable an unknown law: {code}"
         self.ignored_laws.remove(code)
 
     def disable_law(self, code: str) -> "Theory":
         """Disables a law, represented as a code string taken from the output of explain(...).
 
-        The law should not result from a structure (e.g., from ``p:=true``)
+        The law should not result from a structure (e.g., from ``p:=true.``)
         or from a types (e.g., from ``T:={1..10}`` and ``c: () -> T``).
 
         Args:
             code (str): the code of the law to be disabled
 
         Raises:
             AssertionError: if code is unknown
@@ -578,14 +578,16 @@
             if different:
                 solver.add(Or(different))
 
             if solver.check() == sat:
                 count += 1
                 ass = self._from_model(solver, todo, complete)
                 yield ass
+                if not todo:  # empty theory
+                    break
             else:
                 break
 
         solver.pop()
 
         maxed = (0 < max <= count)
         timeouted = (0 < timeout <= time.process_time()-start)
```

### Comparing `idp-engine-0.9.1/idp_engine/Propagate.py` & `idp-engine-0.9.2/idp_engine/Propagate.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from z3 import (Solver, sat, unsat, unknown, Not, Or, is_false, is_true, is_not, is_eq)
 
 from .Assignments import Status as S, Assignments
 from .Expression import (Expression, AQuantification,
                     ADisjunction, AConjunction, AppliedSymbol,
                     AComparison, AUnary, Brackets, TRUE, FALSE)
 from .Parse import str_to_IDP
-from .Problem import Theory
+from .Theory import Theory
 from .utils import OrderedSet, IDPZ3Error, NOT_SATISFIABLE
 
 start = time.process_time()
 
 ###############################################################################
 #
 #  Symbolic propagation
```

### Comparing `idp-engine-0.9.1/idp_engine/Relevance.py` & `idp-engine-0.9.2/idp_engine/Relevance.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 This module contains the logic for the computation of relevance.
 """
 
 from idp_engine.Assignments import Status as S
 from idp_engine.Expression import (AppliedSymbol, TRUE, Expression, AQuantification,
                                    AConjunction, Brackets, UnappliedSymbol)
-from idp_engine.Problem import Theory
+from idp_engine.Theory import Theory
 from idp_engine.utils import OrderedSet, GOAL_SYMBOL, RELEVANT
 
 
 def split_constraints(constraints: OrderedSet) -> OrderedSet:
     """replace [.., a ∧ b, ..] by [.., a, b, ..]
 
     This is to avoid dependencies between a and b (see issue #95).
@@ -72,15 +72,15 @@
     the resulting M' structure is still a model.
     Relevant questions are those that are not irrelevant.
 
     Call must be made after a propagation, on a Theory created with ``extended=True``.
     The result is found in the ``relevant`` attribute of the assignments in ``self.assignments``.
 
     If ``goal_symbol`` has an enumeration in the theory
-    (e.g., ``goal_symbol := {`tax_amount}``),
+    (e.g., ``goal_symbol := {`tax_amount}.``),
     relevance is computed relative to those goals.
 
     Definitions in the theory are ignored,
     unless they influence axioms in the theory or goals in ``goal_symbol``.
 
     Returns:
         Theory: the Theory with relevant information in ``self.assignments``.
```

### Comparing `idp-engine-0.9.1/idp_engine/Run.py` & `idp-engine-0.9.2/idp_engine/Run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 import time
 import types
 from typing import Any, Iterator, List, Union
 from z3 import Solver
 
 from .Parse import IDP, TheoryBlock, Structure
-from .Problem import Theory
+from .Theory import Theory
 from .Assignments import Status as S, Assignments
 from .utils import NEWL
 
 last_call = time.process_time()  # define it as global
 
 def model_check(*theories: Union[TheoryBlock, Structure, Theory]) -> str:
     """Returns a string stating whether the combination of theories is satisfiable.
@@ -175,15 +175,15 @@
     The questions are preceded with `` ? `` when their answer is unknown.
 
     When an *irrelevant* value is changed in a model M of the theories,
     the resulting M' structure is still a model.
     Relevant questions are those that are not irrelevant.
 
     If ``goal_symbol`` has an enumeration in the theory
-    (e.g., ``goal_symbol := {`tax_amount}``),
+    (e.g., ``goal_symbol := {`tax_amount}.``),
     relevance is computed relative to those goals.
 
     Definitions in the theory are ignored,
     unless they influence axioms in the theory or goals in ``goal_symbol``.
 
     Yields:
         relevant questions
```

### Comparing `idp-engine-0.9.1/idp_engine/Simplify.py` & `idp-engine-0.9.2/idp_engine/Simplify.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
 """
 
 import sys
 from typing import List
 
 from .Expression import (
-    Constructor, Expression, AIfExpr, AQuantification, Quantee, Domain,
+    Constructor, Expression, AIfExpr, AQuantification, Quantee, Subtype,
     Operator, AEquivalence, AImplication, ADisjunction,
     AConjunction, AComparison, ASumMinus, AMultDiv, APower,
     AUnary, AAggregate, SymbolExpr, AppliedSymbol, UnappliedSymbol, Variable,
     Number, Date, Brackets, TRUE, FALSE, NOT, AND, OR)
 from .Parse import Symbol, Enumeration, Tuple, TypeDeclaration
 from .Assignments import Status as S, Assignment
-from .utils import BOOL, INT, CONCEPT, ABS, ARITY, INPUT_DOMAIN, OUTPUT_DOMAIN, RESERVED_SYMBOLS
+from .utils import BOOL, INT, CONCEPT, ABS, RESERVED_SYMBOLS
 
 
 # class Expression  ###########################################################
 
 def _change(self, sub_exprs=None, ops=None, value=None, simpler=None,
             co_constraint=None):
     " change attributes of an expression, and resets derived attributes "
@@ -55,15 +55,15 @@
     elif simpler is not None:
         if simpler.value is not None:  # example: prime.idp
             self.value = simpler.value
         else:
             self.simpler = simpler
     assert (self.value is None
                or type(self.value) in [AppliedSymbol, UnappliedSymbol, Symbol,
-                                       Number, Date, Domain]), \
+                                       Number, Date, Subtype]), \
             f"Incorrect value in _change: {self.value}"
 
     # reset derived attributes
     self.str = sys.intern(str(self))
 
     return self
 Expression._change = _change
@@ -252,15 +252,16 @@
     operands = list(operands)
     operands1 = [e.value for e in operands]
     if all(e is not None for e in operands1):
         self.check(all(hasattr(e, 'py_value') for e in operands1),
                 f"Incorrect numeric type in {self}")
         out = operands1[0].py_value
 
-        for e, op in zip(operands1[1:], self.operator):
+        assert len(self.operator) == len(operands1[1:]), "Internal error"
+        for op, e in zip(self.operator, operands1[1:]):
             function = Operator.MAP[op]
 
             if op == '/' and self.type == INT:  # integer division
                 out //= e.py_value
             else:
                 out = function(out, e.py_value)
         value = Number(number=str(out))
@@ -372,50 +373,14 @@
         and self.decl):
         if self.decl.name in new_exprs[0].decl.parent.accessors:
             i = new_exprs[0].decl.parent.accessors[self.decl.name]
             return self._change(simpler=new_exprs[0].sub_exprs[i], sub_exprs=new_exprs)
         if self.decl.name == new_exprs[0].decl.tester.name:
             return self._change(value=TRUE, sub_exprs=new_exprs)
 
-    # simplify arity(s), input_domain(s,0), output_domain(s)
-    if (self.decl and new_exprs
-        and type(new_exprs[0]) == UnappliedSymbol and new_exprs[0].decl):
-        if self.decl.name == ARITY:
-            self.check(len(new_exprs) == 1,
-                    f"Incorrect number of arguments for '{ARITY}': {len(new_exprs)}")
-            self.check(new_exprs[0].decl.type == CONCEPT,
-                    f"Argument of '{ARITY}' must be a Concept: {new_exprs[0]}")
-            value = Number(number=str(new_exprs[0].decl.symbol.decl.arity))
-            return self._change(value=value, sub_exprs=new_exprs)
-        elif self.decl.name == INPUT_DOMAIN:
-            self.check(len(new_exprs) == 2,
-                    f"Incorrect number of arguments for '{INPUT_DOMAIN}': {len(new_exprs)}")
-            self.check(new_exprs[0].decl.type == CONCEPT
-                       or (new_exprs[0].decl.sort.decl.arity == 1
-                           and new_exprs[0].decl.sort.decl.type == BOOL),
-                    f"First argument of '{INPUT_DOMAIN}' must be a Concept: {new_exprs[0]}")
-            self.check(new_exprs[1].type == INT,
-                    f"Second argument of '{INPUT_DOMAIN}' must be a Int: {new_exprs[1]}")
-            if isinstance(new_exprs[1], Number):
-                # find the Concept for the input domain
-                symbol_string = f"`{new_exprs[0].decl.symbol.decl.sorts[new_exprs[1].py_value - 1]}"
-                value = self.decl.out.decl.map[symbol_string]
-                return self._change(value=value, sub_exprs=new_exprs)
-        elif self.decl.name == OUTPUT_DOMAIN:
-            self.check(len(new_exprs) == 1,
-                    f"Incorrect number of arguments for '{OUTPUT_DOMAIN}': {len(new_exprs)}")
-            self.check(new_exprs[0].decl.type == CONCEPT,
-                    f"Argument of '{OUTPUT_DOMAIN}' must be a Concept: {new_exprs[0]}")
-            # find the Concept for the output domain of the argument
-            symbol_string = f"`{new_exprs[0].decl.symbol.decl.out}"
-            value = self.decl.out.decl.map[symbol_string]
-            return self._change(value=value, sub_exprs=new_exprs)
-        elif type(self.decl) == TypeDeclaration:  # type
-            value = TRUE if self.sub_exprs[0] in self.decl.range else FALSE
-            return self._change(value=value)
     return self._change(sub_exprs=new_exprs)
 AppliedSymbol.update_exprs = update_exprs
 
 def as_set_condition(self):
     # determine core after substitutions
     core = AppliedSymbol.make(self.symbol, self.sub_exprs).copy()
```

### Comparing `idp-engine-0.9.1/idp_engine/utils.py` & `idp-engine-0.9.2/idp_engine/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,19 +56,16 @@
 DATE = "Date"
 CONCEPT = "Concept"
 
 GOAL_SYMBOL = "goal_symbol"
 RELEVANT = " relevant"  # internal.  Leading space to avoid conflict with user vocabulary
 EXPAND = "expand"
 ABS = "abs"
-ARITY = "arity"
-INPUT_DOMAIN = "input_domain"
-OUTPUT_DOMAIN = "output_domain"
 RESERVED_SYMBOLS = [BOOL, INT, REAL, DATE, CONCEPT,
-                    GOAL_SYMBOL, RELEVANT, ABS, ARITY, INPUT_DOMAIN, OUTPUT_DOMAIN]
+                    GOAL_SYMBOL, RELEVANT, ABS, ]
 
 DEFAULT = "default"
 
 NOT_SATISFIABLE ="Not satisfiable."
 
 """ Module that monkey-patches json module when it's imported so
 JSONEncoder.default() automatically checks for a special "to_json()"
@@ -98,46 +95,14 @@
 
 def unquote(s):
     if s[0] == "'" and s[-1] == "'":
         return s[1:-1]
     return s
 
 
-def in_list(q, ls):
-    if not ls:
-        return True  # e.g. for INT, REAL, DATE
-    if len(ls) == 1:
-        return q == ls[0]
-    return Or([q == i for i in ls])
-
-
-def is_number(s):
-    if str(s) in ['True', 'False']:
-        return False
-    try:
-        float(eval(str(s if not s.endswith('?') else s[:-1]))) # accepts "2/3" or "3.1415?"
-        return True
-    except:
-        return False
-
-
-def splitLast(l):
-    return l[:-1], l[-1]
-
-
-def applyTo(sym, arg):
-    if len(arg) == 0:
-        return sym
-    return sym(arg)
-
-
-def mergeDicts(l):
-    # merge a list of dicts (possibly a comprehension
-    return dict(ChainMap(*reversed(list(l))))
-
 # OrderedSet  #############################################
 
 
 class OrderedSet(dict):
     """
     a list of expressions without duplicates (first-in is selected)
     """
```

### Comparing `idp-engine-0.9.1/pyproject.toml` & `idp-engine-0.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idp-engine"
-version = "0.9.1"
+version = "0.9.2"
 description = "IDP-Z3 is a reasoning engine for knowledge represented using the FO(.) (aka FO-dot) language."
 authors = ["pierre.carbonnelle <pierre.carbonnelle@cs.kuleuven.be>"]
 license = "GNU LGPL 3"
 readme = "README-pypi.md"
 homepage = "https://www.idp-z3.be"
 repository = "https://gitlab.com/krr/IDP-Z3"
 documentation = "https://docs.idp-z3.be"
@@ -35,11 +35,12 @@
 sphinxcontrib-youtube = "^1.0.1"
 sphinx-bootstrap-theme = "^0.8.0"
 sphinx-rtd-theme="^0.5.0"
 recommonmark="^0.6.0"
 Cython = "^0.29.21"
 coverage = "^6.1.1"
 pytest-cov = "^3.0.0"
+myst-parser = "^0.16.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `idp-engine-0.9.1/setup.py` & `idp-engine-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Click>=7.0,<8.0', 'textX>=2.1.0,<3.0.0', 'z3-solver==4.8.12.0']
 
 entry_points = \
 {'console_scripts': ['idp-engine = idp_engine.IDP_Z3:cli']}
 
 setup_kwargs = {
     'name': 'idp-engine',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'IDP-Z3 is a reasoning engine for knowledge represented using the FO(.) (aka FO-dot) language.',
     'long_description': 'idp-engine is a reasoning engine for knowledge represented using the FO(.) language.\nFO(.) (aka FO-dot) is First Order logic, with various extensions to make it more expressive:  types, equality, arithmetic, inductive definitions, aggregates, and intensional objects.\nThe idp-engine uses the Z3 SMT solver as a back-end.\n\nIt is developed by the Knowledge Representation group at KU Leuven in Leuven, Belgium, and made available under the [GNU LGPL v3 License](https://www.gnu.org/licenses/lgpl-3.0.txt).\n\nSee more information at [www.IDP-Z3.be](https://www.IDP-Z3.be).\n\n\n# Installation\n\n``idp_engine`` can be installed from [pypi.org](https://pypi.org/), e.g. using [pip](https://pip.pypa.io/en/stable/user_guide/):\n\n```\n   pip install idp_engine\n```\n\n# Get started\n\nThe following code illustrates how to run inferences on a knowledge base.\n\n```\n    from idp_engine import IDP, model_expand\n    kb = IDP.parse("path/to/file.idp")\n    T, S = kb.get_blocks("T, S")\n    for model in model_expand(T,S):\n        print(model)\n```\n\nFor more information, please read [the documentation](http://docs.idp-z3.be/en/latest/).\n\n# Contribute\n\nContributions are welcome!  The repository is [on GitLab](https://gitlab.com/krr/IDP-Z3).',
     'author': 'pierre.carbonnelle',
     'author_email': 'pierre.carbonnelle@cs.kuleuven.be',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.idp-z3.be',
```

### Comparing `idp-engine-0.9.1/PKG-INFO` & `idp-engine-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idp-engine
-Version: 0.9.1
+Version: 0.9.2
 Summary: IDP-Z3 is a reasoning engine for knowledge represented using the FO(.) (aka FO-dot) language.
 Home-page: https://www.idp-z3.be
 License: GNU LGPL 3
 Author: pierre.carbonnelle
 Author-email: pierre.carbonnelle@cs.kuleuven.be
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

