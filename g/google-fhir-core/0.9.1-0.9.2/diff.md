# Comparing `tmp/google_fhir_core-0.9.1-py3-none-any.whl.zip` & `tmp/google_fhir_core-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,178 +1,95 @@
-Zip file size: 631763 bytes, number of entries: 176
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/__init__.py
--rw-r-----  2.0 unx    12193 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/codes.py
--rw-r-----  2.0 unx    18626 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/extensions.py
--rw-r-----  2.0 unx     2275 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/extensions_test.py
--rw-r-----  2.0 unx     7281 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_errors.py
--rw-r-----  2.0 unx     5706 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_errors_test.py
--rw-r-----  2.0 unx     7054 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/references.py
--rw-r-----  2.0 unx    19632 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
--rw-r-----  2.0 unx    66224 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/FhirPathParser.py
--rw-r-----  2.0 unx     8088 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
--rw-r-----  2.0 unx      579 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/__init__.py
--rw-r-----  2.0 unx    39499 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_ast.py
--rw-r-----  2.0 unx    12220 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_ast_test.py
--rw-r-----  2.0 unx    25380 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
--rw-r-----  2.0 unx    43338 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
--rw-r-----  2.0 unx    52954 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_evaluation.py
--rw-r-----  2.0 unx    25010 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
--rw-r-----  2.0 unx    59561 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
--rw-r-----  2.0 unx    79712 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
--rw-r-----  2.0 unx    12297 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_navigation.py
--rw-r-----  2.0 unx     8116 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_navigation_test.py
--rw-r-----  2.0 unx    30292 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_python_interpreter.py
--rw-r-----  2.0 unx    32521 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_semant.py
--rw-r-----  2.0 unx    36633 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_semant_test.py
--rw-r-----  2.0 unx    22613 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
--rw-r-----  2.0 unx    13460 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
--rw-r-----  2.0 unx    34114 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_sql_data_types.py
--rw-r-----  2.0 unx     7696 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
--rw-r-----  2.0 unx     6296 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_structure_definitions.py
--rw-r-----  2.0 unx     9517 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_utils.py
--rw-r-----  2.0 unx    11122 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/_utils_test.py
--rw-r-----  2.0 unx    14392 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/context.py
--rw-r-----  2.0 unx     6461 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/context_test.py
--rw-r-----  2.0 unx    27062 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/expressions.py
--rw-r-----  2.0 unx    37619 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path.py
--rw-r-----  2.0 unx     1298 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_options.py
--rw-r-----  2.0 unx    49814 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
--rw-r-----  2.0 unx   214354 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_test.py
--rw-r-----  2.0 unx    16788 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
--rw-r-----  2.0 unx    46839 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
--rw-r-----  2.0 unx    56541 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
--rw-r-----  2.0 unx     1945 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
--rw-r-----  2.0 unx     5908 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
--rw-r-----  2.0 unx     3861 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/quantity.py
--rw-r-----  2.0 unx     4404 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/fhir_path/quantity_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/__init__.py
--rw-r-----  2.0 unx     6663 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/_primitive_time_utils.py
--rw-r-----  2.0 unx    14323 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/primitive_handler.py
--rw-r-----  2.0 unx     8859 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/resource_validation.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/__init__.py
--rw-r-----  2.0 unx    15207 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/_json_parser.py
--rw-r-----  2.0 unx    15656 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/_json_printer.py
--rw-r-----  2.0 unx     6464 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/json_format_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
--rw-r-----  2.0 unx     5417 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
--rw-r-----  2.0 unx     4301 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
--rw-r-----  2.0 unx     5736 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
--rw-r-----  2.0 unx     2408 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
--rw-r-----  2.0 unx     4502 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
--rw-r-----  2.0 unx    16137 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
--rw-r-----  2.0 unx     4791 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/proto/__init__.py
--rw-r-----  2.0 unx     9188 b- defN 23-Apr-04 16:21 build/lib/google/fhir/core/proto/annotations_pb2.py
--rw-r-----  2.0 unx     1411 b- defN 23-Apr-04 16:21 build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
--rw-r-----  2.0 unx     2354 b- defN 23-Apr-04 16:21 build/lib/google/fhir/core/proto/validation_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/testing/__init__.py
--rw-r-----  2.0 unx     6706 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/testing/protobuf_compare.py
--rw-r-----  2.0 unx     3745 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/testing/testdata_utils.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/__init__.py
--rw-r-----  2.0 unx    13789 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/annotation_utils.py
--rw-r-----  2.0 unx    15883 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/annotation_utils_test.py
--rw-r-----  2.0 unx    17494 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/fhir_package.py
--rw-r-----  2.0 unx    23767 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/fhir_package_test_base.py
--rw-r-----  2.0 unx     9127 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/fhir_types.py
--rw-r-----  2.0 unx     7750 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/fhir_types_test.py
--rw-r-----  2.0 unx     1637 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/path_utils.py
--rw-r-----  2.0 unx     1922 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/path_utils_test.py
--rw-r-----  2.0 unx    12011 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/proto_utils.py
--rw-r-----  2.0 unx    15754 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/proto_utils_test.py
--rw-r-----  2.0 unx     3040 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/resource_utils.py
--rw-r-----  2.0 unx     3789 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/resource_utils_test.py
--rw-r-----  2.0 unx     1876 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/url_utils.py
--rw-r-----  2.0 unx     1870 b- defN 23-Apr-04 16:12 build/lib/google/fhir/core/utils/url_utils_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/__init__.py
--rw-r-----  2.0 unx    12193 b- defN 23-Apr-04 16:12 google/fhir/core/codes.py
--rw-r-----  2.0 unx    18626 b- defN 23-Apr-04 16:12 google/fhir/core/extensions.py
--rw-r-----  2.0 unx     2275 b- defN 23-Apr-04 16:12 google/fhir/core/extensions_test.py
--rw-r-----  2.0 unx     7281 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_errors.py
--rw-r-----  2.0 unx     5706 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_errors_test.py
--rw-r-----  2.0 unx     7054 b- defN 23-Apr-04 16:12 google/fhir/core/references.py
--rw-r-----  2.0 unx    19632 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/FhirPathLexer.py
--rw-r-----  2.0 unx    66224 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/FhirPathParser.py
--rw-r-----  2.0 unx     8088 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/FhirPathVisitor.py
--rw-r-----  2.0 unx      579 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/__init__.py
--rw-r-----  2.0 unx    39499 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_ast.py
--rw-r-----  2.0 unx    12220 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_ast_test.py
--rw-r-----  2.0 unx    25380 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_bigquery_interpreter.py
--rw-r-----  2.0 unx    43338 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_bigquery_sql_functions.py
--rw-r-----  2.0 unx    52954 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_evaluation.py
--rw-r-----  2.0 unx    25010 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_fhir_path_data_types.py
--rw-r-----  2.0 unx    59561 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
--rw-r-----  2.0 unx    79712 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_interpreter_test_base.py
--rw-r-----  2.0 unx    12297 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_navigation.py
--rw-r-----  2.0 unx     8116 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_navigation_test.py
--rw-r-----  2.0 unx    30292 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_python_interpreter.py
--rw-r-----  2.0 unx    32521 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_semant.py
--rw-r-----  2.0 unx    36633 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_semant_test.py
--rw-r-----  2.0 unx    22613 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_spark_interpreter.py
--rw-r-----  2.0 unx    13460 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_spark_sql_functions.py
--rw-r-----  2.0 unx    34114 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_sql_data_types.py
--rw-r-----  2.0 unx     7696 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_sql_data_types_test.py
--rw-r-----  2.0 unx     6296 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_structure_definitions.py
--rw-r-----  2.0 unx     9517 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_utils.py
--rw-r-----  2.0 unx    11122 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/_utils_test.py
--rw-r-----  2.0 unx    14392 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/context.py
--rw-r-----  2.0 unx     6461 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/context_test.py
--rw-r-----  2.0 unx    27062 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/expressions.py
--rw-r-----  2.0 unx    37619 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path.py
--rw-r-----  2.0 unx     1298 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_options.py
--rw-r-----  2.0 unx    49814 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_spark_test.py
--rw-r-----  2.0 unx   214354 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_test.py
--rw-r-----  2.0 unx    16788 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_test_base.py
--rw-r-----  2.0 unx    46839 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_validator.py
--rw-r-----  2.0 unx    56541 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_validator_v2.py
--rw-r-----  2.0 unx     1945 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
--rw-r-----  2.0 unx     5908 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/python_compiled_expressions.py
--rw-r-----  2.0 unx     3861 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/quantity.py
--rw-r-----  2.0 unx     4404 b- defN 23-Apr-04 16:12 google/fhir/core/fhir_path/quantity_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/internal/__init__.py
--rw-r-----  2.0 unx     6663 b- defN 23-Apr-04 16:12 google/fhir/core/internal/_primitive_time_utils.py
--rw-r-----  2.0 unx    14323 b- defN 23-Apr-04 16:12 google/fhir/core/internal/primitive_handler.py
--rw-r-----  2.0 unx     8859 b- defN 23-Apr-04 16:12 google/fhir/core/internal/resource_validation.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/__init__.py
--rw-r-----  2.0 unx    15207 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/_json_parser.py
--rw-r-----  2.0 unx    15656 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/_json_printer.py
--rw-r-----  2.0 unx     6464 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/json_format_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/__init__.py
--rw-r-----  2.0 unx     5417 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_base64_binary.py
--rw-r-----  2.0 unx     4301 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_date.py
--rw-r-----  2.0 unx     5736 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_date_time.py
--rw-r-----  2.0 unx     2408 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_decimal.py
--rw-r-----  2.0 unx     4502 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_instant.py
--rw-r-----  2.0 unx    16137 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
--rw-r-----  2.0 unx     4791 b- defN 23-Apr-04 16:12 google/fhir/core/internal/json_format/wrappers/_time.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/proto/__init__.py
--rwxr-x---  2.0 unx     7697 b- defN 23-Apr-04 16:12 google/fhir/core/proto/annotations.proto
--rw-r-----  2.0 unx     9188 b- defN 23-Apr-04 16:21 google/fhir/core/proto/annotations_pb2.py
--rw-r-----  2.0 unx     1576 b- defN 23-Apr-04 16:12 google/fhir/core/proto/fhirpath_replacement_list.proto
--rw-r-----  2.0 unx     1411 b- defN 23-Apr-04 16:21 google/fhir/core/proto/fhirpath_replacement_list_pb2.py
--rw-r-----  2.0 unx     4935 b- defN 23-Apr-04 16:12 google/fhir/core/proto/validation.proto
--rw-r-----  2.0 unx     2354 b- defN 23-Apr-04 16:21 google/fhir/core/proto/validation_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/testing/__init__.py
--rw-r-----  2.0 unx     6706 b- defN 23-Apr-04 16:12 google/fhir/core/testing/protobuf_compare.py
--rw-r-----  2.0 unx     3745 b- defN 23-Apr-04 16:12 google/fhir/core/testing/testdata_utils.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/core/utils/__init__.py
--rw-r-----  2.0 unx    13789 b- defN 23-Apr-04 16:12 google/fhir/core/utils/annotation_utils.py
--rw-r-----  2.0 unx    15883 b- defN 23-Apr-04 16:12 google/fhir/core/utils/annotation_utils_test.py
--rw-r-----  2.0 unx    17494 b- defN 23-Apr-04 16:12 google/fhir/core/utils/fhir_package.py
--rw-r-----  2.0 unx    23767 b- defN 23-Apr-04 16:12 google/fhir/core/utils/fhir_package_test_base.py
--rw-r-----  2.0 unx     9127 b- defN 23-Apr-04 16:12 google/fhir/core/utils/fhir_types.py
--rw-r-----  2.0 unx     7750 b- defN 23-Apr-04 16:12 google/fhir/core/utils/fhir_types_test.py
--rw-r-----  2.0 unx     1637 b- defN 23-Apr-04 16:12 google/fhir/core/utils/path_utils.py
--rw-r-----  2.0 unx     1922 b- defN 23-Apr-04 16:12 google/fhir/core/utils/path_utils_test.py
--rw-r-----  2.0 unx    12011 b- defN 23-Apr-04 16:12 google/fhir/core/utils/proto_utils.py
--rw-r-----  2.0 unx    15754 b- defN 23-Apr-04 16:12 google/fhir/core/utils/proto_utils_test.py
--rw-r-----  2.0 unx     3040 b- defN 23-Apr-04 16:12 google/fhir/core/utils/resource_utils.py
--rw-r-----  2.0 unx     3789 b- defN 23-Apr-04 16:12 google/fhir/core/utils/resource_utils_test.py
--rw-r-----  2.0 unx     1876 b- defN 23-Apr-04 16:12 google/fhir/core/utils/url_utils.py
--rw-r-----  2.0 unx     1870 b- defN 23-Apr-04 16:12 google/fhir/core/utils/url_utils_test.py
--rwxr-x---  2.0 unx     7697 b- defN 23-Apr-04 16:12 google_fhir_core-0.9.1.data/data/annotations.proto
--rw-r-----  2.0 unx     1576 b- defN 23-Apr-04 16:12 google_fhir_core-0.9.1.data/data/fhirpath_replacement_list.proto
--rw-r-----  2.0 unx     4935 b- defN 23-Apr-04 16:12 google_fhir_core-0.9.1.data/data/validation.proto
--rw-r-----  2.0 unx     1361 b- defN 23-Apr-04 17:13 google_fhir_core-0.9.1.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 23-Apr-04 17:13 google_fhir_core-0.9.1.dist-info/WHEEL
--rw-r-----  2.0 unx       13 b- defN 23-Apr-04 17:13 google_fhir_core-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18746 b- defN 23-Apr-04 17:13 google_fhir_core-0.9.1.dist-info/RECORD
-176 files, 2978450 bytes uncompressed, 600945 bytes compressed:  79.8%
+Zip file size: 323537 bytes, number of entries: 93
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/__init__.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-Apr-17 20:06 google/fhir/core/codes.py
+-rw-r--r--  2.0 unx    18626 b- defN 23-Apr-17 20:06 google/fhir/core/extensions.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Apr-17 20:06 google/fhir/core/extensions_test.py
+-rw-r--r--  2.0 unx     7281 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_errors.py
+-rw-r--r--  2.0 unx     5706 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_errors_test.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-Apr-17 20:06 google/fhir/core/references.py
+-rw-r--r--  2.0 unx    19632 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathLexer.py
+-rw-r--r--  2.0 unx    66224 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathParser.py
+-rw-r--r--  2.0 unx     8088 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/FhirPathVisitor.py
+-rw-r--r--  2.0 unx      579 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/__init__.py
+-rw-r--r--  2.0 unx    39499 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_ast.py
+-rw-r--r--  2.0 unx    12220 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_ast_test.py
+-rw-r--r--  2.0 unx    25380 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_bigquery_interpreter.py
+-rw-r--r--  2.0 unx    43338 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_bigquery_sql_functions.py
+-rw-r--r--  2.0 unx    52892 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_evaluation.py
+-rw-r--r--  2.0 unx    25010 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_fhir_path_data_types.py
+-rw-r--r--  2.0 unx    59561 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
+-rw-r--r--  2.0 unx    79712 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_interpreter_test_base.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_navigation.py
+-rw-r--r--  2.0 unx     8116 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_navigation_test.py
+-rw-r--r--  2.0 unx    30292 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_python_interpreter.py
+-rw-r--r--  2.0 unx    32521 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_semant.py
+-rw-r--r--  2.0 unx    36633 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_semant_test.py
+-rw-r--r--  2.0 unx    22613 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_spark_interpreter.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_spark_sql_functions.py
+-rw-r--r--  2.0 unx    34114 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_sql_data_types.py
+-rw-r--r--  2.0 unx     7696 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_sql_data_types_test.py
+-rw-r--r--  2.0 unx     6296 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_structure_definitions.py
+-rw-r--r--  2.0 unx     9517 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_utils.py
+-rw-r--r--  2.0 unx    11122 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/_utils_test.py
+-rw-r--r--  2.0 unx    14392 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/context.py
+-rw-r--r--  2.0 unx     6461 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/context_test.py
+-rw-r--r--  2.0 unx    27062 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/expressions.py
+-rw-r--r--  2.0 unx    37619 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_options.py
+-rw-r--r--  2.0 unx    49814 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_spark_test.py
+-rw-r--r--  2.0 unx   214354 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_test.py
+-rw-r--r--  2.0 unx    16788 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_test_base.py
+-rw-r--r--  2.0 unx    46839 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator.py
+-rw-r--r--  2.0 unx    56541 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator_v2.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
+-rw-r--r--  2.0 unx     5908 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/python_compiled_expressions.py
+-rw-r--r--  2.0 unx     3861 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/quantity.py
+-rw-r--r--  2.0 unx     4404 b- defN 23-Apr-17 20:06 google/fhir/core/fhir_path/quantity_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/__init__.py
+-rw-r--r--  2.0 unx     6663 b- defN 23-Apr-17 20:06 google/fhir/core/internal/_primitive_time_utils.py
+-rw-r--r--  2.0 unx    14323 b- defN 23-Apr-17 20:06 google/fhir/core/internal/primitive_handler.py
+-rw-r--r--  2.0 unx     8859 b- defN 23-Apr-17 20:06 google/fhir/core/internal/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/__init__.py
+-rw-r--r--  2.0 unx    15207 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/_json_parser.py
+-rw-r--r--  2.0 unx    15656 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/_json_printer.py
+-rw-r--r--  2.0 unx     6464 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/json_format_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5417 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_base64_binary.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_date.py
+-rw-r--r--  2.0 unx     5736 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_date_time.py
+-rw-r--r--  2.0 unx     2408 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_decimal.py
+-rw-r--r--  2.0 unx     4502 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_instant.py
+-rw-r--r--  2.0 unx    16137 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
+-rw-r--r--  2.0 unx     4791 b- defN 23-Apr-17 20:06 google/fhir/core/internal/json_format/wrappers/_time.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/proto/__init__.py
+-rwxr-xr-x  2.0 unx     7697 b- defN 23-Apr-17 20:06 google/fhir/core/proto/annotations.proto
+-rw-r--r--  2.0 unx     9188 b- defN 23-Apr-17 20:07 google/fhir/core/proto/annotations_pb2.py
+-rw-r--r--  2.0 unx     1576 b- defN 23-Apr-17 20:06 google/fhir/core/proto/fhirpath_replacement_list.proto
+-rw-r--r--  2.0 unx     1411 b- defN 23-Apr-17 20:07 google/fhir/core/proto/fhirpath_replacement_list_pb2.py
+-rw-r--r--  2.0 unx     4935 b- defN 23-Apr-17 20:06 google/fhir/core/proto/validation.proto
+-rw-r--r--  2.0 unx     2354 b- defN 23-Apr-17 20:07 google/fhir/core/proto/validation_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/testing/__init__.py
+-rw-r--r--  2.0 unx     6706 b- defN 23-Apr-17 20:06 google/fhir/core/testing/protobuf_compare.py
+-rw-r--r--  2.0 unx     3745 b- defN 23-Apr-17 20:06 google/fhir/core/testing/testdata_utils.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/core/utils/__init__.py
+-rw-r--r--  2.0 unx    13789 b- defN 23-Apr-17 20:06 google/fhir/core/utils/annotation_utils.py
+-rw-r--r--  2.0 unx    15883 b- defN 23-Apr-17 20:06 google/fhir/core/utils/annotation_utils_test.py
+-rw-r--r--  2.0 unx    17494 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_package.py
+-rw-r--r--  2.0 unx    23767 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_package_test_base.py
+-rw-r--r--  2.0 unx     9127 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_types.py
+-rw-r--r--  2.0 unx     7750 b- defN 23-Apr-17 20:06 google/fhir/core/utils/fhir_types_test.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-Apr-17 20:06 google/fhir/core/utils/path_utils.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-Apr-17 20:06 google/fhir/core/utils/path_utils_test.py
+-rw-r--r--  2.0 unx    12011 b- defN 23-Apr-17 20:06 google/fhir/core/utils/proto_utils.py
+-rw-r--r--  2.0 unx    15754 b- defN 23-Apr-17 20:06 google/fhir/core/utils/proto_utils_test.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Apr-17 20:06 google/fhir/core/utils/resource_utils.py
+-rw-r--r--  2.0 unx     3789 b- defN 23-Apr-17 20:06 google/fhir/core/utils/resource_utils_test.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-Apr-17 20:06 google/fhir/core/utils/url_utils.py
+-rw-r--r--  2.0 unx     1870 b- defN 23-Apr-17 20:06 google/fhir/core/utils/url_utils_test.py
+-rwxr-xr-x  2.0 unx     7697 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/annotations.proto
+-rw-r--r--  2.0 unx     1576 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto
+-rw-r--r--  2.0 unx     4935 b- defN 23-Apr-17 20:06 google_fhir_core-0.9.2.data/data/validation.proto
+-rw-r--r--  2.0 unx     1311 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9443 b- defN 23-Apr-17 20:07 google_fhir_core-0.9.2.dist-info/RECORD
+93 files, 1504118 bytes uncompressed, 308107 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -1,256 +1,7 @@
-Filename: build/lib/google/fhir/core/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/codes.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/extensions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/extensions_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_errors.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_errors_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/references.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/FhirPathLexer.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/FhirPathParser.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/FhirPathVisitor.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_ast.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_ast_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_bigquery_interpreter.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_bigquery_sql_functions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_evaluation.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_fhir_path_data_types.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_fhir_path_to_sql_functions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_interpreter_test_base.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_navigation.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_navigation_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_python_interpreter.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_semant.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_semant_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_spark_interpreter.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_spark_sql_functions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_sql_data_types.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_sql_data_types_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_structure_definitions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/_utils_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/context.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/context_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/expressions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_options.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_spark_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_test_base.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/fhir_path_validator_v2_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/python_compiled_expressions.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/quantity.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/fhir_path/quantity_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/_primitive_time_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/primitive_handler.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/resource_validation.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/_json_parser.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/_json_printer.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/json_format_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_base64_binary.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_date.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_date_time.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_decimal.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_instant.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_primitive_wrappers.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/internal/json_format/wrappers/_time.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/proto/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/proto/annotations_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/proto/fhirpath_replacement_list_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/proto/validation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/testing/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/testing/protobuf_compare.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/testing/testdata_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/annotation_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/annotation_utils_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/fhir_package.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/fhir_package_test_base.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/fhir_types.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/fhir_types_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/path_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/path_utils_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/proto_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/proto_utils_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/resource_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/resource_utils_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/url_utils.py
-Comment: 
-
-Filename: build/lib/google/fhir/core/utils/url_utils_test.py
-Comment: 
-
 Filename: google/fhir/core/__init__.py
 Comment: 
 
 Filename: google/fhir/core/codes.py
 Comment: 
 
 Filename: google/fhir/core/extensions.py
@@ -501,29 +252,29 @@
 
 Filename: google/fhir/core/utils/url_utils.py
 Comment: 
 
 Filename: google/fhir/core/utils/url_utils_test.py
 Comment: 
 
-Filename: google_fhir_core-0.9.1.data/data/annotations.proto
+Filename: google_fhir_core-0.9.2.data/data/annotations.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.1.data/data/fhirpath_replacement_list.proto
+Filename: google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.1.data/data/validation.proto
+Filename: google_fhir_core-0.9.2.data/data/validation.proto
 Comment: 
 
-Filename: google_fhir_core-0.9.1.dist-info/METADATA
+Filename: google_fhir_core-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: google_fhir_core-0.9.1.dist-info/WHEEL
+Filename: google_fhir_core-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: google_fhir_core-0.9.1.dist-info/top_level.txt
+Filename: google_fhir_core-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: google_fhir_core-0.9.1.dist-info/RECORD
+Filename: google_fhir_core-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## google/fhir/core/fhir_path/_evaluation.py

```diff
@@ -429,15 +429,14 @@
 
   def __init__(
       self,
       fhir_context: context.FhirPathContext,
       identifier: str,
       parent_node: ExpressionNode,
   ) -> None:
-    """Prefer calling the `new` classmethod over __init__."""
     self._identifier = identifier
     self._parent_node = parent_node
     return_type = None
     if self._identifier == '$this':
       return_type = self._parent_node.return_type()
     else:
       return_type = fhir_context.get_child_data_type(
```

## Comparing `google_fhir_core-0.9.1.data/data/annotations.proto` & `google_fhir_core-0.9.2.data/data/annotations.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.1.data/data/fhirpath_replacement_list.proto` & `google_fhir_core-0.9.2.data/data/fhirpath_replacement_list.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.1.data/data/validation.proto` & `google_fhir_core-0.9.2.data/data/validation.proto`

 * *Files identical despite different names*

## Comparing `google_fhir_core-0.9.1.dist-info/METADATA` & `google_fhir_core-0.9.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: google-fhir-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Core components for working with FHIR.
 Home-page: https://github.com/google/fhir-py
 Download-URL: https://github.com/google-py/fhir/releases
 Author: Google LLC
 Author-email: google-fhir-pypi@google.com
 License: Apache 2.0
 Keywords: google,fhir,python,healthcare
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py (~=1.1)
 Requires-Dist: antlr4-python3-runtime (~=4.9.3)
 Requires-Dist: immutabledict (~=2.2)
 Requires-Dist: protobuf (~=3.19)
 Requires-Dist: python-dateutil (~=2.8)
 Requires-Dist: backports.zoneinfo (~=0.2.1) ; python_version < "3.9"
```

