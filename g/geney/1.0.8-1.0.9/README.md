# Comparing `tmp/geney-1.0.8-py2.py3-none-any.whl.zip` & `tmp/geney-1.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,28 @@
-Zip file size: 413911 bytes, number of entries: 23
+Zip file size: 422114 bytes, number of entries: 26
 -rw-r--r--  2.0 unx    11255 b- defN 24-Mar-12 09:56 geney/Fasta_segment.py
 -rw-r--r--  2.0 unx     8421 b- defN 24-Mar-13 16:51 geney/Gene.py
 -rw-r--r--  2.0 unx       65 b- defN 24-Mar-13 10:00 geney/__init__.py
 -rw-r--r--  2.0 unx      385 b- defN 24-Mar-13 08:48 geney/config_setup.py
 -rw-r--r--  2.0 unx    10161 b- defN 24-Mar-13 07:35 geney/data_setup.py
--rw-r--r--  2.0 unx    22570 b- defN 24-Mar-13 09:54 geney/oncosplice_pipeline.py
+-rw-r--r--  2.0 unx    22576 b- defN 24-Mar-14 11:50 geney/oncosplice_pipeline.py
 -rw-r--r--  2.0 unx     2374 b- defN 24-Mar-13 17:03 geney/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-13 17:27 geney/analyzers/__init__.py
+-rw-r--r--  2.0 unx    15384 b- defN 24-Mar-14 11:37 geney/analyzers/survival.py
+-rw-r--r--  2.0 unx    10726 b- defN 24-Mar-13 17:43 geney/analyzers/visualize_protein_conservation.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-12 10:01 geney/mutations/__init__.py
 -rw-r--r--  2.0 unx    10271 b- defN 24-Mar-12 10:11 geney/mutations/variant_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-13 06:45 geney/pipelines/__init__.py
--rw-r--r--  2.0 unx     5635 b- defN 24-Mar-13 17:10 geney/pipelines/dask_utils.py
+-rw-r--r--  2.0 unx     5666 b- defN 24-Mar-14 11:39 geney/pipelines/dask_utils.py
 -rw-r--r--  2.0 unx       60 b- defN 24-Mar-12 11:11 geney/splicing/__init__.py
--rw-r--r--  2.0 unx    11800 b- defN 24-Mar-13 09:59 geney/splicing/spliceai_utils.py
+-rw-r--r--  2.0 unx    11779 b- defN 24-Mar-14 11:45 geney/splicing/spliceai_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-12 09:59 geney/translation_initiation/__init__.py
 -rw-r--r--  2.0 unx     4446 b- defN 24-Mar-13 16:50 geney/translation_initiation/tis_utils.py
 -rw-r--r--  2.0 unx     1165 b- defN 24-Jan-18 09:07 geney/translation_initiation/resources/kozak_pssm.json
 -rw-r--r--  2.0 unx  2592025 b- defN 24-Jan-18 09:07 geney/translation_initiation/resources/tis_regressor_model.joblib
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-12 09:59 geney/translation_termination/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-12 10:15 geney/translation_termination/tts_utils.py
--rw-r--r--  2.0 unx     1070 b- defN 24-Mar-13 17:10 geney-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-13 17:10 geney-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-13 17:10 geney-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1951 b- defN 24-Mar-13 17:10 geney-1.0.8.dist-info/RECORD
-23 files, 2683770 bytes uncompressed, 410721 bytes compressed:  84.7%
+-rw-r--r--  2.0 unx     1070 b- defN 24-Mar-14 11:51 geney-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Mar-14 11:51 geney-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Mar-14 11:51 geney-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2224 b- defN 24-Mar-14 11:51 geney-1.0.9.dist-info/RECORD
+26 files, 2710169 bytes uncompressed, 418490 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -15,14 +15,23 @@
 
 Filename: geney/oncosplice_pipeline.py
 Comment: 
 
 Filename: geney/utils.py
 Comment: 
 
+Filename: geney/analyzers/__init__.py
+Comment: 
+
+Filename: geney/analyzers/survival.py
+Comment: 
+
+Filename: geney/analyzers/visualize_protein_conservation.py
+Comment: 
+
 Filename: geney/mutations/__init__.py
 Comment: 
 
 Filename: geney/mutations/variant_utils.py
 Comment: 
 
 Filename: geney/pipelines/__init__.py
@@ -51,20 +60,20 @@
 
 Filename: geney/translation_termination/__init__.py
 Comment: 
 
 Filename: geney/translation_termination/tts_utils.py
 Comment: 
 
-Filename: geney-1.0.8.dist-info/METADATA
+Filename: geney-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: geney-1.0.8.dist-info/WHEEL
+Filename: geney-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: geney-1.0.8.dist-info/top_level.txt
+Filename: geney-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: geney-1.0.8.dist-info/RECORD
+Filename: geney-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geney/oncosplice_pipeline.py

```diff
@@ -23,15 +23,15 @@
                 will contain columns pertinant to assessing mutation pathogenicity including pipelines score, GOF score, legacy pipelines score, missplicing,
     '''
 
     print(f'>> Processing: {mutation}')
     mutation = Variations(mutation)                                             # Generate mutation object
     # Gene annotations should be available in the target directory under the file name mrna_gene.json
     gene = Gene(mutation.gene)                                                      # We obtain the annotation file and convert it into a Gene object
-    aberrant_splicing = PredictSpliceAI(mutation, threshold=sai_threshold)      # SpliceAI predictions are processed and obtained for each mutation
+    aberrant_splicing = PredictSpliceAI(mutation, gene, threshold=sai_threshold)      # SpliceAI predictions are processed and obtained for each mutation
     # Oncosplice obtains predictions for each transcript in the annotation file
     results = pd.concat([oncosplice_transcript(reference_transcript.generate_protein(), mutation, aberrant_splicing, prevalence_threshold, annotate) for
                          reference_transcript in gene if reference_transcript.transcript_biotype == 'protein_coding'])
 
     # Append some additional, uniform information to the results dataframe
     results['mut_id'] = mutation.mut_id
     results['missplicing'] = aberrant_splicing.get_max_missplicing_delta()
```

## geney/pipelines/dask_utils.py

```diff
@@ -59,47 +59,42 @@
         res = None
     return res
 
 
 def process_and_save_tasks(tasks, save_loc, dask_client, num_workers=10, save_increment=20, file_index=0):
     """
     Process a list of tasks using Dask, saving the results incrementally.
-
     Parameters:
     tasks (list): List of tasks to be processed.
     save_loc (str): Location to save results.
     dask_client (Client): Dask client for task submission.
     num_workers (int): Number of workers to use.
     save_increment (int): Number of iterations after which to save results.
     file_index (int): Starting index for output files.
-
     Returns:
     None
     """
     def save_results(results, index):
+        print(results)
         if results:
             df = pd.concat(results)
             df.to_csv(os.path.join(save_loc, f'results_{index}.csv'))
             return []
         return results
-
     futures, all_results = [], []
     for i, task in tqdm(enumerate(tasks), total=len(tasks)):
         futures.append(dask_client.submit(main_single, task))
-
         if (i + 1) % num_workers == 0:
             wait(futures)
             all_results.extend([f.result() for f in futures if f.status == 'finished' and f.result() is not None])
             futures = []
-
         if (i + 1) % (save_increment * num_workers) == 0:
             all_results = save_results(all_results, file_index)
             file_index += 1
             gc.collect()
-
     wait(futures)
     all_results.extend([f.result() for f in futures if f.status == 'finished' and f.result() is not None])
     save_results(all_results, file_index)
 
 
 def restart_checkpoint(result_dir):
     """
@@ -131,15 +126,15 @@
         print(f"Error processing file {files}: {e}")
         return [], 0
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Run oncosplice with dask.')
     parser.add_argument('--input_file', '-i', required=True, help='input text file')
-    parser.add_argument('--results_directory', '-r', required=False, help='result directory', default=config_setup)
+    parser.add_argument('--results_directory', '-r', required=False, help='result directory', default=config_setup['ONCOSPLICE'])
     parser.add_argument('--num_workers', '-n', type=int, required=False, help='number of dask workers to recruit', default=10)
     parser.add_argument('--worker_size', '-m', type=str, required=False, help='dask worker memory allocation', default="3GB")
     args = parser.parse_args()
 
     client, cluster = launch_dask_cluster(memory_size=args.worker_size, num_workers=args.num_workers)
     muts = open(args.input_file, 'r').read().splitlines()
     processed_mutations, last_count = restart_checkpoint(args.results_directory)
```

## geney/splicing/spliceai_utils.py

```diff
@@ -75,32 +75,32 @@
     deleted_pos = {k: {'delta': round(float(v), 3), 'absolute': round(float(mut_dct.get(k, 0)), 3)} for k, v in
                    new_dict.items() if k in known_splice_sites and v <= -threshold}
 
 
     return discovered_pos, deleted_pos
 
 
-def run_spliceai(mutations, sai_mrg_context=5000, min_coverage=2500, sai_threshold=0.5):
+def run_spliceai(mutations, gene_data, sai_mrg_context=5000, min_coverage=2500, sai_threshold=0.5):
     positions = mutations.positions #[m.start for m in mutations]
     seq_start_pos = min(positions) - sai_mrg_context - min_coverage
     seq_end_pos = max(positions) + sai_mrg_context + min_coverage  # + 1
 
     # ref_seq, ref_indices = pull_fasta_seq_endpoints(mutations.chrom, seq_start_pos, seq_end_pos)
     fasta_obj = Fasta_segment()
     ref_seq, ref_indices = fasta_obj.read_segment_endpoints(config_setup['CHROM_SOURCE'] / f'chr{mutations.chrom}.fasta',
                                                 seq_start_pos,
                                                 seq_end_pos)
 
 
-    gene_data = unload_pickle(
-        find_files_by_gene_name(gene_name=mutations.gene, directory=config_setup['MRNA_PATH'] / 'protein_coding'))
-    gene_start, gene_end, rev = gene_data['gene_start'], gene_data['gene_end'], gene_data['rev']
+    # gene_data = unload_pickle(
+    #     find_files_by_gene_name(gene_name=mutations.gene))
+    gene_start, gene_end, rev = gene_data.gene_start, gene_data.gene_end, gene_data.rev
 
     mrna_acceptors = sorted(list(set([lst for lsts in
-                                      [mrna.get('acceptors', []) for mrna in gene_data['transcripts'].values() if
+                                      [mrna.get('acceptors', []) for mrna in gene_data.transcripts.values() if
                                        mrna['transcript_biotype'] == 'protein_coding'] for lst in lsts])))
     mrna_donors = sorted(list(set([lst for lsts in
                                    [mrna.get('donors', []) for mrna in gene_data['transcripts'].values() if
                                     mrna['transcript_biotype'] == 'protein_coding'] for lst in lsts])))
 
     visible_donors = np.intersect1d(mrna_donors, ref_indices)
     visible_acceptors = np.intersect1d(mrna_acceptors, ref_indices)
@@ -149,30 +149,30 @@
     missplicing = {'missed_acceptors': dap, 'missed_donors': ddp, 'discovered_acceptors': iap, 'discovered_donors': idp}
     missplicing = {outk: {float(k): v for k, v in outv.items()} for outk, outv in missplicing.items()}
     return {outk: {int(k) if k.is_integer() else k: v for k, v in outv.items()} for outk, outv in missplicing.items()}
 
 
 
 class PredictSpliceAI:
-    def __init__(self, mutation, threshold=0.5, force=False, sai_mrg_context=5000, min_coverage=2500):
+    def __init__(self, mutation, gene_data, threshold=0.5, force=False, sai_mrg_context=5000, min_coverage=2500):
         self.modification = mutation
         self.threshold = threshold
 
         if '|' in mutation.mut_id:
             self.spliceai_db = config_setup['MISSPLICING_PATH'] / f'spliceai_epistatic'
         else:
             self.spliceai_db = config_setup['MISSPLICING_PATH'] / f'spliceai_individual'
 
         self.missplicing = {}
 
         if self.prediction_file_exists() and not force:
             self.missplicing = self.load_sai_predictions()
 
         else:
-            self.missplicing = run_spliceai(self.modification, sai_mrg_context=sai_mrg_context, min_coverage=min_coverage, sai_threshold=0.1)
+            self.missplicing = run_spliceai(self.modification, gene_data=gene_data, sai_mrg_context=sai_mrg_context, min_coverage=min_coverage, sai_threshold=0.1)
             self.save_sai_predictions()
 
     def __repr__(self):
         return f'Missplicing({self.modification.mut_id}) --> {self.missplicing}'
 
     def __str__(self):
         return self.aberrant_splicing
```

## Comparing `geney-1.0.8.dist-info/METADATA` & `geney-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geney
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package for gene expression modeling.
 Home-page: https://github.com/nicolaslynn/geney
 Author: Nicolas Lynn
 Author-email: nicolasalynn@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

## Comparing `geney-1.0.8.dist-info/RECORD` & `geney-1.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 geney/Fasta_segment.py,sha256=0zCdzPUbDeM9Rz642woH5Q94pwI46O0fE3H8w0XWebc,11255
 geney/Gene.py,sha256=bUYnVTxrOlZ0HcEhOEhzLXI74--bycidnPDzWLfFmNc,8421
 geney/__init__.py,sha256=0H8pdM-c9Btl8lOpW-LcnTJavCMjkDnmsOYNclYxfjo,65
 geney/config_setup.py,sha256=SePeooA4RWAtR_KAT1-W1hkD3MT5tH6YMyp80t_RNPQ,385
 geney/data_setup.py,sha256=NT_cO-s1LPaYtzRA-C3YKpldDdUUPKop-Sd8Ng7I6Zw,10161
-geney/oncosplice_pipeline.py,sha256=U3Q8touQM4X5fXH6Bp3cBIXPSAqKvJ-nJCban1mkxLw,22570
+geney/oncosplice_pipeline.py,sha256=ZrbbQRShtCgG1IVawIrvUfsPHdkUMpYdbaU6yAA_9vE,22576
 geney/utils.py,sha256=QhkElpgzqIRqx38kiVHJqAbc0OFNPNHsGfvXUTEGx60,2374
+geney/analyzers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+geney/analyzers/survival.py,sha256=DvyXLmke-N7dBeLYGcIRSBFFJvAwMp0DR1to-0_X3DM,15384
+geney/analyzers/visualize_protein_conservation.py,sha256=kBIjGcj9DL7BayyxVdnmUHfOqxzO6pF9O1ErYDxkQnk,10726
 geney/mutations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geney/mutations/variant_utils.py,sha256=87EU6gPI6tSEqVRLDAjaohsKI_-1_SaBEchH89WoVpI,10271
 geney/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-geney/pipelines/dask_utils.py,sha256=oZ7qgUHCcDbr48LX7tYHptoRJKBhWVeWwjvy4neXkvI,5635
+geney/pipelines/dask_utils.py,sha256=S2xHMuTQSCl53QspKQgzB2_y_xnkhWjDEmQgmXBPN9Q,5666
 geney/splicing/__init__.py,sha256=ovCOjEniyTPMcUzqIptZF8O5ZVm3DoSA10GzYB6aZ3Y,60
-geney/splicing/spliceai_utils.py,sha256=SJss-53iytOOLRl1iqz-bmTH9TdpfOcKWbe3r_FofNA,11800
+geney/splicing/spliceai_utils.py,sha256=ePglck0iroTwsUBdiuiCCJ1SdGo4miKRmILRzeaPVh4,11779
 geney/translation_initiation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geney/translation_initiation/tis_utils.py,sha256=iXrWVijyPe-f8I9rEVGdxNnXBrOGPoKFjmvaOEnQYNE,4446
 geney/translation_initiation/resources/kozak_pssm.json,sha256=pcd0Olziutq-6H3mFWDCD9cujQ_AlZO-iiOvBl82hqE,1165
 geney/translation_initiation/resources/tis_regressor_model.joblib,sha256=IXb4DUDhJ5rBDKcqMk9zE3ECTZZcdj7Jixz3KpoZ7OA,2592025
 geney/translation_termination/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geney/translation_termination/tts_utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-geney-1.0.8.dist-info/METADATA,sha256=KezFB5XBvBZV4aKsfQOOqM92N6XAIe1Hing0YvqRHDM,1070
-geney-1.0.8.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-geney-1.0.8.dist-info/top_level.txt,sha256=O-FuNUMb5fn9dhZ-dYCgF0aZtfi1EslMstnzhc5IIVo,6
-geney-1.0.8.dist-info/RECORD,,
+geney-1.0.9.dist-info/METADATA,sha256=UI9KwdMYPOOeDXEQnZx8N3AOiVzNJ3HP2iAGqzHOVFo,1070
+geney-1.0.9.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+geney-1.0.9.dist-info/top_level.txt,sha256=O-FuNUMb5fn9dhZ-dYCgF0aZtfi1EslMstnzhc5IIVo,6
+geney-1.0.9.dist-info/RECORD,,
```

