# Comparing `tmp/mimllearning-0.3.9.tar.gz` & `tmp/mimllearning-0.4.0.tar.gz`

## Comparing `mimllearning-0.3.9.tar` & `mimllearning-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.9/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.9/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/data/instance.py
--rw-r--r--   0        0        0    18278 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.9/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.9/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.9/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.0/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.0/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10536 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/data/instance.py
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/tutorial/miml_data.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.0/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.0/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.0/PKG-INFO
```

### Comparing `mimllearning-0.3.9/readme.md` & `mimllearning-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.4.0/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/classifier/miml_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,113 @@
 import numpy as np
-from abc import ABC, abstractmethod
+from abc import abstractmethod
+from ..miml_classifier import MIMLClassifier
+from ...data import Bag
+from ...data import MIMLDataset
 
-from ..data import Bag
-from ..data import MIMLDataset
 
-
-class MIMLClassifier(ABC):
+class MIMLtoMIClassifier(MIMLClassifier):
     """
-    Class to represent a MIMLClassifier
+    Class to represent a multi-instance classifier
     """
 
-    def __init__(self) -> None:
-        """
-        Constructor of the class MIMLClassifier
-        """
-        self.classifier = None
-
-    def fit(self, dataset_train: MIMLDataset) -> None:
+    def __init__(self, mi_classifier) -> None:
         """
-        Training the classifier
+        Constructor of the class MIMLtoMIClassifier
 
         Parameters
         ----------
-        dataset_train : MIMLDataset
-            Dataset to train the classifier
+        mi_classifier
+            Specific classifier to be used
         """
-        # if not isinstance(dataset_train, MIMLDataset):
-        #    raise Exception("Fit function should receive a MIMLDataset as parameter")
-
-        self.fit_internal(dataset_train)
+        super().__init__()
+        self.classifier = mi_classifier
 
     @abstractmethod
     def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
-        Internal method to train the classifier
+        Training the classifier
 
         Parameters
         ----------
-        dataset_train : MIMLDataset
+        dataset_train: MIMLDataset
             Dataset to train the classifier
         """
         pass
 
     @abstractmethod
     def predict(self, x: np.ndarray) -> np.ndarray:
         """
-         Predict labels of given data
+        Predict labels of given data
 
-         Parameters
-         ----------
-         x : ndarray of shape (n, n_labels)
-             Data to predict their labels
+        Parameters
+        ----------
+        x : ndarray of shape (n_instances, n_labels)
+            Data to predict their labels
 
         Returns
-        ----------
-        results : ndarray of shape (n_bags, n_labels)
-            Predicted labels of data
+        -------
+        results : ndarray of shape (n_labels)
+            Predicted labels
         """
-        # if not isinstance(x, np.ndarray):
-        #    raise Exception("Predict function should receive a Numpy array as parameter")
+        pass
 
-    @abstractmethod
     def predict_bag(self, bag: Bag) -> np.ndarray:
         """
         Predict labels of a given bag
 
         Parameters
         ----------
         bag : Bag
             Bag to predict their labels
 
         Returns
-        ----------
-        results : ndarray of shape (n_bags, n_labels)
+        -------
+        results : ndarray of shape (n_labels)
             Predicted labels of the bag
         """
-        # if not isinstance(bag, Bag):
-        #    raise Exception("Predict function should receive a Numpy array as parameter")
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        return self.predict(bag.get_features())
 
     @abstractmethod
     def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
-        # TODO: DOC
+        """
+        Predict probabilities of given dataset of having a positive label
+
+        Parameters
+        ----------
+        dataset_test : MIMLDataset
+            Dataset to predict probabilities
+
+        Returns
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given dataset
+        """
+
         pass
 
-    @abstractmethod
     def evaluate(self, dataset_test: MIMLDataset) -> np.ndarray:
         """
         Evaluate the model on a test dataset
 
         Parameters
         ----------
         dataset_test : MIMLDataset
-            Test dataset to evaluate the model on.
+            Test dataset to evaluate the model on
 
         Returns
         ----------
         results : ndarray of shape (n_bags, n_labels)
             Predicted labels of dataset_test
         """
-        # if not isinstance(dataset_test, MIMLDataset):
-        #    raise Exception("Evaluate function should receive a MIMLDataset as parameter")
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
+        # Features are the same in all datasets
+        for i, bag in enumerate(dataset_test.get_features_by_bag()):
+            results[i] = self.predict(bag)
+
+        return results
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,27 @@
         """
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
     def predict_proba(self, x: np.ndarray):
+        """
+        Predict probabilities of given data of having a positive label
+
+        Parameters
+        ----------
+        x : np.ndarray of shape (n_instances, n_features)
+            Data to predict probabilities
+
+        Returns
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given data
+        """
         result = np.zeros(x.shape[0])
         for i in range(x.shape[0]):
             result[i] = self.predict(x[i])
         return result
 
     def generate_apr(self, x_train, y_train) -> None:
         """
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mi/apr_classifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
     Approach is to construct an APR by starting with
     a single positive instance and “growing” the APR by expanding it to cover additional
     positive instances.
     We call it the “iterated discrimination” algorithm, and it has three basic procedures:
     -Grow. An algorithm for growing an APR with “tight” bounds along a specified set
     of features.
-    -Discrim. An algorithm for choosing a set of discriminating features by analyzing
+    -Discriminate. An algorithm for choosing a set of discriminating features by analyzing
     an APR.
     -Expand. An algorithm for expanding the bounds of an APR to improve its generalization ability.
 
     Attributes
     ----------
     classifier
         Classifier used from mil library
@@ -56,16 +56,29 @@
             features values of a bag
 
         Returns
         -------
         label: int
             Predicted label of the bag
         """
-        # TODO: Revisar dimensiones de x, que pasa si llamo a predict con varias bolsas
+        # TODO: Check x shape, what happens if i call predict with various bags
         x = x.reshape(1, x.shape[0], x.shape[1])
         return self.classifier.predict(x)
 
     def predict_proba(self, x: np.ndarray):
+        """
+        Predict probabilities of given data
+
+        Parameters
+        ----------
+        x : np.ndarray of shape (n_instances, n_features)
+            Probabilities of data of being a positive label.
+
+        Returns
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+             Predicted probabilities for given data
+        """
         result = np.zeros(x.shape[0])
         for i in range(x.shape[0]):
             result[i] = self.predict(x[i])
         return result
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mi/miles_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sklearn.tree import DecisionTreeClassifier
 import numpy as np
 
 
 class MILESClassifier:
 
     """
-    Mapping bags to a instance based feature space, from paper
+    Mapping bags to an instance based feature space, from paper
 
     Attributes
     ----------
     classifier
         Classifier used from mil library
 
     model
@@ -56,15 +56,15 @@
 
         # train the SVM
         # self.model = LinearSVC(penalty="l1", C=self.c, dual=False, class_weight='balanced',max_iter=100000)
 
         self.model = DecisionTreeClassifier()
         self.model.fit(mapped_bags, y_train.flatten())
 
-    def predict(self, bag) -> int:
+    def predict(self, bag: np.ndarray) -> int:
         """
         Predict the label of the bag
 
         Parameters
         ----------
         bag: np.ndarray of shape(n_instances, n_features)
             features values of a bag
@@ -76,12 +76,26 @@
 
         """
         bag = bag.reshape(1, bag.shape[0], bag.shape[1])
         mapped_bag = self.mapping.transform(bag)
         return self.model.predict(mapped_bag)
 
     def predict_proba(self, x: np.ndarray):
-        # TODO: DOC y test, esto esta mal por concepto. Ver como implementarlo
+        """
+        Predict probabilities of given data
+
+        Parameters
+        ----------
+        x : np.ndarray of shape (n_instances, n_features)
+            Probabilities of data of being a positive label.
+
+        Returns
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given data
+        """
+        # TODO: fix, this is a patch. Dont know how to implement it
+
         result = np.zeros(x.shape[0])
         for i in range(x.shape[0]):
             result[i] = self.predict(x[i])
         return result
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,107 @@
 import numpy as np
-from copy import deepcopy
-
-from .miml_to_mi_classifier import MIMLtoMIClassifier
-from ...transformation import BinaryRelevanceTransformation
-from ...data import Bag
 from ...data import MIMLDataset
+from ...data import Bag
+from ..miml_classifier import MIMLClassifier
+from ...transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
 
 
-class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
-    """
-    Class to represent a multiinstance classifier
-    """
+class MIMLtoMLClassifier(MIMLClassifier):
 
-    def __init__(self, classifier) -> None:
+    def __init__(self, ml_classifier, transformation: MIMLtoMLTransformation) -> None:
         """
-        Constructor of the class MIMLtoMIBRClassifier
+        Constructor of the class MIMLtoMIClassifier
 
         Parameters
         ----------
-        classifier
+        ml_classifier
             Specific classifier to be used
+
+        transformation : MIMLtoMLTransformation
+            Transformation to be used
         """
-        super().__init__(classifier)
-        self.transformation = BinaryRelevanceTransformation()
-        self.classifiers = []
+        super().__init__()
+        self.classifier = ml_classifier
+        self.transformation = transformation
 
     def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
         Training the classifier
 
         Parameters
         ----------
-        dataset_train: MIMLDataset
+        dataset_train : MIMLDataset
             Dataset to train the classifier
         """
-        for x in range(dataset_train.get_number_labels()):
-            classifier = deepcopy(self.classifier)
-            self.classifiers.append(classifier)
-
-        datasets = self.transformation.transform_dataset(dataset_train)
-        for i, dataset in enumerate(datasets):
-            self.classifiers[i].fit(dataset.get_features_by_bag(), dataset.get_labels_by_bag())
+        transformed_dataset_train = self.transformation.transform_dataset(dataset_train)
+        self.classifier.fit(transformed_dataset_train.get_features(), transformed_dataset_train.get_labels())
+        self.trained = True
 
     def predict(self, x: np.ndarray) -> np.ndarray:
         """
-        Predict labels of given data
+         Predict labels of given data
 
-        Parameters
-        ----------
-        x : ndarray of shape (n_instances, n_labels)
-            Data to predict their labels
+         Parameters
+         ----------
+         x : ndarray of shape (n_instances, n_labels)
+             Data to predict their labels
+
+         Returns
+         ----------
+         results : ndarray of shape (n_instances, n_labels)
+             Predicted labels of data
+         """
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        Returns
-        -------
-        results : ndarray of shape (n_labels)
-            Predicted labels
-        """
-        results = np.zeros((len(self.classifiers)))
-        # Prediction of each label
-        for i in range(len(self.classifiers)):
-            results[i] = self.classifiers[i].predict(x)
-        return results
+        return self.classifier.predict(x)
 
     def predict_bag(self, bag: Bag) -> np.ndarray:
         """
         Predict labels of a given bag
 
         Parameters
         ----------
         bag : Bag
             Bag to predict their labels
 
         Returns
-        -------
-        results : ndarray of shape (n_labels)
-            Predicted labels of the bag
+         ----------
+         results : ndarray of shape (n_labels)
+             Predicted labels of data
         """
-        # super().predict_bag(bag)
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+        transformed_bag = self.transformation.transform_bag(bag)
 
-        bags = self.transformation.transform_bag(bag)
+        return self.predict(transformed_bag.get_features())
 
-        return self.predict(bags[0].get_features())
+    def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
+        """
+        Predict probabilities of given dataset of having a positive label
 
-    def predict_proba(self, dataset_test: MIMLDataset):
-        # TODO: DOC
-        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
-        datasets = self.transformation.transform_dataset(dataset_test)
+        Parameters
+        ----------
+        dataset_test : MIMLDataset
+            Dataset to predict probabilities
 
-        for i in range(len(datasets)):
-            results[0:, i] = self.classifiers[i].predict_proba(datasets[i].get_features_by_bag())
+        Returns
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given dataset
+        """
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
+        transformed_dataset_test = self.transformation.transform_dataset(dataset_test)
+        probs = self.classifier.predict_proba(transformed_dataset_test.get_features())
+        for i, label in enumerate(probs):
+            # It takes the probability of being a positive class
+            results[0:, i] = label[0:, 1]
         return results
 
     def evaluate(self, dataset_test: MIMLDataset) -> np.ndarray:
         """
         Evaluate the model on a test dataset
 
         Parameters
@@ -101,17 +110,14 @@
             Test dataset to evaluate the model on
 
         Returns
         ----------
         results : ndarray of shape (n_bags, n_labels)
             Predicted labels of dataset_test
         """
-        # super().evaluate(dataset_test)
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        datasets = self.transformation.transform_dataset(dataset_test)
-
-        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
-        # Features are the same in all datasets
-        for i, bag in enumerate(datasets[0].get_features_by_bag()):
-            results[i] = self.predict(bag)
+        transformed_dataset_test = self.transformation.transform_dataset(dataset_test)
+        results = self.predict(transformed_dataset_test.get_features())
 
         return results
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,80 @@
 import numpy as np
-from abc import abstractmethod
-from ..miml_classifier import MIMLClassifier
+from copy import deepcopy
+
+from .miml_to_mi_classifier import MIMLtoMIClassifier
+from ...transformation import LabelPowersetTransformation
 from ...data import Bag
 from ...data import MIMLDataset
 
 
-class MIMLtoMIClassifier(MIMLClassifier):
+class MIMLtoMILPClassifier(MIMLtoMIClassifier):
     """
-    Class to represent a multiinstance classifier
+    Class to represent a multi-instance classifier
     """
 
-    def __init__(self, mi_classifier) -> None:
+    def __init__(self, classifier) -> None:
         """
-        Constructor of the class MIMLtoMIClassifier
+        Constructor of the class MIMLtoMILPClassifier
 
         Parameters
         ----------
-        mi_classifier
+        classifier
             Specific classifier to be used
         """
-        super().__init__()
-        self.classifier = mi_classifier
+        super().__init__(classifier)
+        self.transformation = LabelPowersetTransformation()
 
-    @abstractmethod
     def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
         Training the classifier
 
         Parameters
         ----------
         dataset_train: MIMLDataset
             Dataset to train the classifier
         """
-        pass
+        dataset = self.transformation.transform_dataset(dataset_train)
+        self.classifier.fit(dataset.get_features_by_bag(), dataset.get_labels_by_bag())
+        self.trained = True
 
-    @abstractmethod
     def predict(self, x: np.ndarray) -> np.ndarray:
         """
         Predict labels of given data
 
         Parameters
         ----------
-        x : ndarray of shape (n_instances, n_labels)
+        x : ndarray of shape (n_instances, n_features)
             Data to predict their labels
 
         Returns
         -------
         results : ndarray of shape (n_labels)
             Predicted labels
         """
-        pass
-
-    @abstractmethod
-    def predict_bag(self, bag: Bag) -> np.ndarray:
-        """
-        Predict labels of a given bag
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        Parameters
-        ----------
-        bag : Bag
-            Bag to predict their labels
-
-        Returns
-        -------
-        results : ndarray of shape (n_labels)
-            Predicted labels of the bag
-        """
-        pass
+        # Prediction of each label
+        results = self.classifier.predict(x)
+        binary_str = np.binary_repr(results, width=self.transformation.dataset.get_number_labels())
+        return np.array([int(bit) for bit in binary_str])
 
-    @abstractmethod
     def predict_proba(self, dataset_test: MIMLDataset):
         """
-
-        """
-        pass
-
-    @abstractmethod
-    def evaluate(self, dataset_test: MIMLDataset) -> np.ndarray:
-        """
-        Evaluate the model on a test dataset
+        Predict probabilities of given dataset of having a positive label
 
         Parameters
         ----------
         dataset_test : MIMLDataset
-            Test dataset to evaluate the model on
+            Dataset to predict probabilities
 
         Returns
-        ----------
-        results : ndarray of shape (n_bags, n_labels)
-            Predicted labels of dataset_test
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given dataset
         """
-        pass
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        return self.classifier.predict_proba(dataset_test.get_features_by_bag())
+
```

### Comparing `mimllearning-0.3.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.4.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,91 @@
 import numpy as np
-from ...data import MIMLDataset
+from copy import deepcopy
+
+from .miml_to_mi_classifier import MIMLtoMIClassifier
+from ...transformation import BinaryRelevanceTransformation
 from ...data import Bag
-from ..miml_classifier import MIMLClassifier
-from ...transformation.mimlTOml.miml_to_ml_transformation import MIMLtoMLTransformation
+from ...data import MIMLDataset
 
 
-class MIMLtoMLClassifier(MIMLClassifier):
+class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
+    """
+    Class to represent a multi-instance classifier
+    """
 
-    def __init__(self, ml_classifier, transformation: MIMLtoMLTransformation) -> None:
+    def __init__(self, classifier) -> None:
         """
-        Constructor of the class MIMLtoMIClassifier
+        Constructor of the class MIMLtoMIBRClassifier
 
         Parameters
         ----------
-        ml_classifier
+        classifier
             Specific classifier to be used
-
-        transformation : MIMLtoMLTransformation
-            Transformation to be used
         """
-        super().__init__()
-        self.classifier = ml_classifier
-        self.transformation = transformation
+        super().__init__(classifier)
+        self.transformation = BinaryRelevanceTransformation()
+        self.classifiers = []
 
     def fit_internal(self, dataset_train: MIMLDataset) -> None:
         """
         Training the classifier
 
         Parameters
         ----------
-        dataset_train : MIMLDataset
+        dataset_train: MIMLDataset
             Dataset to train the classifier
         """
-        transformed_dataset_train = self.transformation.transform_dataset(dataset_train)
-        self.classifier.fit(transformed_dataset_train.get_features(), transformed_dataset_train.get_labels())
+        for x in range(dataset_train.get_number_labels()):
+            classifier = deepcopy(self.classifier)
+            self.classifiers.append(classifier)
+
+        datasets = self.transformation.transform_dataset(dataset_train)
+        for i, dataset in enumerate(datasets):
+            self.classifiers[i].fit(dataset.get_features_by_bag(), dataset.get_labels_by_bag())
 
-    def predict(self, x: np.ndarray) -> np.ndarray:
-        """
-         Predict labels of given data
-
-         Parameters
-         ----------
-         x : ndarray of shape (n_instances, n_labels)
-             Data to predict their labels
-
-         Returns
-         ----------
-         results : ndarray of shape (n_instances, n_labels)
-             Predicted labels of data
-         """
-        return self.classifier.predict(x)
+        self.trained = True
 
-    def predict_bag(self, bag: Bag) -> np.ndarray:
+    def predict(self, x: np.ndarray) -> np.ndarray:
         """
-        Predict labels of a given bag
+        Predict labels of given data
 
         Parameters
         ----------
-        bag : Bag
-            Bag to predict their labels
+        x : ndarray of shape (n_instances, n_labels)
+            Data to predict their labels
 
         Returns
-         ----------
-         results : ndarray of shape (n_labels)
-             Predicted labels of data
-        """
-
-        # TODO: La bag por parametro tambien tiene que tener un dataset asociada para coger las features,
-        # sino no se puede predecir. Mostrar error
-        transformed_bag = self.transformation.transform_bag(bag)
-
-        return self.predict(transformed_bag.get_features())
-
-    def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
-        # TODO: DOC
-        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
-        transformed_dataset_test = self.transformation.transform_dataset(dataset_test)
-        probs = self.classifier.predict_proba(transformed_dataset_test.get_features())
-        for i, label in enumerate(probs):
-            # It takes the probability of being a positive class
-            results[0:, i] = label[0:, 1]
+        -------
+        results : ndarray of shape (n_labels)
+            Predicted labels
+        """
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        results = np.zeros((len(self.classifiers)))
+        # Prediction of each label
+        for i in range(len(self.classifiers)):
+            results[i] = self.classifiers[i].predict(x)
         return results
 
-    def evaluate(self, dataset_test: MIMLDataset) -> np.ndarray:
+    def predict_proba(self, dataset_test: MIMLDataset):
         """
-        Evaluate the model on a test dataset
+        Predict probabilities of given dataset of having a positive label
 
-        Parameters
+       Parameters
         ----------
         dataset_test : MIMLDataset
-            Test dataset to evaluate the model on
+            Dataset to predict probabilities
 
         Returns
-        ----------
-        results : ndarray of shape (n_bags, n_labels)
-            Predicted labels of dataset_test
+        -------
+        results: np.ndarray of shape (n_instances, n_features)
+            Predicted probabilities for given dataset
         """
-        # super().evaluate(dataset_test)
-        transformed_dataset_test = self.transformation.transform_dataset(dataset_test)
-        results = self.predict(transformed_dataset_test.get_features())
+        if not self.trained:
+            raise Exception("The classifier is not trained. You need to call fit before predict anything")
+
+        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
 
+        for i in range(len(self.classifiers)):
+            results[0:, i] = self.classifiers[i].predict_proba(dataset_test.get_features_by_bag())
         return results
```

### Comparing `mimllearning-0.3.9/src/miml/data/bag.py` & `mimllearning-0.4.0/src/miml/data/bag.py`

 * *Files 10% similar despite different names*

```diff
@@ -285,32 +285,51 @@
         Parameters
         ----------
         dataset : MIMLDataset
             Dataset for the bag
         """
         self.dataset = dataset
 
-    def show_bag(self, mode="table") -> None:
+    def show_bag(self, attributes: list[str], mode="table") -> None:
         """
         Show bag info in table format
 
         Parameters
         ----------
         mode : str
             Mode to show the bag. Modes available are "table" and "compact" (csv format)
+        attributes : list[str]
+            List of attributes to display. If empty, all attributes will be displayed.
         """
-        header = [self.key] + [""] * self.get_number_attributes()
-        if self.dataset is not None:
-            header = [self.key] + self.get_features_name() + self.get_labels_name()
+        header = [self.key]
+
+        if not attributes:
+            header += [""] * self.get_number_attributes()
+            if self.dataset is not None:
+                header = [self.key] + self.get_features_name() + self.get_labels_name()
+        else:
+            header = [self.key] + attributes
+
         if mode == "table":
             table = [header]
             for index_instance in range(self.get_number_instances()):
-                table.append([index_instance] + list(self.get_instance(index_instance).get_attributes()))
+                instance_attributes = list(self.get_instance(index_instance).get_attributes())
+                if not attributes:
+                    table.append([index_instance] + instance_attributes)
+                else:
+                    filtered_instance_attributes = [instance_attributes[i] for i in range(len(instance_attributes)) if
+                                                    self.get_attributes_name()[i] in attributes]
+                    table.append([index_instance] + filtered_instance_attributes)
+
             print(tabulate(table, headers='firstrow', tablefmt="grid", numalign="center"))
 
         elif mode == "compact":
             print(", ".join(header))
             for index_instance in range(self.get_number_instances()):
-                print(", ".join([self.key] + list(self.get_instance(index_instance).get_attributes())))
+                instance_attributes = list(self.get_instance(index_instance).get_attributes())
+                if attributes:
+                    instance_attributes = [instance_attributes[i] for i in range(len(instance_attributes))
+                                           if header[i + 1] in attributes]
+                print(", ".join([self.key] + instance_attributes))
 
         else:
             raise Exception("Mode not available. Mode options are \"table\" and \"compact\"")
```

### Comparing `mimllearning-0.3.9/src/miml/data/instance.py` & `mimllearning-0.4.0/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/data/miml_dataset.py` & `mimllearning-0.4.0/src/miml/data/miml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -303,40 +303,40 @@
 
     def add_instance(self, bag, instance: Instance) -> None:
         """
         Add an Instance to a Bag of the dataset
 
         Parameters
         ----------
-        bag : str
+        bag : int/str
             Index or key of the bag where the instance will be added
 
         instance : Instance
             Instance of Instance class to be added
         """
-        #TODO: Test if it works
-        bag = self.get_bag(bag)
-        bag.add_instance(instance)
-        self.data[bag] = bag
+        # TODO: Test if it works
+        new_bag = self.get_bag(bag)
+        new_bag.add_instance(instance)
+        self.data[new_bag.key] = new_bag
 
     def delete_instance(self, bag, index_instance: int) -> None:
         """
         Delete an instance of a bag of the dataset
 
         Parameters
         ----------
         bag : int/str
             Index or key of the bag which contains the instance to be deleted
 
         index_instance : int
             Index of the instance to be deleted
         """
-        bag = self.get_bag(bag)
-        bag.delete_instance(index_instance)
-        self.data[bag] = bag
+        new_bag = self.get_bag(bag)
+        new_bag.delete_instance(index_instance)
+        self.data[new_bag.key] = new_bag
 
     def get_attribute(self, bag, instance, attribute) -> float:
         """
         Get value of an attribute of the bag
 
         Parameters
         ----------
@@ -370,36 +370,39 @@
 
         attribute: int/str
             Attribute of the dataset
 
         value: float
             New value for the update
         """
-        bag = self.get_bag(bag)
-        bag.set_attribute(index_instance, attribute, value)
-        self.data[bag] = bag
+        new_bag = self.get_bag(bag)
+        new_bag.set_attribute(index_instance, attribute, value)
+        self.data[new_bag.key] = new_bag
 
     def add_attribute(self, position: int, values=None) -> None:
         """
         Add attribute to the dataset
 
         Parameters
         ----------
         position : int
             Index for the new attribute
 
         values:  ndarray of shape(n_instances)
             Values for the new attribute
         """
-        # TODO: Arreglar
-        for bag_index, bag in enumerate(self.data.keys()):
-            add_values = values[bag_index]
+        # TODO: Test on tutorial
+        count = 0
+        for bag_index in enumerate(range(self.get_number_bags())):
+            bag = self.get_bag(bag_index)
+            add_values = values[count:bag.get_number_instances()+count]
             if values is None:
                 add_values = np.zeros(self.data[bag].get_number_instances())
-            self.data[bag].add_attribute(position, add_values)
+            self.data[bag.key].add_attribute(position, add_values)
+            count += bag.get_number_instances()
 
     def delete_attribute(self, position: int) -> None:
 
         """
         Delete attribute of the dataset
 
         Parameters
@@ -407,101 +410,116 @@
         position : int
             Index of the attribute to be deleted
         """
         for bag in self.data.keys():
             self.data[bag].data = np.delete(self.data[bag].data, position, axis=1)
         self.attributes.pop(list(self.attributes)[position])
 
-    def show_dataset(self, mode: str="table", head: int = None, attributes=None, labels=None, info=True) -> None:
+    def show_dataset(self, mode: str = "table", start: int = 0, end: int = None, attributes=None, info=False) -> None:
         """
         Function to show information about the dataset
 
         Parameters
         ----------
-            head : int
-                Number of the nth firsts bag to show
+            start : int
+                Index of bag to start showing
+
+            end : int
+                Index of bag to end showing
 
             attributes: List of string
                 Attributes to show
 
-            labels : List of string
-                Labels to show
-
             info: Boolean
                 Show more info
         """
-        # TODO: Hacer algo como head y tail de pandas, ponerlo como parametro quizas, tambien lista atributos y labels
-        #  a mostrar opcionales
+        # TODO: implement head and tail functionality from pandas, optional attributes list too
         if info:
             print("Name: ", self.get_name())
             print("Features: ", self.get_features_name())
             print("Labels: ", self.get_labels_name())
             print("Bags:")
 
+        if end is None:
+            end = self.get_number_bags()-1
+
         if mode == "table":
-            for bag_index in range(self.get_number_bags()):
+            for bag_index in range(start, end+1):
                 bag = self.get_bag(bag_index)
-                bag.show_bag()
-                if head is not None:
-                    if bag_index+1 >= head:
-                        break
+                bag.show_bag(attributes)
 
         elif mode == "compact":
-            header = [self.name] + self.get_features_name() + self.get_labels_name()
+            header = ["bag_id"] + self.get_features_name() + self.get_labels_name()
+            if attributes:
+                header = ["bag_id"] + attributes
             print(", ".join(header))
-            for bag_index in range(self.get_number_bags()):
+            for bag_index in range(start, end+1):
                 bag = self.get_bag(bag_index)
                 for index_instance in range(bag.get_number_instances()):
-                    print(", ".join([bag.key] + list(bag.get_instance(index_instance).get_attributes())))
-
-                if head is not None:
-                    if bag_index+1 >= head:
-                        break
-
+                    instance_attributes = list(bag.get_instance(index_instance).get_attributes().astype(str))
+                    if attributes:
+                        instance_attributes = [instance_attributes[i] for i in range(len(instance_attributes))
+                                               if self.get_attributes_name()[i] in attributes]
+                    print(",".join(list([bag.key] + instance_attributes)))
         else:
             raise Exception("Mode not available. Mode options are \"table\" and \"compact\"")
 
-    def split_dataset(self, train_percentage: float=0.8, seed=0):
-        for count_label in np.sum(self.get_features_by_bag(), 1):
-            print(count_label)
+    def split_dataset(self, train_percentage: float = 0.8, seed=0):
+
+        for count_label in np.sum(self.get_labels_by_bag(), 0):
+            # print(count_label)
             if count_label == 0:
-                raise Exception("Dataset contain a label with no positive instance for a label")
+                raise Exception("Dataset contain a label with no positive instance")
 
         random.seed(seed)
-        labels_train = [range(self.get_number_labels())]
-        bags_not_used = [range(self.get_number_bags())]
+        labels_train = list(range(self.get_number_labels()))
+        bags_not_used = list(range(self.get_number_bags()))
+
+        number_bags_train = self.get_number_bags() * train_percentage
 
         dataset_train = MIMLDataset()
-        dataset_train.set_name(self.get_name()+"_train")
+        dataset_train.set_name(self.get_name() + "_train")
         dataset_train.set_features_name(self.get_features_name())
         dataset_train.set_labels_name(self.get_labels_name())
 
         dataset_test = MIMLDataset()
         dataset_test.set_name(self.get_name() + "_test")
         dataset_test.set_features_name(self.get_features_name())
         dataset_test.set_labels_name(self.get_labels_name())
 
         while bags_not_used and labels_train:
-            bag_index = random.randint(0, len(bags_not_used)-1)
+            bag_index = random.randint(0, len(bags_not_used) - 1)
             bag = self.get_bag(bags_not_used[bag_index])
             used = False
 
-            for label_index in range(len(bag.get_labels())):
-                if bag.get_labels()[label_index] == 1 and label_index in labels_train:
+            for label_index in range(bag.get_number_labels()):
+                if bag.get_labels()[0][label_index] == 1 and label_index in labels_train:
                     used = True
-                    del labels_train[label_index]
+                    labels_train.remove(label_index)
             if used:
-                del bags_not_used[bag_index]
-
+                dataset_train.add_bag(bag)
+                bags_not_used.pop(bag_index)
 
+        while dataset_train.get_number_bags() < number_bags_train:
+            bag_index = random.randint(0, len(bags_not_used) - 1)
+            bag = self.get_bag(bags_not_used[bag_index])
+            dataset_train.add_bag(bag)
+            bags_not_used.pop(bag_index)
 
+        while bags_not_used:
+            bag_index = random.randint(0, len(bags_not_used) - 1)
+            bag = self.get_bag(bags_not_used[bag_index])
+            dataset_test.add_bag(bag)
+            bags_not_used.pop(bag_index)
 
+        if dataset_test.get_number_bags() == 0:
+            raise Exception("Dataset is too small to split")
 
+        return dataset_train, dataset_test
 
-    # TODO: Ver si separar esto
     def cardinality(self):
         """
         Computes the Cardinality as the average number of labels per pattern.
 
         Returns
         ----------
         cardinality : float
```

### Comparing `mimllearning-0.3.9/src/miml/datasets/miml_birds.arff` & `mimllearning-0.4.0/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/datasets/miml_birds.csv` & `mimllearning-0.4.0/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.4.0/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.4.0/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/report/report.py` & `mimllearning-0.4.0/src/miml/report/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     all_metrics.append(metric + "-" + label)
 
         if metrics is None:
             metrics = all_metrics
         else:
             for metric in metrics:
                 if metric not in all_metrics:
-                    raise Exception("Metric ", metric, "is not valid\n", "Metrics availables: ", all_metrics)
+                    raise Exception("Metric ", metric, "is not valid\n", "Metrics available: ", all_metrics)
         self.header = header
         self.metrics_name = metrics
         self.per_label = per_label
         self.metrics_value = dict()
 
     def calculate_metrics(self):
         self.metrics_value["precision-score-macro"] = precision_score(self.y_true, self.y_pred, average="macro",
@@ -72,23 +72,23 @@
         self.metrics_value["jaccard-score-macro"] = jaccard_score(self.y_true, self.y_pred, average="macro",
                                                                   zero_division=0)
         self.metrics_value["jaccard-score-micro"] = jaccard_score(self.y_true, self.y_pred, average="micro",
                                                                   zero_division=0)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             # When log_loss called raise this warning, it is not true for multilabel classification
-            # UserWarning: The y_pred values do not sum to one. Starting from 1.5 thiswill result in an error.
+            # UserWarning: The y_pred values do not sum to one. Starting from 1.5 this will result in an error.
             self.metrics_value["log-loss"] = log_loss(self.y_true, self.probs)
 
         if self.per_label:
             precision_score_per_label = list(precision_score(self.y_true, self.y_pred, average=None, zero_division=0))
             recall_score_per_label = list(recall_score(self.y_true, self.y_pred, average=None, zero_division=0))
             f1_score_per_label = list(f1_score(self.y_true, self.y_pred, average=None, zero_division=0))
             fbeta_score_per_label = list(fbeta_score(self.y_true, self.y_pred, beta=0.5, average=None, zero_division=0))
-            # roc_auc_score_per_label = list(roc_auc_score(self.y_true, self.probs, average="None"))
+            # roc_auc_score_per_label = list(roc_auc_score(self.y_true, self.probs, average=None))
             jaccard_score_per_label = list(jaccard_score(self.y_true, self.y_pred, average=None, zero_division=0))
             for i, label in enumerate(self.dataset.get_labels_name()):
                 self.metrics_value["precision-score-" + label] = precision_score_per_label[i]
                 self.metrics_value["recall-score-" + label] = recall_score_per_label[i]
                 self.metrics_value["f1-score-" + label] = f1_score_per_label[i]
                 self.metrics_value["fbeta-score-" + label] = fbeta_score_per_label[i]
                 # self.metrics_value["roc-auc-score-"+label] = roc_auc_score_per_label[i]
```

### Comparing `mimllearning-0.3.9/src/miml/test/data_test.py` & `mimllearning-0.4.0/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.4.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,56 +2,53 @@
 from copy import deepcopy
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class BinaryRelevanceTransformation:
     """
-    Class that performs a binary relevance transformation to convert a MIMLDataset class to numpy ndarrays.
+    Class that performs a binary relevance transformation to convert a MIMLDataset class to numpy ndarray.
     """
 
     def __init__(self):
         self.dataset = None
 
     def transform_dataset(self, dataset: MIMLDataset) -> list:
         """
-        Transform the dataset to multiinstance datasets dividing the original dataset into n datasets with a single
+        Transform the dataset to multi-instance datasets dividing the original dataset into n datasets with a single
         label, where n is the number of labels.
 
         Returns
         -------
 
         datasets: list
             Multi instance datasets
 
         """
-        self.dataset = dataset
+        self.dataset = deepcopy(dataset)
         datasets = []
         for i in range(self.dataset.get_number_labels()):
             dataset = deepcopy(self.dataset)
             count = 0
             for j in range(self.dataset.get_number_labels()):
                 if i != j:
                     dataset.delete_attribute(self.dataset.get_number_features()-count+j)
-                    labels_name = dataset.get_labels_name()
-                    labels_name.pop(j-count)
-                    dataset.set_labels_name(labels_name)
                     count += 1
             datasets.append(dataset)
 
         return datasets
 
     def transform_bag(self, bag: Bag) -> list:
         """
         Transform miml bag to multi instance bags
 
         Parameters
         ----------
         bag :
-            Bag to be transformed to multiinstance bag
+            Bag to be transformed to multi-instance bag
 
         Returns
         -------
         bags : list[Bag]
             List of n_labels transformed bags
 
         """
@@ -61,15 +58,16 @@
 
         bags = []
         for i in range(bag.get_number_labels()):
             transformed_bag = deepcopy(bag)
             count = 0
             for j in range(bag.get_number_labels()):
                 if i != j:
-                    transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features() - count + j, axis=1)
+                    transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features() - count + j,
+                                                     axis=1)
                     labels_name = transformed_bag.dataset.get_labels_name()
                     labels_name.pop(j - count)
                     transformed_bag.dataset.set_labels_name(labels_name)
                     count += 1
             bags.append(transformed_bag)
 
         return bags
```

### Comparing `mimllearning-0.3.9/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.4.0/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...data import Instance
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class ArithmeticTransformation(MIMLtoMLTransformation):
     """
-    Class that performs an arithmetic transformation to convert a MIMLDataset class to numpy ndarrays.
+    Class that performs an arithmetic transformation to convert a MIMLDataset class to numpy ndarray.
     """
 
     def __init__(self):
         super().__init__()
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
@@ -58,14 +58,16 @@
         features = bag.get_features()
         labels = bag.get_labels()[0]
         features = np.mean(features, axis=0)
 
         transformed_bag = Bag(bag.key)
         transformed_bag.add_instance(Instance(list(np.hstack((features, labels)))))
 
+        # Create dataset with attribute data modified of original dataset of the bag in case we need to use get_features
+        # like in predict_bag
         dataset = MIMLDataset()
         dataset.set_name(bag.dataset.get_name())
         dataset.set_features_name(bag.dataset.get_features_name())
         dataset.set_labels_name(bag.dataset.get_labels_name())
         dataset.add_bag(transformed_bag)
 
         return transformed_bag
```

### Comparing `mimllearning-0.3.9/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.4.0/src/miml/transformation/mimlTOml/geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...data import Instance
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class GeometricTransformation(MIMLtoMLTransformation):
     """
-    Class that performs a geometric transformation to convert a MIMLDataset class to numpy ndarrays.
+    Class that performs a geometric transformation to convert a MIMLDataset class to numpy ndarray.
     """
 
     def __init__(self):
         super().__init__()
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
```

### Comparing `mimllearning-0.3.9/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.4.0/src/miml/transformation/mimlTOml/minmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...data import Instance
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class MinMaxTransformation(MIMLtoMLTransformation):
     """
-    Class that performs a minmax transformation to convert a MIMLDataset class to numpy ndarrays.
+    Class that performs a minmax transformation to convert a MIMLDataset class to numpy ndarray.
     """
 
     def __init__(self):
         super().__init__()
 
     def transform_dataset(self, dataset: MIMLDataset):
         """
```

### Comparing `mimllearning-0.3.9/src/miml/tutorial/demo.ipynb` & `mimllearning-0.4.0/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/tutorial/miml_data.ipynb` & `mimllearning-0.4.0/src/miml/tutorial/miml_data.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.4.0/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.4.0/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/README.md` & `mimllearning-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.9/pyproject.toml` & `mimllearning-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.3.9"
+version = "0.4.0"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.3.9/PKG-INFO` & `mimllearning-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.3.9
+Version: 0.4.0
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

