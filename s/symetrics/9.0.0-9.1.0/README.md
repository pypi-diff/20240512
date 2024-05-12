# Comparing `tmp/symetrics-9.0.0.tar.gz` & `tmp/symetrics-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symetrics-9.0.0.tar", last modified: Tue Apr 30 06:52:16 2024, max compression
+gzip compressed data, was "symetrics-9.1.0.tar", last modified: Sun May 12 17:06:35 2024, max compression
```

## Comparing `symetrics-9.0.0.tar` & `symetrics-9.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.049873 symetrics-9.0.0/
--rw-rw-rw-   0        0        0     1151 2024-04-30 06:52:16.049873 symetrics-9.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 06:52:16.049873 symetrics-9.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2024-04-30 06:52:13.000000 symetrics-9.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.022906 symetrics-9.0.0/symetrics/
--rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-9.0.0/symetrics/__init__.py
--rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-9.0.0/symetrics/dbcontext.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.049873 symetrics-9.0.0/symetrics/src/
--rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-9.0.0/symetrics/src/__init__.py
--rw-rw-rw-   0        0        0     1035 2024-04-30 06:51:43.000000 symetrics-9.0.0/symetrics/src/datastruct.py
--rw-rw-rw-   0        0        0    22249 2024-04-30 06:26:19.000000 symetrics-9.0.0/symetrics/symetrics_api.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.044515 symetrics-9.0.0/symetrics.egg-info/
--rw-rw-rw-   0        0        0     1151 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 17:06:35.082712 symetrics-9.1.0/
+-rw-rw-rw-   0        0        0     1151 2024-05-12 17:06:35.081712 symetrics-9.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-12 17:06:35.082712 symetrics-9.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2024-05-12 17:05:17.000000 symetrics-9.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:06:35.033641 symetrics-9.1.0/symetrics/
+-rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-9.1.0/symetrics/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-9.1.0/symetrics/dbcontext.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:06:35.077734 symetrics-9.1.0/symetrics/src/
+-rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-9.1.0/symetrics/src/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-04-30 06:51:43.000000 symetrics-9.1.0/symetrics/src/datastruct.py
+-rw-rw-rw-   0        0        0    27303 2024-05-12 17:03:04.000000 symetrics-9.1.0/symetrics/symetrics_api.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:06:35.072503 symetrics-9.1.0/symetrics.egg-info/
+-rw-rw-rw-   0        0        0     1151 2024-05-12 17:06:34.000000 symetrics-9.1.0/symetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-05-12 17:06:34.000000 symetrics-9.1.0/symetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 17:06:34.000000 symetrics-9.1.0/symetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-12 17:06:34.000000 symetrics-9.1.0/symetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 17:06:34.000000 symetrics-9.1.0/symetrics.egg-info/top_level.txt
```

### Comparing `symetrics-9.0.0/PKG-INFO` & `symetrics-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 9.0.0
+Version: 9.1.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `symetrics-9.0.0/setup.py` & `symetrics-9.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '9.0.0' 
+VERSION = '9.1.0' 
 DESCRIPTION = 'Symetrics API'
 LONG_DESCRIPTION = '''A package to access SYMETRICS database. 
 SYMETRICS database is a consolidation of metrics for synonymous variants which were derived from a number of computational tools each of which contributing to 
 attribute specific metrics such as SYNVEP for general functional constraints, SpliceAI for splicing effect, SILVA for obtaining GERP++ (phylogenetic related constraints)
 CpG/CpG_Exon, dRSCU/RSCU for codon usage and SURF for rna stability. The package also includes a result of the analysis of the influence of each variants exceeding set threshold
 per metrics defined constituting to a score assigned to a gene'''
 REQUIRED_PACKAGES = [
```

### Comparing `symetrics-9.0.0/symetrics/dbcontext.py` & `symetrics-9.1.0/symetrics/dbcontext.py`

 * *Files identical despite different names*

### Comparing `symetrics-9.0.0/symetrics/src/datastruct.py` & `symetrics-9.1.0/symetrics/src/datastruct.py`

 * *Files identical despite different names*

### Comparing `symetrics-9.0.0/symetrics/symetrics_api.py` & `symetrics-9.1.0/symetrics/symetrics_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -569,24 +569,105 @@
         variant_list = None
 
         try:
             # synvep is hg38 (pos_GRCh38) abd hg19 (pos)
             with self._db as dbhandler:
                 synvep_cursor = dbhandler._conn.cursor()
                 synvep_query = ''
-                synvep_query = f'SELECT chr as CHR,pos as POS,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE HGNC_gene_symbol = "{gene}"'                    
                 
-                query = "SELECT chr as CHR,pos as POS,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE HGNC_gene_symbol = ?"
-                            
-                params = (gene,)
+                # query = "SELECT chr as CHR,pos_GRCh38 as POS, pos as POS_HG19,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE HGNC_gene_symbol = ?"
+                # query = """
+                #     SELECT SYNVEP.*,
+                #     COALESCE(SURF.SURF, 'Not Found') AS SURF,
+                #     COALESCE(SILVA_SCORE.GERP, 'Not Found') AS GERP,
+                #     COALESCE(SILVA_SCORE.RSCU, 'Not Found') AS RSCU,
+                #     COALESCE(SILVA_SCORE.dRSCU, 'Not Found') AS dRSCU,
+                #     COALESCE(SILVA_SCORE.CpG, 'Not Found') AS CpG,
+                #     COALESCE(SILVA_SCORE.CpG_exon, 'Not Found') AS CpG_exon,
+                #     COALESCE(SILVA_SCORE.MES, 'Not Found') AS MES,
+                #     COALESCE(SILVA_SCORE.F_PREMRNA, 'Not Found') AS F_PREMRNA,
+                #     COALESCE(SILVA_SCORE.F_MRNA, 'Not Found') AS F_MRNA,
+                #     COALESCE(SURF.SURF, 'Not Found') AS SURF,
+                #     COALESCE(SPLICEAI.INFO, 'Not Found') AS SPLICEAI
+                # FROM SYNVEP
+                # LEFT JOIN SILVA_SCORE ON SYNVEP.CHR = SILVA_SCORE.CHROM
+                #                     AND SYNVEP.POS = SILVA_SCORE.POS
+                #                     AND SYNVEP.REF = SILVA_SCORE.REF
+                #                     AND SYNVEP.ALT = SILVA_SCORE.ALT
+                #                     AND SYNVEP.HGNC_gene_symbol = SILVA_SCORE.GENE
+                # LEFT JOIN SURF ON SYNVEP.CHR = SURF.CHR
+                #             AND SYNVEP.pos_GRCh38 = SURF.POS
+                #             AND SYNVEP.REF = SURF.REF
+                #             AND SYNVEP.ALT = SURF.ALT
+                #             AND SYNVEP.HGNC_gene_symbol = SURF.GENE
+                # LEFT JOIN SPLICEAI ON SYNVEP.CHR = SPLICEAI.CHR
+                #                 AND SYNVEP.pos_GRCh38 = SPLICEAI.POS
+                #                 AND SYNVEP.REF = SPLICEAI.REF
+                #                 AND SYNVEP.ALT = SPLICEAI.ALT
+                #                 AND SPLICEAI.INFO LIKE '%' || SYNVEP.HGNC_gene_symbol || '%'
+                # WHERE SYNVEP.HGNC_gene_symbol = ?
+                # """
                 
+                # params = (gene,)
+                # synvep_cursor.execute(query,params)
+                # synvep_rows = synvep_cursor.fetchall()  
                 
+                query = "SELECT chr as CHR,pos_GRCh38 as POS, pos as POS_HG19,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE HGNC_gene_symbol = ?"
+                params = (gene,)
                 synvep_cursor.execute(query,params)
                 synvep_rows = synvep_cursor.fetchall()
-                variant_list = synvep_rows
+                synvep_df = pd.DataFrame(synvep_rows)
+                synvep_df.columns = ['CHR','POS','POS_HG19','REF','ALT','GENE','SYNVEP']
+
+                query = "SELECT CHROM as CHR, POS, REF,ALT, GENE,GERP, RSCU, dRSCU, CpG, CpG_exon, MES, F_PREMRNA, F_MRNA FROM SILVA_SCORE WHERE GENE = ?"
+                params = (gene,)
+                synvep_cursor.execute(query,params)
+                silva_rows = synvep_cursor.fetchall()
+                silva_df = pd.DataFrame(silva_rows)
+                silva_df.columns = ['CHR','POS_HG19','REF','ALT','GENE','GERP','RSCU','dRSCU','CpG','CpG_exon','MES','F_PREMRNA', 'F_MRNA']
+
+
+                query = "SELECT CHR, POS, REF,ALT, GENE, SURF FROM SURF WHERE GENE = ?"
+                params = (gene,)
+                synvep_cursor.execute(query,params)
+                surf_rows = synvep_cursor.fetchall()
+                surf_df = pd.DataFrame(surf_rows)
+                surf_df.columns = ['CHR','POS','REF','ALT','GENE','SURF']
+
+                query = "SELECT chr as CHR, pos as POS, ref as REF,alt as ALT, INFO FROM SPLICEAI WHERE INFO like ?"
+                params = ('%' + gene + '%',)
+                synvep_cursor.execute(query,params)
+                splice_rows = synvep_cursor.fetchall()
+                splice_df = pd.DataFrame(splice_rows)
+                splice_df.columns = ['CHR','POS','REF','ALT','INFO']
+                vcf_header = "ALLELE|SYMBOL|DS_AG|DS_AL|DS_DG|DS_DL|DP_AG|DP_AL|DP_DG|DP_DL"
+                vcf_header = vcf_header.split('|')
+                splice_df[vcf_header] = splice_df['INFO'].str.split('|', expand=True)
+                splice_df['MAX_DS'] = splice_df.apply(lambda row: max(row['DS_AG'],row['DS_AL'],row['DS_DG'],row['DS_DL']), axis=1)
+                splice_df = splice_df[['CHR','POS','REF','ALT','MAX_DS']]
+
+
+
+                synvep_df['CHR'] = synvep_df['CHR'].astype(str)
+                synvep_df['POS'] = synvep_df['POS'].astype(str)
+                synvep_df['POS_HG19'] = synvep_df['POS_HG19'].astype(str)
+                silva_df['CHR'] = silva_df['CHR'].astype(str)
+                silva_df['POS_HG19'] = silva_df['POS_HG19'].astype(str)
+                surf_df['CHR'] = surf_df['CHR'].astype(str)
+                surf_df['POS'] = surf_df['POS'].astype(str)
+                splice_df['CHR'] = splice_df['CHR'].astype(str)
+                splice_df['POS'] = splice_df['POS'].astype(str)
+
+                
+                merged_df = pd.merge(synvep_df, silva_df, on=['CHR', 'POS_HG19', 'REF', 'ALT', 'GENE'], how='outer')
+                merged_df = pd.merge(merged_df, surf_df, on=['CHR', 'POS', 'REF', 'ALT', 'GENE'], how='outer')
+                merged_df = pd.merge(merged_df, splice_df, on=['CHR', 'POS', 'REF', 'ALT'], how='outer')
+                merged_df.fillna('N/A', inplace=True)
+                
+                variant_list = merged_df.to_dict(orient='records')
             
         except Error as e:
             logging.error(f"Connection to {self._db} failed")
     
         return variant_list
```

### Comparing `symetrics-9.0.0/symetrics.egg-info/PKG-INFO` & `symetrics-9.1.0/symetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 9.0.0
+Version: 9.1.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

