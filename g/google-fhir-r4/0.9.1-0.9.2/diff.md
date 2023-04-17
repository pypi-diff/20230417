# Comparing `tmp/google_fhir_r4-0.9.1-py3-none-any.whl.zip` & `tmp/google_fhir_r4-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,363 +1,185 @@
-Zip file size: 6192478 bytes, number of entries: 361
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/__init__.py
--rw-r-----  2.0 unx     2568 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/fhir_path.py
--rw-r-----  2.0 unx     8224 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/json_format.py
--rw-r-----  2.0 unx     8526 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/primitive_handler.py
--rw-r-----  2.0 unx     2262 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/r4_package.py
--rw-r-----  2.0 unx     1045 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/resource_validation.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/proto/__init__.py
--rw-r-----  2.0 unx     4145 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
--rw-r-----  2.0 unx     6354 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/fhirproto_pb2.py
--rw-r-----  2.0 unx     8181 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/google_extensions_pb2.py
--rw-r-----  2.0 unx     5430 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
--rw-r-----  2.0 unx     3609 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
--rw-r-----  2.0 unx  1363080 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
--rw-r-----  2.0 unx   490992 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/uscore_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/proto/core/__init__.py
--rw-r-----  2.0 unx   481645 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/codes_pb2.py
--rw-r-----  2.0 unx   192704 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
--rw-r-----  2.0 unx   430564 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/extensions_pb2.py
--rw-r-----  2.0 unx   256371 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/proto/core/resources/__init__.py
--rw-r-----  2.0 unx     8207 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
--rw-r-----  2.0 unx    20009 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
--rw-r-----  2.0 unx    12409 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
--rw-r-----  2.0 unx    20459 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
--rw-r-----  2.0 unx    13544 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
--rw-r-----  2.0 unx     6800 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
--rw-r-----  2.0 unx    15947 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
--rw-r-----  2.0 unx     4453 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
--rw-r-----  2.0 unx     3381 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
--rw-r-----  2.0 unx    12077 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
--rw-r-----  2.0 unx     4000 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
--rw-r-----  2.0 unx    57948 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
--rw-r-----  2.0 unx    52078 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
--rw-r-----  2.0 unx    26499 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
--rw-r-----  2.0 unx    13460 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
--rw-r-----  2.0 unx     7681 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
--rw-r-----  2.0 unx    12070 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
--rw-r-----  2.0 unx    14188 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
--rw-r-----  2.0 unx    32406 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
--rw-r-----  2.0 unx    28636 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
--rw-r-----  2.0 unx    15685 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
--rw-r-----  2.0 unx    31726 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
--rw-r-----  2.0 unx    13084 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
--rw-r-----  2.0 unx    14646 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
--rw-r-----  2.0 unx    21926 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
--rw-r-----  2.0 unx    24927 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
--rw-r-----  2.0 unx    30618 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
--rw-r-----  2.0 unx    18941 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
--rw-r-----  2.0 unx    22205 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
--rw-r-----  2.0 unx    40639 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
--rw-r-----  2.0 unx    15086 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
--rw-r-----  2.0 unx    16937 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
--rw-r-----  2.0 unx    10797 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
--rw-r-----  2.0 unx    13803 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
--rw-r-----  2.0 unx    12389 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
--rw-r-----  2.0 unx     9691 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
--rw-r-----  2.0 unx    13617 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
--rw-r-----  2.0 unx    21906 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
--rw-r-----  2.0 unx    11028 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
--rw-r-----  2.0 unx    18783 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
--rw-r-----  2.0 unx    13747 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
--rw-r-----  2.0 unx    21174 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
--rw-r-----  2.0 unx     2668 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
--rw-r-----  2.0 unx    16416 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
--rw-r-----  2.0 unx    24578 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
--rw-r-----  2.0 unx     6808 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
--rw-r-----  2.0 unx     5661 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
--rw-r-----  2.0 unx     6272 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
--rw-r-----  2.0 unx    15586 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
--rw-r-----  2.0 unx    10854 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
--rw-r-----  2.0 unx    10239 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
--rw-r-----  2.0 unx    15011 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
--rw-r-----  2.0 unx    17163 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
--rw-r-----  2.0 unx    51948 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
--rw-r-----  2.0 unx    17644 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
--rw-r-----  2.0 unx    10517 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
--rw-r-----  2.0 unx    14696 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
--rw-r-----  2.0 unx    27335 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
--rw-r-----  2.0 unx     9644 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
--rw-r-----  2.0 unx     8195 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
--rw-r-----  2.0 unx    10292 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
--rw-r-----  2.0 unx    19394 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
--rw-r-----  2.0 unx     8356 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
--rw-r-----  2.0 unx    20660 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
--rw-r-----  2.0 unx    10630 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
--rw-r-----  2.0 unx    40492 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
--rw-r-----  2.0 unx    15742 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
--rw-r-----  2.0 unx    11997 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
--rw-r-----  2.0 unx    10737 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
--rw-r-----  2.0 unx     5474 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
--rw-r-----  2.0 unx    15879 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
--rw-r-----  2.0 unx    10784 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
--rw-r-----  2.0 unx    15256 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
--rw-r-----  2.0 unx    13798 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
--rw-r-----  2.0 unx     9603 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
--rw-r-----  2.0 unx    20081 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
--rw-r-----  2.0 unx    20813 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
--rw-r-----  2.0 unx    25122 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
--rw-r-----  2.0 unx     8655 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
--rw-r-----  2.0 unx    25736 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
--rw-r-----  2.0 unx    16838 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
--rw-r-----  2.0 unx     8121 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
--rw-r-----  2.0 unx     6396 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
--rw-r-----  2.0 unx     6399 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
--rw-r-----  2.0 unx     8172 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
--rw-r-----  2.0 unx     5575 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
--rw-r-----  2.0 unx     4252 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
--rw-r-----  2.0 unx     8256 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
--rw-r-----  2.0 unx    12806 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
--rw-r-----  2.0 unx     9456 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
--rw-r-----  2.0 unx     3655 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
--rw-r-----  2.0 unx    27083 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
--rw-r-----  2.0 unx    12434 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
--rw-r-----  2.0 unx     4736 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
--rw-r-----  2.0 unx    20413 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
--rw-r-----  2.0 unx    22452 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
--rw-r-----  2.0 unx    19470 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
--rw-r-----  2.0 unx     9643 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
--rw-r-----  2.0 unx    30284 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
--rw-r-----  2.0 unx    33371 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
--rw-r-----  2.0 unx     5813 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
--rw-r-----  2.0 unx     7402 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
--rw-r-----  2.0 unx     6931 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
--rw-r-----  2.0 unx     7778 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
--rw-r-----  2.0 unx    16878 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
--rw-r-----  2.0 unx     7546 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
--rw-r-----  2.0 unx    12640 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
--rw-r-----  2.0 unx    11234 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
--rw-r-----  2.0 unx    29886 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
--rw-r-----  2.0 unx    10079 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
--rw-r-----  2.0 unx    10255 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
--rw-r-----  2.0 unx    21341 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
--rw-r-----  2.0 unx     9745 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
--rw-r-----  2.0 unx    23215 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
--rw-r-----  2.0 unx    11758 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
--rw-r-----  2.0 unx    10112 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
--rw-r-----  2.0 unx    23693 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
--rw-r-----  2.0 unx    12354 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
--rw-r-----  2.0 unx    20107 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
--rw-r-----  2.0 unx    10004 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
--rw-r-----  2.0 unx     5870 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
--rw-r-----  2.0 unx     3335 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
--rw-r-----  2.0 unx    17088 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
--rw-r-----  2.0 unx    13588 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
--rw-r-----  2.0 unx     4777 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
--rw-r-----  2.0 unx    28042 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
--rw-r-----  2.0 unx    22943 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
--rw-r-----  2.0 unx     5952 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
--rw-r-----  2.0 unx    10042 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
--rw-r-----  2.0 unx    12144 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
--rw-r-----  2.0 unx    37026 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
--rw-r-----  2.0 unx    41607 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
--rw-r-----  2.0 unx     8013 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
--rw-r-----  2.0 unx     5348 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
--rw-r-----  2.0 unx     7494 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
--rw-r-----  2.0 unx     7301 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
--rw-r-----  2.0 unx     3919 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
--rw-r-----  2.0 unx     7891 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
--rw-r-----  2.0 unx     8179 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
--rw-r-----  2.0 unx    19386 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
--rw-r-----  2.0 unx    13065 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
--rw-r-----  2.0 unx    13766 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
--rw-r-----  2.0 unx    24739 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
--rw-r-----  2.0 unx    31441 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
--rw-r-----  2.0 unx    16193 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
--rw-r-----  2.0 unx    39144 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
--rw-r-----  2.0 unx    31172 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
--rw-r-----  2.0 unx     9345 b- defN 23-Apr-04 16:21 build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
--rw-r-----  2.0 unx    16474 b- defN 23-Apr-04 16:22 build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/__init__.py
--rw-r-----  2.0 unx     8965 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
--rw-r-----  2.0 unx    10349 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
--rw-r-----  2.0 unx    12355 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/terminology_service_client.py
--rw-r-----  2.0 unx     9061 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
--rw-r-----  2.0 unx     7948 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/value_set_tables.py
--rw-r-----  2.0 unx     8259 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/value_set_tables_test.py
--rw-r-----  2.0 unx    10248 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/value_sets.py
--rw-r-----  2.0 unx    14084 b- defN 23-Apr-04 16:12 build/lib/google/fhir/r4/terminology/value_sets_test.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/r4/__init__.py
--rw-r-----  2.0 unx     2568 b- defN 23-Apr-04 16:12 google/fhir/r4/fhir_path.py
--rw-r-----  2.0 unx     8224 b- defN 23-Apr-04 16:12 google/fhir/r4/json_format.py
--rw-r-----  2.0 unx     8526 b- defN 23-Apr-04 16:12 google/fhir/r4/primitive_handler.py
--rw-r-----  2.0 unx     2262 b- defN 23-Apr-04 16:12 google/fhir/r4/r4_package.py
--rw-r-----  2.0 unx     1045 b- defN 23-Apr-04 16:12 google/fhir/r4/resource_validation.py
--rw-r-----  2.0 unx  4531911 b- defN 23-Apr-04 16:22 google/fhir/r4/data/hl7.fhir.r4.core.tgz
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/r4/proto/__init__.py
--rw-r-----  2.0 unx     4145 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/fhirproto_extensions_pb2.py
--rw-r-----  2.0 unx     6354 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/fhirproto_pb2.py
--rw-r-----  2.0 unx     8181 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/google_extensions_pb2.py
--rw-r-----  2.0 unx     5430 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/ml_extensions_pb2.py
--rw-r-----  2.0 unx     3609 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/primitive_test_suite_pb2.py
--rw-r-----  2.0 unx  1363080 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/uscore_codes_pb2.py
--rw-r-----  2.0 unx   490992 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/uscore_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/r4/proto/core/__init__.py
--rw-r-----  2.0 unx   481645 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/codes_pb2.py
--rw-r-----  2.0 unx   192704 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/datatypes_pb2.py
--rw-r-----  2.0 unx   430564 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/extensions_pb2.py
--rw-r-----  2.0 unx   256371 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/valuesets_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/r4/proto/core/resources/__init__.py
--rw-r-----  2.0 unx     8207 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/account_pb2.py
--rw-r-----  2.0 unx    20009 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/activity_definition_pb2.py
--rw-r-----  2.0 unx    12409 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/adverse_event_pb2.py
--rw-r-----  2.0 unx    20459 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
--rw-r-----  2.0 unx    13544 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/appointment_pb2.py
--rw-r-----  2.0 unx     6800 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/appointment_response_pb2.py
--rw-r-----  2.0 unx    15947 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/audit_event_pb2.py
--rw-r-----  2.0 unx     4453 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/basic_pb2.py
--rw-r-----  2.0 unx     3381 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/binary_pb2.py
--rw-r-----  2.0 unx    12077 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
--rw-r-----  2.0 unx     4000 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/body_structure_pb2.py
--rw-r-----  2.0 unx    57948 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
--rw-r-----  2.0 unx    52078 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/capability_statement_pb2.py
--rw-r-----  2.0 unx    26499 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/care_plan_pb2.py
--rw-r-----  2.0 unx    13460 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/care_team_pb2.py
--rw-r-----  2.0 unx     7681 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
--rw-r-----  2.0 unx    12070 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
--rw-r-----  2.0 unx    14188 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/charge_item_pb2.py
--rw-r-----  2.0 unx    32406 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/claim_pb2.py
--rw-r-----  2.0 unx    28636 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/claim_response_pb2.py
--rw-r-----  2.0 unx    15685 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
--rw-r-----  2.0 unx    31726 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/code_system_pb2.py
--rw-r-----  2.0 unx    13084 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/communication_pb2.py
--rw-r-----  2.0 unx    14646 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/communication_request_pb2.py
--rw-r-----  2.0 unx    21926 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
--rw-r-----  2.0 unx    24927 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/composition_pb2.py
--rw-r-----  2.0 unx    30618 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/concept_map_pb2.py
--rw-r-----  2.0 unx    18941 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/condition_pb2.py
--rw-r-----  2.0 unx    22205 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/consent_pb2.py
--rw-r-----  2.0 unx    40639 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/contract_pb2.py
--rw-r-----  2.0 unx    15086 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
--rw-r-----  2.0 unx    16937 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
--rw-r-----  2.0 unx    10797 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/coverage_pb2.py
--rw-r-----  2.0 unx    13803 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/detected_issue_pb2.py
--rw-r-----  2.0 unx    12389 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/device_definition_pb2.py
--rw-r-----  2.0 unx     9691 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/device_metric_pb2.py
--rw-r-----  2.0 unx    13617 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/device_pb2.py
--rw-r-----  2.0 unx    21906 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/device_request_pb2.py
--rw-r-----  2.0 unx    11028 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
--rw-r-----  2.0 unx    18783 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
--rw-r-----  2.0 unx    13747 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/document_manifest_pb2.py
--rw-r-----  2.0 unx    21174 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/document_reference_pb2.py
--rw-r-----  2.0 unx     2668 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/domain_resource_pb2.py
--rw-r-----  2.0 unx    16416 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
--rw-r-----  2.0 unx    24578 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/encounter_pb2.py
--rw-r-----  2.0 unx     6808 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/endpoint_pb2.py
--rw-r-----  2.0 unx     5661 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
--rw-r-----  2.0 unx     6272 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
--rw-r-----  2.0 unx    15586 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
--rw-r-----  2.0 unx    10854 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/event_definition_pb2.py
--rw-r-----  2.0 unx    10239 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/evidence_pb2.py
--rw-r-----  2.0 unx    15011 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
--rw-r-----  2.0 unx    17163 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/example_scenario_pb2.py
--rw-r-----  2.0 unx    51948 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
--rw-r-----  2.0 unx    17644 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/family_member_history_pb2.py
--rw-r-----  2.0 unx    10517 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/flag_pb2.py
--rw-r-----  2.0 unx    14696 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/goal_pb2.py
--rw-r-----  2.0 unx    27335 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/graph_definition_pb2.py
--rw-r-----  2.0 unx     9644 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/group_pb2.py
--rw-r-----  2.0 unx     8195 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/guidance_response_pb2.py
--rw-r-----  2.0 unx    10292 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
--rw-r-----  2.0 unx    19394 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/imaging_study_pb2.py
--rw-r-----  2.0 unx     8356 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
--rw-r-----  2.0 unx    20660 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/immunization_pb2.py
--rw-r-----  2.0 unx    10630 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
--rw-r-----  2.0 unx    40492 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
--rw-r-----  2.0 unx    15742 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
--rw-r-----  2.0 unx    11997 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/invoice_pb2.py
--rw-r-----  2.0 unx    10737 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/library_pb2.py
--rw-r-----  2.0 unx     5474 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/linkage_pb2.py
--rw-r-----  2.0 unx    15879 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/list_pb2.py
--rw-r-----  2.0 unx    10784 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/location_pb2.py
--rw-r-----  2.0 unx    15256 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/measure_pb2.py
--rw-r-----  2.0 unx    13798 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/measure_report_pb2.py
--rw-r-----  2.0 unx     9603 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/media_pb2.py
--rw-r-----  2.0 unx    20081 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medication_administration_pb2.py
--rw-r-----  2.0 unx    20813 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
--rw-r-----  2.0 unx    25122 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
--rw-r-----  2.0 unx     8655 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medication_pb2.py
--rw-r-----  2.0 unx    25736 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medication_request_pb2.py
--rw-r-----  2.0 unx    16838 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medication_statement_pb2.py
--rw-r-----  2.0 unx     8121 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
--rw-r-----  2.0 unx     6396 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
--rw-r-----  2.0 unx     6399 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
--rw-r-----  2.0 unx     8172 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
--rw-r-----  2.0 unx     5575 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
--rw-r-----  2.0 unx     4252 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
--rw-r-----  2.0 unx     8256 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
--rw-r-----  2.0 unx    12806 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
--rw-r-----  2.0 unx     9456 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
--rw-r-----  2.0 unx     3655 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
--rw-r-----  2.0 unx    27083 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/message_definition_pb2.py
--rw-r-----  2.0 unx    12434 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/message_header_pb2.py
--rw-r-----  2.0 unx     4736 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
--rw-r-----  2.0 unx    20413 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
--rw-r-----  2.0 unx    22452 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/naming_system_pb2.py
--rw-r-----  2.0 unx    19470 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
--rw-r-----  2.0 unx     9643 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/observation_definition_pb2.py
--rw-r-----  2.0 unx    30284 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/observation_pb2.py
--rw-r-----  2.0 unx    33371 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/operation_definition_pb2.py
--rw-r-----  2.0 unx     5813 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
--rw-r-----  2.0 unx     7402 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
--rw-r-----  2.0 unx     6931 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/organization_pb2.py
--rw-r-----  2.0 unx     7778 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/parameters_pb2.py
--rw-r-----  2.0 unx    16878 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/patient_pb2.py
--rw-r-----  2.0 unx     7546 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/payment_notice_pb2.py
--rw-r-----  2.0 unx    12640 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
--rw-r-----  2.0 unx    11234 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/person_pb2.py
--rw-r-----  2.0 unx    29886 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/plan_definition_pb2.py
--rw-r-----  2.0 unx    10079 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/practitioner_pb2.py
--rw-r-----  2.0 unx    10255 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
--rw-r-----  2.0 unx    21341 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/procedure_pb2.py
--rw-r-----  2.0 unx     9745 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/provenance_pb2.py
--rw-r-----  2.0 unx    23215 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/questionnaire_pb2.py
--rw-r-----  2.0 unx    11758 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
--rw-r-----  2.0 unx    10112 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/related_person_pb2.py
--rw-r-----  2.0 unx    23693 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/request_group_pb2.py
--rw-r-----  2.0 unx    12354 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/research_definition_pb2.py
--rw-r-----  2.0 unx    20107 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
--rw-r-----  2.0 unx    10004 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/research_study_pb2.py
--rw-r-----  2.0 unx     5870 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/research_subject_pb2.py
--rw-r-----  2.0 unx     3335 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/resource_pb2.py
--rw-r-----  2.0 unx    17088 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
--rw-r-----  2.0 unx    13588 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
--rw-r-----  2.0 unx     4777 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/schedule_pb2.py
--rw-r-----  2.0 unx    28042 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/search_parameter_pb2.py
--rw-r-----  2.0 unx    22943 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/service_request_pb2.py
--rw-r-----  2.0 unx     5952 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/slot_pb2.py
--rw-r-----  2.0 unx    10042 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
--rw-r-----  2.0 unx    12144 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/specimen_pb2.py
--rw-r-----  2.0 unx    37026 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/structure_definition_pb2.py
--rw-r-----  2.0 unx    41607 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/structure_map_pb2.py
--rw-r-----  2.0 unx     8013 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/subscription_pb2.py
--rw-r-----  2.0 unx     5348 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
--rw-r-----  2.0 unx     7494 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/substance_pb2.py
--rw-r-----  2.0 unx     7301 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
--rw-r-----  2.0 unx     3919 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/substance_protein_pb2.py
--rw-r-----  2.0 unx     7891 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
--rw-r-----  2.0 unx     8179 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
--rw-r-----  2.0 unx    19386 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/substance_specification_pb2.py
--rw-r-----  2.0 unx    13065 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
--rw-r-----  2.0 unx    13766 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/supply_request_pb2.py
--rw-r-----  2.0 unx    24739 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/task_pb2.py
--rw-r-----  2.0 unx    31441 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
--rw-r-----  2.0 unx    16193 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/test_report_pb2.py
--rw-r-----  2.0 unx    39144 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/test_script_pb2.py
--rw-r-----  2.0 unx    31172 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/value_set_pb2.py
--rw-r-----  2.0 unx     9345 b- defN 23-Apr-04 16:21 google/fhir/r4/proto/core/resources/verification_result_pb2.py
--rw-r-----  2.0 unx    16474 b- defN 23-Apr-04 16:22 google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
--rw-r-----  2.0 unx      577 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/__init__.py
--rw-r-----  2.0 unx     8965 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/local_value_set_resolver.py
--rw-r-----  2.0 unx    10349 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/local_value_set_resolver_test.py
--rw-r-----  2.0 unx    12355 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/terminology_service_client.py
--rw-r-----  2.0 unx     9061 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/terminology_service_client_test.py
--rw-r-----  2.0 unx     7948 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/value_set_tables.py
--rw-r-----  2.0 unx     8259 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/value_set_tables_test.py
--rw-r-----  2.0 unx    10248 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/value_sets.py
--rw-r-----  2.0 unx    14084 b- defN 23-Apr-04 16:12 google/fhir/r4/terminology/value_sets_test.py
--rw-r-----  2.0 unx     1100 b- defN 23-Apr-04 17:13 google_fhir_r4-0.9.1.dist-info/METADATA
--rw-r-----  2.0 unx       92 b- defN 23-Apr-04 17:13 google_fhir_r4-0.9.1.dist-info/WHEEL
--rw-r-----  2.0 unx       13 b- defN 23-Apr-04 17:13 google_fhir_r4-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    42662 b- defN 23-Apr-04 17:13 google_fhir_r4-0.9.1.dist-info/RECORD
-361 files, 16023906 bytes uncompressed, 6121200 bytes compressed:  61.8%
+Zip file size: 5360934 bytes, number of entries: 183
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Apr-17 20:06 google/fhir/r4/fhir_path.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-Apr-17 20:06 google/fhir/r4/json_format.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-Apr-17 20:06 google/fhir/r4/primitive_handler.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-Apr-17 20:06 google/fhir/r4/r4_package.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-Apr-17 20:06 google/fhir/r4/resource_validation.py
+-rw-r--r--  2.0 unx  4531911 b- defN 23-Apr-17 20:07 google/fhir/r4/data/hl7.fhir.r4.core.tgz
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/__init__.py
+-rw-r--r--  2.0 unx     4145 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/fhirproto_extensions_pb2.py
+-rw-r--r--  2.0 unx     6354 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/fhirproto_pb2.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/google_extensions_pb2.py
+-rw-r--r--  2.0 unx     5430 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/ml_extensions_pb2.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/primitive_test_suite_pb2.py
+-rw-r--r--  2.0 unx  1363080 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/uscore_codes_pb2.py
+-rw-r--r--  2.0 unx   490992 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/uscore_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/core/__init__.py
+-rw-r--r--  2.0 unx   481645 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/codes_pb2.py
+-rw-r--r--  2.0 unx   192704 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/datatypes_pb2.py
+-rw-r--r--  2.0 unx   430564 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/extensions_pb2.py
+-rw-r--r--  2.0 unx   256371 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/valuesets_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/core/resources/__init__.py
+-rw-r--r--  2.0 unx     8207 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/account_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+-rw-r--r--  2.0 unx    12409 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+-rw-r--r--  2.0 unx    20459 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+-rw-r--r--  2.0 unx    13544 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/appointment_pb2.py
+-rw-r--r--  2.0 unx     6800 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/audit_event_pb2.py
+-rw-r--r--  2.0 unx     4453 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/basic_pb2.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/binary_pb2.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/body_structure_pb2.py
+-rw-r--r--  2.0 unx    57948 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+-rw-r--r--  2.0 unx    52078 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+-rw-r--r--  2.0 unx    26499 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/care_plan_pb2.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/care_team_pb2.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+-rw-r--r--  2.0 unx    12070 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/charge_item_pb2.py
+-rw-r--r--  2.0 unx    32406 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/claim_pb2.py
+-rw-r--r--  2.0 unx    28636 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/claim_response_pb2.py
+-rw-r--r--  2.0 unx    15685 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+-rw-r--r--  2.0 unx    31726 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/code_system_pb2.py
+-rw-r--r--  2.0 unx    13084 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/communication_pb2.py
+-rw-r--r--  2.0 unx    14646 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/communication_request_pb2.py
+-rw-r--r--  2.0 unx    21926 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/composition_pb2.py
+-rw-r--r--  2.0 unx    30618 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/concept_map_pb2.py
+-rw-r--r--  2.0 unx    18941 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/condition_pb2.py
+-rw-r--r--  2.0 unx    22205 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/consent_pb2.py
+-rw-r--r--  2.0 unx    40639 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/contract_pb2.py
+-rw-r--r--  2.0 unx    15086 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+-rw-r--r--  2.0 unx    16937 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_pb2.py
+-rw-r--r--  2.0 unx    13803 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+-rw-r--r--  2.0 unx    12389 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_definition_pb2.py
+-rw-r--r--  2.0 unx     9691 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_metric_pb2.py
+-rw-r--r--  2.0 unx    13617 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_pb2.py
+-rw-r--r--  2.0 unx    21906 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_request_pb2.py
+-rw-r--r--  2.0 unx    11028 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+-rw-r--r--  2.0 unx    18783 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+-rw-r--r--  2.0 unx    13747 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+-rw-r--r--  2.0 unx    21174 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/document_reference_pb2.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+-rw-r--r--  2.0 unx    16416 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx    24578 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/encounter_pb2.py
+-rw-r--r--  2.0 unx     6808 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/endpoint_pb2.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+-rw-r--r--  2.0 unx    15586 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+-rw-r--r--  2.0 unx    10854 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/event_definition_pb2.py
+-rw-r--r--  2.0 unx    10239 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/evidence_pb2.py
+-rw-r--r--  2.0 unx    15011 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+-rw-r--r--  2.0 unx    17163 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+-rw-r--r--  2.0 unx    51948 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+-rw-r--r--  2.0 unx    10517 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/flag_pb2.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/goal_pb2.py
+-rw-r--r--  2.0 unx    27335 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+-rw-r--r--  2.0 unx     9644 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/group_pb2.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+-rw-r--r--  2.0 unx    10292 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+-rw-r--r--  2.0 unx    19394 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+-rw-r--r--  2.0 unx     8356 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+-rw-r--r--  2.0 unx    20660 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_pb2.py
+-rw-r--r--  2.0 unx    10630 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+-rw-r--r--  2.0 unx    40492 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+-rw-r--r--  2.0 unx    15742 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+-rw-r--r--  2.0 unx    11997 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/invoice_pb2.py
+-rw-r--r--  2.0 unx    10737 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/library_pb2.py
+-rw-r--r--  2.0 unx     5474 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/linkage_pb2.py
+-rw-r--r--  2.0 unx    15879 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/list_pb2.py
+-rw-r--r--  2.0 unx    10784 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/location_pb2.py
+-rw-r--r--  2.0 unx    15256 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/measure_pb2.py
+-rw-r--r--  2.0 unx    13798 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/measure_report_pb2.py
+-rw-r--r--  2.0 unx     9603 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/media_pb2.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+-rw-r--r--  2.0 unx    20813 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+-rw-r--r--  2.0 unx    25122 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+-rw-r--r--  2.0 unx     8655 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_pb2.py
+-rw-r--r--  2.0 unx    25736 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_request_pb2.py
+-rw-r--r--  2.0 unx    16838 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+-rw-r--r--  2.0 unx     6399 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+-rw-r--r--  2.0 unx     5575 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+-rw-r--r--  2.0 unx     8256 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+-rw-r--r--  2.0 unx    12806 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+-rw-r--r--  2.0 unx     3655 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+-rw-r--r--  2.0 unx    27083 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/message_definition_pb2.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/message_header_pb2.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+-rw-r--r--  2.0 unx    20413 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+-rw-r--r--  2.0 unx    22452 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/naming_system_pb2.py
+-rw-r--r--  2.0 unx    19470 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+-rw-r--r--  2.0 unx    30284 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/observation_pb2.py
+-rw-r--r--  2.0 unx    33371 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+-rw-r--r--  2.0 unx     6931 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/organization_pb2.py
+-rw-r--r--  2.0 unx     7778 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/parameters_pb2.py
+-rw-r--r--  2.0 unx    16878 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/patient_pb2.py
+-rw-r--r--  2.0 unx     7546 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+-rw-r--r--  2.0 unx    12640 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/person_pb2.py
+-rw-r--r--  2.0 unx    29886 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/practitioner_pb2.py
+-rw-r--r--  2.0 unx    10255 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+-rw-r--r--  2.0 unx    21341 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/procedure_pb2.py
+-rw-r--r--  2.0 unx     9745 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/provenance_pb2.py
+-rw-r--r--  2.0 unx    23215 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+-rw-r--r--  2.0 unx    11758 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/related_person_pb2.py
+-rw-r--r--  2.0 unx    23693 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/request_group_pb2.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_definition_pb2.py
+-rw-r--r--  2.0 unx    20107 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_study_pb2.py
+-rw-r--r--  2.0 unx     5870 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_subject_pb2.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/resource_pb2.py
+-rw-r--r--  2.0 unx    17088 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+-rw-r--r--  2.0 unx    13588 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx     4777 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/schedule_pb2.py
+-rw-r--r--  2.0 unx    28042 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+-rw-r--r--  2.0 unx    22943 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/service_request_pb2.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/slot_pb2.py
+-rw-r--r--  2.0 unx    10042 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/specimen_pb2.py
+-rw-r--r--  2.0 unx    37026 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+-rw-r--r--  2.0 unx    41607 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/structure_map_pb2.py
+-rw-r--r--  2.0 unx     8013 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/subscription_pb2.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_pb2.py
+-rw-r--r--  2.0 unx     7301 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+-rw-r--r--  2.0 unx     7891 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+-rw-r--r--  2.0 unx     8179 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+-rw-r--r--  2.0 unx    19386 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+-rw-r--r--  2.0 unx    13065 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+-rw-r--r--  2.0 unx    13766 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/supply_request_pb2.py
+-rw-r--r--  2.0 unx    24739 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/task_pb2.py
+-rw-r--r--  2.0 unx    31441 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/test_report_pb2.py
+-rw-r--r--  2.0 unx    39144 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/test_script_pb2.py
+-rw-r--r--  2.0 unx    31172 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/value_set_pb2.py
+-rw-r--r--  2.0 unx     9345 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/verification_result_pb2.py
+-rw-r--r--  2.0 unx    16474 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/__init__.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/local_value_set_resolver.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/local_value_set_resolver_test.py
+-rw-r--r--  2.0 unx    12355 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/terminology_service_client.py
+-rw-r--r--  2.0 unx     9061 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/terminology_service_client_test.py
+-rw-r--r--  2.0 unx     7948 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_set_tables.py
+-rw-r--r--  2.0 unx     8259 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_set_tables_test.py
+-rw-r--r--  2.0 unx    10248 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_sets.py
+-rw-r--r--  2.0 unx    14084 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_sets_test.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    20653 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/RECORD
+183 files, 10277777 bytes uncompressed, 5326678 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -1,541 +1,7 @@
-Filename: build/lib/google/fhir/r4/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/fhir_path.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/json_format.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/primitive_handler.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/r4_package.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/resource_validation.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/fhirproto_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/google_extensions_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/uscore_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/codes_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/extensions_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/__init__.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/terminology_service_client.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/value_set_tables.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/value_set_tables_test.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/value_sets.py
-Comment: 
-
-Filename: build/lib/google/fhir/r4/terminology/value_sets_test.py
-Comment: 
-
 Filename: google/fhir/r4/__init__.py
 Comment: 
 
 Filename: google/fhir/r4/fhir_path.py
 Comment: 
 
 Filename: google/fhir/r4/json_format.py
@@ -1065,20 +531,20 @@
 
 Filename: google/fhir/r4/terminology/value_sets.py
 Comment: 
 
 Filename: google/fhir/r4/terminology/value_sets_test.py
 Comment: 
 
-Filename: google_fhir_r4-0.9.1.dist-info/METADATA
+Filename: google_fhir_r4-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: google_fhir_r4-0.9.1.dist-info/WHEEL
+Filename: google_fhir_r4-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: google_fhir_r4-0.9.1.dist-info/top_level.txt
+Filename: google_fhir_r4-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: google_fhir_r4-0.9.1.dist-info/RECORD
+Filename: google_fhir_r4-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `google_fhir_r4-0.9.1.dist-info/METADATA` & `google_fhir_r4-0.9.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: google-fhir-r4
-Version: 0.9.1
+Version: 0.9.2
 Summary: Components for working with FHIR R4.
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
-Requires-Dist: google-fhir-core (~=0.9.1)
+Requires-Dist: google-fhir-core (~=0.9.2)
 Requires-Dist: immutabledict (~=2.2)
 Requires-Dist: protobuf (~=3.19)
 Requires-Dist: python-dateutil (~=2.8)
 Requires-Dist: backports.zoneinfo (~=0.2.1) ; python_version < "3.9"
 
 Protocol buffer conversion and validation for with FHIR R4 resources.
```

