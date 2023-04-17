# Comparing `tmp/calcasa-api-1.2.0.tar.gz` & `tmp/calcasa-api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcasa-api-1.2.0.tar", last modified: Thu Aug  4 09:33:11 2022, max compression
+gzip compressed data, was "calcasa-api-1.2.1.tar", last modified: Mon Apr 17 10:45:27 2023, max compression
```

## Comparing `calcasa-api-1.2.0.tar` & `calcasa-api-1.2.1.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:11.302766 calcasa-api-1.2.0/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    28615 2022-08-04 09:33:11.308136 calcasa-api-1.2.0/PKG-INFO
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    24509 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/README.md
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:05.018614 calcasa-api-1.2.0/calcasa/
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:05.471529 calcasa-api-1.2.0/calcasa/api/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1252 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/__init__.py
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:06.287793 calcasa-api-1.2.0/calcasa/api/api/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)      216 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/api/__init__.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12217 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/adressen_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7163 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/bestemmingsplannen_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7084 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/bodem_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6854 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/buurt_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    22859 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/callbacks_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11733 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/configuratie_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6554 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/facturen_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6619 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/fotos_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7131 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/api/funderingen_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6907 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/api/geldverstrekkers_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6552 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/api/rapporten_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    28996 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/api/waarderingen_api.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    39577 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/api_client.py
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:06.350182 calcasa-api-1.2.0/calcasa/api/apis/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1106 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/apis/__init__.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17243 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/configuration.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     5608 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/exceptions.py
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:11.049079 calcasa-api-1.2.0/calcasa/api/model/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)      345 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/model/__init__.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15103 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/aanvraagdoel.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13075 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/adres.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13066 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/adres_info.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15501 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/adres_info_adres.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    19109 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/adres_info_notities.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12257 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/bestemmingsdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14422 2022-08-04 09:32:22.000000 calcasa-api-1.2.0/calcasa/api/model/bodem_status_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13611 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/bodemdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18498 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/business_rules_code.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13508 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/business_rules_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12490 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/callback.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12750 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/callback_inschrijving.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12584 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/cbs_indeling.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13681 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/energielabel.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11955 2022-08-04 09:32:23.000000 calcasa-api-1.2.0/calcasa/api/model/factuur.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11647 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/foto.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13124 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_data_bron.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14209 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_herstel_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13363 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_risico.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13485 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_risico_label.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13597 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_soort_bron.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18400 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14755 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/fundering_typering.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15264 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/funderingdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15816 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/funderingdata_bio_infectie_risico.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15813 2022-08-04 09:32:24.000000 calcasa-api-1.2.0/calcasa/api/model/funderingdata_droogstand_risico.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15828 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/funderingdata_optrekkend_vocht_risico.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17185 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/funderingdata_typering.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15008 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/gebiedsdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12152 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/geldverstrekker.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15292 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/http_validation_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13141 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/invalid_argument_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12512 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/json_patch_document.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13462 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/klantwaarde_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11883 2022-08-04 09:32:25.000000 calcasa-api-1.2.0/calcasa/api/model/kwartaal.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13159 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/modeldata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13101 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/not_found_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13822 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/notitie.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16711 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/notities.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15101 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/objectdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13370 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17457 2022-08-04 09:32:26.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_buurt.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17466 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_gemeente.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17454 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_land.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17469 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_provincie.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17454 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_wijk.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12860 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/operation.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13368 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/operation_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13192 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/permissions_denied_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12856 2022-08-04 09:32:27.000000 calcasa-api-1.2.0/calcasa/api/model/problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15300 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/product_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11662 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/rapport.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16139 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/referentieobject.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15522 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/referentieobject_adres.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15062 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/referentieobject_cbs_indeling.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17519 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/referentieobject_object.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13138 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/resource_exhausted_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13627 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/taxatiedata.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13624 2022-08-04 09:32:28.000000 calcasa-api-1.2.0/calcasa/api/model/taxatiestatus.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13110 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/validation_problem_details.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16768 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/verkoop_bijzonderheden.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13903 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/vorige_verkoop.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18178 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/waardering.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15043 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_cbs_indeling.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14393 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_factuur.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    23276 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_input_parameters.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15595 2022-08-04 09:32:29.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_model.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17500 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_object.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16408 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12306 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling_kwartaal.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14387 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling_kwartaal_kwartaal.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    25416 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_originele_input.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14100 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_rapport.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15911 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_status.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16031 2022-08-04 09:32:30.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_taxatie.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16866 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_webhook_payload.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15507 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/model/waardering_zoek_parameters.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15371 2022-08-04 09:32:31.000000 calcasa-api-1.2.0/calcasa/api/model/woning_type.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    83107 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/model_utils.py
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:11.098102 calcasa-api-1.2.0/calcasa/api/models/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     5652 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/models/__init__.py
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14809 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/calcasa/api/rest.py
-drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2022-08-04 09:33:11.267572 calcasa-api-1.2.0/calcasa_api.egg-info/
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)    28615 2022-08-04 09:33:03.000000 calcasa-api-1.2.0/calcasa_api.egg-info/PKG-INFO
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     4031 2022-08-04 09:33:04.000000 calcasa-api-1.2.0/calcasa_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)        1 2022-08-04 09:33:03.000000 calcasa-api-1.2.0/calcasa_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       32 2022-08-04 09:33:03.000000 calcasa-api-1.2.0/calcasa_api.egg-info/requires.txt
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)        8 2022-08-04 09:33:03.000000 calcasa-api-1.2.0/calcasa_api.egg-info/top_level.txt
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)       69 2022-08-04 09:33:11.318134 calcasa-api-1.2.0/setup.cfg
--rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1943 2022-08-04 09:32:32.000000 calcasa-api-1.2.0/setup.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:27.256003 calcasa-api-1.2.1/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11358 2021-11-26 15:44:52.000000 calcasa-api-1.2.1/LICENSE
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    25152 2023-04-17 10:45:27.259002 calcasa-api-1.2.1/PKG-INFO
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    24635 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/README.md
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:17.881936 calcasa-api-1.2.1/calcasa/
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:18.647152 calcasa-api-1.2.1/calcasa/api/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1252 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/__init__.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:20.180217 calcasa-api-1.2.1/calcasa/api/api/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)      216 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api/__init__.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12217 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/adressen_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7163 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/bestemmingsplannen_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7084 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/bodem_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6854 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/buurt_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    22859 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/callbacks_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11733 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/configuratie_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6554 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/facturen_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6619 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/api/fotos_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     7131 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api/funderingen_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6907 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api/geldverstrekkers_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     6552 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api/rapporten_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    28996 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api/waarderingen_api.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    39577 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/api_client.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:20.279241 calcasa-api-1.2.1/calcasa/api/apis/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1106 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/apis/__init__.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17243 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/configuration.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     5608 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/exceptions.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:26.745536 calcasa-api-1.2.1/calcasa/api/model/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)      345 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/model/__init__.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15103 2023-04-17 10:41:20.000000 calcasa-api-1.2.1/calcasa/api/model/aanvraagdoel.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13075 2023-04-17 10:41:20.000000 calcasa-api-1.2.1/calcasa/api/model/adres.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13066 2023-04-17 10:41:20.000000 calcasa-api-1.2.1/calcasa/api/model/adres_info.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15501 2023-04-17 10:41:20.000000 calcasa-api-1.2.1/calcasa/api/model/adres_info_adres.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    19109 2023-04-17 10:41:20.000000 calcasa-api-1.2.1/calcasa/api/model/adres_info_notities.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12257 2023-04-17 10:41:21.000000 calcasa-api-1.2.1/calcasa/api/model/bestemmingsdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14422 2023-04-17 10:41:21.000000 calcasa-api-1.2.1/calcasa/api/model/bodem_status_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13611 2023-04-17 10:41:21.000000 calcasa-api-1.2.1/calcasa/api/model/bodemdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18498 2023-04-17 10:41:21.000000 calcasa-api-1.2.1/calcasa/api/model/business_rules_code.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13508 2023-04-17 10:41:21.000000 calcasa-api-1.2.1/calcasa/api/model/business_rules_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12490 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/callback.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13262 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/callback_inschrijving.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12584 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/cbs_indeling.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13681 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/energielabel.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11955 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/factuur.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11647 2023-04-17 10:41:22.000000 calcasa-api-1.2.1/calcasa/api/model/foto.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13124 2023-04-17 10:41:23.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_data_bron.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14209 2023-04-17 10:41:23.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_herstel_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13363 2023-04-17 10:41:23.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_risico.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13485 2023-04-17 10:41:23.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_risico_label.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13597 2023-04-17 10:41:23.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_soort_bron.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18400 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14755 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/fundering_typering.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15264 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/funderingdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15816 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/funderingdata_bio_infectie_risico.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15813 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/funderingdata_droogstand_risico.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15828 2023-04-17 10:41:24.000000 calcasa-api-1.2.1/calcasa/api/model/funderingdata_optrekkend_vocht_risico.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17185 2023-04-17 10:41:25.000000 calcasa-api-1.2.1/calcasa/api/model/funderingdata_typering.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15008 2023-04-17 10:41:25.000000 calcasa-api-1.2.1/calcasa/api/model/gebiedsdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12152 2023-04-17 10:41:25.000000 calcasa-api-1.2.1/calcasa/api/model/geldverstrekker.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15292 2023-04-17 10:41:25.000000 calcasa-api-1.2.1/calcasa/api/model/http_validation_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13141 2023-04-17 10:41:25.000000 calcasa-api-1.2.1/calcasa/api/model/invalid_argument_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12512 2023-04-17 10:41:26.000000 calcasa-api-1.2.1/calcasa/api/model/json_patch_document.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13462 2023-04-17 10:41:26.000000 calcasa-api-1.2.1/calcasa/api/model/klantwaarde_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11883 2023-04-17 10:41:26.000000 calcasa-api-1.2.1/calcasa/api/model/kwartaal.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13159 2023-04-17 10:41:26.000000 calcasa-api-1.2.1/calcasa/api/model/modeldata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13101 2023-04-17 10:41:26.000000 calcasa-api-1.2.1/calcasa/api/model/not_found_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13822 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/notitie.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16711 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/notities.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15101 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/objectdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13370 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17457 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_buurt.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17466 2023-04-17 10:41:27.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_gemeente.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17454 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_land.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17469 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_provincie.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17454 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_wijk.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12860 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/operation.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13368 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/operation_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13192 2023-04-17 10:41:28.000000 calcasa-api-1.2.1/calcasa/api/model/permissions_denied_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12856 2023-04-17 10:41:29.000000 calcasa-api-1.2.1/calcasa/api/model/problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15300 2023-04-17 10:41:29.000000 calcasa-api-1.2.1/calcasa/api/model/product_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    11662 2023-04-17 10:41:29.000000 calcasa-api-1.2.1/calcasa/api/model/rapport.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16139 2023-04-17 10:41:29.000000 calcasa-api-1.2.1/calcasa/api/model/referentieobject.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15522 2023-04-17 10:41:29.000000 calcasa-api-1.2.1/calcasa/api/model/referentieobject_adres.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15062 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/referentieobject_cbs_indeling.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17519 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/referentieobject_object.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13138 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/resource_exhausted_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13627 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/taxatiedata.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13624 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/taxatiestatus.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13110 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/validation_problem_details.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16768 2023-04-17 10:41:30.000000 calcasa-api-1.2.1/calcasa/api/model/verkoop_bijzonderheden.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    13903 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/vorige_verkoop.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    18178 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15043 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_cbs_indeling.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14393 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_factuur.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    23276 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_input_parameters.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15595 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_model.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17500 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_object.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16408 2023-04-17 10:41:31.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    12306 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling_kwartaal.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14387 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling_kwartaal_kwartaal.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    25416 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_originele_input.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14100 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_rapport.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15911 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_status.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    16031 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_taxatie.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    17476 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_webhook_payload.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15507 2023-04-17 10:41:32.000000 calcasa-api-1.2.1/calcasa/api/model/waardering_zoek_parameters.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    15371 2023-04-17 10:41:33.000000 calcasa-api-1.2.1/calcasa/api/model/woning_type.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    83107 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/model_utils.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:26.827408 calcasa-api-1.2.1/calcasa/api/models/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     5652 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/models/__init__.py
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    14809 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/calcasa/api/rest.py
+drwxrwxrwx   0 erwin     (1000) erwin     (1000)        0 2023-04-17 10:45:27.183682 calcasa-api-1.2.1/calcasa_api.egg-info/
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)    25152 2023-04-17 10:45:16.000000 calcasa-api-1.2.1/calcasa_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     4039 2023-04-17 10:45:17.000000 calcasa-api-1.2.1/calcasa_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)        1 2023-04-17 10:45:16.000000 calcasa-api-1.2.1/calcasa_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)       32 2023-04-17 10:45:16.000000 calcasa-api-1.2.1/calcasa_api.egg-info/requires.txt
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)        8 2023-04-17 10:45:16.000000 calcasa-api-1.2.1/calcasa_api.egg-info/top_level.txt
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)       69 2023-04-17 10:45:27.279534 calcasa-api-1.2.1/setup.cfg
+-rwxrwxrwx   0 erwin     (1000) erwin     (1000)     1943 2023-04-17 10:41:34.000000 calcasa-api-1.2.1/setup.py
```

### Comparing `calcasa-api-1.2.0/PKG-INFO` & `calcasa-api-1.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,465 +1,471 @@
 Metadata-Version: 2.1
 Name: calcasa-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Calcasa Public API v1
 Home-page: https://github.com/calcasa/api-python
 Author: Calcasa B.V.
 Author-email: info@calcasa.nl
 License: Apache-2.0
-Description: # calcasa-api
-        The Calcasa API is used to connect to Calcasa provided services. This is the first production version of the service
-        
-        ## Client packages
-        [Nuget](https://www.nuget.org/packages/Calcasa.Api) - [Packagist](https://packagist.org/packages/calcasa/api) - [PyPI](https://pypi.org/project/calcasa.api)
-        ## Client implementation notes
-        Clients should at all times be tolerant to the following:
-        
-        - Extra fields in responses
-        - Empty or hidden fields in responses
-        - Extra values in enumerations
-        - Unexpected error responses in the form of [Problem Details](https://rfc-editor.org/rfc/rfc7807)
-        
-        ## OpenAPI Specification
-        This API is documented in **OpenAPI format version 3** you can use tools like the [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) to generate API clients for for example the languages we don't provide a pre-built client for. This is documented [here](/api/v1/articles/clients/generation).
-        
-        ## Changelog
-        
-        ### 2022-08-04 (v1.2.0)
-        - Add support for managing `CallbackSubscription`'s, this allows you to subscribe to callbacks for valuations that were not created with your API client.
-            - `GET /v1/callbacks/inschrijvingen`
-            - `POST /v1/callbacks/inschrijvingen`
-            - `GET /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
-            - `DELETE /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
-        - Add `taxateurnaam` field to the `Taxatiedata` model.
-        - Callback URIs should now end in `/` not just contain it to help stop common errors (ending in `=` is also still allowed when using a query string).
-        - Updating configuration in the `POST /v1/configuratie/callbacks` endpoint now clears stored but decommissioned versions from the configuration object.
-        - Add `klantkenmerk` to the `WaarderingInputParameters` and `Waardering` models.
-        
-        ### 2022-07-12 (v1.1.7)
-        - Added support for the OAuth 2.0 authorization code flow for use of the API with user accounts.
-        - Add `bouweenheid` to `FunderingSoortBron` enumeration.
-        
-        ### 2022-05-19 (v1.1.6)
-        - Added `ltvTeHoogOverbrugging` value to the `BusinessRulesCode` enumeration.
-        
-        ### 2022-04-13 (v1.1.5)
-        - Fix the schema for `Operation` `value` field for the benefit of the PHP and Python code generators, these will now correctly support any value type.
-        
-        ### 2022-04-12 (v1.1.4)
-        - Added proper Content-Disposition headers to the `GET /v1/rapporten/{id}` and `GET /v1/facturen/{id}` endpoints with the correct filename.
-        - Fix Mime Types for the `POST /v1/configuratie/callbacks` endpoint to only accept `application/json`.
-        - Fix C# API client to correctly use the `application/json-patch+json` content type in requests that require it.
-        - Fix C# client's `FileParameter` type correct handling of response headers like `Content-Disposition` and `Content-Type`.
-        - Removed C# client's useless implementation of `IValidatableObject`.
-        - Fix Python client's internal namespace name being illegal `calcasa-api` -> `calcasa.api`.
-        
-        ### 2022-03-22 (v1.1.3)
-        - Add 402 (Payment required) and 422 (Unprocessable entity) as potential response for `PATCH /v1/waarderingen/{id}`.
-        
-        ### 2022-03-17 (v1.1.2)
-        - Fixed response type for `GET /v1/geldverstrekkers/{productType}` endpoint.
-        
-        ### 2022-03-08 (v1.1.1)
-        - Added `GET /v1/geldverstrekkers/{productType}` endpoint.
-        - Restored all `ProblemDetails` models.
-        
-        ### 2022-03-07 (v1.1.0)
-        - Added `isErfpacht` to `WaarderingInputParameters`.
-        - Cleaned up serialization of null values, they should no longer appear in the output.
-        
-        ### 2021-02-04
-        - Added extra clarification to the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different input parameter combinations.
-        
-        ### 2022-01-11 (v1.0.2)
-        - Fixed `GET /api/v1/bodem/{id}` endpoint path parameter description, query parameter was never meant to be there.
-        
-        ### 2021-12-23
-        - Clarified the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different product types.
-        
-        ### 2021-12-22 (v1.0.1)
-        - Dates are now serialized in the ISO date-only format `yyyy-MM-dd` to stop any confusion around timezones and are all assumed to be in UTC.
-            - `peildatum` in `WaarderingsInputParameters`
-            - `datum_bestemmingplan` in `Bestemmingsdata`
-            - `datum_laatste_onderzoek` in `Bodemdata`
-            - `verkoopdatum` in `Referentieobject`
-            - `verkoopdatum` in `VorigeVerkoop`
-            - `waardebepalingsdatum` in `Modeldata`
-        - Reintroduced the `WaarderingWebhookPayload` model that was omitted.
-        
-        ### 2021-12-21
-        - Patching the status of a `Waardering` object will now immediatly reflect its new status in the response object.
-        
-        ### 2021-12-13 (v1.0.0)
-        - Initial release of `v1` based on `v0.0.6`
-        
-        ## Cross-Origin Resource Sharing
-        This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).
-        And that allows cross-domain communication from the browser.
-        All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.
-        
-        ## Authentication
-        Authentication is done via [OAuth2](https://oauth.net/2/) and the [client credentials](https://oauth.net/2/grant-types/client-credentials/) grant type.
-        
-        ## Previous versions changelogs
-        
-        ### 2022-02-02
-        - API version `v0` was removed from service.
-        
-        ### 2021-12-23
-        - Mark `v0` as officially deprecated. No further versions will be released. Every implementation should move to `v1`
-        
-        ### 2021-12-10 (v0.0.6)
-        - Added extra field `peildatum` to the `WaarderingInputParameters` model.
-        
-        ### 2021-11-25 (v0.0.5)
-        - Updated all reported OAuth2 scopes and reduced the superflous scope information on each endpoint.
-        
-        ### 2021-11-23 (v0.0.4)
-        - Added per square meter developments to the `WaarderingOntwikkeling` object (fields with the `PerVierkantemeter` suffix).
-        
-        ### 2021-11-15 (v0.0.3)
-        - Added callback update and read endpoints and models.
-        - Updated documentation.
-        
-        ### 2021-11-11
-        - Renamed /fundering endpoint to /funderingen to be more in line with other endpoints
-        - Renamed `HerstelType` to `FunderingHerstelType`.
-        - Added `FunderingType` values.
-        
-        ### 2021-11-10
-        - Adjusted OpenAPI Spec generation to fix some issues with certain generators. This also means that the nullable nature of certain fields is now correctly represented. Please refer to the Generation article for more information, the config files were updated aswell.
-        
-        ### 2021-11-09
-        - Added `Status` and `Taxatiedatum` to `Taxatiedata` model.
-        
-        ### 2021-11-08
-        - Renamed `id` field in `AdresInfo` model to `bagNummeraanduidingId`.
-        - Added `GET /v0/fundering/{id}` endpoint with corresponding models.
-        - Changed HTTP response code for the `BusinessRulesProblemDetails` error return type of `POST /v0/waardering` from `422 Unprocessable Entity` to `406 Not Acceptable` to fix a duplicate.
-        
-        ### 2021-10-13
-        - Added `taxatie` field to `Waardering` model.
-        - Added `Taxatiedata` model containing the `taxatieorganisatie` field for desktop valuations.
-        
-        ### 2021-09-29
-        - Added `aangemaakt` timestamp field to `Waardering` model.
-        - Added `WaarderingZoekParameters` model to replace `WaarderingInputParameters` in the `POST /v0/waarderingen/zoeken` endpoint.
-        - Split `Omgevingsdata` model into a set of separate `Gebiedsdata` models that also contain extra statistics.
-        - Added `bijzonderheden` field to `VorigeVerkoop` model.
-        - Renamed `ReferentieBijzonderheden` model to `VerkoopBijzonderheden`.
-        
-        ### 2021-09-22
-        - Initial release of `v0`
-        
-        This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-        
-        - API version: 1.2.0
-        - Package version: 1.2.0
-        - Build package: org.openapitools.codegen.languages.PythonClientCodegen
-        For more information, please visit [https://www.calcasa.nl/contact](https://www.calcasa.nl/contact)
-        
-        ## Requirements.
-        
-        Python >=3.6
-        
-        ## Installation & Usage
-        ### pip install
-        
-        If the python package is hosted on a repository, you can install directly using:
-        
-        ```sh
-        pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-        ```
-        (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-        
-        Then import the package:
-        ```python
-        import calcasa.api
-        ```
-        
-        ### Setuptools
-        
-        Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-        
-        ```sh
-        python setup.py install --user
-        ```
-        (or `sudo python setup.py install` to install the package for all users)
-        
-        Then import the package:
-        ```python
-        import calcasa.api
-        ```
-        
-        ## Getting Started
-        
-        Please follow the [installation procedure](#installation--usage) and then run the following:
-        
-        ```python
-        
-        import time
-        import calcasa.api
-        from pprint import pprint
-        from calcasa.api.api import adressen_api
-        from calcasa.api.model.adres import Adres
-        from calcasa.api.model.adres_info import AdresInfo
-        from calcasa.api.model.not_found_problem_details import NotFoundProblemDetails
-        from calcasa.api.model.permissions_denied_problem_details import PermissionsDeniedProblemDetails
-        from calcasa.api.model.problem_details import ProblemDetails
-        # Defining the host is optional and defaults to https://api.calcasa.nl
-        # See configuration.py for a list of all supported configuration parameters.
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        
-        # The client must configure the authentication and authorization parameters
-        # in accordance with the API server security policy.
-        # Examples for each auth method are provided below, use the example that
-        # satisfies your auth use case.
-        
-        # Configure OAuth2 access token for authorization: oauth
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        configuration.access_token = 'YOUR_ACCESS_TOKEN'
-        
-        # Configure OAuth2 access token for authorization: oauth
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        configuration.access_token = 'YOUR_ACCESS_TOKEN'
-        
-        
-        # Enter a context with an instance of the API client
-        with calcasa.api.ApiClient(configuration) as api_client:
-            # Create an instance of the API class
-            api_instance = adressen_api.AdressenApi(api_client)
-            bag_nummeraanduiding_id = 1 # int | Een BAG Nummeraanduiding ID om een adres te specificeren.
-        
-            try:
-                # Adres info op basis van BAG Nummeraanduiding Id.
-                api_response = api_instance.get_adres(bag_nummeraanduiding_id)
-                pprint(api_response)
-            except calcasa.api.ApiException as e:
-                print("Exception when calling AdressenApi->get_adres: %s\n" % e)
-        ```
-        
-        ## Documentation for API Endpoints
-        
-        All URIs are relative to *https://api.calcasa.nl*
-        
-        Class | Method | HTTP request | Description
-        ------------ | ------------- | ------------- | -------------
-        *AdressenApi* | [**get_adres**](docs/AdressenApi.md#get_adres) | **GET** /api/v1/adressen/{bagNummeraanduidingId} | Adres info op basis van BAG Nummeraanduiding Id.
-        *AdressenApi* | [**search_adres**](docs/AdressenApi.md#search_adres) | **POST** /api/v1/adressen/zoeken | Zoek adres info op basis van het gegeven adres.
-        *BestemmingsplannenApi* | [**get_bestemming_by_id**](docs/BestemmingsplannenApi.md#get_bestemming_by_id) | **GET** /api/v1/bestemmingsplannen/{bagNummeraanduidingId} | Gegevens over de bestemmingsplannen op de locatie van een adres (BAG Nummeraanduiding ID).
-        *BodemApi* | [**get_bodem_by_id**](docs/BodemApi.md#get_bodem_by_id) | **GET** /api/v1/bodem/{bagNummeraanduidingId} | Gegevens over de bodemkwaliteit op de locatie van een adres (BAG Nummeraanduiding ID).
-        *BuurtApi* | [**get_buurt**](docs/BuurtApi.md#get_buurt) | **GET** /api/v1/buurt/{buurtId} | Gegevens over een buurt en de wijk, gemeente en land waarin deze buurt gesitueerd is.
-        *CallbacksApi* | [**add_or_update_callback_subscription**](docs/CallbacksApi.md#add_or_update_callback_subscription) | **POST** /api/v1/callbacks/inschrijvingen | Voeg een callback inschrijving toe (of werk bij) voor de huidige client voor een adres.
-        *CallbacksApi* | [**delete_notification_subscription**](docs/CallbacksApi.md#delete_notification_subscription) | **DELETE** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Verwijder de callback inschrijving voor deze client en dit adres.
-        *CallbacksApi* | [**get_notification_subscription**](docs/CallbacksApi.md#get_notification_subscription) | **GET** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Haal de callback inschrijving op voor deze client en dit adres.
-        *CallbacksApi* | [**get_notification_subscriptions**](docs/CallbacksApi.md#get_notification_subscriptions) | **GET** /api/v1/callbacks/inschrijvingen | Haal de callback inschrijvingen binnen voor deze client.
-        *ConfiguratieApi* | [**get_callbacks**](docs/ConfiguratieApi.md#get_callbacks) | **GET** /api/v1/configuratie/callbacks | Haal de geconfigureerde callback URL&#39;s op voor de huidige client.
-        *ConfiguratieApi* | [**update_callbacks**](docs/ConfiguratieApi.md#update_callbacks) | **POST** /api/v1/configuratie/callbacks | Configureer callback URL voor een specifieke API versie voor de huidige client.
-        *FacturenApi* | [**get_factuur**](docs/FacturenApi.md#get_factuur) | **GET** /api/v1/facturen/{id} | Factuur op basis van een waardering Id.
-        *FotosApi* | [**get_foto**](docs/FotosApi.md#get_foto) | **GET** /api/v1/fotos/{id} | Foto op basis van een foto Id.
-        *FunderingenApi* | [**get_fundering_by_id**](docs/FunderingenApi.md#get_fundering_by_id) | **GET** /api/v1/funderingen/{bagNummeraanduidingId} | Gegevens over de fundering op de locatie van een adres (BAG Nummeraanduiding ID).
-        *GeldverstrekkersApi* | [**get_geldverstrekkers**](docs/GeldverstrekkersApi.md#get_geldverstrekkers) | **GET** /api/v1/geldverstrekkers/{productType} | Alle geldverstrekkers die te gebruiken zijn voor aanvragen.
-        *RapportenApi* | [**get_rapport**](docs/RapportenApi.md#get_rapport) | **GET** /api/v1/rapporten/{id} | Rapport op basis van waardering Id.
-        *WaarderingenApi* | [**create_waardering**](docs/WaarderingenApi.md#create_waardering) | **POST** /api/v1/waarderingen | Creërt een waardering.
-        *WaarderingenApi* | [**get_waardering**](docs/WaarderingenApi.md#get_waardering) | **GET** /api/v1/waarderingen/{id} | Waardering op basis van Id.
-        *WaarderingenApi* | [**get_waardering_ontwikkeling**](docs/WaarderingenApi.md#get_waardering_ontwikkeling) | **GET** /api/v1/waarderingen/{id}/ontwikkeling | Waardering ontwikkeling op basis van waardering Id.
-        *WaarderingenApi* | [**patch_waarderingen**](docs/WaarderingenApi.md#patch_waarderingen) | **PATCH** /api/v1/waarderingen/{id} | Patcht een waardering.
-        *WaarderingenApi* | [**search_waarderingen**](docs/WaarderingenApi.md#search_waarderingen) | **POST** /api/v1/waarderingen/zoeken | Zoek waardering op basis van input parameters.
-        
-        
-        ## Documentation For Models
-        
-         - [Aanvraagdoel](docs/Aanvraagdoel.md)
-         - [Adres](docs/Adres.md)
-         - [AdresInfo](docs/AdresInfo.md)
-         - [AdresInfoAdres](docs/AdresInfoAdres.md)
-         - [AdresInfoNotities](docs/AdresInfoNotities.md)
-         - [Bestemmingsdata](docs/Bestemmingsdata.md)
-         - [BodemStatusType](docs/BodemStatusType.md)
-         - [Bodemdata](docs/Bodemdata.md)
-         - [BusinessRulesCode](docs/BusinessRulesCode.md)
-         - [BusinessRulesProblemDetails](docs/BusinessRulesProblemDetails.md)
-         - [Callback](docs/Callback.md)
-         - [CallbackInschrijving](docs/CallbackInschrijving.md)
-         - [CbsIndeling](docs/CbsIndeling.md)
-         - [Energielabel](docs/Energielabel.md)
-         - [Factuur](docs/Factuur.md)
-         - [Foto](docs/Foto.md)
-         - [FunderingDataBron](docs/FunderingDataBron.md)
-         - [FunderingHerstelType](docs/FunderingHerstelType.md)
-         - [FunderingRisico](docs/FunderingRisico.md)
-         - [FunderingRisicoLabel](docs/FunderingRisicoLabel.md)
-         - [FunderingSoortBron](docs/FunderingSoortBron.md)
-         - [FunderingType](docs/FunderingType.md)
-         - [FunderingTypering](docs/FunderingTypering.md)
-         - [Funderingdata](docs/Funderingdata.md)
-         - [FunderingdataBioInfectieRisico](docs/FunderingdataBioInfectieRisico.md)
-         - [FunderingdataDroogstandRisico](docs/FunderingdataDroogstandRisico.md)
-         - [FunderingdataOptrekkendVochtRisico](docs/FunderingdataOptrekkendVochtRisico.md)
-         - [FunderingdataTypering](docs/FunderingdataTypering.md)
-         - [Gebiedsdata](docs/Gebiedsdata.md)
-         - [Geldverstrekker](docs/Geldverstrekker.md)
-         - [HttpValidationProblemDetails](docs/HttpValidationProblemDetails.md)
-         - [InvalidArgumentProblemDetails](docs/InvalidArgumentProblemDetails.md)
-         - [JsonPatchDocument](docs/JsonPatchDocument.md)
-         - [KlantwaardeType](docs/KlantwaardeType.md)
-         - [Kwartaal](docs/Kwartaal.md)
-         - [Modeldata](docs/Modeldata.md)
-         - [NotFoundProblemDetails](docs/NotFoundProblemDetails.md)
-         - [Notitie](docs/Notitie.md)
-         - [Notities](docs/Notities.md)
-         - [Objectdata](docs/Objectdata.md)
-         - [Omgevingsdata](docs/Omgevingsdata.md)
-         - [OmgevingsdataBuurt](docs/OmgevingsdataBuurt.md)
-         - [OmgevingsdataGemeente](docs/OmgevingsdataGemeente.md)
-         - [OmgevingsdataLand](docs/OmgevingsdataLand.md)
-         - [OmgevingsdataProvincie](docs/OmgevingsdataProvincie.md)
-         - [OmgevingsdataWijk](docs/OmgevingsdataWijk.md)
-         - [Operation](docs/Operation.md)
-         - [OperationType](docs/OperationType.md)
-         - [PermissionsDeniedProblemDetails](docs/PermissionsDeniedProblemDetails.md)
-         - [ProblemDetails](docs/ProblemDetails.md)
-         - [ProductType](docs/ProductType.md)
-         - [Rapport](docs/Rapport.md)
-         - [Referentieobject](docs/Referentieobject.md)
-         - [ReferentieobjectAdres](docs/ReferentieobjectAdres.md)
-         - [ReferentieobjectCbsIndeling](docs/ReferentieobjectCbsIndeling.md)
-         - [ReferentieobjectObject](docs/ReferentieobjectObject.md)
-         - [ResourceExhaustedProblemDetails](docs/ResourceExhaustedProblemDetails.md)
-         - [Taxatiedata](docs/Taxatiedata.md)
-         - [Taxatiestatus](docs/Taxatiestatus.md)
-         - [ValidationProblemDetails](docs/ValidationProblemDetails.md)
-         - [VerkoopBijzonderheden](docs/VerkoopBijzonderheden.md)
-         - [VorigeVerkoop](docs/VorigeVerkoop.md)
-         - [Waardering](docs/Waardering.md)
-         - [WaarderingCbsIndeling](docs/WaarderingCbsIndeling.md)
-         - [WaarderingFactuur](docs/WaarderingFactuur.md)
-         - [WaarderingInputParameters](docs/WaarderingInputParameters.md)
-         - [WaarderingModel](docs/WaarderingModel.md)
-         - [WaarderingObject](docs/WaarderingObject.md)
-         - [WaarderingOntwikkeling](docs/WaarderingOntwikkeling.md)
-         - [WaarderingOntwikkelingKwartaal](docs/WaarderingOntwikkelingKwartaal.md)
-         - [WaarderingOntwikkelingKwartaalKwartaal](docs/WaarderingOntwikkelingKwartaalKwartaal.md)
-         - [WaarderingOrigineleInput](docs/WaarderingOrigineleInput.md)
-         - [WaarderingRapport](docs/WaarderingRapport.md)
-         - [WaarderingStatus](docs/WaarderingStatus.md)
-         - [WaarderingTaxatie](docs/WaarderingTaxatie.md)
-         - [WaarderingWebhookPayload](docs/WaarderingWebhookPayload.md)
-         - [WaarderingZoekParameters](docs/WaarderingZoekParameters.md)
-         - [WoningType](docs/WoningType.md)
-        
-        
-        ## Documentation For Authorization
-        
-        
-        ## oauth
-        
-        - **Type**: OAuth
-        - **Flow**: application
-        - **Authorization URL**: 
-        - **Scopes**: 
-         - **all**: Full permissions for all areas.
-         - **api:all**: Full permissions for all areas of the public API.
-         - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:all**: Full permissions for the bodem area of the public API.
-         - **api:buurt:all**: Full permissions for the buurt area of the public API.
-         - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
-         - **api:callback:all**: Full permissions for the callback area of the public API.
-         - **api:facturen:all**: Full permissions for the facturen area of the public API.
-         - **api:fotos:all**: Full permissions for the fotos area of the public API.
-         - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
-         - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
-         - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
-         - **api:adressen:read**: Read permissions for the adressen area of the public API.
-         - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:read**: Read permissions for the bodem area of the public API.
-         - **api:buurt:read**: Read permissions for the buurt area of the public API.
-         - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
-         - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
-         - **api:callback:read**: Read permissions for the callback area of the public API.
-         - **api:callback:write**: Write permissions for the callback area of the public API.
-         - **api:facturen:read**: Read permissions for the facturen area of the public API.
-         - **api:fotos:read**: Read permissions for the fotos area of the public API.
-         - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
-         - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
-         - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
-         - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
-         - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
-         - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
-         - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
-        
-        
-        ## oauth
-        
-        - **Type**: OAuth
-        - **Flow**: accessCode
-        - **Authorization URL**: https://authentication.calcasa.nl/oauth2/v2.0/authorize
-        - **Scopes**: 
-         - **all**: Full permissions for all areas.
-         - **api:all**: Full permissions for all areas of the public API.
-         - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:all**: Full permissions for the bodem area of the public API.
-         - **api:buurt:all**: Full permissions for the buurt area of the public API.
-         - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
-         - **api:callback:all**: Full permissions for the callback area of the public API.
-         - **api:facturen:all**: Full permissions for the facturen area of the public API.
-         - **api:fotos:all**: Full permissions for the fotos area of the public API.
-         - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
-         - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
-         - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
-         - **api:adressen:read**: Read permissions for the adressen area of the public API.
-         - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:read**: Read permissions for the bodem area of the public API.
-         - **api:buurt:read**: Read permissions for the buurt area of the public API.
-         - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
-         - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
-         - **api:callback:read**: Read permissions for the callback area of the public API.
-         - **api:callback:write**: Write permissions for the callback area of the public API.
-         - **api:facturen:read**: Read permissions for the facturen area of the public API.
-         - **api:fotos:read**: Read permissions for the fotos area of the public API.
-         - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
-         - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
-         - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
-         - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
-         - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
-         - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
-         - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
-        
-        
-        ## Author
-        
-        info@calcasa.nl
-        
-        
-        ## Notes for Large OpenAPI documents
-        If the OpenAPI document is large, imports in calcasa.api.apis and calcasa.api.models may fail with a
-        RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-        
-        Solution 1:
-        Use specific imports for apis and models like:
-        - `from calcasa.api.api.default_api import DefaultApi`
-        - `from calcasa.api.model.pet import Pet`
-        
-        Solution 2:
-        Before importing the package, adjust the maximum recursion limit as shown below:
-        ```
-        import sys
-        sys.setrecursionlimit(1500)
-        import calcasa.api
-        from calcasa.api.apis import *
-        from calcasa.api.models import *
-        ```
-        
-        
 Keywords: OpenAPI,OpenAPI-Generator,Calcasa Public API v1
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE
+
+# calcasa-api
+The Calcasa API is used to connect to Calcasa provided services. This is the first production version of the service
+
+## Client packages
+[Nuget](https://www.nuget.org/packages/Calcasa.Api) - [Packagist](https://packagist.org/packages/calcasa/api) - [PyPI](https://pypi.org/project/calcasa.api)
+## Client implementation notes
+Clients should at all times be tolerant to the following:
+
+- Extra fields in responses
+- Empty or hidden fields in responses
+- Extra values in enumerations
+- Unexpected error responses in the form of [Problem Details](https://rfc-editor.org/rfc/rfc7807)
+
+## OpenAPI Specification
+This API is documented in **OpenAPI format version 3** you can use tools like the [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) to generate API clients for for example the languages we don't provide a pre-built client for. This is documented [here](/api/v1/articles/clients/generation).
+
+## Changelog
+
+### 2023-04-17 (v1.2.1)
+- Add `externeReferentie` field to the `CallbackInschrijving` and `WaarderingWebhookPayload` models.
+
+### 2022-08-04 (v1.2.0)
+- Add support for managing `CallbackSubscription`'s, this allows you to subscribe to callbacks for valuations that were not created with your API client.
+    - `GET /v1/callbacks/inschrijvingen`
+    - `POST /v1/callbacks/inschrijvingen`
+    - `GET /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
+    - `DELETE /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
+- Add `taxateurnaam` field to the `Taxatiedata` model.
+- Callback URIs should now end in `/` not just contain it to help stop common errors (ending in `=` is also still allowed when using a query string).
+- Updating configuration in the `POST /v1/configuratie/callbacks` endpoint now clears stored but decommissioned versions from the configuration object.
+- Add `klantkenmerk` to the `WaarderingInputParameters` and `Waardering` models.
+
+### 2022-07-12 (v1.1.7)
+- Added support for the OAuth 2.0 authorization code flow for use of the API with user accounts.
+- Add `bouweenheid` to `FunderingSoortBron` enumeration.
+
+### 2022-05-19 (v1.1.6)
+- Added `ltvTeHoogOverbrugging` value to the `BusinessRulesCode` enumeration.
+
+### 2022-04-13 (v1.1.5)
+- Fix the schema for `Operation` `value` field for the benefit of the PHP and Python code generators, these will now correctly support any value type.
+
+### 2022-04-12 (v1.1.4)
+- Added proper Content-Disposition headers to the `GET /v1/rapporten/{id}` and `GET /v1/facturen/{id}` endpoints with the correct filename.
+- Fix Mime Types for the `POST /v1/configuratie/callbacks` endpoint to only accept `application/json`.
+- Fix C# API client to correctly use the `application/json-patch+json` content type in requests that require it.
+- Fix C# client's `FileParameter` type correct handling of response headers like `Content-Disposition` and `Content-Type`.
+- Removed C# client's useless implementation of `IValidatableObject`.
+- Fix Python client's internal namespace name being illegal `calcasa-api` -> `calcasa.api`.
+
+### 2022-03-22 (v1.1.3)
+- Add 402 (Payment required) and 422 (Unprocessable entity) as potential response for `PATCH /v1/waarderingen/{id}`.
+
+### 2022-03-17 (v1.1.2)
+- Fixed response type for `GET /v1/geldverstrekkers/{productType}` endpoint.
+
+### 2022-03-08 (v1.1.1)
+- Added `GET /v1/geldverstrekkers/{productType}` endpoint.
+- Restored all `ProblemDetails` models.
+
+### 2022-03-07 (v1.1.0)
+- Added `isErfpacht` to `WaarderingInputParameters`.
+- Cleaned up serialization of null values, they should no longer appear in the output.
+
+### 2021-02-04
+- Added extra clarification to the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different input parameter combinations.
+
+### 2022-01-11 (v1.0.2)
+- Fixed `GET /api/v1/bodem/{id}` endpoint path parameter description, query parameter was never meant to be there.
+
+### 2021-12-23
+- Clarified the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different product types.
+
+### 2021-12-22 (v1.0.1)
+- Dates are now serialized in the ISO date-only format `yyyy-MM-dd` to stop any confusion around timezones and are all assumed to be in UTC.
+    - `peildatum` in `WaarderingsInputParameters`
+    - `datum_bestemmingplan` in `Bestemmingsdata`
+    - `datum_laatste_onderzoek` in `Bodemdata`
+    - `verkoopdatum` in `Referentieobject`
+    - `verkoopdatum` in `VorigeVerkoop`
+    - `waardebepalingsdatum` in `Modeldata`
+- Reintroduced the `WaarderingWebhookPayload` model that was omitted.
+
+### 2021-12-21
+- Patching the status of a `Waardering` object will now immediatly reflect its new status in the response object.
+
+### 2021-12-13 (v1.0.0)
+- Initial release of `v1` based on `v0.0.6`
+
+## Cross-Origin Resource Sharing
+This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).
+And that allows cross-domain communication from the browser.
+All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.
+
+## Authentication
+Authentication is done via [OAuth2](https://oauth.net/2/) and the [client credentials](https://oauth.net/2/grant-types/client-credentials/) grant type.
+
+## Previous versions changelogs
+
+### 2022-02-02
+- API version `v0` was removed from service.
+
+### 2021-12-23
+- Mark `v0` as officially deprecated. No further versions will be released. Every implementation should move to `v1`
+
+### 2021-12-10 (v0.0.6)
+- Added extra field `peildatum` to the `WaarderingInputParameters` model.
+
+### 2021-11-25 (v0.0.5)
+- Updated all reported OAuth2 scopes and reduced the superflous scope information on each endpoint.
+
+### 2021-11-23 (v0.0.4)
+- Added per square meter developments to the `WaarderingOntwikkeling` object (fields with the `PerVierkantemeter` suffix).
+
+### 2021-11-15 (v0.0.3)
+- Added callback update and read endpoints and models.
+- Updated documentation.
+
+### 2021-11-11
+- Renamed /fundering endpoint to /funderingen to be more in line with other endpoints
+- Renamed `HerstelType` to `FunderingHerstelType`.
+- Added `FunderingType` values.
+
+### 2021-11-10
+- Adjusted OpenAPI Spec generation to fix some issues with certain generators. This also means that the nullable nature of certain fields is now correctly represented. Please refer to the Generation article for more information, the config files were updated aswell.
+
+### 2021-11-09
+- Added `Status` and `Taxatiedatum` to `Taxatiedata` model.
+
+### 2021-11-08
+- Renamed `id` field in `AdresInfo` model to `bagNummeraanduidingId`.
+- Added `GET /v0/fundering/{id}` endpoint with corresponding models.
+- Changed HTTP response code for the `BusinessRulesProblemDetails` error return type of `POST /v0/waardering` from `422 Unprocessable Entity` to `406 Not Acceptable` to fix a duplicate.
+
+### 2021-10-13
+- Added `taxatie` field to `Waardering` model.
+- Added `Taxatiedata` model containing the `taxatieorganisatie` field for desktop valuations.
+
+### 2021-09-29
+- Added `aangemaakt` timestamp field to `Waardering` model.
+- Added `WaarderingZoekParameters` model to replace `WaarderingInputParameters` in the `POST /v0/waarderingen/zoeken` endpoint.
+- Split `Omgevingsdata` model into a set of separate `Gebiedsdata` models that also contain extra statistics.
+- Added `bijzonderheden` field to `VorigeVerkoop` model.
+- Renamed `ReferentieBijzonderheden` model to `VerkoopBijzonderheden`.
+
+### 2021-09-22
+- Initial release of `v0`
+
+This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 1.2.1
+- Package version: 1.2.1
+- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+For more information, please visit [https://www.calcasa.nl/contact](https://www.calcasa.nl/contact)
+
+## Requirements.
+
+Python >=3.6
+
+## Installation & Usage
+### pip install
+
+If the python package is hosted on a repository, you can install directly using:
+
+```sh
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+```
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+
+Then import the package:
+```python
+import calcasa.api
+```
+
+### Setuptools
+
+Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+
+```sh
+python setup.py install --user
+```
+(or `sudo python setup.py install` to install the package for all users)
+
+Then import the package:
+```python
+import calcasa.api
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+
+import time
+import calcasa.api
+from pprint import pprint
+from calcasa.api.api import adressen_api
+from calcasa.api.model.adres import Adres
+from calcasa.api.model.adres_info import AdresInfo
+from calcasa.api.model.not_found_problem_details import NotFoundProblemDetails
+from calcasa.api.model.permissions_denied_problem_details import PermissionsDeniedProblemDetails
+from calcasa.api.model.problem_details import ProblemDetails
+# Defining the host is optional and defaults to https://api.calcasa.nl
+# See configuration.py for a list of all supported configuration parameters.
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure OAuth2 access token for authorization: oauth
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+configuration.access_token = 'YOUR_ACCESS_TOKEN'
+
+# Configure OAuth2 access token for authorization: oauth
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+configuration.access_token = 'YOUR_ACCESS_TOKEN'
+
+
+# Enter a context with an instance of the API client
+with calcasa.api.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = adressen_api.AdressenApi(api_client)
+    bag_nummeraanduiding_id = 1 # int | Een BAG Nummeraanduiding ID om een adres te specificeren.
+
+    try:
+        # Adres info op basis van BAG Nummeraanduiding Id.
+        api_response = api_instance.get_adres(bag_nummeraanduiding_id)
+        pprint(api_response)
+    except calcasa.api.ApiException as e:
+        print("Exception when calling AdressenApi->get_adres: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *https://api.calcasa.nl*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AdressenApi* | [**get_adres**](docs/AdressenApi.md#get_adres) | **GET** /api/v1/adressen/{bagNummeraanduidingId} | Adres info op basis van BAG Nummeraanduiding Id.
+*AdressenApi* | [**search_adres**](docs/AdressenApi.md#search_adres) | **POST** /api/v1/adressen/zoeken | Zoek adres info op basis van het gegeven adres.
+*BestemmingsplannenApi* | [**get_bestemming_by_id**](docs/BestemmingsplannenApi.md#get_bestemming_by_id) | **GET** /api/v1/bestemmingsplannen/{bagNummeraanduidingId} | Gegevens over de bestemmingsplannen op de locatie van een adres (BAG Nummeraanduiding ID).
+*BodemApi* | [**get_bodem_by_id**](docs/BodemApi.md#get_bodem_by_id) | **GET** /api/v1/bodem/{bagNummeraanduidingId} | Gegevens over de bodemkwaliteit op de locatie van een adres (BAG Nummeraanduiding ID).
+*BuurtApi* | [**get_buurt**](docs/BuurtApi.md#get_buurt) | **GET** /api/v1/buurt/{buurtId} | Gegevens over een buurt en de wijk, gemeente en land waarin deze buurt gesitueerd is.
+*CallbacksApi* | [**add_or_update_callback_subscription**](docs/CallbacksApi.md#add_or_update_callback_subscription) | **POST** /api/v1/callbacks/inschrijvingen | Voeg een callback inschrijving toe (of werk bij) voor de huidige client voor een adres.
+*CallbacksApi* | [**delete_notification_subscription**](docs/CallbacksApi.md#delete_notification_subscription) | **DELETE** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Verwijder de callback inschrijving voor deze client en dit adres.
+*CallbacksApi* | [**get_notification_subscription**](docs/CallbacksApi.md#get_notification_subscription) | **GET** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Haal de callback inschrijving op voor deze client en dit adres.
+*CallbacksApi* | [**get_notification_subscriptions**](docs/CallbacksApi.md#get_notification_subscriptions) | **GET** /api/v1/callbacks/inschrijvingen | Haal de callback inschrijvingen binnen voor deze client.
+*ConfiguratieApi* | [**get_callbacks**](docs/ConfiguratieApi.md#get_callbacks) | **GET** /api/v1/configuratie/callbacks | Haal de geconfigureerde callback URL&#39;s op voor de huidige client.
+*ConfiguratieApi* | [**update_callbacks**](docs/ConfiguratieApi.md#update_callbacks) | **POST** /api/v1/configuratie/callbacks | Configureer callback URL voor een specifieke API versie voor de huidige client.
+*FacturenApi* | [**get_factuur**](docs/FacturenApi.md#get_factuur) | **GET** /api/v1/facturen/{id} | Factuur op basis van een waardering Id.
+*FotosApi* | [**get_foto**](docs/FotosApi.md#get_foto) | **GET** /api/v1/fotos/{id} | Foto op basis van een foto Id.
+*FunderingenApi* | [**get_fundering_by_id**](docs/FunderingenApi.md#get_fundering_by_id) | **GET** /api/v1/funderingen/{bagNummeraanduidingId} | Gegevens over de fundering op de locatie van een adres (BAG Nummeraanduiding ID).
+*GeldverstrekkersApi* | [**get_geldverstrekkers**](docs/GeldverstrekkersApi.md#get_geldverstrekkers) | **GET** /api/v1/geldverstrekkers/{productType} | Alle geldverstrekkers die te gebruiken zijn voor aanvragen.
+*RapportenApi* | [**get_rapport**](docs/RapportenApi.md#get_rapport) | **GET** /api/v1/rapporten/{id} | Rapport op basis van waardering Id.
+*WaarderingenApi* | [**create_waardering**](docs/WaarderingenApi.md#create_waardering) | **POST** /api/v1/waarderingen | Creërt een waardering.
+*WaarderingenApi* | [**get_waardering**](docs/WaarderingenApi.md#get_waardering) | **GET** /api/v1/waarderingen/{id} | Waardering op basis van Id.
+*WaarderingenApi* | [**get_waardering_ontwikkeling**](docs/WaarderingenApi.md#get_waardering_ontwikkeling) | **GET** /api/v1/waarderingen/{id}/ontwikkeling | Waardering ontwikkeling op basis van waardering Id.
+*WaarderingenApi* | [**patch_waarderingen**](docs/WaarderingenApi.md#patch_waarderingen) | **PATCH** /api/v1/waarderingen/{id} | Patcht een waardering.
+*WaarderingenApi* | [**search_waarderingen**](docs/WaarderingenApi.md#search_waarderingen) | **POST** /api/v1/waarderingen/zoeken | Zoek waardering op basis van input parameters.
+
+
+## Documentation For Models
+
+ - [Aanvraagdoel](docs/Aanvraagdoel.md)
+ - [Adres](docs/Adres.md)
+ - [AdresInfo](docs/AdresInfo.md)
+ - [AdresInfoAdres](docs/AdresInfoAdres.md)
+ - [AdresInfoNotities](docs/AdresInfoNotities.md)
+ - [Bestemmingsdata](docs/Bestemmingsdata.md)
+ - [BodemStatusType](docs/BodemStatusType.md)
+ - [Bodemdata](docs/Bodemdata.md)
+ - [BusinessRulesCode](docs/BusinessRulesCode.md)
+ - [BusinessRulesProblemDetails](docs/BusinessRulesProblemDetails.md)
+ - [Callback](docs/Callback.md)
+ - [CallbackInschrijving](docs/CallbackInschrijving.md)
+ - [CbsIndeling](docs/CbsIndeling.md)
+ - [Energielabel](docs/Energielabel.md)
+ - [Factuur](docs/Factuur.md)
+ - [Foto](docs/Foto.md)
+ - [FunderingDataBron](docs/FunderingDataBron.md)
+ - [FunderingHerstelType](docs/FunderingHerstelType.md)
+ - [FunderingRisico](docs/FunderingRisico.md)
+ - [FunderingRisicoLabel](docs/FunderingRisicoLabel.md)
+ - [FunderingSoortBron](docs/FunderingSoortBron.md)
+ - [FunderingType](docs/FunderingType.md)
+ - [FunderingTypering](docs/FunderingTypering.md)
+ - [Funderingdata](docs/Funderingdata.md)
+ - [FunderingdataBioInfectieRisico](docs/FunderingdataBioInfectieRisico.md)
+ - [FunderingdataDroogstandRisico](docs/FunderingdataDroogstandRisico.md)
+ - [FunderingdataOptrekkendVochtRisico](docs/FunderingdataOptrekkendVochtRisico.md)
+ - [FunderingdataTypering](docs/FunderingdataTypering.md)
+ - [Gebiedsdata](docs/Gebiedsdata.md)
+ - [Geldverstrekker](docs/Geldverstrekker.md)
+ - [HttpValidationProblemDetails](docs/HttpValidationProblemDetails.md)
+ - [InvalidArgumentProblemDetails](docs/InvalidArgumentProblemDetails.md)
+ - [JsonPatchDocument](docs/JsonPatchDocument.md)
+ - [KlantwaardeType](docs/KlantwaardeType.md)
+ - [Kwartaal](docs/Kwartaal.md)
+ - [Modeldata](docs/Modeldata.md)
+ - [NotFoundProblemDetails](docs/NotFoundProblemDetails.md)
+ - [Notitie](docs/Notitie.md)
+ - [Notities](docs/Notities.md)
+ - [Objectdata](docs/Objectdata.md)
+ - [Omgevingsdata](docs/Omgevingsdata.md)
+ - [OmgevingsdataBuurt](docs/OmgevingsdataBuurt.md)
+ - [OmgevingsdataGemeente](docs/OmgevingsdataGemeente.md)
+ - [OmgevingsdataLand](docs/OmgevingsdataLand.md)
+ - [OmgevingsdataProvincie](docs/OmgevingsdataProvincie.md)
+ - [OmgevingsdataWijk](docs/OmgevingsdataWijk.md)
+ - [Operation](docs/Operation.md)
+ - [OperationType](docs/OperationType.md)
+ - [PermissionsDeniedProblemDetails](docs/PermissionsDeniedProblemDetails.md)
+ - [ProblemDetails](docs/ProblemDetails.md)
+ - [ProductType](docs/ProductType.md)
+ - [Rapport](docs/Rapport.md)
+ - [Referentieobject](docs/Referentieobject.md)
+ - [ReferentieobjectAdres](docs/ReferentieobjectAdres.md)
+ - [ReferentieobjectCbsIndeling](docs/ReferentieobjectCbsIndeling.md)
+ - [ReferentieobjectObject](docs/ReferentieobjectObject.md)
+ - [ResourceExhaustedProblemDetails](docs/ResourceExhaustedProblemDetails.md)
+ - [Taxatiedata](docs/Taxatiedata.md)
+ - [Taxatiestatus](docs/Taxatiestatus.md)
+ - [ValidationProblemDetails](docs/ValidationProblemDetails.md)
+ - [VerkoopBijzonderheden](docs/VerkoopBijzonderheden.md)
+ - [VorigeVerkoop](docs/VorigeVerkoop.md)
+ - [Waardering](docs/Waardering.md)
+ - [WaarderingCbsIndeling](docs/WaarderingCbsIndeling.md)
+ - [WaarderingFactuur](docs/WaarderingFactuur.md)
+ - [WaarderingInputParameters](docs/WaarderingInputParameters.md)
+ - [WaarderingModel](docs/WaarderingModel.md)
+ - [WaarderingObject](docs/WaarderingObject.md)
+ - [WaarderingOntwikkeling](docs/WaarderingOntwikkeling.md)
+ - [WaarderingOntwikkelingKwartaal](docs/WaarderingOntwikkelingKwartaal.md)
+ - [WaarderingOntwikkelingKwartaalKwartaal](docs/WaarderingOntwikkelingKwartaalKwartaal.md)
+ - [WaarderingOrigineleInput](docs/WaarderingOrigineleInput.md)
+ - [WaarderingRapport](docs/WaarderingRapport.md)
+ - [WaarderingStatus](docs/WaarderingStatus.md)
+ - [WaarderingTaxatie](docs/WaarderingTaxatie.md)
+ - [WaarderingWebhookPayload](docs/WaarderingWebhookPayload.md)
+ - [WaarderingZoekParameters](docs/WaarderingZoekParameters.md)
+ - [WoningType](docs/WoningType.md)
+
+
+## Documentation For Authorization
+
+
+## oauth
+
+- **Type**: OAuth
+- **Flow**: application
+- **Authorization URL**: 
+- **Scopes**: 
+ - **all**: Full permissions for all areas.
+ - **api:all**: Full permissions for all areas of the public API.
+ - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:all**: Full permissions for the bodem area of the public API.
+ - **api:buurt:all**: Full permissions for the buurt area of the public API.
+ - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
+ - **api:callback:all**: Full permissions for the callback area of the public API.
+ - **api:facturen:all**: Full permissions for the facturen area of the public API.
+ - **api:fotos:all**: Full permissions for the fotos area of the public API.
+ - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
+ - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
+ - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
+ - **api:adressen:read**: Read permissions for the adressen area of the public API.
+ - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:read**: Read permissions for the bodem area of the public API.
+ - **api:buurt:read**: Read permissions for the buurt area of the public API.
+ - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
+ - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
+ - **api:callback:read**: Read permissions for the callback area of the public API.
+ - **api:callback:write**: Write permissions for the callback area of the public API.
+ - **api:facturen:read**: Read permissions for the facturen area of the public API.
+ - **api:fotos:read**: Read permissions for the fotos area of the public API.
+ - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
+ - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
+ - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
+ - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
+ - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
+ - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
+ - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
+
+
+## oauth
+
+- **Type**: OAuth
+- **Flow**: accessCode
+- **Authorization URL**: https://authentication.calcasa.nl/oauth2/v2.0/authorize
+- **Scopes**: 
+ - **all**: Full permissions for all areas.
+ - **api:all**: Full permissions for all areas of the public API.
+ - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:all**: Full permissions for the bodem area of the public API.
+ - **api:buurt:all**: Full permissions for the buurt area of the public API.
+ - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
+ - **api:callback:all**: Full permissions for the callback area of the public API.
+ - **api:facturen:all**: Full permissions for the facturen area of the public API.
+ - **api:fotos:all**: Full permissions for the fotos area of the public API.
+ - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
+ - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
+ - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
+ - **api:adressen:read**: Read permissions for the adressen area of the public API.
+ - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:read**: Read permissions for the bodem area of the public API.
+ - **api:buurt:read**: Read permissions for the buurt area of the public API.
+ - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
+ - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
+ - **api:callback:read**: Read permissions for the callback area of the public API.
+ - **api:callback:write**: Write permissions for the callback area of the public API.
+ - **api:facturen:read**: Read permissions for the facturen area of the public API.
+ - **api:fotos:read**: Read permissions for the fotos area of the public API.
+ - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
+ - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
+ - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
+ - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
+ - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
+ - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
+ - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
+
+
+## Author
+
+info@calcasa.nl
+
+
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in calcasa.api.apis and calcasa.api.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from calcasa.api.api.default_api import DefaultApi`
+- `from calcasa.api.model.pet import Pet`
+
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import calcasa.api
+from calcasa.api.apis import *
+from calcasa.api.models import *
+```
+
+
+
```

### Comparing `calcasa-api-1.2.0/README.md` & `calcasa-api-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 - Unexpected error responses in the form of [Problem Details](https://rfc-editor.org/rfc/rfc7807)
 
 ## OpenAPI Specification
 This API is documented in **OpenAPI format version 3** you can use tools like the [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) to generate API clients for for example the languages we don't provide a pre-built client for. This is documented [here](/api/v1/articles/clients/generation).
 
 ## Changelog
 
+### 2023-04-17 (v1.2.1)
+- Add `externeReferentie` field to the `CallbackInschrijving` and `WaarderingWebhookPayload` models.
+
 ### 2022-08-04 (v1.2.0)
 - Add support for managing `CallbackSubscription`'s, this allows you to subscribe to callbacks for valuations that were not created with your API client.
     - `GET /v1/callbacks/inschrijvingen`
     - `POST /v1/callbacks/inschrijvingen`
     - `GET /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
     - `DELETE /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
 - Add `taxateurnaam` field to the `Taxatiedata` model.
@@ -141,16 +144,16 @@
 - Renamed `ReferentieBijzonderheden` model to `VerkoopBijzonderheden`.
 
 ### 2021-09-22
 - Initial release of `v0`
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.2.0
-- Package version: 1.2.0
+- API version: 1.2.1
+- Package version: 1.2.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.calcasa.nl/contact](https://www.calcasa.nl/contact)
 
 ## Requirements.
 
 Python >=3.6
```

### Comparing `calcasa-api-1.2.0/calcasa/api/__init__.py` & `calcasa-api-1.2.1/calcasa/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 # import ApiClient
 from calcasa.api.api_client import ApiClient
 
 # import Configuration
 from calcasa.api.configuration import Configuration
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/adressen_api.py` & `calcasa-api-1.2.1/calcasa/api/api/adressen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/bestemmingsplannen_api.py` & `calcasa-api-1.2.1/calcasa/api/api/bestemmingsplannen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/bodem_api.py` & `calcasa-api-1.2.1/calcasa/api/api/bodem_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/buurt_api.py` & `calcasa-api-1.2.1/calcasa/api/api/buurt_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/callbacks_api.py` & `calcasa-api-1.2.1/calcasa/api/api/callbacks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/configuratie_api.py` & `calcasa-api-1.2.1/calcasa/api/api/configuratie_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/facturen_api.py` & `calcasa-api-1.2.1/calcasa/api/api/facturen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/fotos_api.py` & `calcasa-api-1.2.1/calcasa/api/api/fotos_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/funderingen_api.py` & `calcasa-api-1.2.1/calcasa/api/api/funderingen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/geldverstrekkers_api.py` & `calcasa-api-1.2.1/calcasa/api/api/geldverstrekkers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/rapporten_api.py` & `calcasa-api-1.2.1/calcasa/api/api/rapporten_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api/waarderingen_api.py` & `calcasa-api-1.2.1/calcasa/api/api/waarderingen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/api_client.py` & `calcasa-api-1.2.1/calcasa/api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import json
 import atexit
 import mimetypes
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Calcasa Python Api Client/1.2.0'
+        self.user_agent = 'Calcasa Python Api Client/1.2.1'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `calcasa-api-1.2.0/calcasa/api/apis/__init__.py` & `calcasa-api-1.2.1/calcasa/api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `calcasa-api-1.2.0/calcasa/api/configuration.py` & `calcasa-api-1.2.1/calcasa/api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
@@ -402,16 +402,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.2.0\n"\
-               "SDK Package Version: 1.2.0".\
+               "Version of the API: 1.2.1\n"\
+               "SDK Package Version: 1.2.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `calcasa-api-1.2.0/calcasa/api/exceptions.py` & `calcasa-api-1.2.1/calcasa/api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/aanvraagdoel.py` & `calcasa-api-1.2.1/calcasa/api/model/aanvraagdoel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/adres.py` & `calcasa-api-1.2.1/calcasa/api/model/adres.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/adres_info.py` & `calcasa-api-1.2.1/calcasa/api/model/adres_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/adres_info_adres.py` & `calcasa-api-1.2.1/calcasa/api/model/adres_info_adres.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/adres_info_notities.py` & `calcasa-api-1.2.1/calcasa/api/model/adres_info_notities.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/bestemmingsdata.py` & `calcasa-api-1.2.1/calcasa/api/model/bestemmingsdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/bodem_status_type.py` & `calcasa-api-1.2.1/calcasa/api/model/bodem_status_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/bodemdata.py` & `calcasa-api-1.2.1/calcasa/api/model/bodemdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/business_rules_code.py` & `calcasa-api-1.2.1/calcasa/api/model/business_rules_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/business_rules_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/business_rules_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/callback.py` & `calcasa-api-1.2.1/calcasa/api/model/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/callback_inschrijving.py` & `calcasa-api-1.2.1/calcasa/api/model/callback_inschrijving.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -85,24 +85,26 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'bag_nummeraanduiding_id': (int,),  # noqa: E501
             'geldig_tot': (datetime,),  # noqa: E501
+            'externe_referentie': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'bag_nummeraanduiding_id': 'bagNummeraanduidingId',  # noqa: E501
         'geldig_tot': 'geldigTot',  # noqa: E501
+        'externe_referentie': 'externeReferentie',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -142,14 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            externe_referentie (str, none_type): Een vrij veld dat terug komt met de callback payload om callbacks aan de juiste callback inschrijving te koppelen.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,14 +236,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            externe_referentie (str, none_type): Een vrij veld dat terug komt met de callback payload om callbacks aan de juiste callback inschrijving te koppelen.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/cbs_indeling.py` & `calcasa-api-1.2.1/calcasa/api/model/cbs_indeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/energielabel.py` & `calcasa-api-1.2.1/calcasa/api/model/energielabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/factuur.py` & `calcasa-api-1.2.1/calcasa/api/model/factuur.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/foto.py` & `calcasa-api-1.2.1/calcasa/api/model/foto.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_data_bron.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_data_bron.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_herstel_type.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_herstel_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_risico.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_risico.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_risico_label.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_risico_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_soort_bron.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_soort_bron.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_type.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/fundering_typering.py` & `calcasa-api-1.2.1/calcasa/api/model/fundering_typering.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/funderingdata.py` & `calcasa-api-1.2.1/calcasa/api/model/funderingdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/funderingdata_bio_infectie_risico.py` & `calcasa-api-1.2.1/calcasa/api/model/funderingdata_bio_infectie_risico.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/funderingdata_droogstand_risico.py` & `calcasa-api-1.2.1/calcasa/api/model/funderingdata_droogstand_risico.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/funderingdata_optrekkend_vocht_risico.py` & `calcasa-api-1.2.1/calcasa/api/model/funderingdata_optrekkend_vocht_risico.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/funderingdata_typering.py` & `calcasa-api-1.2.1/calcasa/api/model/funderingdata_typering.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/gebiedsdata.py` & `calcasa-api-1.2.1/calcasa/api/model/gebiedsdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/geldverstrekker.py` & `calcasa-api-1.2.1/calcasa/api/model/geldverstrekker.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/http_validation_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/http_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/invalid_argument_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/invalid_argument_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/json_patch_document.py` & `calcasa-api-1.2.1/calcasa/api/model/json_patch_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/klantwaarde_type.py` & `calcasa-api-1.2.1/calcasa/api/model/klantwaarde_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/kwartaal.py` & `calcasa-api-1.2.1/calcasa/api/model/kwartaal.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/modeldata.py` & `calcasa-api-1.2.1/calcasa/api/model/modeldata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/not_found_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/not_found_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/notitie.py` & `calcasa-api-1.2.1/calcasa/api/model/notitie.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/notities.py` & `calcasa-api-1.2.1/calcasa/api/model/notities.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/objectdata.py` & `calcasa-api-1.2.1/calcasa/api/model/objectdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_buurt.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_buurt.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_gemeente.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_gemeente.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_land.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_land.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_provincie.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_provincie.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/omgevingsdata_wijk.py` & `calcasa-api-1.2.1/calcasa/api/model/omgevingsdata_wijk.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/operation.py` & `calcasa-api-1.2.1/calcasa/api/model/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/operation_type.py` & `calcasa-api-1.2.1/calcasa/api/model/operation_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/permissions_denied_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/permissions_denied_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/product_type.py` & `calcasa-api-1.2.1/calcasa/api/model/product_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/rapport.py` & `calcasa-api-1.2.1/calcasa/api/model/rapport.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/referentieobject.py` & `calcasa-api-1.2.1/calcasa/api/model/referentieobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/referentieobject_adres.py` & `calcasa-api-1.2.1/calcasa/api/model/referentieobject_adres.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/referentieobject_cbs_indeling.py` & `calcasa-api-1.2.1/calcasa/api/model/referentieobject_cbs_indeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/referentieobject_object.py` & `calcasa-api-1.2.1/calcasa/api/model/referentieobject_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/resource_exhausted_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/resource_exhausted_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/taxatiedata.py` & `calcasa-api-1.2.1/calcasa/api/model/taxatiedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/taxatiestatus.py` & `calcasa-api-1.2.1/calcasa/api/model/taxatiestatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/validation_problem_details.py` & `calcasa-api-1.2.1/calcasa/api/model/validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/verkoop_bijzonderheden.py` & `calcasa-api-1.2.1/calcasa/api/model/verkoop_bijzonderheden.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/vorige_verkoop.py` & `calcasa-api-1.2.1/calcasa/api/model/vorige_verkoop.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_cbs_indeling.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_cbs_indeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_factuur.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_factuur.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_input_parameters.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_input_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_model.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_object.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling_kwartaal.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling_kwartaal.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_ontwikkeling_kwartaal_kwartaal.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_ontwikkeling_kwartaal_kwartaal.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_originele_input.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_originele_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_rapport.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_rapport.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_status.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_taxatie.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_taxatie.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_webhook_payload.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_webhook_payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -95,14 +95,15 @@
             'callback_name': (str,),  # noqa: E501
             'event_id': (str,),  # noqa: E501
             'waardering_id': (str,),  # noqa: E501
             'old_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'new_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'timestamp': (datetime,),  # noqa: E501
             'is_test': (bool,),  # noqa: E501
+            'externe_referentie': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -110,14 +111,15 @@
         'callback_name': 'callbackName',  # noqa: E501
         'event_id': 'eventId',  # noqa: E501
         'waardering_id': 'waarderingId',  # noqa: E501
         'old_status': 'oldStatus',  # noqa: E501
         'new_status': 'newStatus',  # noqa: E501
         'timestamp': 'timestamp',  # noqa: E501
         'is_test': 'isTest',  # noqa: E501
+        'externe_referentie': 'externeReferentie',  # noqa: E501
     }
 
     read_only_vars = {
         'callback_name',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -161,14 +163,15 @@
             callback_name (str): [optional]  # noqa: E501
             event_id (str): Uniek Id voor deze callback.. [optional]  # noqa: E501
             waardering_id (str): Het Id van de waardering waarop deze callback betrekking heeft.. [optional]  # noqa: E501
             old_status (bool, date, datetime, dict, float, int, list, str, none_type): De oude status van de waardering. | Waarde | Omschrijving | | --- | --- | | `onbekend` | Status onbekend. | | `initialiseren` | Deze waardering is geinitialiseerd maar moet nog bevestigd worden. | | `open` | Deze waardering is bevestigd maar moet nog uitgevoerd worden. | | `voltooid` | Deze waardering is voltooid. | | `opgewaardeerd` | Deze waardering is geupgrade naar een ander waardering type. | | `ongeldig` | Deze waardering is niet geldig, bijvoorbeeld omdat hij niet door de business rules is gekomen. | | `verlopen` | Deze waardering is verlopen omdat hij niet op tijd bevestigd is. | | `error` | Er is iets mis gegaan voor deze waardering. | | `inBehandeling` | Deze waardering is in behandeling door het systeem. |   . [optional]  # noqa: E501
             new_status (bool, date, datetime, dict, float, int, list, str, none_type): De nieuwe status van de waardering. | Waarde | Omschrijving | | --- | --- | | `onbekend` | Status onbekend. | | `initialiseren` | Deze waardering is geinitialiseerd maar moet nog bevestigd worden. | | `open` | Deze waardering is bevestigd maar moet nog uitgevoerd worden. | | `voltooid` | Deze waardering is voltooid. | | `opgewaardeerd` | Deze waardering is geupgrade naar een ander waardering type. | | `ongeldig` | Deze waardering is niet geldig, bijvoorbeeld omdat hij niet door de business rules is gekomen. | | `verlopen` | Deze waardering is verlopen omdat hij niet op tijd bevestigd is. | | `error` | Er is iets mis gegaan voor deze waardering. | | `inBehandeling` | Deze waardering is in behandeling door het systeem. |   . [optional]  # noqa: E501
             timestamp (datetime): Het tijdstip van het event, in UTC.. [optional]  # noqa: E501
             is_test (bool): Geeft aan of de betreffende waardering aangevraagd is met een test token.. [optional]  # noqa: E501
+            externe_referentie (str, none_type): Dit is de externe referentie opgegeven bij de callback inschrijving of als dit een normale API waardering is waarvoor geen callback inschrijving was dit veld null.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,14 +256,15 @@
             callback_name (str): [optional]  # noqa: E501
             event_id (str): Uniek Id voor deze callback.. [optional]  # noqa: E501
             waardering_id (str): Het Id van de waardering waarop deze callback betrekking heeft.. [optional]  # noqa: E501
             old_status (bool, date, datetime, dict, float, int, list, str, none_type): De oude status van de waardering. | Waarde | Omschrijving | | --- | --- | | `onbekend` | Status onbekend. | | `initialiseren` | Deze waardering is geinitialiseerd maar moet nog bevestigd worden. | | `open` | Deze waardering is bevestigd maar moet nog uitgevoerd worden. | | `voltooid` | Deze waardering is voltooid. | | `opgewaardeerd` | Deze waardering is geupgrade naar een ander waardering type. | | `ongeldig` | Deze waardering is niet geldig, bijvoorbeeld omdat hij niet door de business rules is gekomen. | | `verlopen` | Deze waardering is verlopen omdat hij niet op tijd bevestigd is. | | `error` | Er is iets mis gegaan voor deze waardering. | | `inBehandeling` | Deze waardering is in behandeling door het systeem. |   . [optional]  # noqa: E501
             new_status (bool, date, datetime, dict, float, int, list, str, none_type): De nieuwe status van de waardering. | Waarde | Omschrijving | | --- | --- | | `onbekend` | Status onbekend. | | `initialiseren` | Deze waardering is geinitialiseerd maar moet nog bevestigd worden. | | `open` | Deze waardering is bevestigd maar moet nog uitgevoerd worden. | | `voltooid` | Deze waardering is voltooid. | | `opgewaardeerd` | Deze waardering is geupgrade naar een ander waardering type. | | `ongeldig` | Deze waardering is niet geldig, bijvoorbeeld omdat hij niet door de business rules is gekomen. | | `verlopen` | Deze waardering is verlopen omdat hij niet op tijd bevestigd is. | | `error` | Er is iets mis gegaan voor deze waardering. | | `inBehandeling` | Deze waardering is in behandeling door het systeem. |   . [optional]  # noqa: E501
             timestamp (datetime): Het tijdstip van het event, in UTC.. [optional]  # noqa: E501
             is_test (bool): Geeft aan of de betreffende waardering aangevraagd is met een test token.. [optional]  # noqa: E501
+            externe_referentie (str, none_type): Dit is de externe referentie opgegeven bij de callback inschrijving of als dit een normale API waardering is waarvoor geen callback inschrijving was dit veld null.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/waardering_zoek_parameters.py` & `calcasa-api-1.2.1/calcasa/api/model/waardering_zoek_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model/woning_type.py` & `calcasa-api-1.2.1/calcasa/api/model/woning_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `calcasa-api-1.2.0/calcasa/api/model_utils.py` & `calcasa-api-1.2.1/calcasa/api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `calcasa-api-1.2.0/calcasa/api/models/__init__.py` & `calcasa-api-1.2.1/calcasa/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `calcasa-api-1.2.0/calcasa/api/rest.py` & `calcasa-api-1.2.1/calcasa/api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 import io
 import json
 import logging
```

### Comparing `calcasa-api-1.2.0/calcasa_api.egg-info/PKG-INFO` & `calcasa-api-1.2.1/calcasa_api.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,465 +1,471 @@
 Metadata-Version: 2.1
 Name: calcasa-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Calcasa Public API v1
 Home-page: https://github.com/calcasa/api-python
 Author: Calcasa B.V.
 Author-email: info@calcasa.nl
 License: Apache-2.0
-Description: # calcasa-api
-        The Calcasa API is used to connect to Calcasa provided services. This is the first production version of the service
-        
-        ## Client packages
-        [Nuget](https://www.nuget.org/packages/Calcasa.Api) - [Packagist](https://packagist.org/packages/calcasa/api) - [PyPI](https://pypi.org/project/calcasa.api)
-        ## Client implementation notes
-        Clients should at all times be tolerant to the following:
-        
-        - Extra fields in responses
-        - Empty or hidden fields in responses
-        - Extra values in enumerations
-        - Unexpected error responses in the form of [Problem Details](https://rfc-editor.org/rfc/rfc7807)
-        
-        ## OpenAPI Specification
-        This API is documented in **OpenAPI format version 3** you can use tools like the [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) to generate API clients for for example the languages we don't provide a pre-built client for. This is documented [here](/api/v1/articles/clients/generation).
-        
-        ## Changelog
-        
-        ### 2022-08-04 (v1.2.0)
-        - Add support for managing `CallbackSubscription`'s, this allows you to subscribe to callbacks for valuations that were not created with your API client.
-            - `GET /v1/callbacks/inschrijvingen`
-            - `POST /v1/callbacks/inschrijvingen`
-            - `GET /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
-            - `DELETE /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
-        - Add `taxateurnaam` field to the `Taxatiedata` model.
-        - Callback URIs should now end in `/` not just contain it to help stop common errors (ending in `=` is also still allowed when using a query string).
-        - Updating configuration in the `POST /v1/configuratie/callbacks` endpoint now clears stored but decommissioned versions from the configuration object.
-        - Add `klantkenmerk` to the `WaarderingInputParameters` and `Waardering` models.
-        
-        ### 2022-07-12 (v1.1.7)
-        - Added support for the OAuth 2.0 authorization code flow for use of the API with user accounts.
-        - Add `bouweenheid` to `FunderingSoortBron` enumeration.
-        
-        ### 2022-05-19 (v1.1.6)
-        - Added `ltvTeHoogOverbrugging` value to the `BusinessRulesCode` enumeration.
-        
-        ### 2022-04-13 (v1.1.5)
-        - Fix the schema for `Operation` `value` field for the benefit of the PHP and Python code generators, these will now correctly support any value type.
-        
-        ### 2022-04-12 (v1.1.4)
-        - Added proper Content-Disposition headers to the `GET /v1/rapporten/{id}` and `GET /v1/facturen/{id}` endpoints with the correct filename.
-        - Fix Mime Types for the `POST /v1/configuratie/callbacks` endpoint to only accept `application/json`.
-        - Fix C# API client to correctly use the `application/json-patch+json` content type in requests that require it.
-        - Fix C# client's `FileParameter` type correct handling of response headers like `Content-Disposition` and `Content-Type`.
-        - Removed C# client's useless implementation of `IValidatableObject`.
-        - Fix Python client's internal namespace name being illegal `calcasa-api` -> `calcasa.api`.
-        
-        ### 2022-03-22 (v1.1.3)
-        - Add 402 (Payment required) and 422 (Unprocessable entity) as potential response for `PATCH /v1/waarderingen/{id}`.
-        
-        ### 2022-03-17 (v1.1.2)
-        - Fixed response type for `GET /v1/geldverstrekkers/{productType}` endpoint.
-        
-        ### 2022-03-08 (v1.1.1)
-        - Added `GET /v1/geldverstrekkers/{productType}` endpoint.
-        - Restored all `ProblemDetails` models.
-        
-        ### 2022-03-07 (v1.1.0)
-        - Added `isErfpacht` to `WaarderingInputParameters`.
-        - Cleaned up serialization of null values, they should no longer appear in the output.
-        
-        ### 2021-02-04
-        - Added extra clarification to the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different input parameter combinations.
-        
-        ### 2022-01-11 (v1.0.2)
-        - Fixed `GET /api/v1/bodem/{id}` endpoint path parameter description, query parameter was never meant to be there.
-        
-        ### 2021-12-23
-        - Clarified the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different product types.
-        
-        ### 2021-12-22 (v1.0.1)
-        - Dates are now serialized in the ISO date-only format `yyyy-MM-dd` to stop any confusion around timezones and are all assumed to be in UTC.
-            - `peildatum` in `WaarderingsInputParameters`
-            - `datum_bestemmingplan` in `Bestemmingsdata`
-            - `datum_laatste_onderzoek` in `Bodemdata`
-            - `verkoopdatum` in `Referentieobject`
-            - `verkoopdatum` in `VorigeVerkoop`
-            - `waardebepalingsdatum` in `Modeldata`
-        - Reintroduced the `WaarderingWebhookPayload` model that was omitted.
-        
-        ### 2021-12-21
-        - Patching the status of a `Waardering` object will now immediatly reflect its new status in the response object.
-        
-        ### 2021-12-13 (v1.0.0)
-        - Initial release of `v1` based on `v0.0.6`
-        
-        ## Cross-Origin Resource Sharing
-        This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).
-        And that allows cross-domain communication from the browser.
-        All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.
-        
-        ## Authentication
-        Authentication is done via [OAuth2](https://oauth.net/2/) and the [client credentials](https://oauth.net/2/grant-types/client-credentials/) grant type.
-        
-        ## Previous versions changelogs
-        
-        ### 2022-02-02
-        - API version `v0` was removed from service.
-        
-        ### 2021-12-23
-        - Mark `v0` as officially deprecated. No further versions will be released. Every implementation should move to `v1`
-        
-        ### 2021-12-10 (v0.0.6)
-        - Added extra field `peildatum` to the `WaarderingInputParameters` model.
-        
-        ### 2021-11-25 (v0.0.5)
-        - Updated all reported OAuth2 scopes and reduced the superflous scope information on each endpoint.
-        
-        ### 2021-11-23 (v0.0.4)
-        - Added per square meter developments to the `WaarderingOntwikkeling` object (fields with the `PerVierkantemeter` suffix).
-        
-        ### 2021-11-15 (v0.0.3)
-        - Added callback update and read endpoints and models.
-        - Updated documentation.
-        
-        ### 2021-11-11
-        - Renamed /fundering endpoint to /funderingen to be more in line with other endpoints
-        - Renamed `HerstelType` to `FunderingHerstelType`.
-        - Added `FunderingType` values.
-        
-        ### 2021-11-10
-        - Adjusted OpenAPI Spec generation to fix some issues with certain generators. This also means that the nullable nature of certain fields is now correctly represented. Please refer to the Generation article for more information, the config files were updated aswell.
-        
-        ### 2021-11-09
-        - Added `Status` and `Taxatiedatum` to `Taxatiedata` model.
-        
-        ### 2021-11-08
-        - Renamed `id` field in `AdresInfo` model to `bagNummeraanduidingId`.
-        - Added `GET /v0/fundering/{id}` endpoint with corresponding models.
-        - Changed HTTP response code for the `BusinessRulesProblemDetails` error return type of `POST /v0/waardering` from `422 Unprocessable Entity` to `406 Not Acceptable` to fix a duplicate.
-        
-        ### 2021-10-13
-        - Added `taxatie` field to `Waardering` model.
-        - Added `Taxatiedata` model containing the `taxatieorganisatie` field for desktop valuations.
-        
-        ### 2021-09-29
-        - Added `aangemaakt` timestamp field to `Waardering` model.
-        - Added `WaarderingZoekParameters` model to replace `WaarderingInputParameters` in the `POST /v0/waarderingen/zoeken` endpoint.
-        - Split `Omgevingsdata` model into a set of separate `Gebiedsdata` models that also contain extra statistics.
-        - Added `bijzonderheden` field to `VorigeVerkoop` model.
-        - Renamed `ReferentieBijzonderheden` model to `VerkoopBijzonderheden`.
-        
-        ### 2021-09-22
-        - Initial release of `v0`
-        
-        This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-        
-        - API version: 1.2.0
-        - Package version: 1.2.0
-        - Build package: org.openapitools.codegen.languages.PythonClientCodegen
-        For more information, please visit [https://www.calcasa.nl/contact](https://www.calcasa.nl/contact)
-        
-        ## Requirements.
-        
-        Python >=3.6
-        
-        ## Installation & Usage
-        ### pip install
-        
-        If the python package is hosted on a repository, you can install directly using:
-        
-        ```sh
-        pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-        ```
-        (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-        
-        Then import the package:
-        ```python
-        import calcasa.api
-        ```
-        
-        ### Setuptools
-        
-        Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-        
-        ```sh
-        python setup.py install --user
-        ```
-        (or `sudo python setup.py install` to install the package for all users)
-        
-        Then import the package:
-        ```python
-        import calcasa.api
-        ```
-        
-        ## Getting Started
-        
-        Please follow the [installation procedure](#installation--usage) and then run the following:
-        
-        ```python
-        
-        import time
-        import calcasa.api
-        from pprint import pprint
-        from calcasa.api.api import adressen_api
-        from calcasa.api.model.adres import Adres
-        from calcasa.api.model.adres_info import AdresInfo
-        from calcasa.api.model.not_found_problem_details import NotFoundProblemDetails
-        from calcasa.api.model.permissions_denied_problem_details import PermissionsDeniedProblemDetails
-        from calcasa.api.model.problem_details import ProblemDetails
-        # Defining the host is optional and defaults to https://api.calcasa.nl
-        # See configuration.py for a list of all supported configuration parameters.
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        
-        # The client must configure the authentication and authorization parameters
-        # in accordance with the API server security policy.
-        # Examples for each auth method are provided below, use the example that
-        # satisfies your auth use case.
-        
-        # Configure OAuth2 access token for authorization: oauth
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        configuration.access_token = 'YOUR_ACCESS_TOKEN'
-        
-        # Configure OAuth2 access token for authorization: oauth
-        configuration = calcasa.api.Configuration(
-            host = "https://api.calcasa.nl"
-        )
-        configuration.access_token = 'YOUR_ACCESS_TOKEN'
-        
-        
-        # Enter a context with an instance of the API client
-        with calcasa.api.ApiClient(configuration) as api_client:
-            # Create an instance of the API class
-            api_instance = adressen_api.AdressenApi(api_client)
-            bag_nummeraanduiding_id = 1 # int | Een BAG Nummeraanduiding ID om een adres te specificeren.
-        
-            try:
-                # Adres info op basis van BAG Nummeraanduiding Id.
-                api_response = api_instance.get_adres(bag_nummeraanduiding_id)
-                pprint(api_response)
-            except calcasa.api.ApiException as e:
-                print("Exception when calling AdressenApi->get_adres: %s\n" % e)
-        ```
-        
-        ## Documentation for API Endpoints
-        
-        All URIs are relative to *https://api.calcasa.nl*
-        
-        Class | Method | HTTP request | Description
-        ------------ | ------------- | ------------- | -------------
-        *AdressenApi* | [**get_adres**](docs/AdressenApi.md#get_adres) | **GET** /api/v1/adressen/{bagNummeraanduidingId} | Adres info op basis van BAG Nummeraanduiding Id.
-        *AdressenApi* | [**search_adres**](docs/AdressenApi.md#search_adres) | **POST** /api/v1/adressen/zoeken | Zoek adres info op basis van het gegeven adres.
-        *BestemmingsplannenApi* | [**get_bestemming_by_id**](docs/BestemmingsplannenApi.md#get_bestemming_by_id) | **GET** /api/v1/bestemmingsplannen/{bagNummeraanduidingId} | Gegevens over de bestemmingsplannen op de locatie van een adres (BAG Nummeraanduiding ID).
-        *BodemApi* | [**get_bodem_by_id**](docs/BodemApi.md#get_bodem_by_id) | **GET** /api/v1/bodem/{bagNummeraanduidingId} | Gegevens over de bodemkwaliteit op de locatie van een adres (BAG Nummeraanduiding ID).
-        *BuurtApi* | [**get_buurt**](docs/BuurtApi.md#get_buurt) | **GET** /api/v1/buurt/{buurtId} | Gegevens over een buurt en de wijk, gemeente en land waarin deze buurt gesitueerd is.
-        *CallbacksApi* | [**add_or_update_callback_subscription**](docs/CallbacksApi.md#add_or_update_callback_subscription) | **POST** /api/v1/callbacks/inschrijvingen | Voeg een callback inschrijving toe (of werk bij) voor de huidige client voor een adres.
-        *CallbacksApi* | [**delete_notification_subscription**](docs/CallbacksApi.md#delete_notification_subscription) | **DELETE** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Verwijder de callback inschrijving voor deze client en dit adres.
-        *CallbacksApi* | [**get_notification_subscription**](docs/CallbacksApi.md#get_notification_subscription) | **GET** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Haal de callback inschrijving op voor deze client en dit adres.
-        *CallbacksApi* | [**get_notification_subscriptions**](docs/CallbacksApi.md#get_notification_subscriptions) | **GET** /api/v1/callbacks/inschrijvingen | Haal de callback inschrijvingen binnen voor deze client.
-        *ConfiguratieApi* | [**get_callbacks**](docs/ConfiguratieApi.md#get_callbacks) | **GET** /api/v1/configuratie/callbacks | Haal de geconfigureerde callback URL&#39;s op voor de huidige client.
-        *ConfiguratieApi* | [**update_callbacks**](docs/ConfiguratieApi.md#update_callbacks) | **POST** /api/v1/configuratie/callbacks | Configureer callback URL voor een specifieke API versie voor de huidige client.
-        *FacturenApi* | [**get_factuur**](docs/FacturenApi.md#get_factuur) | **GET** /api/v1/facturen/{id} | Factuur op basis van een waardering Id.
-        *FotosApi* | [**get_foto**](docs/FotosApi.md#get_foto) | **GET** /api/v1/fotos/{id} | Foto op basis van een foto Id.
-        *FunderingenApi* | [**get_fundering_by_id**](docs/FunderingenApi.md#get_fundering_by_id) | **GET** /api/v1/funderingen/{bagNummeraanduidingId} | Gegevens over de fundering op de locatie van een adres (BAG Nummeraanduiding ID).
-        *GeldverstrekkersApi* | [**get_geldverstrekkers**](docs/GeldverstrekkersApi.md#get_geldverstrekkers) | **GET** /api/v1/geldverstrekkers/{productType} | Alle geldverstrekkers die te gebruiken zijn voor aanvragen.
-        *RapportenApi* | [**get_rapport**](docs/RapportenApi.md#get_rapport) | **GET** /api/v1/rapporten/{id} | Rapport op basis van waardering Id.
-        *WaarderingenApi* | [**create_waardering**](docs/WaarderingenApi.md#create_waardering) | **POST** /api/v1/waarderingen | Creërt een waardering.
-        *WaarderingenApi* | [**get_waardering**](docs/WaarderingenApi.md#get_waardering) | **GET** /api/v1/waarderingen/{id} | Waardering op basis van Id.
-        *WaarderingenApi* | [**get_waardering_ontwikkeling**](docs/WaarderingenApi.md#get_waardering_ontwikkeling) | **GET** /api/v1/waarderingen/{id}/ontwikkeling | Waardering ontwikkeling op basis van waardering Id.
-        *WaarderingenApi* | [**patch_waarderingen**](docs/WaarderingenApi.md#patch_waarderingen) | **PATCH** /api/v1/waarderingen/{id} | Patcht een waardering.
-        *WaarderingenApi* | [**search_waarderingen**](docs/WaarderingenApi.md#search_waarderingen) | **POST** /api/v1/waarderingen/zoeken | Zoek waardering op basis van input parameters.
-        
-        
-        ## Documentation For Models
-        
-         - [Aanvraagdoel](docs/Aanvraagdoel.md)
-         - [Adres](docs/Adres.md)
-         - [AdresInfo](docs/AdresInfo.md)
-         - [AdresInfoAdres](docs/AdresInfoAdres.md)
-         - [AdresInfoNotities](docs/AdresInfoNotities.md)
-         - [Bestemmingsdata](docs/Bestemmingsdata.md)
-         - [BodemStatusType](docs/BodemStatusType.md)
-         - [Bodemdata](docs/Bodemdata.md)
-         - [BusinessRulesCode](docs/BusinessRulesCode.md)
-         - [BusinessRulesProblemDetails](docs/BusinessRulesProblemDetails.md)
-         - [Callback](docs/Callback.md)
-         - [CallbackInschrijving](docs/CallbackInschrijving.md)
-         - [CbsIndeling](docs/CbsIndeling.md)
-         - [Energielabel](docs/Energielabel.md)
-         - [Factuur](docs/Factuur.md)
-         - [Foto](docs/Foto.md)
-         - [FunderingDataBron](docs/FunderingDataBron.md)
-         - [FunderingHerstelType](docs/FunderingHerstelType.md)
-         - [FunderingRisico](docs/FunderingRisico.md)
-         - [FunderingRisicoLabel](docs/FunderingRisicoLabel.md)
-         - [FunderingSoortBron](docs/FunderingSoortBron.md)
-         - [FunderingType](docs/FunderingType.md)
-         - [FunderingTypering](docs/FunderingTypering.md)
-         - [Funderingdata](docs/Funderingdata.md)
-         - [FunderingdataBioInfectieRisico](docs/FunderingdataBioInfectieRisico.md)
-         - [FunderingdataDroogstandRisico](docs/FunderingdataDroogstandRisico.md)
-         - [FunderingdataOptrekkendVochtRisico](docs/FunderingdataOptrekkendVochtRisico.md)
-         - [FunderingdataTypering](docs/FunderingdataTypering.md)
-         - [Gebiedsdata](docs/Gebiedsdata.md)
-         - [Geldverstrekker](docs/Geldverstrekker.md)
-         - [HttpValidationProblemDetails](docs/HttpValidationProblemDetails.md)
-         - [InvalidArgumentProblemDetails](docs/InvalidArgumentProblemDetails.md)
-         - [JsonPatchDocument](docs/JsonPatchDocument.md)
-         - [KlantwaardeType](docs/KlantwaardeType.md)
-         - [Kwartaal](docs/Kwartaal.md)
-         - [Modeldata](docs/Modeldata.md)
-         - [NotFoundProblemDetails](docs/NotFoundProblemDetails.md)
-         - [Notitie](docs/Notitie.md)
-         - [Notities](docs/Notities.md)
-         - [Objectdata](docs/Objectdata.md)
-         - [Omgevingsdata](docs/Omgevingsdata.md)
-         - [OmgevingsdataBuurt](docs/OmgevingsdataBuurt.md)
-         - [OmgevingsdataGemeente](docs/OmgevingsdataGemeente.md)
-         - [OmgevingsdataLand](docs/OmgevingsdataLand.md)
-         - [OmgevingsdataProvincie](docs/OmgevingsdataProvincie.md)
-         - [OmgevingsdataWijk](docs/OmgevingsdataWijk.md)
-         - [Operation](docs/Operation.md)
-         - [OperationType](docs/OperationType.md)
-         - [PermissionsDeniedProblemDetails](docs/PermissionsDeniedProblemDetails.md)
-         - [ProblemDetails](docs/ProblemDetails.md)
-         - [ProductType](docs/ProductType.md)
-         - [Rapport](docs/Rapport.md)
-         - [Referentieobject](docs/Referentieobject.md)
-         - [ReferentieobjectAdres](docs/ReferentieobjectAdres.md)
-         - [ReferentieobjectCbsIndeling](docs/ReferentieobjectCbsIndeling.md)
-         - [ReferentieobjectObject](docs/ReferentieobjectObject.md)
-         - [ResourceExhaustedProblemDetails](docs/ResourceExhaustedProblemDetails.md)
-         - [Taxatiedata](docs/Taxatiedata.md)
-         - [Taxatiestatus](docs/Taxatiestatus.md)
-         - [ValidationProblemDetails](docs/ValidationProblemDetails.md)
-         - [VerkoopBijzonderheden](docs/VerkoopBijzonderheden.md)
-         - [VorigeVerkoop](docs/VorigeVerkoop.md)
-         - [Waardering](docs/Waardering.md)
-         - [WaarderingCbsIndeling](docs/WaarderingCbsIndeling.md)
-         - [WaarderingFactuur](docs/WaarderingFactuur.md)
-         - [WaarderingInputParameters](docs/WaarderingInputParameters.md)
-         - [WaarderingModel](docs/WaarderingModel.md)
-         - [WaarderingObject](docs/WaarderingObject.md)
-         - [WaarderingOntwikkeling](docs/WaarderingOntwikkeling.md)
-         - [WaarderingOntwikkelingKwartaal](docs/WaarderingOntwikkelingKwartaal.md)
-         - [WaarderingOntwikkelingKwartaalKwartaal](docs/WaarderingOntwikkelingKwartaalKwartaal.md)
-         - [WaarderingOrigineleInput](docs/WaarderingOrigineleInput.md)
-         - [WaarderingRapport](docs/WaarderingRapport.md)
-         - [WaarderingStatus](docs/WaarderingStatus.md)
-         - [WaarderingTaxatie](docs/WaarderingTaxatie.md)
-         - [WaarderingWebhookPayload](docs/WaarderingWebhookPayload.md)
-         - [WaarderingZoekParameters](docs/WaarderingZoekParameters.md)
-         - [WoningType](docs/WoningType.md)
-        
-        
-        ## Documentation For Authorization
-        
-        
-        ## oauth
-        
-        - **Type**: OAuth
-        - **Flow**: application
-        - **Authorization URL**: 
-        - **Scopes**: 
-         - **all**: Full permissions for all areas.
-         - **api:all**: Full permissions for all areas of the public API.
-         - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:all**: Full permissions for the bodem area of the public API.
-         - **api:buurt:all**: Full permissions for the buurt area of the public API.
-         - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
-         - **api:callback:all**: Full permissions for the callback area of the public API.
-         - **api:facturen:all**: Full permissions for the facturen area of the public API.
-         - **api:fotos:all**: Full permissions for the fotos area of the public API.
-         - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
-         - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
-         - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
-         - **api:adressen:read**: Read permissions for the adressen area of the public API.
-         - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:read**: Read permissions for the bodem area of the public API.
-         - **api:buurt:read**: Read permissions for the buurt area of the public API.
-         - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
-         - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
-         - **api:callback:read**: Read permissions for the callback area of the public API.
-         - **api:callback:write**: Write permissions for the callback area of the public API.
-         - **api:facturen:read**: Read permissions for the facturen area of the public API.
-         - **api:fotos:read**: Read permissions for the fotos area of the public API.
-         - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
-         - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
-         - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
-         - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
-         - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
-         - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
-         - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
-        
-        
-        ## oauth
-        
-        - **Type**: OAuth
-        - **Flow**: accessCode
-        - **Authorization URL**: https://authentication.calcasa.nl/oauth2/v2.0/authorize
-        - **Scopes**: 
-         - **all**: Full permissions for all areas.
-         - **api:all**: Full permissions for all areas of the public API.
-         - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:all**: Full permissions for the bodem area of the public API.
-         - **api:buurt:all**: Full permissions for the buurt area of the public API.
-         - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
-         - **api:callback:all**: Full permissions for the callback area of the public API.
-         - **api:facturen:all**: Full permissions for the facturen area of the public API.
-         - **api:fotos:all**: Full permissions for the fotos area of the public API.
-         - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
-         - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
-         - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
-         - **api:adressen:read**: Read permissions for the adressen area of the public API.
-         - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
-         - **api:bodem:read**: Read permissions for the bodem area of the public API.
-         - **api:buurt:read**: Read permissions for the buurt area of the public API.
-         - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
-         - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
-         - **api:callback:read**: Read permissions for the callback area of the public API.
-         - **api:callback:write**: Write permissions for the callback area of the public API.
-         - **api:facturen:read**: Read permissions for the facturen area of the public API.
-         - **api:fotos:read**: Read permissions for the fotos area of the public API.
-         - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
-         - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
-         - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
-         - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
-         - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
-         - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
-         - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
-        
-        
-        ## Author
-        
-        info@calcasa.nl
-        
-        
-        ## Notes for Large OpenAPI documents
-        If the OpenAPI document is large, imports in calcasa.api.apis and calcasa.api.models may fail with a
-        RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
-        
-        Solution 1:
-        Use specific imports for apis and models like:
-        - `from calcasa.api.api.default_api import DefaultApi`
-        - `from calcasa.api.model.pet import Pet`
-        
-        Solution 2:
-        Before importing the package, adjust the maximum recursion limit as shown below:
-        ```
-        import sys
-        sys.setrecursionlimit(1500)
-        import calcasa.api
-        from calcasa.api.apis import *
-        from calcasa.api.models import *
-        ```
-        
-        
 Keywords: OpenAPI,OpenAPI-Generator,Calcasa Public API v1
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE
+
+# calcasa-api
+The Calcasa API is used to connect to Calcasa provided services. This is the first production version of the service
+
+## Client packages
+[Nuget](https://www.nuget.org/packages/Calcasa.Api) - [Packagist](https://packagist.org/packages/calcasa/api) - [PyPI](https://pypi.org/project/calcasa.api)
+## Client implementation notes
+Clients should at all times be tolerant to the following:
+
+- Extra fields in responses
+- Empty or hidden fields in responses
+- Extra values in enumerations
+- Unexpected error responses in the form of [Problem Details](https://rfc-editor.org/rfc/rfc7807)
+
+## OpenAPI Specification
+This API is documented in **OpenAPI format version 3** you can use tools like the [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) to generate API clients for for example the languages we don't provide a pre-built client for. This is documented [here](/api/v1/articles/clients/generation).
+
+## Changelog
+
+### 2023-04-17 (v1.2.1)
+- Add `externeReferentie` field to the `CallbackInschrijving` and `WaarderingWebhookPayload` models.
+
+### 2022-08-04 (v1.2.0)
+- Add support for managing `CallbackSubscription`'s, this allows you to subscribe to callbacks for valuations that were not created with your API client.
+    - `GET /v1/callbacks/inschrijvingen`
+    - `POST /v1/callbacks/inschrijvingen`
+    - `GET /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
+    - `DELETE /v1/callbacks/inschrijvingen/{bagNummeraanduidingId}`
+- Add `taxateurnaam` field to the `Taxatiedata` model.
+- Callback URIs should now end in `/` not just contain it to help stop common errors (ending in `=` is also still allowed when using a query string).
+- Updating configuration in the `POST /v1/configuratie/callbacks` endpoint now clears stored but decommissioned versions from the configuration object.
+- Add `klantkenmerk` to the `WaarderingInputParameters` and `Waardering` models.
+
+### 2022-07-12 (v1.1.7)
+- Added support for the OAuth 2.0 authorization code flow for use of the API with user accounts.
+- Add `bouweenheid` to `FunderingSoortBron` enumeration.
+
+### 2022-05-19 (v1.1.6)
+- Added `ltvTeHoogOverbrugging` value to the `BusinessRulesCode` enumeration.
+
+### 2022-04-13 (v1.1.5)
+- Fix the schema for `Operation` `value` field for the benefit of the PHP and Python code generators, these will now correctly support any value type.
+
+### 2022-04-12 (v1.1.4)
+- Added proper Content-Disposition headers to the `GET /v1/rapporten/{id}` and `GET /v1/facturen/{id}` endpoints with the correct filename.
+- Fix Mime Types for the `POST /v1/configuratie/callbacks` endpoint to only accept `application/json`.
+- Fix C# API client to correctly use the `application/json-patch+json` content type in requests that require it.
+- Fix C# client's `FileParameter` type correct handling of response headers like `Content-Disposition` and `Content-Type`.
+- Removed C# client's useless implementation of `IValidatableObject`.
+- Fix Python client's internal namespace name being illegal `calcasa-api` -> `calcasa.api`.
+
+### 2022-03-22 (v1.1.3)
+- Add 402 (Payment required) and 422 (Unprocessable entity) as potential response for `PATCH /v1/waarderingen/{id}`.
+
+### 2022-03-17 (v1.1.2)
+- Fixed response type for `GET /v1/geldverstrekkers/{productType}` endpoint.
+
+### 2022-03-08 (v1.1.1)
+- Added `GET /v1/geldverstrekkers/{productType}` endpoint.
+- Restored all `ProblemDetails` models.
+
+### 2022-03-07 (v1.1.0)
+- Added `isErfpacht` to `WaarderingInputParameters`.
+- Cleaned up serialization of null values, they should no longer appear in the output.
+
+### 2021-02-04
+- Added extra clarification to the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different input parameter combinations.
+
+### 2022-01-11 (v1.0.2)
+- Fixed `GET /api/v1/bodem/{id}` endpoint path parameter description, query parameter was never meant to be there.
+
+### 2021-12-23
+- Clarified the documentation pertaining to the `WaarderingInputParameters` and which fields are required for the different product types.
+
+### 2021-12-22 (v1.0.1)
+- Dates are now serialized in the ISO date-only format `yyyy-MM-dd` to stop any confusion around timezones and are all assumed to be in UTC.
+    - `peildatum` in `WaarderingsInputParameters`
+    - `datum_bestemmingplan` in `Bestemmingsdata`
+    - `datum_laatste_onderzoek` in `Bodemdata`
+    - `verkoopdatum` in `Referentieobject`
+    - `verkoopdatum` in `VorigeVerkoop`
+    - `waardebepalingsdatum` in `Modeldata`
+- Reintroduced the `WaarderingWebhookPayload` model that was omitted.
+
+### 2021-12-21
+- Patching the status of a `Waardering` object will now immediatly reflect its new status in the response object.
+
+### 2021-12-13 (v1.0.0)
+- Initial release of `v1` based on `v0.0.6`
+
+## Cross-Origin Resource Sharing
+This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).
+And that allows cross-domain communication from the browser.
+All responses have a wildcard same-origin which makes them completely public and accessible to everyone, including any code on any site.
+
+## Authentication
+Authentication is done via [OAuth2](https://oauth.net/2/) and the [client credentials](https://oauth.net/2/grant-types/client-credentials/) grant type.
+
+## Previous versions changelogs
+
+### 2022-02-02
+- API version `v0` was removed from service.
+
+### 2021-12-23
+- Mark `v0` as officially deprecated. No further versions will be released. Every implementation should move to `v1`
+
+### 2021-12-10 (v0.0.6)
+- Added extra field `peildatum` to the `WaarderingInputParameters` model.
+
+### 2021-11-25 (v0.0.5)
+- Updated all reported OAuth2 scopes and reduced the superflous scope information on each endpoint.
+
+### 2021-11-23 (v0.0.4)
+- Added per square meter developments to the `WaarderingOntwikkeling` object (fields with the `PerVierkantemeter` suffix).
+
+### 2021-11-15 (v0.0.3)
+- Added callback update and read endpoints and models.
+- Updated documentation.
+
+### 2021-11-11
+- Renamed /fundering endpoint to /funderingen to be more in line with other endpoints
+- Renamed `HerstelType` to `FunderingHerstelType`.
+- Added `FunderingType` values.
+
+### 2021-11-10
+- Adjusted OpenAPI Spec generation to fix some issues with certain generators. This also means that the nullable nature of certain fields is now correctly represented. Please refer to the Generation article for more information, the config files were updated aswell.
+
+### 2021-11-09
+- Added `Status` and `Taxatiedatum` to `Taxatiedata` model.
+
+### 2021-11-08
+- Renamed `id` field in `AdresInfo` model to `bagNummeraanduidingId`.
+- Added `GET /v0/fundering/{id}` endpoint with corresponding models.
+- Changed HTTP response code for the `BusinessRulesProblemDetails` error return type of `POST /v0/waardering` from `422 Unprocessable Entity` to `406 Not Acceptable` to fix a duplicate.
+
+### 2021-10-13
+- Added `taxatie` field to `Waardering` model.
+- Added `Taxatiedata` model containing the `taxatieorganisatie` field for desktop valuations.
+
+### 2021-09-29
+- Added `aangemaakt` timestamp field to `Waardering` model.
+- Added `WaarderingZoekParameters` model to replace `WaarderingInputParameters` in the `POST /v0/waarderingen/zoeken` endpoint.
+- Split `Omgevingsdata` model into a set of separate `Gebiedsdata` models that also contain extra statistics.
+- Added `bijzonderheden` field to `VorigeVerkoop` model.
+- Renamed `ReferentieBijzonderheden` model to `VerkoopBijzonderheden`.
+
+### 2021-09-22
+- Initial release of `v0`
+
+This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 1.2.1
+- Package version: 1.2.1
+- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+For more information, please visit [https://www.calcasa.nl/contact](https://www.calcasa.nl/contact)
+
+## Requirements.
+
+Python >=3.6
+
+## Installation & Usage
+### pip install
+
+If the python package is hosted on a repository, you can install directly using:
+
+```sh
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+```
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+
+Then import the package:
+```python
+import calcasa.api
+```
+
+### Setuptools
+
+Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+
+```sh
+python setup.py install --user
+```
+(or `sudo python setup.py install` to install the package for all users)
+
+Then import the package:
+```python
+import calcasa.api
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```python
+
+import time
+import calcasa.api
+from pprint import pprint
+from calcasa.api.api import adressen_api
+from calcasa.api.model.adres import Adres
+from calcasa.api.model.adres_info import AdresInfo
+from calcasa.api.model.not_found_problem_details import NotFoundProblemDetails
+from calcasa.api.model.permissions_denied_problem_details import PermissionsDeniedProblemDetails
+from calcasa.api.model.problem_details import ProblemDetails
+# Defining the host is optional and defaults to https://api.calcasa.nl
+# See configuration.py for a list of all supported configuration parameters.
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure OAuth2 access token for authorization: oauth
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+configuration.access_token = 'YOUR_ACCESS_TOKEN'
+
+# Configure OAuth2 access token for authorization: oauth
+configuration = calcasa.api.Configuration(
+    host = "https://api.calcasa.nl"
+)
+configuration.access_token = 'YOUR_ACCESS_TOKEN'
+
+
+# Enter a context with an instance of the API client
+with calcasa.api.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = adressen_api.AdressenApi(api_client)
+    bag_nummeraanduiding_id = 1 # int | Een BAG Nummeraanduiding ID om een adres te specificeren.
+
+    try:
+        # Adres info op basis van BAG Nummeraanduiding Id.
+        api_response = api_instance.get_adres(bag_nummeraanduiding_id)
+        pprint(api_response)
+    except calcasa.api.ApiException as e:
+        print("Exception when calling AdressenApi->get_adres: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *https://api.calcasa.nl*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AdressenApi* | [**get_adres**](docs/AdressenApi.md#get_adres) | **GET** /api/v1/adressen/{bagNummeraanduidingId} | Adres info op basis van BAG Nummeraanduiding Id.
+*AdressenApi* | [**search_adres**](docs/AdressenApi.md#search_adres) | **POST** /api/v1/adressen/zoeken | Zoek adres info op basis van het gegeven adres.
+*BestemmingsplannenApi* | [**get_bestemming_by_id**](docs/BestemmingsplannenApi.md#get_bestemming_by_id) | **GET** /api/v1/bestemmingsplannen/{bagNummeraanduidingId} | Gegevens over de bestemmingsplannen op de locatie van een adres (BAG Nummeraanduiding ID).
+*BodemApi* | [**get_bodem_by_id**](docs/BodemApi.md#get_bodem_by_id) | **GET** /api/v1/bodem/{bagNummeraanduidingId} | Gegevens over de bodemkwaliteit op de locatie van een adres (BAG Nummeraanduiding ID).
+*BuurtApi* | [**get_buurt**](docs/BuurtApi.md#get_buurt) | **GET** /api/v1/buurt/{buurtId} | Gegevens over een buurt en de wijk, gemeente en land waarin deze buurt gesitueerd is.
+*CallbacksApi* | [**add_or_update_callback_subscription**](docs/CallbacksApi.md#add_or_update_callback_subscription) | **POST** /api/v1/callbacks/inschrijvingen | Voeg een callback inschrijving toe (of werk bij) voor de huidige client voor een adres.
+*CallbacksApi* | [**delete_notification_subscription**](docs/CallbacksApi.md#delete_notification_subscription) | **DELETE** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Verwijder de callback inschrijving voor deze client en dit adres.
+*CallbacksApi* | [**get_notification_subscription**](docs/CallbacksApi.md#get_notification_subscription) | **GET** /api/v1/callbacks/inschrijvingen/{bagNummeraanduidingId} | Haal de callback inschrijving op voor deze client en dit adres.
+*CallbacksApi* | [**get_notification_subscriptions**](docs/CallbacksApi.md#get_notification_subscriptions) | **GET** /api/v1/callbacks/inschrijvingen | Haal de callback inschrijvingen binnen voor deze client.
+*ConfiguratieApi* | [**get_callbacks**](docs/ConfiguratieApi.md#get_callbacks) | **GET** /api/v1/configuratie/callbacks | Haal de geconfigureerde callback URL&#39;s op voor de huidige client.
+*ConfiguratieApi* | [**update_callbacks**](docs/ConfiguratieApi.md#update_callbacks) | **POST** /api/v1/configuratie/callbacks | Configureer callback URL voor een specifieke API versie voor de huidige client.
+*FacturenApi* | [**get_factuur**](docs/FacturenApi.md#get_factuur) | **GET** /api/v1/facturen/{id} | Factuur op basis van een waardering Id.
+*FotosApi* | [**get_foto**](docs/FotosApi.md#get_foto) | **GET** /api/v1/fotos/{id} | Foto op basis van een foto Id.
+*FunderingenApi* | [**get_fundering_by_id**](docs/FunderingenApi.md#get_fundering_by_id) | **GET** /api/v1/funderingen/{bagNummeraanduidingId} | Gegevens over de fundering op de locatie van een adres (BAG Nummeraanduiding ID).
+*GeldverstrekkersApi* | [**get_geldverstrekkers**](docs/GeldverstrekkersApi.md#get_geldverstrekkers) | **GET** /api/v1/geldverstrekkers/{productType} | Alle geldverstrekkers die te gebruiken zijn voor aanvragen.
+*RapportenApi* | [**get_rapport**](docs/RapportenApi.md#get_rapport) | **GET** /api/v1/rapporten/{id} | Rapport op basis van waardering Id.
+*WaarderingenApi* | [**create_waardering**](docs/WaarderingenApi.md#create_waardering) | **POST** /api/v1/waarderingen | Creërt een waardering.
+*WaarderingenApi* | [**get_waardering**](docs/WaarderingenApi.md#get_waardering) | **GET** /api/v1/waarderingen/{id} | Waardering op basis van Id.
+*WaarderingenApi* | [**get_waardering_ontwikkeling**](docs/WaarderingenApi.md#get_waardering_ontwikkeling) | **GET** /api/v1/waarderingen/{id}/ontwikkeling | Waardering ontwikkeling op basis van waardering Id.
+*WaarderingenApi* | [**patch_waarderingen**](docs/WaarderingenApi.md#patch_waarderingen) | **PATCH** /api/v1/waarderingen/{id} | Patcht een waardering.
+*WaarderingenApi* | [**search_waarderingen**](docs/WaarderingenApi.md#search_waarderingen) | **POST** /api/v1/waarderingen/zoeken | Zoek waardering op basis van input parameters.
+
+
+## Documentation For Models
+
+ - [Aanvraagdoel](docs/Aanvraagdoel.md)
+ - [Adres](docs/Adres.md)
+ - [AdresInfo](docs/AdresInfo.md)
+ - [AdresInfoAdres](docs/AdresInfoAdres.md)
+ - [AdresInfoNotities](docs/AdresInfoNotities.md)
+ - [Bestemmingsdata](docs/Bestemmingsdata.md)
+ - [BodemStatusType](docs/BodemStatusType.md)
+ - [Bodemdata](docs/Bodemdata.md)
+ - [BusinessRulesCode](docs/BusinessRulesCode.md)
+ - [BusinessRulesProblemDetails](docs/BusinessRulesProblemDetails.md)
+ - [Callback](docs/Callback.md)
+ - [CallbackInschrijving](docs/CallbackInschrijving.md)
+ - [CbsIndeling](docs/CbsIndeling.md)
+ - [Energielabel](docs/Energielabel.md)
+ - [Factuur](docs/Factuur.md)
+ - [Foto](docs/Foto.md)
+ - [FunderingDataBron](docs/FunderingDataBron.md)
+ - [FunderingHerstelType](docs/FunderingHerstelType.md)
+ - [FunderingRisico](docs/FunderingRisico.md)
+ - [FunderingRisicoLabel](docs/FunderingRisicoLabel.md)
+ - [FunderingSoortBron](docs/FunderingSoortBron.md)
+ - [FunderingType](docs/FunderingType.md)
+ - [FunderingTypering](docs/FunderingTypering.md)
+ - [Funderingdata](docs/Funderingdata.md)
+ - [FunderingdataBioInfectieRisico](docs/FunderingdataBioInfectieRisico.md)
+ - [FunderingdataDroogstandRisico](docs/FunderingdataDroogstandRisico.md)
+ - [FunderingdataOptrekkendVochtRisico](docs/FunderingdataOptrekkendVochtRisico.md)
+ - [FunderingdataTypering](docs/FunderingdataTypering.md)
+ - [Gebiedsdata](docs/Gebiedsdata.md)
+ - [Geldverstrekker](docs/Geldverstrekker.md)
+ - [HttpValidationProblemDetails](docs/HttpValidationProblemDetails.md)
+ - [InvalidArgumentProblemDetails](docs/InvalidArgumentProblemDetails.md)
+ - [JsonPatchDocument](docs/JsonPatchDocument.md)
+ - [KlantwaardeType](docs/KlantwaardeType.md)
+ - [Kwartaal](docs/Kwartaal.md)
+ - [Modeldata](docs/Modeldata.md)
+ - [NotFoundProblemDetails](docs/NotFoundProblemDetails.md)
+ - [Notitie](docs/Notitie.md)
+ - [Notities](docs/Notities.md)
+ - [Objectdata](docs/Objectdata.md)
+ - [Omgevingsdata](docs/Omgevingsdata.md)
+ - [OmgevingsdataBuurt](docs/OmgevingsdataBuurt.md)
+ - [OmgevingsdataGemeente](docs/OmgevingsdataGemeente.md)
+ - [OmgevingsdataLand](docs/OmgevingsdataLand.md)
+ - [OmgevingsdataProvincie](docs/OmgevingsdataProvincie.md)
+ - [OmgevingsdataWijk](docs/OmgevingsdataWijk.md)
+ - [Operation](docs/Operation.md)
+ - [OperationType](docs/OperationType.md)
+ - [PermissionsDeniedProblemDetails](docs/PermissionsDeniedProblemDetails.md)
+ - [ProblemDetails](docs/ProblemDetails.md)
+ - [ProductType](docs/ProductType.md)
+ - [Rapport](docs/Rapport.md)
+ - [Referentieobject](docs/Referentieobject.md)
+ - [ReferentieobjectAdres](docs/ReferentieobjectAdres.md)
+ - [ReferentieobjectCbsIndeling](docs/ReferentieobjectCbsIndeling.md)
+ - [ReferentieobjectObject](docs/ReferentieobjectObject.md)
+ - [ResourceExhaustedProblemDetails](docs/ResourceExhaustedProblemDetails.md)
+ - [Taxatiedata](docs/Taxatiedata.md)
+ - [Taxatiestatus](docs/Taxatiestatus.md)
+ - [ValidationProblemDetails](docs/ValidationProblemDetails.md)
+ - [VerkoopBijzonderheden](docs/VerkoopBijzonderheden.md)
+ - [VorigeVerkoop](docs/VorigeVerkoop.md)
+ - [Waardering](docs/Waardering.md)
+ - [WaarderingCbsIndeling](docs/WaarderingCbsIndeling.md)
+ - [WaarderingFactuur](docs/WaarderingFactuur.md)
+ - [WaarderingInputParameters](docs/WaarderingInputParameters.md)
+ - [WaarderingModel](docs/WaarderingModel.md)
+ - [WaarderingObject](docs/WaarderingObject.md)
+ - [WaarderingOntwikkeling](docs/WaarderingOntwikkeling.md)
+ - [WaarderingOntwikkelingKwartaal](docs/WaarderingOntwikkelingKwartaal.md)
+ - [WaarderingOntwikkelingKwartaalKwartaal](docs/WaarderingOntwikkelingKwartaalKwartaal.md)
+ - [WaarderingOrigineleInput](docs/WaarderingOrigineleInput.md)
+ - [WaarderingRapport](docs/WaarderingRapport.md)
+ - [WaarderingStatus](docs/WaarderingStatus.md)
+ - [WaarderingTaxatie](docs/WaarderingTaxatie.md)
+ - [WaarderingWebhookPayload](docs/WaarderingWebhookPayload.md)
+ - [WaarderingZoekParameters](docs/WaarderingZoekParameters.md)
+ - [WoningType](docs/WoningType.md)
+
+
+## Documentation For Authorization
+
+
+## oauth
+
+- **Type**: OAuth
+- **Flow**: application
+- **Authorization URL**: 
+- **Scopes**: 
+ - **all**: Full permissions for all areas.
+ - **api:all**: Full permissions for all areas of the public API.
+ - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:all**: Full permissions for the bodem area of the public API.
+ - **api:buurt:all**: Full permissions for the buurt area of the public API.
+ - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
+ - **api:callback:all**: Full permissions for the callback area of the public API.
+ - **api:facturen:all**: Full permissions for the facturen area of the public API.
+ - **api:fotos:all**: Full permissions for the fotos area of the public API.
+ - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
+ - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
+ - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
+ - **api:adressen:read**: Read permissions for the adressen area of the public API.
+ - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:read**: Read permissions for the bodem area of the public API.
+ - **api:buurt:read**: Read permissions for the buurt area of the public API.
+ - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
+ - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
+ - **api:callback:read**: Read permissions for the callback area of the public API.
+ - **api:callback:write**: Write permissions for the callback area of the public API.
+ - **api:facturen:read**: Read permissions for the facturen area of the public API.
+ - **api:fotos:read**: Read permissions for the fotos area of the public API.
+ - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
+ - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
+ - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
+ - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
+ - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
+ - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
+ - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
+
+
+## oauth
+
+- **Type**: OAuth
+- **Flow**: accessCode
+- **Authorization URL**: https://authentication.calcasa.nl/oauth2/v2.0/authorize
+- **Scopes**: 
+ - **all**: Full permissions for all areas.
+ - **api:all**: Full permissions for all areas of the public API.
+ - **api:bestemmingsplannen:all**: Full permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:all**: Full permissions for the bodem area of the public API.
+ - **api:buurt:all**: Full permissions for the buurt area of the public API.
+ - **api:configuratie:all**: Full permissions for the configuratie area of the public API.
+ - **api:callback:all**: Full permissions for the callback area of the public API.
+ - **api:facturen:all**: Full permissions for the facturen area of the public API.
+ - **api:fotos:all**: Full permissions for the fotos area of the public API.
+ - **api:funderingen:all**: Full permissions for the funderingen area of the public API.
+ - **api:rapporten:all**: Full permissions for the rapporten area of the public API.
+ - **api:waarderingen:all**: Full permissions for the waarderingen area of the public API.
+ - **api:adressen:read**: Read permissions for the adressen area of the public API.
+ - **api:bestemmingsplannen:read**: Read permissions for the bestemmingsplannen area of the public API.
+ - **api:bodem:read**: Read permissions for the bodem area of the public API.
+ - **api:buurt:read**: Read permissions for the buurt area of the public API.
+ - **api:configuratie:read**: Read permissions for the configuratie area of the public API.
+ - **api:configuratie:write**: Write permissions for the configuratie area of the public API.
+ - **api:callback:read**: Read permissions for the callback area of the public API.
+ - **api:callback:write**: Write permissions for the callback area of the public API.
+ - **api:facturen:read**: Read permissions for the facturen area of the public API.
+ - **api:fotos:read**: Read permissions for the fotos area of the public API.
+ - **api:funderingen:read**: Read permissions for the funderingen area of the public API.
+ - **api:geldverstrekkers:read**: Read permissions for the geldverstrekkers area of the public API.
+ - **api:rapporten:read**: Read permissions for the rapporten area of the public API.
+ - **api:waarderingen:create**: Create permissions for the waarderingen area of the public API.
+ - **api:waarderingen:patch**: Patch permissions for the waarderingen area of the public API.
+ - **api:waarderingen:read**: Read permissions for the waarderingen area of the public API.
+ - **api:waarderingen:ontwikkeling**: Read permissions for the ontwikkelingen endpoint in the waarderingen area of the public API.
+
+
+## Author
+
+info@calcasa.nl
+
+
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in calcasa.api.apis and calcasa.api.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from calcasa.api.api.default_api import DefaultApi`
+- `from calcasa.api.model.pet import Pet`
+
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import calcasa.api
+from calcasa.api.apis import *
+from calcasa.api.models import *
+```
+
+
+
```

### Comparing `calcasa-api-1.2.0/calcasa_api.egg-info/SOURCES.txt` & `calcasa-api-1.2.1/calcasa_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 calcasa/api/__init__.py
 calcasa/api/api_client.py
 calcasa/api/configuration.py
 calcasa/api/exceptions.py
```

### Comparing `calcasa-api-1.2.0/setup.py` & `calcasa-api-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Calcasa Public API v1
 
-    The version of the OpenAPI document: 1.2.0
+    The version of the OpenAPI document: 1.2.1
     Contact: info@calcasa.nl
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_namespace_packages  # noqa: H301
 
 NAME = "calcasa-api"
-VERSION = "1.2.0"
+VERSION = "1.2.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

