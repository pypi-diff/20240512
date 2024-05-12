# Comparing `tmp/SimplePBI-0.1.8-py3-none-any.whl.zip` & `tmp/SimplePBI-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,27 @@
-Zip file size: 55328 bytes, number of entries: 22
+Zip file size: 60079 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat      643 b- defN 22-Sep-15 17:59 simplepbi/__init__.py
 -rw-rw-rw-  2.0 fat    88324 b- defN 23-Oct-23 17:55 simplepbi/admin/__init__.py
 -rw-rw-rw-  2.0 fat     9878 b- defN 22-Sep-15 17:56 simplepbi/apps/__init__.py
 -rw-rw-rw-  2.0 fat     6276 b- defN 23-Jun-29 20:35 simplepbi/azpause/__init__.py
 -rw-rw-rw-  2.0 fat    15534 b- defN 22-Sep-15 17:56 simplepbi/capacities/__init__.py
 -rw-rw-rw-  2.0 fat    17252 b- defN 22-Sep-15 17:56 simplepbi/dashboards/__init__.py
 -rw-rw-rw-  2.0 fat    15322 b- defN 22-Sep-15 17:56 simplepbi/dataflows/__init__.py
 -rw-rw-rw-  2.0 fat    64782 b- defN 23-Sep-19 13:38 simplepbi/datasets/__init__.py
+-rw-rw-rw-  2.0 fat      643 b- defN 24-Feb-26 20:21 simplepbi/fabric/__init__.py
+-rw-rw-rw-  2.0 fat    19752 b- defN 24-Feb-27 20:19 simplepbi/fabric/core/__init__.py
+-rw-rw-rw-  2.0 fat     4010 b- defN 24-Feb-26 20:18 simplepbi/fabric/items/__init__.py
 -rw-rw-rw-  2.0 fat    16099 b- defN 22-Sep-15 17:56 simplepbi/gateways/__init__.py
 -rw-rw-rw-  2.0 fat    14147 b- defN 22-Sep-15 17:57 simplepbi/groups/__init__.py
--rw-rw-rw-  2.0 fat    26469 b- defN 24-Mar-23 19:19 simplepbi/imports/__init__.py
+-rw-rw-rw-  2.0 fat    26516 b- defN 24-May-12 21:25 simplepbi/imports/__init__.py
 -rw-rw-rw-  2.0 fat    24126 b- defN 22-Sep-15 17:57 simplepbi/pipelines/__init__.py
 -rw-rw-rw-  2.0 fat    18577 b- defN 24-Mar-25 16:35 simplepbi/pushdatasets/__init__.py
 -rw-rw-rw-  2.0 fat    44427 b- defN 23-Mar-10 18:36 simplepbi/reports/__init__.py
 -rw-rw-rw-  2.0 fat    12740 b- defN 22-Sep-15 17:57 simplepbi/scorecards/__init__.py
 -rw-rw-rw-  2.0 fat     4093 b- defN 22-Sep-15 17:57 simplepbi/token/__init__.py
 -rw-rw-rw-  2.0 fat     3457 b- defN 23-May-08 15:36 simplepbi/utils/__init__.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Mar-25 18:28 SimplePBI-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12798 b- defN 24-Mar-25 18:28 SimplePBI-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 18:28 SimplePBI-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-25 18:28 SimplePBI-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1872 b- defN 24-Mar-25 18:28 SimplePBI-0.1.8.dist-info/RECORD
-22 files, 397990 bytes uncompressed, 52306 bytes compressed:  86.9%
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-May-12 21:30 SimplePBI-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13095 b- defN 24-May-12 21:30 SimplePBI-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 21:30 SimplePBI-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-12 21:30 SimplePBI-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2138 b- defN 24-May-12 21:30 SimplePBI-0.1.9.dist-info/RECORD
+25 files, 423005 bytes uncompressed, 56639 bytes compressed:  86.6%
```

## zipnote {}

```diff
@@ -18,14 +18,23 @@
 
 Filename: simplepbi/dataflows/__init__.py
 Comment: 
 
 Filename: simplepbi/datasets/__init__.py
 Comment: 
 
+Filename: simplepbi/fabric/__init__.py
+Comment: 
+
+Filename: simplepbi/fabric/core/__init__.py
+Comment: 
+
+Filename: simplepbi/fabric/items/__init__.py
+Comment: 
+
 Filename: simplepbi/gateways/__init__.py
 Comment: 
 
 Filename: simplepbi/groups/__init__.py
 Comment: 
 
 Filename: simplepbi/imports/__init__.py
@@ -45,23 +54,23 @@
 
 Filename: simplepbi/token/__init__.py
 Comment: 
 
 Filename: simplepbi/utils/__init__.py
 Comment: 
 
-Filename: SimplePBI-0.1.8.dist-info/LICENSE
+Filename: SimplePBI-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: SimplePBI-0.1.8.dist-info/METADATA
+Filename: SimplePBI-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: SimplePBI-0.1.8.dist-info/WHEEL
+Filename: SimplePBI-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: SimplePBI-0.1.8.dist-info/top_level.txt
+Filename: SimplePBI-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: SimplePBI-0.1.8.dist-info/RECORD
+Filename: SimplePBI-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplepbi/imports/__init__.py

```diff
@@ -433,43 +433,43 @@
             return res
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
             print("Request exception: ", e)
             
     def simple_import_from_github(self, owner, repo, path, github_pat, workspace_id):
-        '''This function will import a PBIX file from GitHub to Power BI
+        '''This function will import a PBIX file from GitHub to Power BI. The maximun size is 100Mb.
          ### Parameters
         ----
         owner: str
             The account owner of the repository. The name is not case sensitive. For example: https://dev.azure.com/ibarrau/ the organization name is ibarrau
         repo: str
             The name of the repository without the .git extension. The name is not case sensitive.
         path: str
-            The path of the file in GitHub. For example: Prod/PBITenantOverview.pbix
+            The path of the file in GitHub. For example: /Prod/PBITenantOverview.pbix
         github_pat: str
             The GitHub Personal Access Token. You can turn it on from Settings > Developer Settings > Personal Access Tokens
         workspace_id: str uuid
             The Power Bi workspace id. You can take it from PBI Service URL    
         ### Returns
         ----
         Dict:
             Response 202 Ok
         '''
         file_name = path.split("/")[-1]
         try:
             url = "https://api.github.com/repos/{}/{}/contents/{}".format(owner, repo, path)
-            pbix_str = requests.get(url, headers={'Accept': 'application/vnd.github+json', "Authorization": "Bearer {}".format(github_pat), 'X-GitHub-Api-Version': '2022-11-28' })
-            pbix_bytes = bytes(pbix_str.json()["content"], 'utf-8')
-            pbix = base64.decodebytes(pbix_bytes)
+            pbix_str = requests.get(url, headers={'Accept': 'application/vnd.github.raw+json', "Authorization": "Bearer {}".format(github_pat), 'X-GitHub-Api-Version': '2022-11-28' })
+            #pbix_bytes = bytes(pbix_str.json()["content"], 'utf-8')
+            #pbix = base64.decodebytes(pbix_bytes)
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
             print("Request exception: ", e)
         try:
-            res = self.simple_import_pbix_as_parameter(workspace_id, pbix, file_name)
+            res = self.simple_import_pbix_as_parameter(workspace_id, pbix_str.content, file_name)
             res.raise_for_status()
             return res
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
             print("Request exception: ", e)
```

## Comparing `SimplePBI-0.1.8.dist-info/LICENSE` & `SimplePBI-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SimplePBI-0.1.8.dist-info/METADATA` & `SimplePBI-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplePBI
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simplify usage of Power Bi Rest API
 Home-page: 
 Download-URL: 
 Author: Ignacio Barrau <igna_barrau@hotmail.com>, Martin Zurita <martinzurita1@gmail.com>
 License: MIT
 Project-URL: Documentation, https://docs.microsoft.com/en-us/rest/api/power-bi/
 Project-URL: Say Thanks!, https://www.ladataweb.com.ar/contacto.html
@@ -89,14 +89,15 @@
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Apps_details.txt" target="_blank">Apps</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Imports_details.txt" target="_blank">Imports</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Gateways_details.txt" target="_blank">Gateways</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Capacities_details.txt" target="_blank">Capacities</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Pipelines_details.txt" target="_blank">Pipelines (Preview)</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Scorecards_details.txt" target="_blank">Scorecards (Preview)</a>
 - <a href="https://github.com/ladataweb/SimplePBI/blob/main/Az_Pause_Resume_details.txt" target="_blank">Azure Pause and Resume resource (Preview)</a>
+- <a href="https://github.com/ladataweb/SimplePBI/blob/main/Push_Datasets_details.txt" target="_blank">Push Datasets</a>
 
 ## Complex requests
 If you want to get a deeper look on complex __Admin__ methods and unique methods. 
 <a href="https://github.com/ladataweb/SimplePBI/blob/main/Admin_complex.md" target="_blank">Check this doc</a>
 
 ## Azure Pause Resume Resources
 We have added a new feature to include some Azure Resource API Manager. The new "azpause" class will let you Pause or Resume Azure tabular or capacity resources. With SimplePBI you can pause and resume Fabric, Power Bi Embedded or Azure Analysis Services resources.
@@ -109,14 +110,15 @@
 
 ### Example of our amazing unique requests
 - get_orphan_dataflows_preview: get dataflows without dataset
 - simple_import_pbix: makes publishing a pbix file easier
 - simple_import_pbix_as_parameter: import a pbix from api response content
 - simple_import_pbix_folder_in_group_preview: post a all pbix files in a local folder
 - simple_import_from_devops: import a pbix from azure devops repo
+- simple_import_from_github: import a pbix from azure github repo
 - simple_copy_reports_between_groups: copy report from workspace to a workspace
 - enhanced_refresh_dataset_in_group: a special request feature that not only eliminates the need for synchronous client connections to perform a refresh, but also unlocks enterprise-grade refresh capabilities.
 - get_activity_events_preview (already iterating): makes the get activity events specified by date easier
 - get_user_artifact_access_preview (already iterating): makes the get user artifact access easier
 - get_widely shared_artifacts_published_to_web (already iterating): makes geting the published to web repos info easier
 
 ## Small categories
@@ -265,9 +267,13 @@
 
 0.1.7 (16/12/2023)
 ------------------
 Fixing request for importing powerbi desktop file from Azure DevOps.
 
 0.1.8 (25/03/2024)
 ------------------
-Adding new request for importing pbix from GitHub like the one for DevOps.
+Adding new request for importing pbix from GitHub (less 1Mb) like the one for DevOps.
 New Object category. Adding all Push Dataset category requests.
+
+0.1.9 (12/05/2024)
+------------------
+Adding support for GitHub pbix importing up to 100Mb.
```

## Comparing `SimplePBI-0.1.8.dist-info/RECORD` & `SimplePBI-0.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 simplepbi/admin/__init__.py,sha256=o2JWyI38qNMFfLq0ZR5EeQbPb1BSyj46beebJfeJyk4,88324
 simplepbi/apps/__init__.py,sha256=vo6-DtuprZx9dfLqc6jeMvRVGYvNNj9QX4mpSfK15GY,9878
 simplepbi/azpause/__init__.py,sha256=-BtjrmaMod3Q-DPpHpRlHsnvueqjVrAPac9S_MxeX0E,6276
 simplepbi/capacities/__init__.py,sha256=1t9ancMJvpzht931qvto3Oah3Zjn-Ut2KFEq3-Ap10o,15534
 simplepbi/dashboards/__init__.py,sha256=TtH4u-wxKF7_C7byIFODavxb8flJiIyzxc-PdnpM7Ns,17252
 simplepbi/dataflows/__init__.py,sha256=QGP2rX4zeVQ44NUf0W8eP5Wm_zzwj8G52TxFNG3jnSA,15322
 simplepbi/datasets/__init__.py,sha256=Gq1pwpKaAD8icreSGbag0_dRqt4D3vHurxyTjg7eXho,64782
+simplepbi/fabric/__init__.py,sha256=NeBbh0qJgXSr7iMzaWDZyGDQX5UVZiMSSuUaxWByAkA,643
+simplepbi/fabric/core/__init__.py,sha256=SGQbvZuFl1YThwKGXE40JerBSGnAc7p4Bt6I2KkmSt0,19752
+simplepbi/fabric/items/__init__.py,sha256=W1XYmyVz87ok0IbfOcjx8AhE_N1No37Dkr9j_Edzcr0,4010
 simplepbi/gateways/__init__.py,sha256=ol1eZBIAT0v764BCUSHMzhA4-e3FDh77I8D_wCWLSz8,16099
 simplepbi/groups/__init__.py,sha256=acPort3e99ajdTKXhLWvnGWevVIuaM3IBRrUjkIYTsY,14147
-simplepbi/imports/__init__.py,sha256=Kr1a3SnSaGEFvwtRGilclzgi8uFkLiQSiJDjEH3fbi0,26469
+simplepbi/imports/__init__.py,sha256=0Qrv94wuZMhW-FAzRtWSCuVgtU3qfKH8qjqD42FF6BU,26516
 simplepbi/pipelines/__init__.py,sha256=KtmtGa1049qqtCCclaNB7_fBAv56PGIVMrWp4v-B9uQ,24126
 simplepbi/pushdatasets/__init__.py,sha256=TsW46qZGgV1Ae_J3HuJ514ZDfrnhHxx3g31WeqTmf7Q,18577
 simplepbi/reports/__init__.py,sha256=x25_H-PVITI37luFK73BQdwIRD60nG9zRmnMhYPoJvU,44427
 simplepbi/scorecards/__init__.py,sha256=eb6Z4q6dasdPcGtsxTqbupkIhMo_sAHM98fgtqiCH4A,12740
 simplepbi/token/__init__.py,sha256=sT8EgSn3RQ-gbqmVPxVux37S_mUnLIm_0qQRkd6qqAw,4093
 simplepbi/utils/__init__.py,sha256=k2Opnd02zwaXUocHmgUvaqFRjfvU14L5IfA0LaMHzjQ,3457
-SimplePBI-0.1.8.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
-SimplePBI-0.1.8.dist-info/METADATA,sha256=-r4gREycroGc9XrxKEdZ10Nmt2-yAa8cR0cbBMdldBA,12798
-SimplePBI-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-SimplePBI-0.1.8.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
-SimplePBI-0.1.8.dist-info/RECORD,,
+SimplePBI-0.1.9.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
+SimplePBI-0.1.9.dist-info/METADATA,sha256=stqPHwPUE_wRUDm5dgWnq9xogOnJTHW3QdEMGpwq_RY,13095
+SimplePBI-0.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+SimplePBI-0.1.9.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
+SimplePBI-0.1.9.dist-info/RECORD,,
```

