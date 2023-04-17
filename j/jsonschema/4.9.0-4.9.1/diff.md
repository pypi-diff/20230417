# Comparing `tmp/jsonschema-4.9.0.tar.gz` & `tmp/jsonschema-4.9.1.tar.gz`

## Comparing `jsonschema-4.9.0.tar` & `jsonschema-4.9.1.tar`

### file list

```diff
@@ -1,518 +1,518 @@
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.coveragerc
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.flake8
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.readthedocs.yml
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 jsonschema-4.9.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 jsonschema-4.9.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jsonschema-4.9.0/codecov.yml
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 jsonschema-4.9.0/tox.ini
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.github/SECURITY.md
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/Makefile
--rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/conf.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/creating.rst
--rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/errors.rst
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/faq.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/index.rst
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/jsonschema_role.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/make.bat
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/references.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/requirements.in
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/requirements.txt
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jsonschema-4.9.0/docs/validate.rst
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/LICENSE
--rw-r--r--   0        0        0    15718 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/README.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/package.json
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/test-schema.json
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tox.ini
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/.github/CODEOWNERS
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/.github/workflows/ci.yml
--rwxr-xr-x   0        0        0     8492 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/bin/jsonschema_suite
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/extendible-dynamic-ref.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/integer.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/locationIndependentIdentifier.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/locationIndependentIdentifierDraft4.json
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/locationIndependentIdentifierPre2019.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/name-defs.json
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/name.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/ref-and-definitions.json
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/ref-and-defs.json
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/subSchemas-defs.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/subSchemas.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/tree.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/baseUriChange/folderInteger.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/baseUriChangeFolder/folderInteger.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/baseUriChangeFolderInSubschema/folderInteger.json
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft-next/format-assertion-false.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft-next/format-assertion-true.json
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft-next/metaschema-no-validation.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft2019-09/metaschema-no-validation.json
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft2020-12/format-assertion-false.json
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft2020-12/format-assertion-true.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/draft2020-12/metaschema-no-validation.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/nested/foo-ref-string.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/remotes/nested/string.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/additionalProperties.json
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/allOf.json
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/anchor.json
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/anyOf.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/boolean_schema.json
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/const.json
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/contains.json
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/content.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/default.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/defs.json
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/dependentRequired.json
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/dependentSchemas.json
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/dynamicRef.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/enum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/exclusiveMaximum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/exclusiveMinimum.json
--rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/format.json
--rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/id.json
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/if-then-else.json
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/infinite-loop-detection.json
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/items.json
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/maxContains.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/maxItems.json
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/maxLength.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/maxProperties.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/maximum.json
--rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/minContains.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/minItems.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/minLength.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/minProperties.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/multipleOf.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/not.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/pattern.json
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/patternProperties.json
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/prefixItems.json
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/properties.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/propertyNames.json
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/ref.json
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/refRemote.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/required.json
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/type.json
--rw-r--r--   0        0        0    18072 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/unevaluatedItems.json
--rw-r--r--   0        0        0    40391 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/unevaluatedProperties.json
--rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/uniqueItems.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/unknownKeyword.json
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/vocabulary.json
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/bignum.json
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/dependencies-compatibility.json
--rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/float-overflow.json
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format-assertion.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/non-bmp-regex.json
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/refOfUnknownKeyword.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/date-time.json
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/date.json
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/duration.json
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/hostname.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/idn-email.json
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/idn-hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/ipv6.json
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/iri-reference.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/iri.json
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/json-pointer.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/regex.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/relative-json-pointer.json
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/time.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/uri-reference.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/uri-template.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/uri.json
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft-next/optional/format/uuid.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/additionalItems.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/additionalProperties.json
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/allOf.json
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/anchor.json
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/anyOf.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/boolean_schema.json
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/const.json
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/contains.json
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/content.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/default.json
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/defs.json
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/dependentRequired.json
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/dependentSchemas.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/enum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/exclusiveMaximum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/exclusiveMinimum.json
--rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/format.json
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/id.json
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/if-then-else.json
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/infinite-loop-detection.json
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/items.json
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/maxContains.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/maxItems.json
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/maxLength.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/maxProperties.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/maximum.json
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/minContains.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/minItems.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/minLength.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/minProperties.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/multipleOf.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/not.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/pattern.json
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/patternProperties.json
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/properties.json
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/propertyNames.json
--rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/recursiveRef.json
--rw-r--r--   0        0        0    24690 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/ref.json
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/refRemote.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/required.json
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/type.json
--rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/unevaluatedItems.json
--rw-r--r--   0        0        0    39154 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/unevaluatedProperties.json
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/uniqueItems.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/unknownKeyword.json
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/vocabulary.json
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/bignum.json
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/dependencies-compatibility.json
--rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/float-overflow.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/non-bmp-regex.json
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/refOfUnknownKeyword.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/date-time.json
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/date.json
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/duration.json
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/hostname.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/idn-email.json
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/idn-hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/ipv6.json
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/iri-reference.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/iri.json
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/json-pointer.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/regex.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/relative-json-pointer.json
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/time.json
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/unknown.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri-reference.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri-template.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri.json
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uuid.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/additionalProperties.json
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/allOf.json
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/anchor.json
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/anyOf.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/boolean_schema.json
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/const.json
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/contains.json
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/content.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/default.json
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/defs.json
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/dependentRequired.json
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/dependentSchemas.json
--rw-r--r--   0        0        0    20575 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/dynamicRef.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/enum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/exclusiveMaximum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/exclusiveMinimum.json
--rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/format.json
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/id.json
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/if-then-else.json
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/infinite-loop-detection.json
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/items.json
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/maxContains.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/maxItems.json
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/maxLength.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/maxProperties.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/maximum.json
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/minContains.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/minItems.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/minLength.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/minProperties.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/multipleOf.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/not.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/pattern.json
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/patternProperties.json
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/prefixItems.json
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/properties.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/propertyNames.json
--rw-r--r--   0        0        0    24702 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/ref.json
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/refRemote.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/required.json
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/type.json
--rw-r--r--   0        0        0    18072 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/unevaluatedItems.json
--rw-r--r--   0        0        0    39154 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/unevaluatedProperties.json
--rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/uniqueItems.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/unknownKeyword.json
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/vocabulary.json
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/bignum.json
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/dependencies-compatibility.json
--rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/float-overflow.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format-assertion.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/non-bmp-regex.json
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/refOfUnknownKeyword.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/date-time.json
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/date.json
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/duration.json
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/hostname.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/idn-email.json
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/idn-hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/ipv6.json
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/iri-reference.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/iri.json
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/json-pointer.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/regex.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/relative-json-pointer.json
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/time.json
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/unknown.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri-reference.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri-template.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri.json
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uuid.json
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/additionalItems.json
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/additionalProperties.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/default.json
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/dependencies.json
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/disallow.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/divisibleBy.json
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/enum.json
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/extends.json
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/format.json
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/infinite-loop-detection.json
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/items.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/maxItems.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/maxLength.json
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/maximum.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/minItems.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/minLength.json
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/minimum.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/pattern.json
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/patternProperties.json
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/properties.json
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/ref.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/refRemote.json
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/required.json
--rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/type.json
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/uniqueItems.json
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/bignum.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/ecmascript-regex.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/non-bmp-regex.json
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/color.json
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/date-time.json
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/date.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/email.json
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/host-name.json
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/ip-address.json
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/ipv6.json
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/regex.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/time.json
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft3/optional/format/uri.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/additionalItems.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/additionalProperties.json
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/allOf.json
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/anyOf.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/default.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/definitions.json
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/dependencies.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/enum.json
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/format.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/id.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/infinite-loop-detection.json
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/items.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/maxItems.json
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/maxLength.json
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/maxProperties.json
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/maximum.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/minItems.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/minLength.json
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/minProperties.json
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/multipleOf.json
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/not.json
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/pattern.json
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/patternProperties.json
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/properties.json
--rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/ref.json
--rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/refRemote.json
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/required.json
--rw-r--r--   0        0        0    13221 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/type.json
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/uniqueItems.json
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/bignum.json
--rw-r--r--   0        0        0    18555 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/float-overflow.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/non-bmp-regex.json
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/date-time.json
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/ipv6.json
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/unknown.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft4/optional/format/uri.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/additionalItems.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/additionalProperties.json
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/allOf.json
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/anyOf.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/boolean_schema.json
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/const.json
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/contains.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/default.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/definitions.json
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/dependencies.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/enum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/exclusiveMaximum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/exclusiveMinimum.json
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/format.json
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/id.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/infinite-loop-detection.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/items.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/maxItems.json
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/maxLength.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/maxProperties.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/maximum.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/minItems.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/minLength.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/minProperties.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/multipleOf.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/not.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/pattern.json
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/patternProperties.json
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/properties.json
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/propertyNames.json
--rw-r--r--   0        0        0    23325 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/ref.json
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/refRemote.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/required.json
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/type.json
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/uniqueItems.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/unknownKeyword.json
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/bignum.json
--rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/float-overflow.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/non-bmp-regex.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/date-time.json
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/ipv6.json
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/json-pointer.json
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/unknown.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/uri-reference.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/uri-template.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft6/optional/format/uri.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/additionalItems.json
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/additionalProperties.json
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/allOf.json
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/anyOf.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/boolean_schema.json
--rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/const.json
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/contains.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/default.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/definitions.json
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/dependencies.json
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/enum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/exclusiveMaximum.json
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/exclusiveMinimum.json
--rw-r--r--   0        0        0    18067 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/format.json
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/id.json
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/if-then-else.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/infinite-loop-detection.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/items.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/maxItems.json
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/maxLength.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/maxProperties.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/maximum.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/minItems.json
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/minLength.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/minProperties.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/minimum.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/multipleOf.json
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/not.json
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/oneOf.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/pattern.json
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/patternProperties.json
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/properties.json
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/propertyNames.json
--rw-r--r--   0        0        0    24382 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/ref.json
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/refRemote.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/required.json
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/type.json
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/uniqueItems.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/unknownKeyword.json
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/bignum.json
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/content.json
--rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/ecmascript-regex.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/float-overflow.json
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/non-bmp-regex.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/date-time.json
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/date.json
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/email.json
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/hostname.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/idn-email.json
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/idn-hostname.json
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/ipv4.json
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/ipv6.json
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/iri-reference.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/iri.json
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/json-pointer.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/regex.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/relative-json-pointer.json
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/time.json
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/unknown.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/uri-reference.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/uri-template.json
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.0/json/tests/draft7/optional/format/uri.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/__main__.py
--rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/_format.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/_legacy_validators.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/_types.py
--rw-r--r--   0        0        0    10423 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/_utils.py
--rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/_validators.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/cli.py
--rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/exceptions.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/protocols.py
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/validators.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/benchmarks/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/benchmarks/issue232.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/benchmarks/json_schema_test_suite.py
--rw-r--r--   0        0        0   117105 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/benchmarks/issue232/issue.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft2019-09.json
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft2020-12.json
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft3.json
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft4.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft6.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/draft7.json
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/schemas/vocabularies.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/_helpers.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/_suite.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/fuzz_validate.py
--rw-r--r--   0        0        0    28674 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_cli.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_deprecations.py
--rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_exceptions.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_format.py
--rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_jsonschema_test_suite.py
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_types.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_utils.py
--rw-r--r--   0        0        0    74025 2020-02-02 00:00:00.000000 jsonschema-4.9.0/jsonschema/tests/test_validators.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 jsonschema-4.9.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema-4.9.0/COPYING
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jsonschema-4.9.0/README.rst
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 jsonschema-4.9.0/pyproject.toml
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 jsonschema-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.coveragerc
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.flake8
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     9336 2020-02-02 00:00:00.000000 jsonschema-4.9.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 jsonschema-4.9.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jsonschema-4.9.1/codecov.yml
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 jsonschema-4.9.1/tox.ini
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.github/SECURITY.md
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/Makefile
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/conf.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/creating.rst
+-rw-r--r--   0        0        0    12309 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/errors.rst
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/faq.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/index.rst
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/jsonschema_role.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/make.bat
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/references.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/requirements.in
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/requirements.txt
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 jsonschema-4.9.1/docs/validate.rst
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/LICENSE
+-rw-r--r--   0        0        0    15718 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/README.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/package.json
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/test-schema.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tox.ini
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/.github/CODEOWNERS
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/.github/workflows/ci.yml
+-rwxr-xr-x   0        0        0     8492 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/bin/jsonschema_suite
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/extendible-dynamic-ref.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/integer.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/locationIndependentIdentifier.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/locationIndependentIdentifierDraft4.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/locationIndependentIdentifierPre2019.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/name-defs.json
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/name.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/ref-and-definitions.json
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/ref-and-defs.json
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/subSchemas-defs.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/subSchemas.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/tree.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/baseUriChange/folderInteger.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/baseUriChangeFolder/folderInteger.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/baseUriChangeFolderInSubschema/folderInteger.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft-next/format-assertion-false.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft-next/format-assertion-true.json
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft-next/metaschema-no-validation.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft2019-09/metaschema-no-validation.json
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft2020-12/format-assertion-false.json
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft2020-12/format-assertion-true.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/draft2020-12/metaschema-no-validation.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/nested/foo-ref-string.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/remotes/nested/string.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/additionalProperties.json
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/allOf.json
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/anchor.json
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/anyOf.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/boolean_schema.json
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/const.json
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/contains.json
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/content.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/default.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/defs.json
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/dependentRequired.json
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/dependentSchemas.json
+-rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/dynamicRef.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/enum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/exclusiveMaximum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/exclusiveMinimum.json
+-rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/format.json
+-rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/id.json
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/if-then-else.json
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/infinite-loop-detection.json
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/items.json
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/maxContains.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/maxItems.json
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/maxLength.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/maxProperties.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/maximum.json
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/minContains.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/minItems.json
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/minLength.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/minProperties.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/multipleOf.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/not.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/pattern.json
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/patternProperties.json
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/prefixItems.json
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/properties.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/propertyNames.json
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/ref.json
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/refRemote.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/required.json
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/type.json
+-rw-r--r--   0        0        0    18072 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/unevaluatedItems.json
+-rw-r--r--   0        0        0    40391 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/unevaluatedProperties.json
+-rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/uniqueItems.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/unknownKeyword.json
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/vocabulary.json
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/bignum.json
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/dependencies-compatibility.json
+-rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/float-overflow.json
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format-assertion.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/refOfUnknownKeyword.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/date-time.json
+-rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/date.json
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/duration.json
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/hostname.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/idn-email.json
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/idn-hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/ipv6.json
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/iri-reference.json
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/iri.json
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/json-pointer.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/regex.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/relative-json-pointer.json
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/time.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/uri-reference.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/uri-template.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/uri.json
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft-next/optional/format/uuid.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/additionalItems.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/additionalProperties.json
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/allOf.json
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/anchor.json
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/anyOf.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/boolean_schema.json
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/const.json
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/contains.json
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/content.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/default.json
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/defs.json
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/dependentRequired.json
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/dependentSchemas.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/enum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/exclusiveMaximum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/exclusiveMinimum.json
+-rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/format.json
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/id.json
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/if-then-else.json
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/infinite-loop-detection.json
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/items.json
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/maxContains.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/maxItems.json
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/maxLength.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/maxProperties.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/maximum.json
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/minContains.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/minItems.json
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/minLength.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/minProperties.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/multipleOf.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/not.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/pattern.json
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/patternProperties.json
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/properties.json
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/propertyNames.json
+-rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/recursiveRef.json
+-rw-r--r--   0        0        0    24690 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/ref.json
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/refRemote.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/required.json
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/type.json
+-rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/unevaluatedItems.json
+-rw-r--r--   0        0        0    39154 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/unevaluatedProperties.json
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/uniqueItems.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/unknownKeyword.json
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/vocabulary.json
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/bignum.json
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/dependencies-compatibility.json
+-rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/float-overflow.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/refOfUnknownKeyword.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/date-time.json
+-rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/date.json
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/duration.json
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/hostname.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/idn-email.json
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/idn-hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/ipv6.json
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/iri-reference.json
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/iri.json
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/json-pointer.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/regex.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/relative-json-pointer.json
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/time.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/unknown.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri-reference.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri-template.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri.json
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uuid.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/additionalProperties.json
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/allOf.json
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/anchor.json
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/anyOf.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/boolean_schema.json
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/const.json
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/contains.json
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/content.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/default.json
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/defs.json
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/dependentRequired.json
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/dependentSchemas.json
+-rw-r--r--   0        0        0    20575 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/dynamicRef.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/enum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/exclusiveMaximum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/exclusiveMinimum.json
+-rw-r--r--   0        0        0    20183 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/format.json
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/id.json
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/if-then-else.json
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/infinite-loop-detection.json
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/items.json
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/maxContains.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/maxItems.json
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/maxLength.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/maxProperties.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/maximum.json
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/minContains.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/minItems.json
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/minLength.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/minProperties.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/multipleOf.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/not.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/pattern.json
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/patternProperties.json
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/prefixItems.json
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/properties.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/propertyNames.json
+-rw-r--r--   0        0        0    24702 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/ref.json
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/refRemote.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/required.json
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/type.json
+-rw-r--r--   0        0        0    18072 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/unevaluatedItems.json
+-rw-r--r--   0        0        0    39154 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/unevaluatedProperties.json
+-rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/uniqueItems.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/unknownKeyword.json
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/vocabulary.json
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/bignum.json
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/dependencies-compatibility.json
+-rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/float-overflow.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format-assertion.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/refOfUnknownKeyword.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/date-time.json
+-rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/date.json
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/duration.json
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/hostname.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/idn-email.json
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/idn-hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/ipv6.json
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/iri-reference.json
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/iri.json
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/json-pointer.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/regex.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/relative-json-pointer.json
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/time.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/unknown.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri-reference.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri-template.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri.json
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uuid.json
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/additionalItems.json
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/additionalProperties.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/default.json
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/dependencies.json
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/disallow.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/divisibleBy.json
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/enum.json
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/extends.json
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/format.json
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/infinite-loop-detection.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/items.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/maxItems.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/maxLength.json
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/maximum.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/minItems.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/minLength.json
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/minimum.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/pattern.json
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/patternProperties.json
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/properties.json
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/ref.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/refRemote.json
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/required.json
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/type.json
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/uniqueItems.json
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/bignum.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/color.json
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/date-time.json
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/date.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/email.json
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/host-name.json
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/ip-address.json
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/ipv6.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/regex.json
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/time.json
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft3/optional/format/uri.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/additionalItems.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/additionalProperties.json
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/allOf.json
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/anyOf.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/default.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/definitions.json
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/dependencies.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/enum.json
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/format.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/id.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/infinite-loop-detection.json
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/items.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/maxItems.json
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/maxLength.json
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/maxProperties.json
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/maximum.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/minItems.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/minLength.json
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/minProperties.json
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/multipleOf.json
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/not.json
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/pattern.json
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/patternProperties.json
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/properties.json
+-rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/ref.json
+-rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/refRemote.json
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/required.json
+-rw-r--r--   0        0        0    13221 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/type.json
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/uniqueItems.json
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/bignum.json
+-rw-r--r--   0        0        0    18555 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/float-overflow.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/date-time.json
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/ipv6.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/unknown.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft4/optional/format/uri.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/additionalItems.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/additionalProperties.json
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/allOf.json
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/anyOf.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/boolean_schema.json
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/const.json
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/contains.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/default.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/definitions.json
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/dependencies.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/enum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/exclusiveMaximum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/exclusiveMinimum.json
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/format.json
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/id.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/infinite-loop-detection.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/items.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/maxItems.json
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/maxLength.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/maxProperties.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/maximum.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/minItems.json
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/minLength.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/minProperties.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/multipleOf.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/not.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/pattern.json
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/patternProperties.json
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/properties.json
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/propertyNames.json
+-rw-r--r--   0        0        0    23325 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/ref.json
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/refRemote.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/required.json
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/type.json
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/uniqueItems.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/unknownKeyword.json
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/bignum.json
+-rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/float-overflow.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/date-time.json
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/ipv6.json
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/json-pointer.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/unknown.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/uri-reference.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/uri-template.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft6/optional/format/uri.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/additionalItems.json
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/additionalProperties.json
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/allOf.json
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/anyOf.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/boolean_schema.json
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/const.json
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/contains.json
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/default.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/definitions.json
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/dependencies.json
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/enum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/exclusiveMaximum.json
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/exclusiveMinimum.json
+-rw-r--r--   0        0        0    18067 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/format.json
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/id.json
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/if-then-else.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/infinite-loop-detection.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/items.json
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/maxItems.json
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/maxLength.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/maxProperties.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/maximum.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/minItems.json
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/minLength.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/minProperties.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/minimum.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/multipleOf.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/not.json
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/oneOf.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/pattern.json
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/patternProperties.json
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/properties.json
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/propertyNames.json
+-rw-r--r--   0        0        0    24382 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/ref.json
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/refRemote.json
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/required.json
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/type.json
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/uniqueItems.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/unknownKeyword.json
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/bignum.json
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/content.json
+-rw-r--r--   0        0        0    18565 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/ecmascript-regex.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/float-overflow.json
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/non-bmp-regex.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/date-time.json
+-rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/date.json
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/email.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/hostname.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/idn-email.json
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/idn-hostname.json
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/ipv4.json
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/ipv6.json
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/iri-reference.json
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/iri.json
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/json-pointer.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/regex.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/relative-json-pointer.json
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/time.json
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/unknown.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/uri-reference.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/uri-template.json
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jsonschema-4.9.1/json/tests/draft7/optional/format/uri.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/__main__.py
+-rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/_format.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/_legacy_validators.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/_types.py
+-rw-r--r--   0        0        0    10423 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/_utils.py
+-rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/_validators.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/cli.py
+-rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/exceptions.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/protocols.py
+-rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/validators.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/benchmarks/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/benchmarks/issue232.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/benchmarks/json_schema_test_suite.py
+-rw-r--r--   0        0        0   117105 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/benchmarks/issue232/issue.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft2019-09.json
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft2020-12.json
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft3.json
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft4.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft6.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/draft7.json
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/schemas/vocabularies.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/_helpers.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/_suite.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/fuzz_validate.py
+-rw-r--r--   0        0        0    28674 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_cli.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_deprecations.py
+-rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_format.py
+-rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_jsonschema_test_suite.py
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_types.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_utils.py
+-rw-r--r--   0        0        0    74025 2020-02-02 00:00:00.000000 jsonschema-4.9.1/jsonschema/tests/test_validators.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 jsonschema-4.9.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema-4.9.1/COPYING
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 jsonschema-4.9.1/README.rst
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 jsonschema-4.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 jsonschema-4.9.1/PKG-INFO
```

### Comparing `jsonschema-4.9.0/CHANGELOG.rst` & `jsonschema-4.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v4.9.1
+------
+
+* Update some documentation examples to use newer validator releases in their
+  sample code.
+
 v4.9.0
 ------
 
 * Fix relative ``$ref`` resolution when the base URI is a URN or other scheme
   (#544).
 * ``pkgutil.resolve_name`` is now used to retrieve validators
   provided on the command line. This function is only available on
```

### Comparing `jsonschema-4.9.0/CONTRIBUTING.rst` & `jsonschema-4.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/tox.ini` & `jsonschema-4.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/.github/SECURITY.md` & `jsonschema-4.9.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/.github/workflows/ci.yml` & `jsonschema-4.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/.github/workflows/coverage.yml` & `jsonschema-4.9.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/.github/workflows/fuzz.yml` & `jsonschema-4.9.1/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/Makefile` & `jsonschema-4.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/conf.py` & `jsonschema-4.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/creating.rst` & `jsonschema-4.9.1/docs/creating.rst`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/errors.rst` & `jsonschema-4.9.1/docs/errors.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     .. attribute:: message
 
         A human readable message explaining the error.
 
     .. attribute:: validator
 
         The name of the failed `validator
-        <https://json-schema.org/draft-04/json-schema-validation.html#rfc.section.5>`_.
+        <https://json-schema.org/draft/2020-12/json-schema-validation.html#name-a-vocabulary-for-structural>`_.
 
     .. attribute:: validator_value
 
         The value for the failed validator in the schema.
 
     .. attribute:: schema
 
@@ -136,15 +136,15 @@
             "anyOf": [
                 {"type": "string", "maxLength": 2},
                 {"type": "integer", "minimum": 5}
             ]
         }
     }
     instance = [{}, 3, "foo"]
-    v = Draft7Validator(schema)
+    v = Draft202012Validator(schema)
     errors = sorted(v.iter_errors(instance), key=lambda e: e.path)
 
 The error messages in this situation are not very helpful on their own.
 
 .. testcode::
 
     for error in errors:
@@ -250,15 +250,15 @@
     }
     instance = ["spam", 2]
 
 For clarity's sake, the given instance has three errors under this schema:
 
 .. testcode::
 
-    v = Draft3Validator(schema)
+    v = Draft202012Validator(schema)
     for error in sorted(v.iter_errors(["spam", 2]), key=str):
         print(error.message)
 
 .. testoutput::
 
     'spam' is not of type 'number'
     'spam' is not one of [1, 2, 3]
@@ -346,22 +346,22 @@
 ------------------------
 
 The `best_match` function is a simple but useful function for attempting
 to guess the most relevant error in a given bunch.
 
 .. doctest::
 
-        >>> from jsonschema import Draft7Validator
+        >>> from jsonschema import Draft202012Validator
         >>> from jsonschema.exceptions import best_match
 
         >>> schema = {
         ...     "type": "array",
         ...     "minItems": 3,
         ... }
-        >>> print(best_match(Draft7Validator(schema).iter_errors(11)).message)
+        >>> print(best_match(Draft202012Validator(schema).iter_errors(11)).message)
         11 is not of type 'array'
 
 
 .. autofunction:: best_match
 
 
 .. function:: relevance(validation_error)
@@ -391,15 +391,15 @@
     ...             "properties": {
     ...                 "home": {"type": "string"}
     ...             },
     ...         },
     ...     },
     ... }
     >>> instance = {"name": 123, "phones": {"home": [123]}}
-    >>> errors = Draft7Validator(schema).iter_errors(instance)
+    >>> errors = Draft202012Validator(schema).iter_errors(instance)
     >>> [
     ...     e.path[-1]
     ...     for e in sorted(errors, key=exceptions.relevance)
     ... ]
     ['home', 'name']
```

### Comparing `jsonschema-4.9.0/docs/faq.rst` & `jsonschema-4.9.1/docs/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -146,17 +146,17 @@
 allows you to `define your own validator classes and callables
 <creating>`, so you can easily create an `jsonschema.protocols.Validator`
 that does do default setting. Here's some code to get you started. (In
 this code, we add the default properties to each object *before* the
 properties are validated, so the default values themselves will need to
 be valid under the schema.)
 
-    .. code-block:: python
+    .. testcode::
 
-        from jsonschema import Draft7Validator, validators
+        from jsonschema import Draft202012Validator, validators
 
 
         def extend_with_default(validator_class):
             validate_properties = validator_class.VALIDATORS["properties"]
 
             def set_defaults(validator, properties, instance, schema):
                 for property, subschema in properties.items():
@@ -169,29 +169,29 @@
                     yield error
 
             return validators.extend(
                 validator_class, {"properties" : set_defaults},
             )
 
 
-        DefaultValidatingDraft7Validator = extend_with_default(Draft7Validator)
+        DefaultValidatingValidator = extend_with_default(Draft202012Validator)
 
 
         # Example usage:
         obj = {}
         schema = {'properties': {'foo': {'default': 'bar'}}}
-        # Note jsonschem.validate(obj, schema, cls=DefaultValidatingDraft7Validator)
+        # Note jsonschem.validate(obj, schema, cls=DefaultValidatingValidator)
         # will not work because the metaschema contains `default` directives.
-        DefaultValidatingDraft7Validator(schema).validate(obj)
+        DefaultValidatingValidator(schema).validate(obj)
         assert obj == {'foo': 'bar'}
 
 
 See the above-linked document for more info on how this works, but
 basically, it just extends the :validator:`properties` validator on
-a `jsonschema.Draft7Validator` to then go ahead and update all the
+a `jsonschema.Draft202012Validator` to then go ahead and update all the
 defaults.
 
 .. note::
 
     If you're interested in a more interesting solution to a larger
     class of these types of transformations, keep an eye on `Seep
     <https://github.com/Julian/Seep>`_, which is an experimental
@@ -201,15 +201,15 @@
 
 .. hint::
 
     The above code can provide default values for an entire object and
     all of its properties, but only if your schema provides a default
     value for the object itself, like so:
 
-    .. code-block:: python
+    .. testcode::
 
         schema = {
             "type": "object",
             "properties": {
                 "outer-object": {
                     "type": "object",
                     "properties" : {
@@ -220,26 +220,26 @@
                     },
                     "default": {} # <-- MUST PROVIDE DEFAULT OBJECT
                 }
             }
         }
 
         obj = {}
-        DefaultValidatingDraft7Validator(schema).validate(obj)
+        DefaultValidatingValidator(schema).validate(obj)
         assert obj == {'outer-object': {'inner-object': 'INNER-DEFAULT'}}
 
     ...but if you don't provide a default value for your object, then
     it won't be instantiated at all, much less populated with default
     properties.
 
-    .. code-block:: python
+    .. testcode::
 
         del schema["properties"]["outer-object"]["default"]
         obj2 = {}
-        DefaultValidatingDraft7Validator(schema).validate(obj2)
+        DefaultValidatingValidator(schema).validate(obj2)
         assert obj2 == {} # whoops
 
 
 How do jsonschema version numbers work?
 ---------------------------------------
 
 ``jsonschema`` tries to follow the `Semantic Versioning
```

### Comparing `jsonschema-4.9.0/docs/jsonschema_role.py` & `jsonschema-4.9.1/docs/jsonschema_role.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/make.bat` & `jsonschema-4.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/requirements.txt` & `jsonschema-4.9.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/docs/validate.rst` & `jsonschema-4.9.1/docs/validate.rst`

 * *Files 4% similar despite different names*

```diff
@@ -80,28 +80,35 @@
 given how common validating these types are.
 
 If you *do* want the generality, or just want to add a few specific additional
 types as being acceptable for a validator object, then you should update an
 existing `TypeChecker` or create a new one. You may then create a new
 `Validator` via `jsonschema.validators.extend`.
 
-.. code-block:: python
+.. testcode::
+
+    from jsonschema import validators
 
     class MyInteger(object):
         pass
 
     def is_my_int(checker, instance):
         return (
-            Draft3Validator.TYPE_CHECKER.is_type(instance, "number") or
+            Draft202012Validator.TYPE_CHECKER.is_type(instance, "number") or
             isinstance(instance, MyInteger)
         )
 
-    type_checker = Draft3Validator.TYPE_CHECKER.redefine("number", is_my_int)
-
-    CustomValidator = extend(Draft3Validator, type_checker=type_checker)
+    type_checker = Draft202012Validator.TYPE_CHECKER.redefine(
+        "number", is_my_int,
+    )
+
+    CustomValidator = validators.extend(
+        Draft202012Validator,
+        type_checker=type_checker,
+    )
     validator = CustomValidator(schema={"type" : "number"})
 
 
 .. autoexception:: jsonschema.exceptions.UnknownType
 
 .. _versioned-validators:
 
@@ -123,31 +130,31 @@
 
 .. autoclass:: Draft4Validator
 
 .. autoclass:: Draft3Validator
 
 
 For example, if you wanted to validate a schema you created against the
-Draft 7 meta-schema, you could use:
+Draft 2020-12 meta-schema, you could use:
 
-.. code-block:: python
+.. testcode::
 
-    from jsonschema import Draft7Validator
+    from jsonschema import Draft202012Validator
 
     schema = {
-        "$schema": "http://json-schema.org/draft-07/schema#",
+        "$schema": Draft202012Validator.META_SCHEMA["$id"],
 
         "type": "object",
         "properties": {
             "name": {"type": "string"},
             "email": {"type": "string"},
         },
         "required": ["email"]
     }
-    Draft7Validator.check_schema(schema)
+    Draft202012Validator.check_schema(schema)
 
 
 .. _validating formats:
 
 Validating Formats
 ------------------
 
@@ -159,15 +166,15 @@
 
 .. doctest::
 
     >>> validate("127.0.0.1", {"format" : "ipv4"})
     >>> validate(
     ...     instance="-12",
     ...     schema={"format" : "ipv4"},
-    ...     format_checker=draft7_format_checker,
+    ...     format_checker=draft202012_format_checker,
     ... )
     Traceback (most recent call last):
         ...
     ValidationError: "-12" is not a "ipv4"
 
 .. autoclass:: FormatChecker
     :members:
```

### Comparing `jsonschema-4.9.0/json/.gitignore` & `jsonschema-4.9.1/json/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/LICENSE` & `jsonschema-4.9.1/json/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/README.md` & `jsonschema-4.9.1/json/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/test-schema.json` & `jsonschema-4.9.1/json/test-schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/bin/jsonschema_suite` & `jsonschema-4.9.1/json/bin/jsonschema_suite`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft-next/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/allOf.json` & `jsonschema-4.9.1/json/tests/draft-next/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/anchor.json` & `jsonschema-4.9.1/json/tests/draft-next/anchor.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/anyOf.json` & `jsonschema-4.9.1/json/tests/draft-next/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/boolean_schema.json` & `jsonschema-4.9.1/json/tests/draft-next/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/const.json` & `jsonschema-4.9.1/json/tests/draft-next/const.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/contains.json` & `jsonschema-4.9.1/json/tests/draft-next/contains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/content.json` & `jsonschema-4.9.1/json/tests/draft-next/content.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/default.json` & `jsonschema-4.9.1/json/tests/draft-next/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/defs.json` & `jsonschema-4.9.1/json/tests/draft-next/defs.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/dependentRequired.json` & `jsonschema-4.9.1/json/tests/draft-next/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/dependentSchemas.json` & `jsonschema-4.9.1/json/tests/draft-next/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/dynamicRef.json` & `jsonschema-4.9.1/json/tests/draft-next/dynamicRef.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/enum.json` & `jsonschema-4.9.1/json/tests/draft-next/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/exclusiveMaximum.json` & `jsonschema-4.9.1/json/tests/draft-next/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/exclusiveMinimum.json` & `jsonschema-4.9.1/json/tests/draft-next/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/format.json` & `jsonschema-4.9.1/json/tests/draft-next/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/id.json` & `jsonschema-4.9.1/json/tests/draft-next/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/if-then-else.json` & `jsonschema-4.9.1/json/tests/draft-next/if-then-else.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft-next/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/items.json` & `jsonschema-4.9.1/json/tests/draft-next/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/maxContains.json` & `jsonschema-4.9.1/json/tests/draft-next/maxContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/maxItems.json` & `jsonschema-4.9.1/json/tests/draft-next/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/maxLength.json` & `jsonschema-4.9.1/json/tests/draft-next/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft-next/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/maximum.json` & `jsonschema-4.9.1/json/tests/draft-next/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/minContains.json` & `jsonschema-4.9.1/json/tests/draft-next/minContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/minItems.json` & `jsonschema-4.9.1/json/tests/draft-next/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/minLength.json` & `jsonschema-4.9.1/json/tests/draft-next/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/minProperties.json` & `jsonschema-4.9.1/json/tests/draft-next/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/minimum.json` & `jsonschema-4.9.1/json/tests/draft-next/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft-next/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/not.json` & `jsonschema-4.9.1/json/tests/draft-next/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/oneOf.json` & `jsonschema-4.9.1/json/tests/draft-next/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/pattern.json` & `jsonschema-4.9.1/json/tests/draft-next/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft-next/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/prefixItems.json` & `jsonschema-4.9.1/json/tests/draft-next/prefixItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/properties.json` & `jsonschema-4.9.1/json/tests/draft-next/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/propertyNames.json` & `jsonschema-4.9.1/json/tests/draft-next/propertyNames.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/ref.json` & `jsonschema-4.9.1/json/tests/draft-next/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/refRemote.json` & `jsonschema-4.9.1/json/tests/draft-next/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/required.json` & `jsonschema-4.9.1/json/tests/draft-next/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/type.json` & `jsonschema-4.9.1/json/tests/draft-next/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/unevaluatedItems.json` & `jsonschema-4.9.1/json/tests/draft-next/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/unevaluatedProperties.json` & `jsonschema-4.9.1/json/tests/draft-next/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft-next/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/unknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft-next/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/vocabulary.json` & `jsonschema-4.9.1/json/tests/draft-next/vocabulary.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/dependencies-compatibility.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format-assertion.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format-assertion.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/refOfUnknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/date.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/duration.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/idn-email.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/idn-hostname.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/iri-reference.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/iri.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/json-pointer.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/regex.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/relative-json-pointer.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/time.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/uri-reference.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/uri-template.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft-next/optional/format/uuid.json` & `jsonschema-4.9.1/json/tests/draft-next/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/additionalItems.json` & `jsonschema-4.9.1/json/tests/draft2019-09/additionalItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/allOf.json` & `jsonschema-4.9.1/json/tests/draft2019-09/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/anchor.json` & `jsonschema-4.9.1/json/tests/draft2019-09/anchor.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/anyOf.json` & `jsonschema-4.9.1/json/tests/draft2019-09/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/boolean_schema.json` & `jsonschema-4.9.1/json/tests/draft2019-09/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/const.json` & `jsonschema-4.9.1/json/tests/draft2019-09/const.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/contains.json` & `jsonschema-4.9.1/json/tests/draft2019-09/contains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/content.json` & `jsonschema-4.9.1/json/tests/draft2019-09/content.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/default.json` & `jsonschema-4.9.1/json/tests/draft2019-09/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/defs.json` & `jsonschema-4.9.1/json/tests/draft2019-09/defs.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/dependentRequired.json` & `jsonschema-4.9.1/json/tests/draft2019-09/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/dependentSchemas.json` & `jsonschema-4.9.1/json/tests/draft2019-09/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/enum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/exclusiveMaximum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/exclusiveMinimum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/format.json` & `jsonschema-4.9.1/json/tests/draft2019-09/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/id.json` & `jsonschema-4.9.1/json/tests/draft2019-09/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/if-then-else.json` & `jsonschema-4.9.1/json/tests/draft2019-09/if-then-else.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft2019-09/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/items.json` & `jsonschema-4.9.1/json/tests/draft2019-09/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/maxContains.json` & `jsonschema-4.9.1/json/tests/draft2019-09/maxContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/maxItems.json` & `jsonschema-4.9.1/json/tests/draft2019-09/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/maxLength.json` & `jsonschema-4.9.1/json/tests/draft2019-09/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/maximum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/minContains.json` & `jsonschema-4.9.1/json/tests/draft2019-09/minContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/minItems.json` & `jsonschema-4.9.1/json/tests/draft2019-09/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/minLength.json` & `jsonschema-4.9.1/json/tests/draft2019-09/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/minProperties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/minimum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft2019-09/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/not.json` & `jsonschema-4.9.1/json/tests/draft2019-09/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/oneOf.json` & `jsonschema-4.9.1/json/tests/draft2019-09/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/pattern.json` & `jsonschema-4.9.1/json/tests/draft2019-09/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/properties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/propertyNames.json` & `jsonschema-4.9.1/json/tests/draft2019-09/propertyNames.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/recursiveRef.json` & `jsonschema-4.9.1/json/tests/draft2019-09/recursiveRef.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/ref.json` & `jsonschema-4.9.1/json/tests/draft2019-09/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/refRemote.json` & `jsonschema-4.9.1/json/tests/draft2019-09/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/required.json` & `jsonschema-4.9.1/json/tests/draft2019-09/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/type.json` & `jsonschema-4.9.1/json/tests/draft2019-09/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/unevaluatedItems.json` & `jsonschema-4.9.1/json/tests/draft2019-09/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/unevaluatedProperties.json` & `jsonschema-4.9.1/json/tests/draft2019-09/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft2019-09/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/unknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft2019-09/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/vocabulary.json` & `jsonschema-4.9.1/json/tests/draft2019-09/vocabulary.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/dependencies-compatibility.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/refOfUnknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/date.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/duration.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/idn-email.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/idn-hostname.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/iri-reference.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/iri.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/json-pointer.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/regex.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/relative-json-pointer.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/time.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/unknown.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri-reference.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri-template.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2019-09/optional/format/uuid.json` & `jsonschema-4.9.1/json/tests/draft2019-09/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/allOf.json` & `jsonschema-4.9.1/json/tests/draft2020-12/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/anchor.json` & `jsonschema-4.9.1/json/tests/draft2020-12/anchor.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/anyOf.json` & `jsonschema-4.9.1/json/tests/draft2020-12/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/boolean_schema.json` & `jsonschema-4.9.1/json/tests/draft2020-12/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/const.json` & `jsonschema-4.9.1/json/tests/draft2020-12/const.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/contains.json` & `jsonschema-4.9.1/json/tests/draft2020-12/contains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/content.json` & `jsonschema-4.9.1/json/tests/draft2020-12/content.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/default.json` & `jsonschema-4.9.1/json/tests/draft2020-12/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/defs.json` & `jsonschema-4.9.1/json/tests/draft2020-12/defs.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/dependentRequired.json` & `jsonschema-4.9.1/json/tests/draft2020-12/dependentRequired.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/dependentSchemas.json` & `jsonschema-4.9.1/json/tests/draft2020-12/dependentSchemas.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/dynamicRef.json` & `jsonschema-4.9.1/json/tests/draft2020-12/dynamicRef.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/enum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/exclusiveMaximum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/exclusiveMinimum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/format.json` & `jsonschema-4.9.1/json/tests/draft2020-12/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/id.json` & `jsonschema-4.9.1/json/tests/draft2020-12/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/if-then-else.json` & `jsonschema-4.9.1/json/tests/draft2020-12/if-then-else.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft2020-12/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/items.json` & `jsonschema-4.9.1/json/tests/draft2020-12/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/maxContains.json` & `jsonschema-4.9.1/json/tests/draft2020-12/maxContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/maxItems.json` & `jsonschema-4.9.1/json/tests/draft2020-12/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/maxLength.json` & `jsonschema-4.9.1/json/tests/draft2020-12/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/maximum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/minContains.json` & `jsonschema-4.9.1/json/tests/draft2020-12/minContains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/minItems.json` & `jsonschema-4.9.1/json/tests/draft2020-12/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/minLength.json` & `jsonschema-4.9.1/json/tests/draft2020-12/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/minProperties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/minimum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft2020-12/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/not.json` & `jsonschema-4.9.1/json/tests/draft2020-12/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/oneOf.json` & `jsonschema-4.9.1/json/tests/draft2020-12/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/pattern.json` & `jsonschema-4.9.1/json/tests/draft2020-12/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/prefixItems.json` & `jsonschema-4.9.1/json/tests/draft2020-12/prefixItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/properties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/propertyNames.json` & `jsonschema-4.9.1/json/tests/draft2020-12/propertyNames.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/ref.json` & `jsonschema-4.9.1/json/tests/draft2020-12/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/refRemote.json` & `jsonschema-4.9.1/json/tests/draft2020-12/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/required.json` & `jsonschema-4.9.1/json/tests/draft2020-12/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/type.json` & `jsonschema-4.9.1/json/tests/draft2020-12/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/unevaluatedItems.json` & `jsonschema-4.9.1/json/tests/draft2020-12/unevaluatedItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/unevaluatedProperties.json` & `jsonschema-4.9.1/json/tests/draft2020-12/unevaluatedProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft2020-12/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/unknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft2020-12/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/vocabulary.json` & `jsonschema-4.9.1/json/tests/draft2020-12/vocabulary.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/dependencies-compatibility.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/dependencies-compatibility.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format-assertion.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format-assertion.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/refOfUnknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/refOfUnknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/date.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/duration.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/duration.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/idn-email.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/idn-hostname.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/iri-reference.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/iri.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/json-pointer.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/regex.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/relative-json-pointer.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/time.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/unknown.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri-reference.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri-template.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft2020-12/optional/format/uuid.json` & `jsonschema-4.9.1/json/tests/draft2020-12/optional/format/uuid.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/additionalItems.json` & `jsonschema-4.9.1/json/tests/draft3/additionalItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft3/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/default.json` & `jsonschema-4.9.1/json/tests/draft3/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/dependencies.json` & `jsonschema-4.9.1/json/tests/draft3/dependencies.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/disallow.json` & `jsonschema-4.9.1/json/tests/draft3/disallow.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/divisibleBy.json` & `jsonschema-4.9.1/json/tests/draft3/divisibleBy.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/enum.json` & `jsonschema-4.9.1/json/tests/draft3/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/extends.json` & `jsonschema-4.9.1/json/tests/draft3/extends.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/format.json` & `jsonschema-4.9.1/json/tests/draft3/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft3/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/items.json` & `jsonschema-4.9.1/json/tests/draft3/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/maxItems.json` & `jsonschema-4.9.1/json/tests/draft3/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/maxLength.json` & `jsonschema-4.9.1/json/tests/draft3/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/maximum.json` & `jsonschema-4.9.1/json/tests/draft3/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/minItems.json` & `jsonschema-4.9.1/json/tests/draft3/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/minLength.json` & `jsonschema-4.9.1/json/tests/draft3/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/minimum.json` & `jsonschema-4.9.1/json/tests/draft3/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/pattern.json` & `jsonschema-4.9.1/json/tests/draft3/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft3/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/properties.json` & `jsonschema-4.9.1/json/tests/draft3/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/ref.json` & `jsonschema-4.9.1/json/tests/draft3/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/refRemote.json` & `jsonschema-4.9.1/json/tests/draft3/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/required.json` & `jsonschema-4.9.1/json/tests/draft3/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/type.json` & `jsonschema-4.9.1/json/tests/draft3/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft3/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft3/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft3/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/color.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/color.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/date.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/host-name.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/host-name.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/ip-address.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/ip-address.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft3/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft3/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/additionalItems.json` & `jsonschema-4.9.1/json/tests/draft4/additionalItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft4/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/allOf.json` & `jsonschema-4.9.1/json/tests/draft4/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/anyOf.json` & `jsonschema-4.9.1/json/tests/draft4/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/default.json` & `jsonschema-4.9.1/json/tests/draft4/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/definitions.json` & `jsonschema-4.9.1/json/tests/draft4/definitions.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/dependencies.json` & `jsonschema-4.9.1/json/tests/draft4/dependencies.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/enum.json` & `jsonschema-4.9.1/json/tests/draft4/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/format.json` & `jsonschema-4.9.1/json/tests/draft4/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/id.json` & `jsonschema-4.9.1/json/tests/draft4/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft4/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/items.json` & `jsonschema-4.9.1/json/tests/draft4/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/maxItems.json` & `jsonschema-4.9.1/json/tests/draft4/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/maxLength.json` & `jsonschema-4.9.1/json/tests/draft4/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft4/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/maximum.json` & `jsonschema-4.9.1/json/tests/draft4/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/minItems.json` & `jsonschema-4.9.1/json/tests/draft4/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/minLength.json` & `jsonschema-4.9.1/json/tests/draft4/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/minProperties.json` & `jsonschema-4.9.1/json/tests/draft4/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/minimum.json` & `jsonschema-4.9.1/json/tests/draft4/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft4/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/not.json` & `jsonschema-4.9.1/json/tests/draft4/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/oneOf.json` & `jsonschema-4.9.1/json/tests/draft4/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/pattern.json` & `jsonschema-4.9.1/json/tests/draft4/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft4/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/properties.json` & `jsonschema-4.9.1/json/tests/draft4/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/ref.json` & `jsonschema-4.9.1/json/tests/draft4/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/refRemote.json` & `jsonschema-4.9.1/json/tests/draft4/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/required.json` & `jsonschema-4.9.1/json/tests/draft4/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/type.json` & `jsonschema-4.9.1/json/tests/draft4/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft4/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft4/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft4/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft4/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/unknown.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft4/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft4/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/additionalItems.json` & `jsonschema-4.9.1/json/tests/draft6/additionalItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft6/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/allOf.json` & `jsonschema-4.9.1/json/tests/draft6/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/anyOf.json` & `jsonschema-4.9.1/json/tests/draft6/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/boolean_schema.json` & `jsonschema-4.9.1/json/tests/draft6/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/const.json` & `jsonschema-4.9.1/json/tests/draft6/const.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/contains.json` & `jsonschema-4.9.1/json/tests/draft6/contains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/default.json` & `jsonschema-4.9.1/json/tests/draft6/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/definitions.json` & `jsonschema-4.9.1/json/tests/draft6/definitions.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/dependencies.json` & `jsonschema-4.9.1/json/tests/draft6/dependencies.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/enum.json` & `jsonschema-4.9.1/json/tests/draft6/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/exclusiveMaximum.json` & `jsonschema-4.9.1/json/tests/draft6/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/exclusiveMinimum.json` & `jsonschema-4.9.1/json/tests/draft6/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/format.json` & `jsonschema-4.9.1/json/tests/draft6/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/id.json` & `jsonschema-4.9.1/json/tests/draft6/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft6/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/items.json` & `jsonschema-4.9.1/json/tests/draft6/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/maxItems.json` & `jsonschema-4.9.1/json/tests/draft6/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/maxLength.json` & `jsonschema-4.9.1/json/tests/draft6/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft6/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/maximum.json` & `jsonschema-4.9.1/json/tests/draft6/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/minItems.json` & `jsonschema-4.9.1/json/tests/draft6/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/minLength.json` & `jsonschema-4.9.1/json/tests/draft6/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/minProperties.json` & `jsonschema-4.9.1/json/tests/draft6/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/minimum.json` & `jsonschema-4.9.1/json/tests/draft6/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft6/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/not.json` & `jsonschema-4.9.1/json/tests/draft6/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/oneOf.json` & `jsonschema-4.9.1/json/tests/draft6/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/pattern.json` & `jsonschema-4.9.1/json/tests/draft6/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft6/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/properties.json` & `jsonschema-4.9.1/json/tests/draft6/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/propertyNames.json` & `jsonschema-4.9.1/json/tests/draft6/propertyNames.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/ref.json` & `jsonschema-4.9.1/json/tests/draft6/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/refRemote.json` & `jsonschema-4.9.1/json/tests/draft6/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/required.json` & `jsonschema-4.9.1/json/tests/draft6/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/type.json` & `jsonschema-4.9.1/json/tests/draft6/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft6/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/unknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft6/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft6/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft6/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft6/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/json-pointer.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/unknown.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/uri-reference.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/uri-template.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft6/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft6/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/additionalItems.json` & `jsonschema-4.9.1/json/tests/draft7/additionalItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/additionalProperties.json` & `jsonschema-4.9.1/json/tests/draft7/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/allOf.json` & `jsonschema-4.9.1/json/tests/draft7/allOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/anyOf.json` & `jsonschema-4.9.1/json/tests/draft7/anyOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/boolean_schema.json` & `jsonschema-4.9.1/json/tests/draft7/boolean_schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/const.json` & `jsonschema-4.9.1/json/tests/draft7/const.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/contains.json` & `jsonschema-4.9.1/json/tests/draft7/contains.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/default.json` & `jsonschema-4.9.1/json/tests/draft7/default.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/definitions.json` & `jsonschema-4.9.1/json/tests/draft7/definitions.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/dependencies.json` & `jsonschema-4.9.1/json/tests/draft7/dependencies.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/enum.json` & `jsonschema-4.9.1/json/tests/draft7/enum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/exclusiveMaximum.json` & `jsonschema-4.9.1/json/tests/draft7/exclusiveMaximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/exclusiveMinimum.json` & `jsonschema-4.9.1/json/tests/draft7/exclusiveMinimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/format.json` & `jsonschema-4.9.1/json/tests/draft7/format.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/id.json` & `jsonschema-4.9.1/json/tests/draft7/id.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/if-then-else.json` & `jsonschema-4.9.1/json/tests/draft7/if-then-else.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/infinite-loop-detection.json` & `jsonschema-4.9.1/json/tests/draft7/infinite-loop-detection.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/items.json` & `jsonschema-4.9.1/json/tests/draft7/items.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/maxItems.json` & `jsonschema-4.9.1/json/tests/draft7/maxItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/maxLength.json` & `jsonschema-4.9.1/json/tests/draft7/maxLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/maxProperties.json` & `jsonschema-4.9.1/json/tests/draft7/maxProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/maximum.json` & `jsonschema-4.9.1/json/tests/draft7/maximum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/minItems.json` & `jsonschema-4.9.1/json/tests/draft7/minItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/minLength.json` & `jsonschema-4.9.1/json/tests/draft7/minLength.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/minProperties.json` & `jsonschema-4.9.1/json/tests/draft7/minProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/minimum.json` & `jsonschema-4.9.1/json/tests/draft7/minimum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/multipleOf.json` & `jsonschema-4.9.1/json/tests/draft7/multipleOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/not.json` & `jsonschema-4.9.1/json/tests/draft7/not.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/oneOf.json` & `jsonschema-4.9.1/json/tests/draft7/oneOf.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/pattern.json` & `jsonschema-4.9.1/json/tests/draft7/pattern.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/patternProperties.json` & `jsonschema-4.9.1/json/tests/draft7/patternProperties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/properties.json` & `jsonschema-4.9.1/json/tests/draft7/properties.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/propertyNames.json` & `jsonschema-4.9.1/json/tests/draft7/propertyNames.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/ref.json` & `jsonschema-4.9.1/json/tests/draft7/ref.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/refRemote.json` & `jsonschema-4.9.1/json/tests/draft7/refRemote.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/required.json` & `jsonschema-4.9.1/json/tests/draft7/required.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/type.json` & `jsonschema-4.9.1/json/tests/draft7/type.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/uniqueItems.json` & `jsonschema-4.9.1/json/tests/draft7/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/unknownKeyword.json` & `jsonschema-4.9.1/json/tests/draft7/unknownKeyword.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/bignum.json` & `jsonschema-4.9.1/json/tests/draft7/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/content.json` & `jsonschema-4.9.1/json/tests/draft7/optional/content.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/ecmascript-regex.json` & `jsonschema-4.9.1/json/tests/draft7/optional/ecmascript-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/non-bmp-regex.json` & `jsonschema-4.9.1/json/tests/draft7/optional/non-bmp-regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/date-time.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/date-time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/date.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/date.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/email.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/hostname.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/idn-email.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/idn-email.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/idn-hostname.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/idn-hostname.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/ipv4.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/ipv4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/ipv6.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/ipv6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/iri-reference.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/iri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/iri.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/iri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/json-pointer.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/regex.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/regex.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/relative-json-pointer.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/relative-json-pointer.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/time.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/time.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/unknown.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/unknown.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/uri-reference.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/uri-reference.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/uri-template.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/uri-template.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/json/tests/draft7/optional/format/uri.json` & `jsonschema-4.9.1/json/tests/draft7/optional/format/uri.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/__init__.py` & `jsonschema-4.9.1/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/_format.py` & `jsonschema-4.9.1/jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/_legacy_validators.py` & `jsonschema-4.9.1/jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/_types.py` & `jsonschema-4.9.1/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/_utils.py` & `jsonschema-4.9.1/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/_validators.py` & `jsonschema-4.9.1/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/cli.py` & `jsonschema-4.9.1/jsonschema/cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/exceptions.py` & `jsonschema-4.9.1/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/protocols.py` & `jsonschema-4.9.1/jsonschema/protocols.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/validators.py` & `jsonschema-4.9.1/jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/benchmarks/issue232/issue.json` & `jsonschema-4.9.1/jsonschema/benchmarks/issue232/issue.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft2019-09.json` & `jsonschema-4.9.1/jsonschema/schemas/draft2019-09.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft2020-12.json` & `jsonschema-4.9.1/jsonschema/schemas/draft2020-12.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft3.json` & `jsonschema-4.9.1/jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft4.json` & `jsonschema-4.9.1/jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft6.json` & `jsonschema-4.9.1/jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/draft7.json` & `jsonschema-4.9.1/jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/schemas/vocabularies.json` & `jsonschema-4.9.1/jsonschema/schemas/vocabularies.json`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/_suite.py` & `jsonschema-4.9.1/jsonschema/tests/_suite.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/fuzz_validate.py` & `jsonschema-4.9.1/jsonschema/tests/fuzz_validate.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_cli.py` & `jsonschema-4.9.1/jsonschema/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_deprecations.py` & `jsonschema-4.9.1/jsonschema/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_exceptions.py` & `jsonschema-4.9.1/jsonschema/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_format.py` & `jsonschema-4.9.1/jsonschema/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_jsonschema_test_suite.py` & `jsonschema-4.9.1/jsonschema/tests/test_jsonschema_test_suite.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_types.py` & `jsonschema-4.9.1/jsonschema/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_utils.py` & `jsonschema-4.9.1/jsonschema/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/jsonschema/tests/test_validators.py` & `jsonschema-4.9.1/jsonschema/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/.gitignore` & `jsonschema-4.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/COPYING` & `jsonschema-4.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/README.rst` & `jsonschema-4.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/pyproject.toml` & `jsonschema-4.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonschema-4.9.0/PKG-INFO` & `jsonschema-4.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema
-Version: 4.9.0
+Version: 4.9.1
 Summary: An implementation of JSON Schema validation for Python
 Project-URL: Homepage, https://github.com/python-jsonschema/jsonschema
 Project-URL: Documentation, https://python-jsonschema.readthedocs.io/
 Project-URL: Issues, https://github.com/python-jsonschema/jsonschema/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Tidelift, https://tidelift.com/subscription/pkg/pypi-jsonschema?utm_source=pypi-jsonschema&utm_medium=referral&utm_campaign=pypi-link
 Project-URL: Changelog, https://github.com/python-jsonschema/jsonschema/blob/main/CHANGELOG.rst
```

