# Comparing `tmp/dtlpymetrics-1.0.98-py3-none-any.whl.zip` & `tmp/dtlpymetrics-1.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 35537 bytes, number of entries: 20
+Zip file size: 35675 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      383 b- defN 23-Nov-02 13:51 dtlpymetrics/__init__.py
--rw-rw-rw-  2.0 fat       20 b- defN 23-Nov-08 08:31 dtlpymetrics/__version__.py
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Nov-16 10:05 dtlpymetrics/__version__.py
 -rw-rw-rw-  2.0 fat     9038 b- defN 23-Jul-18 08:51 dtlpymetrics/dtlpy_scores.py
 -rw-rw-rw-  2.0 fat    21387 b- defN 23-Nov-02 14:02 dtlpymetrics/precision_recall.py
--rw-rw-rw-  2.0 fat    19348 b- defN 23-Nov-08 08:31 dtlpymetrics/scoring.py
+-rw-rw-rw-  2.0 fat    19381 b- defN 23-Nov-16 09:47 dtlpymetrics/scoring.py
 -rw-rw-rw-  2.0 fat       68 b- defN 23-Sep-19 11:59 dtlpymetrics/models/__init__.py
 -rw-rw-rw-  2.0 fat     1248 b- defN 23-Sep-19 11:59 dtlpymetrics/models/image.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Sep-19 11:59 dtlpymetrics/quality_tasks/__init__.py
--rw-rw-rw-  2.0 fat    10991 b- defN 23-Oct-02 10:23 dtlpymetrics/quality_tasks/image.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-Nov-16 09:59 dtlpymetrics/quality_tasks/image.py
 -rw-rw-rw-  2.0 fat     7313 b- defN 23-Sep-19 11:59 dtlpymetrics/quality_tasks/video.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Sep-19 11:59 dtlpymetrics/utils/__init__.py
 -rw-rw-rw-  2.0 fat     4661 b- defN 23-Oct-02 09:55 dtlpymetrics/utils/helpers.py
--rw-rw-rw-  2.0 fat    32585 b- defN 23-Oct-02 10:16 dtlpymetrics/utils/metrics_utils.py
+-rw-rw-rw-  2.0 fat    32948 b- defN 23-Nov-08 14:02 dtlpymetrics/utils/metrics_utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-18 08:51 tests/__init__.py
 -rw-rw-rw-  2.0 fat     7995 b- defN 23-Sep-19 14:34 tests/test_main.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Nov-08 08:33 dtlpymetrics-1.0.98.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6272 b- defN 23-Nov-08 08:33 dtlpymetrics-1.0.98.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-08 08:33 dtlpymetrics-1.0.98.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-Nov-08 08:33 dtlpymetrics-1.0.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1695 b- defN 23-Nov-08 08:33 dtlpymetrics-1.0.98.dist-info/RECORD
-20 files, 134942 bytes uncompressed, 32757 bytes compressed:  75.7%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Nov-16 10:05 dtlpymetrics-1.0.99.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6416 b- defN 23-Nov-16 10:05 dtlpymetrics-1.0.99.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-16 10:05 dtlpymetrics-1.0.99.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Nov-16 10:05 dtlpymetrics-1.0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1695 b- defN 23-Nov-16 10:05 dtlpymetrics-1.0.99.dist-info/RECORD
+20 files, 135483 bytes uncompressed, 32895 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_main.py
 Comment: 
 
-Filename: dtlpymetrics-1.0.98.dist-info/LICENSE
+Filename: dtlpymetrics-1.0.99.dist-info/LICENSE
 Comment: 
 
-Filename: dtlpymetrics-1.0.98.dist-info/METADATA
+Filename: dtlpymetrics-1.0.99.dist-info/METADATA
 Comment: 
 
-Filename: dtlpymetrics-1.0.98.dist-info/WHEEL
+Filename: dtlpymetrics-1.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: dtlpymetrics-1.0.98.dist-info/top_level.txt
+Filename: dtlpymetrics-1.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: dtlpymetrics-1.0.98.dist-info/RECORD
+Filename: dtlpymetrics-1.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dtlpymetrics/__version__.py

```diff
@@ -1 +1 @@
-version = "1.0.98"
+version = "1.0.99"
```

## dtlpymetrics/scoring.py

```diff
@@ -229,22 +229,22 @@
                            dataset_id=item.dataset.id)
         all_scores.append(item_score)
 
         #############################
         # upload scores to platform #
         #############################
         # clean previous scores before creating new ones
-        logger.info(f'About to delete all scores with context item ID: {item.id} and task ID: {task.id}')
-        dl_scores = Scores(client_api=dl.client_api)
-        dl_scores.delete(context={'itemId': item.id,
-                                  'taskId': task.id})
-        dl_scores = dl_scores.create(all_scores)
-        logger.info(f'Uploaded {len(dl_scores)} scores to platform.')
-
-        if os.environ.get('SCORES_DEBUG_PATH', None) is not None:
+        if os.environ.get('SCORES_DEBUG_PATH', None) is None:
+            logger.info(f'About to delete all scores with context item ID: {item.id} and task ID: {task.id}')
+            dl_scores = Scores(client_api=dl.client_api)
+            dl_scores.delete(context={'itemId': item.id,
+                                      'taskId': task.id})
+            dl_scores = dl_scores.create(all_scores)
+            logger.info(f'Uploaded {len(dl_scores)} scores to platform.')
+        else:
             debug_path = os.environ.get('SCORES_DEBUG_PATH', None)
             logger.debug('Saving scores locally')
 
             save_filepath = os.path.join(debug_path, task.id, f'{item.id}.json')
             os.makedirs(os.path.dirname(save_filepath), exist_ok=True)
             scores_json = list()
             for score in all_scores:
```

## dtlpymetrics/quality_tasks/image.py

```diff
@@ -49,15 +49,15 @@
             logger.info(
                 f'Comparing assignee: {assignment_annotator_i!r} with assignee: {assignment_annotator_j!r}')
             annot_collection_1 = annots_by_assignment[assignment_annotator_i]
             annot_collection_2 = annots_by_assignment[assignment_annotator_j]
             # score types that can be returned: ANNOTATION_IOU, ANNOTATION_LABEL, ANNOTATION_ATTRIBUTE
             pairwise_scores = calculate_annotation_score(annot_collection_1=annot_collection_1,
                                                          annot_collection_2=annot_collection_2,
-                                                         ignore_labels=True,
+                                                         ignore_labels=False,
                                                          match_threshold=0.01,
                                                          score_types=score_types)
             for score in pairwise_scores:
                 if score.type == ScoreType.USER_CONFUSION:
                     updated_score = add_score_context(
                         score=score,
                         user_id=assignment_annotator_j,
```

## dtlpymetrics/utils/metrics_utils.py

```diff
@@ -1,10 +1,9 @@
-import logging
 import uuid
-
+import logging
 import dtlpy as dl
 import numpy as np
 import pandas as pd
 
 from dtlpy import entities
 from typing import Union, List
 
@@ -295,15 +294,18 @@
 
 class Match:
     def __init__(self,
                  first_annotation_id, first_annotation_creator, first_annotation_label, first_annotation_confidence,
                  second_annotation_id, second_annotation_creator, second_annotation_label, second_annotation_confidence,
                  item_id,
                  # defaults
-                 annotation_score=0, attributes_score=0, geometry_score=0, label_score=0):
+                 annotation_score: float = 0.,
+                 attributes_score: float = 0.,
+                 geometry_score: float = 0.,
+                 label_score: float = 0.):
         """
         Save a match between two annotations with all relevant scores
 
         :param first_annotation_id:
         :param second_annotation_id:
         :param annotation_score:
         :param attributes_score:
@@ -565,26 +567,30 @@
     @staticmethod
     def general_match(matches: Matches,
                       first_set: entities.AnnotationCollection,
                       second_set: entities.AnnotationCollection,
                       match_type,
                       match_threshold: float,
                       ignore_attributes=False,
-                      ignore_labels=False):
+                      ignore_labels=False,
+                      ignore_geometry=False):
         """
         Finds all matches between two sets of annotations
         :param matches: Matches object to populate
         :param first_set: `AnnotationCollection` or list
         :param second_set: `AnnotationCollection` or list
         :param match_type: type of annotation to match (e.g. box, semantic, etc.)
         :param match_threshold: threshold for including a match
         :param ignore_attributes: ignore attribute score for final annotation score
-        :param ignore_labels: ignore label when comparing - measure only geometry
+        :param ignore_labels: ignore label when comparing - take also wrong label as a match
+        :param ignore_geometry: ignore geometry when comparing - for classification
         :return:
         """
+        if ignore_geometry is True and ignore_labels is True and ignore_attributes is True:
+            raise ValueError('Cant compare annotation with all ignore flags set to True, must choose at least one')
         annotation_type_to_func = {
             entities.AnnotationType.BOX: Matchers.calculate_iou_box,
             entities.AnnotationType.CLASSIFICATION: Matchers.calculate_iou_classification,
             entities.AnnotationType.SEGMENTATION: Matchers.calculate_iou_semantic,
             entities.AnnotationType.POLYGON: Matchers.calculate_iou_polygon,
             entities.AnnotationType.POINT: Matchers.calculate_iou_point,
         }
@@ -622,33 +628,38 @@
             row_index = row_index[0]
             col_index = col_index[0]
             first_annotation_id = df.columns[col_index]
             second_annotation_id = df.index[row_index]
             first_annotation = [a for a in first_set if a.id == first_annotation_id][0]
             second_annotation = [a for a in second_set if a.id == second_annotation_id][0]
             geometry_score = df.iloc[row_index, col_index]
-            labels_score = Matchers.match_labels(label1=first_annotation.label,
-                                                 label2=second_annotation.label)
             attribute_score = Matchers.match_attributes(attributes1=first_annotation.attributes,
                                                         attributes2=second_annotation.attributes)
-
-            # TODO use ignores for final score
-            annotation_score = (geometry_score + attribute_score + labels_score) / 3
+            labels_score = Matchers.match_labels(label1=first_annotation.label,
+                                                 label2=second_annotation.label)
+            match_scores = list()
+            if ignore_geometry is False:
+                match_scores.append(geometry_score)
+            if ignore_attributes is False:
+                match_scores.append(attribute_score)
+            if ignore_labels is False:
+                match_scores.append(labels_score)
+            annotation_score = float(np.mean(match_scores))
             matches.add(match=Match(
                 first_annotation_id=first_annotation_id,
                 first_annotation_creator=first_annotation.creator,
                 first_annotation_label=first_annotation.label,
-                first_annotation_confidence=
-                first_annotation.metadata.get('user', dict()).get('model', dict()).get('confidence', 1),
+                first_annotation_confidence=first_annotation.metadata.get('user', dict()).get('model', dict()).get(
+                    'confidence', 1),
                 second_annotation_id=second_annotation_id,
                 second_annotation_creator=second_annotation.creator,
                 second_annotation_label=second_annotation.label,
-                second_annotation_confidence=
-                second_annotation.metadata.get('user', dict()).get('model', dict()).get('confidence', 1),
-                geometry_score=geometry_score,  # TODO: check these scores should be sent
+                second_annotation_confidence=second_annotation.metadata.get('user', dict()).get('model', dict()).get(
+                    'confidence', 1),
+                geometry_score=geometry_score,
                 annotation_score=annotation_score,
                 label_score=labels_score,
                 attributes_score=attribute_score,
                 item_id=second_annotation.item_id
             ))
             df.drop(index=second_annotation_id, inplace=True)
             df.drop(columns=first_annotation_id, inplace=True)
@@ -665,21 +676,21 @@
                                     second_annotation_confidence=
                                     second_annotation.metadata.get('user', dict()).get('model', dict()).get(
                                         'confidence', 1),
                                     item_id=second_annotation.item_id
                                     ))
         for first_id in df.columns:
             first_annotation = [a for a in first_set if a.id == first_id][0]
-            matches.add(match=Match(first_annotation_id=first_id,
-                                    first_annotation_creator=first_annotation.creator,
-                                    first_annotation_label=first_annotation.label,
-                                    first_annotation_confidence=
-                                    first_annotation.metadata.get('user', dict()).get('model', dict()).get('confidence',
-                                                                                                           1),
-                                    second_annotation_id=None,
-                                    second_annotation_creator=None,
-                                    second_annotation_label=None,
-                                    second_annotation_confidence=None,
-                                    item_id=first_annotation.item_id
-                                    ))
+            matches.add(match=Match(
+                first_annotation_id=first_id,
+                first_annotation_creator=first_annotation.creator,
+                first_annotation_label=first_annotation.label,
+                first_annotation_confidence=first_annotation.metadata.get('user', dict()).get('model', dict()).get(
+                    'confidence', 1),
+                second_annotation_id=None,
+                second_annotation_creator=None,
+                second_annotation_label=None,
+                second_annotation_confidence=None,
+                item_id=first_annotation.item_id
+            ))
 
         return matches
```

## Comparing `dtlpymetrics-1.0.98.dist-info/LICENSE` & `dtlpymetrics-1.0.99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dtlpymetrics-1.0.98.dist-info/METADATA` & `dtlpymetrics-1.0.99.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtlpymetrics
-Version: 1.0.98
+Version: 1.0.99
 Summary: Scoring and metrics app
 Home-page: UNKNOWN
 Author: Dataloop Team
 Author-email: yaya.t@dataloop.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -63,39 +63,40 @@
 - point (distance)
 
 
 ## Score Types
 
 During scoring, the following scores will be created for each annotation:
 
-- `raw_annotation_scores` -  e.g. geometry, label, attribute
+- `raw_annotation_scores` -  for each annotation comparison we have `geometry`, `label` and `attribute` matching scores
 - `annotation_overall` - the mean of each annotation’s raw scores
 - `user_confusion_score` - the mean of every annotation overall score, relative to ref or another assignee
 - `item_confusion_score` - the count of the number of label pairs associated with the assignee’s label, relative to the reference’s label
 - `item_overall_score` - the mean value of *each* annotation overall score associated with an item
 
 **1) Raw annotation scores:** 
 
-There are three types of scores for annotations: geometry (such as IOU), label, and attribute. These scores can be determined by the user, and the default is to include all three scores, and the default value is 1 (which can be modified).
+There are three types of scores for annotations: `annotation_iou`, `annotation_label` and `annotation_attribute`.  
+These scores can be determined by the user, and the default is to include all three scores, and the default value is 1 (which can be modified).
 
 **2) Annotation overall**
 
-This is the mean value for all raw annotation scores per annotation. 
+For `annotation_overall` score we calculate the mean value for all raw annotation scores per annotation. 
 
 **3) User confusion score**
 
-The value of this score represents the mean annotation score a given assignee has, relative to raw scores when comparing it to another set of annotations (either the reference or another assignee). 
+The `user_confusion` score represents the mean annotation score a given assignee has, relative to raw scores when comparing it to another set of annotations (either the reference or another assignee). 
 
-**4) Item confusion score**
+**4) Label confusion score**
 
-The value of this score represents the count for a label annotated by a given assignee, relative to label each label class in the other set of annotations (either reference or another assignee).
+The `label_confusion` score represents the count for a label annotated by a given assignee, relative to label each label class in the other set of annotations (either reference or another assignee).
 
 **5) Item overall score**
 
-This is the mean value of all annotations associated with an item, averaging the mean overall annotation score.
+The `item_overall` score is the mean value of all annotations associated with an item, averaging the mean overall annotation score.
 
 Any calculated and uploaded scores will replace any previous scores for all items of a given task.
 
 _Note about videos_: Video scores will differ slightly from image scores. Video sores are calculated frame by frame, and then specific annotation scores will be the average of these scores across all relevant frames for that specific annotation. Confusion scores are not calculated due to the multi-frame nature of videos. Item overall scores remain an average of all annotations of the video item.
 
 ## Confusion Example
```

## Comparing `dtlpymetrics-1.0.98.dist-info/RECORD` & `dtlpymetrics-1.0.99.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dtlpymetrics/__init__.py,sha256=K4BcmjyW4yN4nR_HeJs15Q22zSsnjJAgL5zY8xNqgtg,383
-dtlpymetrics/__version__.py,sha256=Ew66hFyc-xrZJBKtJlkUw_gMJR_4iNWfct3zly9t90s,20
+dtlpymetrics/__version__.py,sha256=xbxt3WVuVdpqQAiAs4cTsME8pT3DqdOcsOkA7s_nJ-s,20
 dtlpymetrics/dtlpy_scores.py,sha256=VkaKlzzaiXzbHh2otuNI9NJB70SY-EGLZM6v4HMDiiA,9038
 dtlpymetrics/precision_recall.py,sha256=3tj-Tm9QYBUHBst_pZf9w6BlvNQvseVJnOXewuISelI,21387
-dtlpymetrics/scoring.py,sha256=W-fhIOS569rHEpVXDYj5Q0TzehLkTKwbM8IcDF3gago,19348
+dtlpymetrics/scoring.py,sha256=xnJBS1dYIHgHcTxhIWk4KLLTsCujAD-Kr7bL_0erFFI,19381
 dtlpymetrics/models/__init__.py,sha256=ADUhMGhythsNlDcnZALmg0Gzpk_gG7cMXk3dP8Kifl4,68
 dtlpymetrics/models/image.py,sha256=qbTPzSWDg_17zGyRExfLd58vQYy4S3RUo57UuiQ3P0I,1248
 dtlpymetrics/quality_tasks/__init__.py,sha256=2ww2H1EAUw1n1Ik18TnHkQVNMVSQZ0sb7m773boFFZQ,55
-dtlpymetrics/quality_tasks/image.py,sha256=8HuZzs2uEJUchxQWnrFSj1Y6NsPY5Gf47TVxIMTlbTg,10991
+dtlpymetrics/quality_tasks/image.py,sha256=kv--SMg0OrnJRzAbo6omQtpcLKI32MM8_PVtYskFvak,10992
 dtlpymetrics/quality_tasks/video.py,sha256=ek3_DZr952GH9IgvUJYF8-iray-flbXTzVs4dHX7YMQ,7313
 dtlpymetrics/utils/__init__.py,sha256=2pBHILWP-_hvdVhkCngVsVNPTj9J3Nzad80f6zeOSAY,214
 dtlpymetrics/utils/helpers.py,sha256=NStAXDaF-0niSStO-9UDijBngp1SWJYtfW9m0vPu52s,4661
-dtlpymetrics/utils/metrics_utils.py,sha256=Ntr4anzdIMeT0TizJgsWKAp84w2b49b3ZWYc2mMEScU,32585
+dtlpymetrics/utils/metrics_utils.py,sha256=Eu7paUJZnB6Z4bPRimGn5HOIXLy97FobBxDMyKN55LY,32948
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_main.py,sha256=1RT5Z4ijW7NnN44Ht0TnFB-SsS3nHKCDxnQ-vpNaL-8,7995
-dtlpymetrics-1.0.98.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-dtlpymetrics-1.0.98.dist-info/METADATA,sha256=XmoM9QGfLJlz3oIOwpwCGvymAukneepr1nYJW1ueF0I,6272
-dtlpymetrics-1.0.98.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-dtlpymetrics-1.0.98.dist-info/top_level.txt,sha256=qRgwy6OXIKUVIH-QSPDVnVfQcIfSjIi38UwVmMqyW2Q,19
-dtlpymetrics-1.0.98.dist-info/RECORD,,
+dtlpymetrics-1.0.99.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+dtlpymetrics-1.0.99.dist-info/METADATA,sha256=2yxhQsGr5kZGF8yiw0kX6jrpPO6t1NUnyIMoo_iBqlU,6416
+dtlpymetrics-1.0.99.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+dtlpymetrics-1.0.99.dist-info/top_level.txt,sha256=qRgwy6OXIKUVIH-QSPDVnVfQcIfSjIi38UwVmMqyW2Q,19
+dtlpymetrics-1.0.99.dist-info/RECORD,,
```

