# Comparing `tmp/sunpy-5.1.1.tar.gz` & `tmp/sunpy-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-5.1.1.tar", last modified: Sat Jan 13 03:20:02 2024, max compression
+gzip compressed data, was "sunpy-5.1.2.tar", last modified: Thu Apr  4 15:06:42 2024, max compression
```

## Comparing `sunpy-5.1.1.tar` & `sunpy-5.1.2.tar`

### file list

```diff
@@ -1,847 +1,848 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:02.027493 sunpy-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)   256289 2024-01-13 03:19:44.000000 sunpy-5.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-13 03:19:44.000000 sunpy-5.1.1/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-13 03:19:44.000000 sunpy-5.1.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-13 03:19:44.000000 sunpy-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-01-13 03:20:02.027493 sunpy-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-01-13 03:19:44.000000 sunpy-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.875493 sunpy-5.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.875493 sunpy-5.1.1/docs/dev_guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.879493 sunpy-5.1.1/docs/dev_guide/contents/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/backports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/ci_jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/code_standards.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/conda_for_dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/example_gallery.rst
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/funding.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.879493 sunpy-5.1.1/docs/dev_guide/contents/images/
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/images/actions_check_pr.png
--rw-r--r--   0 runner    (1001) docker     (127)    88979 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/images/actions_summary_check.png
--rw-r--r--   0 runner    (1001) docker     (127)    27285 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/images/checks.png
--rw-r--r--   0 runner    (1001) docker     (127)    59267 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/images/checks_pr.png
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/logger.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/maintainer_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/newcomers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/pr_checklist.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/pr_review_procedure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/public_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/remote_data_manager.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/contents/units_quantities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/dev_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.879493 sunpy-5.1.1/docs/how_to/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/coord_components.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/create_a_map.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/create_coords.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/create_custom_map.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/create_custom_timeseries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/parse_time.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/remote_data_manager.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/search_multiple_wavelengths.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/search_vso.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/how_to/transform_coords.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.883493 sunpy-5.1.1/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.883493 sunpy-5.1.1/docs/reference/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/coordinates/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/customization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/database.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/io.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/map.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/net.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/physics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/ssw.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/stability.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/sun.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/sunpy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/sunpy_stability.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/time.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/timeseries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/reference/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.883493 sunpy-5.1.1/docs/topic_guide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.887493 sunpy-5.1.1/docs/topic_guide/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/carrington.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/rotatedsunframe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/rsun.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/velocities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/coordinates/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/custom_map_rotate.rst
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/extending_fido.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/helioviewer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/history_comments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/logger.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/new_map_class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/rsun.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/topic_guide/timeseries_metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.887493 sunpy-5.1.1/docs/tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.887493 sunpy-5.1.1/docs/tutorial/acquiring_data/
--rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/acquiring_data/hek.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/acquiring_data/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    37544 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/acquiring_data/jsoc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/maps.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/time.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/timeseries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/tutorial/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.891493 sunpy-5.1.1/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/0.8.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/0.9.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19714 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)    82435 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/1.1-wispr.png
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/5.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-13 03:19:44.000000 sunpy-5.1.1/docs/whatsnew/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.891493 sunpy-5.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.891493 sunpy-5.1.1/examples/acquiring_data/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/downloading_cutouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/fido_metadata_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/querying_and_loading_SHARP_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/querying_the_GOES_event_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/acquiring_data/search_cdaweb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.891493 sunpy-5.1.1/examples/computer_vision_techniques/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/computer_vision_techniques/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/computer_vision_techniques/finding_masking_bright_pixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/computer_vision_techniques/loop_edge_enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/computer_vision_techniques/mask_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/computer_vision_techniques/off_limb_enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.891493 sunpy-5.1.1/examples/differential_rotation/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/differential_rotation/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/differential_rotation/comparing_rotation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/differential_rotation/differentially_rotated_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/differential_rotation/differentially_rotated_gridlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/differential_rotation/reprojected_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.895493 sunpy-5.1.1/examples/map/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/brightness_pixel_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/compare_rotation_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/composite_map_AIA_HMI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/difference_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/hmi_contours_wcsaxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/image_bright_regions_gallery_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/lasco_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_contouring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_data_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_from_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_metadata_modification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_resampling_and_superpixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/map_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/masking_hmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/plot_frameless_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map/submaps_and_cropping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.899493 sunpy-5.1.1/examples/map_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/autoalign_aia_hmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/projection_custom_origin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/reprojection_aia_euvi_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/reprojection_align_aia_hmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/reprojection_carrington.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/reprojection_different_observers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/reprojection_spherical_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/map_transformations/upside_down_hmi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.903493 sunpy-5.1.1/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/AIA_HMI_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/aia_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/arrayanimatorwcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/fading_between_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/finding_local_peaks_in_solar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/finegrained_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/great_arc_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/grid_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/hmi_synoptic_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/lasco_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/lat_lon_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/limb_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/lineAnimator_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/magnetogram_active_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/map_editcolormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/masked_composite_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/mplcairo_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/overplot_hek_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/plot_equator_prime_meridian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/plot_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/plot_rotated_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/plotting_blank_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/quadrangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/simple_differential_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/solar_cycle_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/sunpy_matplotlib_colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/three_map_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/wcsaxes_map_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/wcsaxes_plotting_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/plotting/xy_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.903493 sunpy-5.1.1/examples/saving_and_loading_data/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/saving_and_loading_data/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/saving_and_loading_data/coordinates_in_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/saving_and_loading_data/genericmap_in_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/saving_and_loading_data/genericmap_in_fits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.903493 sunpy-5.1.1/examples/showcase/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/showcase/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/showcase/eclipse_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/showcase/hmi_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/showcase/stereoscopic_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/showcase/where_is_stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.903493 sunpy-5.1.1/examples/time_series/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/goes_hek_m25.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/goes_xrs_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/goes_xrs_nrt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/power_spectra_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/timeseries_convolution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/timeseries_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/timeseries_peak_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/time_series/timeseriesmetadata_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.907493 sunpy-5.1.1/examples/units_and_coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/AIA_limb_STEREO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/AltAz_Coordinate_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/ParkerSolarProbe_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/STEREO_SECCHI_starfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/getting_lasco_observer_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/getting_observer_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/map_slit_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/north_offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/planet_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/radec_to_hpc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/spice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-01-13 03:19:44.000000 sunpy-5.1.1/examples/units_and_coordinates/venus_transit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.907493 sunpy-5.1.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-13 03:19:44.000000 sunpy-5.1.1/licenses/ASTROPY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-01-13 03:19:44.000000 sunpy-5.1.1/licenses/GLUE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-13 03:19:44.000000 sunpy-5.1.1/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-13 03:19:44.000000 sunpy-5.1.1/licenses/SCIKIT-LEARN.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-13 03:19:44.000000 sunpy-5.1.1/licenses/TOWNCRIER.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-13 03:19:44.000000 sunpy-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-01-13 03:20:02.027493 sunpy-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 03:19:44.000000 sunpy-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.907493 sunpy-5.1.1/sunpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.911493 sunpy-5.1.1/sunpy/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55531 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.911493 sunpy-5.1.1/sunpy/coordinates/data/
--rw-r--r--   0 runner    (1001) docker     (127)    40639 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/data/igrf13coeffs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/frameattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    46079 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/metaframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    20161 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/spice.py
--rw-r--r--   0 runner    (1001) docker     (127)    32023 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/sun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.915493 sunpy-5.1.1/sunpy/coordinates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_ephemeris.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_frameattributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19175 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_metaframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_offset_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_spice.py
--rw-r--r--   0 runner    (1001) docker     (127)    25804 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_sun.py
--rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/coordinates/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.915493 sunpy-5.1.1/sunpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.915493 sunpy-5.1.1/sunpy/data/data_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.915493 sunpy-5.1.1/sunpy/data/data_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/db_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/data_manager/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/sunpyrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.931493 sunpy-5.1.1/sunpy/data/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2
--rw-r--r--   0 runner    (1001) docker     (127)    80880 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/20181209_180305_kcor_l2.header
--rw-r--r--   0 runner    (1001) docker     (127)    59987 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.931493 sunpy-5.1.1/sunpy/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT/efz20040301.010016_s.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.935493 sunpy-5.1.1/sunpy/data/test/EIT_header/
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.000010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.010016_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.020010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.030011_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.040010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.050010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.060010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.070014_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.080010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.090010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.100010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.110010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.120010_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/FGMG4_20110214_030443.7.header
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/HinodeSOT.header
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/HinodeXRT.header
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.935493 sunpy-5.1.1/sunpy/data/test/SRS/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/19960106SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/19960430SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/19960513SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20000922SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20000927SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20001001SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20020624SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20020628SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20100621SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20150101SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20150306SRS.txt
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SRS/20150906SRS.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.935493 sunpy-5.1.1/sunpy/data/test/SWAP/
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SWAP/resampled0_swap.header
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SWAP/resampled1_swap.header
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SWAP/resampled2_swap.header
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/SWAP/resampled3_swap.header
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/YohkohSXT.header
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/_generate_asdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   149760 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/aia_171_level1.fits
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/aiamap_genericmap_1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/annotation_ppt.db
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/cor1_20090615_000500_s4c1A.header
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header
--rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/euvi_20090615_000900_n4euA_s.header
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.935493 sunpy-5.1.1/sunpy/data/test/eve/
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve/eve_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve/eve_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve/eve_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve/eve_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve/eve_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89280 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits
--rw-r--r--   0 runner    (1001) docker     (127)    31680 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gbm.fits
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/generated_sample.genx
--rw-r--r--   0 runner    (1001) docker     (127)   694080 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/go1520110607.fits
--rw-r--r--   0 runner    (1001) docker     (127)   219720 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/go1520120601.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    37737 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/goes_13_leap_second.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gong_synoptic.header
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gzip_fits_test.file
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gzip_test.fit.gz
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gzip_test.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/gzip_test.fts.gz
--rw-r--r--   0 runner    (1001) docker     (127)   117097 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/heliographic_phase_map.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/hi_20110910_114721_s7h2A.header
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/hmi_synoptic.header
--rw-r--r--   0 runner    (1001) docker     (127)    95040 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/hsi_image_20101016_191218.fits
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/lasco_c2_25299383_s.header
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/lasco_c3.header
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/mdi_synoptic.header
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/not_actually_fits.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/observed-solar-cycle-indices-truncated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/predicted-solar-cycle-truncated.json
--rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    89280 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/resampled_hmi.fits
--rw-r--r--   0 runner    (1001) docker     (127)    57333 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (127)    59635 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (127)    75990 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (127)    89560 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (127)   101102 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/seit_00171_fd_19961211_1900.header
--rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header
--rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf
--rw-r--r--   0 runner    (1001) docker     (127)   369276 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/swap_lv1_20140606_000113.header
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/tca110810_truncated
--rw-r--r--   0 runner    (1001) docker     (127)   866179 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/test_ana.fz
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/tsi20010130_025823_a2.header
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.939493 sunpy-5.1.1/sunpy/data/test/waveunit/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/waveunit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/waveunit/mq130812.084253.header
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/waveunit/na120701.091058.header
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.939493 sunpy-5.1.1/sunpy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/data/tests/test_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.939493 sunpy-5.1.1/sunpy/database/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    32359 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.939493 sunpy-5.1.1/sunpy/database/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19490 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    35261 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24194 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/database/tests/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.943493 sunpy-5.1.1/sunpy/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/appdirs_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    49330 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/distro.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/distro_license.rst
--rw-r--r--   0 runner    (1001) docker     (127)   102537 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/inflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/inflect_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    52276 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/extern/parse_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.943493 sunpy-5.1.1/sunpy/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.943493 sunpy-5.1.1/sunpy/image/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    19013 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/image/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.943493 sunpy-5.1.1/sunpy/io/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/_cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/_jp2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/ana.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/header.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.943493 sunpy-5.1.1/sunpy/io/special/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.947493 sunpy-5.1.1/sunpy/io/special/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.947493 sunpy-5.1.1/sunpy/io/special/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/converters/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/converters/generic_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.947493 sunpy-5.1.1/sunpy/io/special/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.947493 sunpy-5.1.1/sunpy/io/special/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/manifests/sunpy-1.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.947493 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricsolarmagnetospheric-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geomagnetic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/solarmagnetic-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.951493 sunpy-5.1.1/sunpy/io/special/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/tests/hgc_100.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/tests/test_coordinate_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/asdf/tests/test_genericmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/genx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/special/srs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.867493 sunpy-5.1.1/sunpy/io/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.951493 sunpy-5.1.1/sunpy/io/src/ana/
--rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/_pyana.c
--rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anacompress.c
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anacompress.h
--rw-r--r--   0 runner    (1001) docker     (127)    23203 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anadecompress.c
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anadecompress.h
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anarw.c
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/anarw.h
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/src/ana/types.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.951493 sunpy-5.1.1/sunpy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/generate_genx.pro
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_ana.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_filetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_genx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_jp2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/io/tests/test_srs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.955493 sunpy-5.1.1/sunpy/map/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/compositemap.py
--rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/header_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/map_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)   113824 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/mapbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/mapsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/maputils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.955493 sunpy-5.1.1/sunpy/map/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/gong.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/hinode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/mlso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/proba2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/psp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/rhessi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/sdo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/soho.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/solo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/stereo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/suvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.959493 sunpy-5.1.1/sunpy/map/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_aia_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_cor_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_eit_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_eui_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_euvi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_gong_synoptic_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_hi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_hmi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_hmi_synoptic_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_iris_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_kcor_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_lasco_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_mdi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_rhessi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_sot_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_suvi_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_swap_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_sxt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_trace_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_wispr_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/tests/test_xrt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/sources/yohkoh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.963493 sunpy-5.1.1/sunpy/map/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_compositemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_header_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_map_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    66916 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_mapbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_mapbase_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_mapsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14363 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_maputils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/map/tests/test_reproject_to.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.963493 sunpy-5.1.1/sunpy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24205 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/cdaweb/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/cdaweb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/cdaweb/data/
--rw-r--r--   0 runner    (1001) docker     (127)   378652 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/cdaweb/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/test/test_cdaweb.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/cdaweb/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/dataretriever/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/dataretriever/attrs/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/attrs/goes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.967493 sunpy-5.1.1/sunpy/net/dataretriever/sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/eve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/goes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/gong.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/lyra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/norh.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_eve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_goes_ud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_norh.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/dataretriever/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/dataretriever/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/fido_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/hek/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek/hek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/hek/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek/tests/test_hek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/hek2vso/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek2vso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek2vso/hek2vso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/hek2vso/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek2vso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/hek2vso/tests/test_hek2vso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.971493 sunpy-5.1.1/sunpy/net/helio/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/chaincode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/hec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.975493 sunpy-5.1.1/sunpy/net/helio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/tests/test_chaincode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10543 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helio/tests/test_helio.py
--rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/helioviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.975493 sunpy-5.1.1/sunpy/net/jsoc/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.975493 sunpy-5.1.1/sunpy/net/jsoc/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44219 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (127)    38329 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/jsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.975493 sunpy-5.1.1/sunpy/net/jsoc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/jsoc/tests/test_jsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19514 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.975493 sunpy-5.1.1/sunpy/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_baseclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_fido.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_helioviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/tests/test_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/net/vso/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/net/vso/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/data/attrs.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/legacy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/table_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/net/vso/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/tests/test_vso.py
--rw-r--r--   0 runner    (1001) docker     (127)    27677 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/vso.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/net/vso/zeep_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/physics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/physics/differential_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/physics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/physics/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/physics/tests/reference/
--rw-r--r--   0 runner    (1001) docker     (127)    95355 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/physics/tests/reference/test_differential_rotation.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/physics/tests/test_differential_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/sun/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.979493 sunpy-5.1.1/sunpy/sun/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/sun/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.983493 sunpy-5.1.1/sunpy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/figure_hashes_mpl_353_ft_261_astropy_511_animators_100.json
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/self_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.983493 sunpy-5.1.1/sunpy/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/tests/test_mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/tests/test_self_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/tests/tests/test_sunpy_data_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.983493 sunpy-5.1.1/sunpy/time/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.983493 sunpy-5.1.1/sunpy/time/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/tests/test_taiseconds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/tests/test_timerange.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/tests/test_utime.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/timeformats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/time/timerange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.983493 sunpy-5.1.1/sunpy/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    28718 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.987493 sunpy-5.1.1/sunpy/timeseries/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/eve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/goes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/lyra.py
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/norh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.987493 sunpy-5.1.1/sunpy/timeseries/sources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_eve.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_fermi_gbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_goes.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_lyra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_norh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/sources/tests/test_rhessi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.987493 sunpy-5.1.1/sunpy/timeseries/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/tests/test_timeseries_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    23237 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/tests/test_timeseriesbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    21538 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/tests/test_timeseriesmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/timeseries_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    32814 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/timeseries/timeseriesbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.991493 sunpy-5.1.1/sunpy/util/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/datatype_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/net.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/parfive_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.991493 sunpy-5.1.1/sunpy/util/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/sphinx/doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/sphinx/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.995493 sunpy-5.1.1/sunpy/util/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_datatype_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/tests/test_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/util/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.995493 sunpy-5.1.1/sunpy/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.995493 sunpy-5.1.1/sunpy/visualization/animator/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/animator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/animator/mapsequenceanimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.995493 sunpy-5.1.1/sunpy/visualization/animator/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/animator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/animator/tests/test_mapsequenceanimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.995493 sunpy-5.1.1/sunpy/visualization/colormaps/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/cm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/color_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.999493 sunpy-5.1.1/sunpy/visualization/colormaps/data/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_blue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_green.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_red.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_yellow.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_171.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_195.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_284.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_304.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/grayscale.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/hi1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/hi2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/hmi_mag.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/idl_3.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/lasco_c2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/lasco_c3.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/rhessi.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/std_gamma_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/stereo_cor1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/stereo_cor2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1216.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1550.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1600.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1700.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_171.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_195.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_284.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.999493 sunpy-5.1.1/sunpy/visualization/colormaps/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/colormaps/tests/test_cm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.999493 sunpy-5.1.1/sunpy/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/tests/test_drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-01-13 03:19:44.000000 sunpy-5.1.1/sunpy/visualization/wcsaxes_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:20:01.999493 sunpy-5.1.1/sunpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27891 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-13 03:20:01.000000 sunpy-5.1.1/sunpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.112460 sunpy-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)   258600 2024-04-04 15:06:28.000000 sunpy-5.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-04 15:06:28.000000 sunpy-5.1.2/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-04 15:06:28.000000 sunpy-5.1.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 15:06:28.000000 sunpy-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19653 2024-04-04 15:06:42.112460 sunpy-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-04 15:06:28.000000 sunpy-5.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.940461 sunpy-5.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.944461 sunpy-5.1.2/docs/dev_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.944461 sunpy-5.1.2/docs/dev_guide/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/backports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/ci_jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/code_standards.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/conda_for_dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/example_gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/funding.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.948461 sunpy-5.1.2/docs/dev_guide/contents/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/images/actions_check_pr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88979 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/images/actions_summary_check.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27285 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/images/checks.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59267 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/images/checks_pr.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/logger.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/maintainer_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/newcomers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/pr_checklist.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/pr_review_procedure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/public_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/remote_data_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/contents/units_quantities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/dev_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.948461 sunpy-5.1.2/docs/how_to/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/coord_components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/create_a_map.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/create_coords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/create_custom_map.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/create_custom_timeseries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/fix_map_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/parse_time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/remote_data_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/search_multiple_wavelengths.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/search_vso.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/how_to/transform_coords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.952461 sunpy-5.1.2/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.952461 sunpy-5.1.2/docs/reference/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/coordinates/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/customization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/map.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/net.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/physics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/ssw.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/stability.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/sun.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/sunpy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/sunpy_stability.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/timeseries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/reference/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.952461 sunpy-5.1.2/docs/topic_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.956461 sunpy-5.1.2/docs/topic_guide/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/carrington.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/rotatedsunframe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/rsun.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/velocities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/coordinates/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/custom_map_rotate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/extending_fido.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/helioviewer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/history_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/logger.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/new_map_class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/rsun.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/topic_guide/timeseries_metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.956461 sunpy-5.1.2/docs/tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.956461 sunpy-5.1.2/docs/tutorial/acquiring_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/acquiring_data/hek.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30611 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/acquiring_data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    37544 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/acquiring_data/jsoc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/maps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/timeseries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/tutorial/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.960461 sunpy-5.1.2/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/0.8.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/0.9.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19714 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    82435 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/1.1-wispr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 15:06:28.000000 sunpy-5.1.2/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.960461 sunpy-5.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.960461 sunpy-5.1.2/examples/acquiring_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/downloading_cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/fido_metadata_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/querying_and_loading_SHARP_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/querying_the_GOES_event_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/acquiring_data/search_cdaweb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.960461 sunpy-5.1.2/examples/computer_vision_techniques/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/computer_vision_techniques/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/computer_vision_techniques/finding_masking_bright_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/computer_vision_techniques/loop_edge_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/computer_vision_techniques/mask_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/computer_vision_techniques/off_limb_enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.964461 sunpy-5.1.2/examples/differential_rotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/differential_rotation/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/differential_rotation/comparing_rotation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/differential_rotation/differentially_rotated_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/differential_rotation/differentially_rotated_gridlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/differential_rotation/reprojected_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.964461 sunpy-5.1.2/examples/map/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/brightness_pixel_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/compare_rotation_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/composite_map_AIA_HMI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/difference_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/hmi_contours_wcsaxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/image_bright_regions_gallery_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/lasco_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_contouring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_data_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_from_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_metadata_modification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_resampling_and_superpixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/map_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/masking_hmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/plot_frameless_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map/submaps_and_cropping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.968461 sunpy-5.1.2/examples/map_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/autoalign_aia_hmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/projection_custom_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/reprojection_aia_euvi_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/reprojection_align_aia_hmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/reprojection_carrington.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/reprojection_different_observers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/reprojection_spherical_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/map_transformations/upside_down_hmi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.972461 sunpy-5.1.2/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/AIA_HMI_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/aia_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/arrayanimatorwcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/fading_between_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/finding_local_peaks_in_solar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/finegrained_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/great_arc_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/grid_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/hmi_synoptic_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/lasco_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/lat_lon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/limb_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/lineAnimator_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/magnetogram_active_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/map_editcolormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/masked_composite_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/mplcairo_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/overplot_hek_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/plot_equator_prime_meridian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/plot_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/plot_rotated_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/plotting_blank_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/quadrangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/simple_differential_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/solar_cycle_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/sunpy_matplotlib_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/three_map_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/wcsaxes_map_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/wcsaxes_plotting_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/plotting/xy_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.976461 sunpy-5.1.2/examples/saving_and_loading_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/saving_and_loading_data/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/saving_and_loading_data/coordinates_in_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/saving_and_loading_data/genericmap_in_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/saving_and_loading_data/genericmap_in_fits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.976461 sunpy-5.1.2/examples/showcase/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/showcase/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/showcase/eclipse_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/showcase/hmi_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/showcase/stereoscopic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/showcase/where_is_stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.976461 sunpy-5.1.2/examples/time_series/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/goes_hek_m25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/goes_xrs_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/goes_xrs_nrt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/power_spectra_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/timeseries_convolution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/timeseries_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/timeseries_peak_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/time_series/timeseriesmetadata_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.980461 sunpy-5.1.2/examples/units_and_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/AIA_limb_STEREO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/AltAz_Coordinate_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/ParkerSolarProbe_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/STEREO_SECCHI_starfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/getting_lasco_observer_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/getting_observer_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/map_slit_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/north_offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/planet_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/radec_to_hpc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/spice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-04 15:06:28.000000 sunpy-5.1.2/examples/units_and_coordinates/venus_transit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.980461 sunpy-5.1.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-04 15:06:28.000000 sunpy-5.1.2/licenses/ASTROPY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-04 15:06:28.000000 sunpy-5.1.2/licenses/GLUE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 15:06:28.000000 sunpy-5.1.2/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-04 15:06:28.000000 sunpy-5.1.2/licenses/SCIKIT-LEARN.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 15:06:28.000000 sunpy-5.1.2/licenses/TOWNCRIER.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-04 15:06:28.000000 sunpy-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-04 15:06:42.116460 sunpy-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:06:28.000000 sunpy-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.980461 sunpy-5.1.2/sunpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.984461 sunpy-5.1.2/sunpy/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55681 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.984461 sunpy-5.1.2/sunpy/coordinates/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    40639 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/data/igrf13coeffs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/frameattributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46079 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/metaframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20161 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/spice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31898 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.988461 sunpy-5.1.2/sunpy/coordinates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_ephemeris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_frameattributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19175 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_metaframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_offset_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_spice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25784 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50135 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/coordinates/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.988461 sunpy-5.1.2/sunpy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.992461 sunpy-5.1.2/sunpy/data/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.992461 sunpy-5.1.2/sunpy/data/data_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/db_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/data_manager/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/sunpyrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.008461 sunpy-5.1.2/sunpy/data/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2
+-rw-r--r--   0 runner    (1001) docker     (127)    80880 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/20181209_180305_kcor_l2.header
+-rw-r--r--   0 runner    (1001) docker     (127)    59987 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.008461 sunpy-5.1.2/sunpy/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT/efz20040301.010016_s.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.012461 sunpy-5.1.2/sunpy/data/test/EIT_header/
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.000010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.010016_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.020010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.030011_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.040010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.050010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.060010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.070014_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.080010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.090010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.100010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.110010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.120010_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/FGMG4_20110214_030443.7.header
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/HinodeSOT.header
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/HinodeXRT.header
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.012461 sunpy-5.1.2/sunpy/data/test/SRS/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/19960106SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/19960430SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/19960513SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20000922SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20000927SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20001001SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20020624SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20020628SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20100621SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20150101SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20150306SRS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SRS/20150906SRS.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.012461 sunpy-5.1.2/sunpy/data/test/SWAP/
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SWAP/resampled0_swap.header
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SWAP/resampled1_swap.header
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SWAP/resampled2_swap.header
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/SWAP/resampled3_swap.header
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/YohkohSXT.header
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/_generate_asdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149760 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/aia_171_level1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/aiamap_genericmap_1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/annotation_ppt.db
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/cor1_20090615_000500_s4c1A.header
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/euvi_20090615_000900_n4euA_s.header
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.016461 sunpy-5.1.2/sunpy/data/test/eve/
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve/eve_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve/eve_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve/eve_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve/eve_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve/eve_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89280 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    31680 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gbm.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/generated_sample.genx
+-rw-r--r--   0 runner    (1001) docker     (127)   694080 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/go1520110607.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   219720 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/go1520120601.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    37737 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/goes_13_leap_second.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gong_synoptic.header
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gzip_fits_test.file
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gzip_test.fit.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gzip_test.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/gzip_test.fts.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   117097 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/heliographic_phase_map.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/hi_20110910_114721_s7h2A.header
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/hmi_synoptic.header
+-rw-r--r--   0 runner    (1001) docker     (127)    95040 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/hsi_image_20101016_191218.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/lasco_c2_25299383_s.header
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/lasco_c3.header
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/mdi_synoptic.header
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/not_actually_fits.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/observed-solar-cycle-indices-truncated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/predicted-solar-cycle-truncated.json
+-rw-r--r--   0 runner    (1001) docker     (127)    70003 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    89280 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/resampled_hmi.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    57333 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    59635 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    75990 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (127)    89560 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   101102 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/seit_00171_fd_19961211_1900.header
+-rw-r--r--   0 runner    (1001) docker     (127)    17819 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)   369276 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/swap_lv1_20140606_000113.header
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/tca110810_truncated
+-rw-r--r--   0 runner    (1001) docker     (127)   866179 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/test_ana.fz
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/tsi20010130_025823_a2.header
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.016461 sunpy-5.1.2/sunpy/data/test/waveunit/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/waveunit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/waveunit/mq130812.084253.header
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/waveunit/na120701.091058.header
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.016461 sunpy-5.1.2/sunpy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/data/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.016461 sunpy-5.1.2/sunpy/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32359 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.020461 sunpy-5.1.2/sunpy/database/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19490 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35133 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24194 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/database/tests/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.020461 sunpy-5.1.2/sunpy/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24738 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/appdirs_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    49330 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/distro_license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   102537 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/inflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/inflect_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    52276 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/extern/parse_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.020461 sunpy-5.1.2/sunpy/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.020461 sunpy-5.1.2/sunpy/image/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19013 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/image/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/_jp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/ana.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/special/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/special/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/special/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/converters/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/converters/generic_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/special/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.024461 sunpy-5.1.2/sunpy/io/special/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/manifests/sunpy-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.028461 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricsolarmagnetospheric-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geomagnetic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/solarmagnetic-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.028461 sunpy-5.1.2/sunpy/io/special/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/tests/hgc_100.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/tests/test_coordinate_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/asdf/tests/test_genericmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/genx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/special/srs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:41.932461 sunpy-5.1.2/sunpy/io/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.032461 sunpy-5.1.2/sunpy/io/src/ana/
+-rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/_pyana.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anacompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anacompress.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23203 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anadecompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anadecompress.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anarw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/anarw.h
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/src/ana/types.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.032461 sunpy-5.1.2/sunpy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/generate_genx.pro
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_ana.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_filetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_genx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_jp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/io/tests/test_srs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.032461 sunpy-5.1.2/sunpy/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/compositemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18781 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/header_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113938 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/mapbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/mapsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/maputils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.036460 sunpy-5.1.2/sunpy/map/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/gong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/hinode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/mlso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/proba2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/psp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/rhessi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/sdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/soho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/solo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/stereo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/suvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.040460 sunpy-5.1.2/sunpy/map/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_aia_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_cor_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_eit_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_eui_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_euvi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_gong_synoptic_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_hi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_hmi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_hmi_synoptic_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_iris_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_kcor_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_lasco_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_mdi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_rhessi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_sot_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_suvi_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_swap_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_sxt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_trace_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_wispr_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/tests/test_xrt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/sources/yohkoh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.044461 sunpy-5.1.2/sunpy/map/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_compositemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_header_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69605 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_mapbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_mapbase_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_mapsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14363 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_maputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/map/tests/test_reproject_to.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.044461 sunpy-5.1.2/sunpy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24205 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.048461 sunpy-5.1.2/sunpy/net/cdaweb/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/cdaweb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.048461 sunpy-5.1.2/sunpy/net/cdaweb/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   378652 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.048461 sunpy-5.1.2/sunpy/net/cdaweb/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/test/test_cdaweb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/cdaweb/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.048461 sunpy-5.1.2/sunpy/net/dataretriever/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.048461 sunpy-5.1.2/sunpy/net/dataretriever/attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/attrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/attrs/goes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.052461 sunpy-5.1.2/sunpy/net/dataretriever/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/eve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/goes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/gong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/lyra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/norh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.052461 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_eve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_goes_ud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_norh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.052461 sunpy-5.1.2/sunpy/net/dataretriever/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/dataretriever/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/fido_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.052461 sunpy-5.1.2/sunpy/net/hek/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek/hek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.052461 sunpy-5.1.2/sunpy/net/hek/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek/tests/test_hek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/hek2vso/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek2vso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek2vso/hek2vso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/hek2vso/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek2vso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/hek2vso/tests/test_hek2vso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/helio/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/chaincode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/hec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/helio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/tests/test_chaincode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helio/tests/test_helio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/helioviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/jsoc/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/jsoc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44219 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37655 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/jsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.056460 sunpy-5.1.2/sunpy/net/jsoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/jsoc/tests/test_jsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19514 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.060460 sunpy-5.1.2/sunpy/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_fido.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_helioviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/tests/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.060460 sunpy-5.1.2/sunpy/net/vso/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.060460 sunpy-5.1.2/sunpy/net/vso/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/data/attrs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/legacy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/table_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/net/vso/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/tests/test_vso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27677 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/vso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/net/vso/zeep_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/physics/differential_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/physics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/physics/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/physics/tests/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)    95355 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/physics/tests/reference/test_differential_rotation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/physics/tests/test_differential_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/sun/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/sun/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.064460 sunpy-5.1.2/sunpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/figure_hashes_mpl_353_ft_261_astropy_511_animators_100.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/self_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.068460 sunpy-5.1.2/sunpy/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/tests/test_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/tests/test_self_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/tests/tests/test_sunpy_data_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.068460 sunpy-5.1.2/sunpy/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.068460 sunpy-5.1.2/sunpy/time/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/tests/test_taiseconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/tests/test_timerange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/tests/test_utime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/timeformats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/time/timerange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.068460 sunpy-5.1.2/sunpy/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28718 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.072461 sunpy-5.1.2/sunpy/timeseries/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/eve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/goes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/lyra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/norh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.072461 sunpy-5.1.2/sunpy/timeseries/sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_eve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_fermi_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_goes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_lyra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_norh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/sources/tests/test_rhessi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.072461 sunpy-5.1.2/sunpy/timeseries/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/tests/test_timeseries_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23237 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/tests/test_timeseriesbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21538 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/tests/test_timeseriesmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/timeseries_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32816 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/timeseries/timeseriesbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.076460 sunpy-5.1.2/sunpy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/datatype_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/parfive_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.076460 sunpy-5.1.2/sunpy/util/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/sphinx/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/sphinx/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.076460 sunpy-5.1.2/sunpy/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_datatype_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/tests/test_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/util/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.080460 sunpy-5.1.2/sunpy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.080460 sunpy-5.1.2/sunpy/visualization/animator/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/animator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/animator/mapsequenceanimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.080460 sunpy-5.1.2/sunpy/visualization/animator/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/animator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/animator/tests/test_mapsequenceanimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.080460 sunpy-5.1.2/sunpy/visualization/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/color_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.084460 sunpy-5.1.2/sunpy/visualization/colormaps/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_blue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_green.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_red.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_yellow.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_171.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_195.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_284.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_304.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/grayscale.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/hi1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/hi2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/hmi_mag.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/idl_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/lasco_c2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/lasco_c3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/rhessi.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/std_gamma_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/stereo_cor1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/stereo_cor2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1216.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1550.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1600.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1700.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_171.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_195.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_284.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.084460 sunpy-5.1.2/sunpy/visualization/colormaps/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/colormaps/tests/test_cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.084460 sunpy-5.1.2/sunpy/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/tests/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-04 15:06:28.000000 sunpy-5.1.2/sunpy/visualization/wcsaxes_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:42.084460 sunpy-5.1.2/sunpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19653 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27924 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 15:06:41.000000 sunpy-5.1.2/sunpy.egg-info/top_level.txt
```

### Comparing `sunpy-5.1.1/CHANGELOG.rst` & `sunpy-5.1.2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+5.1.2 (2024-04-04)
+==================
+
+Bug Fixes
+---------
+
+- Fixed the appearance of a double "Notes" heading in `~sunpy.map.Map` subclasses. (`#7376 <https://github.com/sunpy/sunpy/pull/7376>`__)
+- Fix a bug which caused ``Fido.search`` to crash due to SSL certificate verification error for the `~sunpy.net.helio.HECClient` now returns no results and logs a warning in this case. (`#7446 <https://github.com/sunpy/sunpy/pull/7446>`__)
+- The creation of the series string for a JSOC query was not adding the correct escape characters for  comparison values for keywords.
+  This was causing the JSOC to error. (`#7467 <https://github.com/sunpy/sunpy/pull/7467>`__)
+- JPEG2000 files are now saved with the correct orientation. Previously they would be vertically flipped when saved. (`#7486 <https://github.com/sunpy/sunpy/pull/7486>`__)
+- Fixed a very minor inaccuracy in three `sunpy.map` utility functions (:func:`~sunpy.map.contains_full_disk`, :func:`~sunpy.map.coordinate_is_on_solar_disk`, and :func:`~sunpy.map.is_all_off_disk`) resulting from the accidental use of the small-angle approximation. (`#7512 <https://github.com/sunpy/sunpy/pull/7512>`__)
+- The :meth:`~sunpy.map.GenericMap.rotate` function now correctly updates the NAXISi. (`#7522 <https://github.com/sunpy/sunpy/pull/7522>`__)
+- Fixed an inaccuracy in the implementation of `~sunpy.coordinates.HeliocentricEarthEcliptic` and `~sunpy.coordinates.GeocentricSolarEcliptic` such that the Earth was not exactly in the XY plane, but rather had an error of up ~10 meters. (`#7530 <https://github.com/sunpy/sunpy/pull/7530>`__)
+- Fixed a bug with any coordinate transformation starting in `~sunpy.coordinates.GeocentricEarthEquatorial` (GEI) returning output with AU as the length unit, rather than preserving the length unit of the initial coordinate. (`#7545 <https://github.com/sunpy/sunpy/pull/7545>`__)
+
+
+Documentation
+-------------
+
+- Created a how to guide on fixing metadata that is either missing or incorrect before passing the header into the `~sunpy.map.Map` class. (`#7262 <https://github.com/sunpy/sunpy/pull/7262>`__)
+
+
+Internal Changes
+----------------
+
+- ``pyerfa`` is now a new direct dependency.
+  It has been an indirect dependency from sunpy 3.1, over two years ago. (`#7397 <https://github.com/sunpy/sunpy/pull/7397>`__)
+
+
 5.1.1 (2024-01-12)
 ==================
 
 New Features
 ------------
 
 - Add an example of plotting a rectangle on a map with a rotation angle relative to the axes (:ref:`sphx_glr_generated_gallery_plotting_plot_rotated_rectangle.py`). (`#7348 <https://github.com/sunpy/sunpy/pull/7348>`__)
```

### Comparing `sunpy-5.1.1/CITATION.rst` & `sunpy-5.1.2/CITATION.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/LICENSE.rst` & `sunpy-5.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/PKG-INFO` & `sunpy-5.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy
-Version: 5.1.1
+Version: 5.1.2
 Summary: SunPy core package: Python for Solar Physics
 Home-page: https://sunpy.org
 Download-URL: https://pypi.org/project/sunpy/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/sunpy/
@@ -29,14 +29,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: astropy!=5.1.0,>=5.0.6
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: packaging>=19.0
 Requires-Dist: parfive[ftp]>=2.0.0
+Requires-Dist: pyerfa
 Provides-Extra: asdf
 Requires-Dist: asdf-astropy>=0.1.1; extra == "asdf"
 Requires-Dist: asdf>=2.8.0; extra == "asdf"
 Provides-Extra: dask
 Requires-Dist: dask[array]>=2021.4.0; extra == "dask"
 Provides-Extra: database
 Requires-Dist: sqlalchemy>=1.3.4; extra == "database"
@@ -272,65 +273,62 @@
 Requires-Dist: spiceypy; extra == "dev"
 Requires-Dist: sunpy-sphinx-theme>=2.0.0rc1; extra == "dev"
 Requires-Dist: sphinx-hoverxref; extra == "dev"
 
 *********
 ``sunpy``
 *********
-
 |SunPy Logo|
 
-+----------------------+----------------------+----------------------+
-| Release              | Development          | Community            |
-+======================+======================+======================+
-| |Latest PyPi         | |Python Versions|    | |Matrix Chat Room|   |
-| Version|             |                      |                      |
-+----------------------+----------------------+----------------------+
-| |Latest Conda        | |Project Status:     | |OpenAstronomy       |
-| Version|             | Active - The project | Discourse community| |
-|                      | has reached a        |                      |
-|                      | stable, usable state |                      |
-|                      | and is being         |                      |
-|                      | actively developed.| |                      |
-+----------------------+----------------------+----------------------+
-| |Zenodo - Latest     | |Continuous          | |Google Groups       |
-| DOI|                 | Integration Status|  | Mailing List|        |
-+----------------------+----------------------+----------------------+
-| |sunpy Stable        | |CodeCov Code        | |Powered by          |
-| Documentation|       | Coverage|            | NumFOCUS|            |
-+----------------------+----------------------+----------------------+
++-----------------------------------+-----------------------------------+-----------------------------------+
+|           Release                 |           Development             |           Community               |
++===================================+===================================+===================================+
+|       |Latest PyPi Version|       |        |Python Versions|          |         |Matrix Chat Room|        |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|     |Latest Conda Version|        |     |Project Status: Active|      |     |OpenAstronomy Discourse|     |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|      |Zenodo - Latest DOI|        |  |Continuous Integration Status|  |    |Google Groups Mailing List|   |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|    |sunpy stable documentation|   |     |CodeCov Code Coverage|       |       |Powered by NumFOCUS|       |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|         |sunpy citation|          |                                   |            |pyOpenSci|            |
++-----------------------------------+-----------------------------------+-----------------------------------+
 
-.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/sunpy_logo_landscape.svg
+.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.png
    :width: 200px
 .. |Latest PyPi Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/sunpy
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Matrix Chat Room| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=matrix.org
    :target: https://app.element.io/#/room/#sunpy:openastronomy.org
 .. |Latest Conda Version| image:: https://anaconda.org/conda-forge/sunpy/badges/version.svg
    :target: https://anaconda.org/conda-forge/sunpy
-.. |Project Status: Active - The project has reached a stable, usable state and is being actively developed.| image:: https://www.repostatus.org/badges/latest/active.svg
+.. |Project Status: Active| image:: https://www.repostatus.org/badges/latest/active.svg
    :target: https://www.repostatus.org/#active
-.. |OpenAstronomy Discourse community| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
+.. |OpenAstronomy Discourse| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
    :height: 20px
    :target: https://community.openastronomy.org/
 .. |Zenodo - Latest DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |Continuous Integration Status| image:: https://github.com/sunpy/sunpy/actions/workflows/ci.yml/badge.svg?branch=main
    :target: https://github.com/sunpy/sunpy/actions/workflows/ci.yml
-.. |Google Groups Mailing List| image:: https://fonts.gstatic.com/s/i/productlogos/groups/v9/web-48dp/logo_groups_color_1x_web_48dp.png
+.. |Google Groups Mailing List| image:: https://upload.wikimedia.org/wikipedia/commons/2/27/Google_Groups_logo.gif
    :height: 20px
    :target: https://groups.google.com/g/sunpy
-.. |sunpy Stable Documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
+.. |sunpy stable documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
    :target: https://docs.sunpy.org/
 .. |CodeCov Code Coverage| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
+.. |sunpy citation| image:: https://img.shields.io/badge/cite-sunpy-orange
+   :target: https://docs.sunpy.org/en/stable/citation.html
+.. |pyOpenSci| image:: https://tinyurl.com/y22nb8up
+   :target: https://github.com/pyOpenSci/software-submission/issues/147
 
 ``sunpy`` is a Python software package that provides fundamental tools for accessing, loading and interacting with solar physics data in Python.
 It includes an interface for searching and downloading data from multiple data providers, data containers for image and time series data, commonly used solar coordinate frames and associated transformations, as well as other functionality needed for solar data analysis.
 
 Installation
 ============
```

### Comparing `sunpy-5.1.1/README.rst` & `sunpy-5.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 *********
 ``sunpy``
 *********
-
 |SunPy Logo|
 
-+----------------------+----------------------+----------------------+
-| Release              | Development          | Community            |
-+======================+======================+======================+
-| |Latest PyPi         | |Python Versions|    | |Matrix Chat Room|   |
-| Version|             |                      |                      |
-+----------------------+----------------------+----------------------+
-| |Latest Conda        | |Project Status:     | |OpenAstronomy       |
-| Version|             | Active - The project | Discourse community| |
-|                      | has reached a        |                      |
-|                      | stable, usable state |                      |
-|                      | and is being         |                      |
-|                      | actively developed.| |                      |
-+----------------------+----------------------+----------------------+
-| |Zenodo - Latest     | |Continuous          | |Google Groups       |
-| DOI|                 | Integration Status|  | Mailing List|        |
-+----------------------+----------------------+----------------------+
-| |sunpy Stable        | |CodeCov Code        | |Powered by          |
-| Documentation|       | Coverage|            | NumFOCUS|            |
-+----------------------+----------------------+----------------------+
++-----------------------------------+-----------------------------------+-----------------------------------+
+|           Release                 |           Development             |           Community               |
++===================================+===================================+===================================+
+|       |Latest PyPi Version|       |        |Python Versions|          |         |Matrix Chat Room|        |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|     |Latest Conda Version|        |     |Project Status: Active|      |     |OpenAstronomy Discourse|     |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|      |Zenodo - Latest DOI|        |  |Continuous Integration Status|  |    |Google Groups Mailing List|   |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|    |sunpy stable documentation|   |     |CodeCov Code Coverage|       |       |Powered by NumFOCUS|       |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|         |sunpy citation|          |                                   |            |pyOpenSci|            |
++-----------------------------------+-----------------------------------+-----------------------------------+
 
-.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/sunpy_logo_landscape.svg
+.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.png
    :width: 200px
 .. |Latest PyPi Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/sunpy
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Matrix Chat Room| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=matrix.org
    :target: https://app.element.io/#/room/#sunpy:openastronomy.org
 .. |Latest Conda Version| image:: https://anaconda.org/conda-forge/sunpy/badges/version.svg
    :target: https://anaconda.org/conda-forge/sunpy
-.. |Project Status: Active - The project has reached a stable, usable state and is being actively developed.| image:: https://www.repostatus.org/badges/latest/active.svg
+.. |Project Status: Active| image:: https://www.repostatus.org/badges/latest/active.svg
    :target: https://www.repostatus.org/#active
-.. |OpenAstronomy Discourse community| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
+.. |OpenAstronomy Discourse| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
    :height: 20px
    :target: https://community.openastronomy.org/
 .. |Zenodo - Latest DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |Continuous Integration Status| image:: https://github.com/sunpy/sunpy/actions/workflows/ci.yml/badge.svg?branch=main
    :target: https://github.com/sunpy/sunpy/actions/workflows/ci.yml
-.. |Google Groups Mailing List| image:: https://fonts.gstatic.com/s/i/productlogos/groups/v9/web-48dp/logo_groups_color_1x_web_48dp.png
+.. |Google Groups Mailing List| image:: https://upload.wikimedia.org/wikipedia/commons/2/27/Google_Groups_logo.gif
    :height: 20px
    :target: https://groups.google.com/g/sunpy
-.. |sunpy Stable Documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
+.. |sunpy stable documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
    :target: https://docs.sunpy.org/
 .. |CodeCov Code Coverage| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
+.. |sunpy citation| image:: https://img.shields.io/badge/cite-sunpy-orange
+   :target: https://docs.sunpy.org/en/stable/citation.html
+.. |pyOpenSci| image:: https://tinyurl.com/y22nb8up
+   :target: https://github.com/pyOpenSci/software-submission/issues/147
 
 ``sunpy`` is a Python software package that provides fundamental tools for accessing, loading and interacting with solar physics data in Python.
 It includes an interface for searching and downloading data from multiple data providers, data containers for image and time series data, commonly used solar coordinate frames and associated transformations, as well as other functionality needed for solar data analysis.
 
 Installation
 ============
```

### Comparing `sunpy-5.1.1/docs/Makefile` & `sunpy-5.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/conf.py` & `sunpy-5.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/backports.rst` & `sunpy-5.1.2/docs/dev_guide/contents/backports.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/ci_jobs.rst` & `sunpy-5.1.2/docs/dev_guide/contents/ci_jobs.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/code_standards.rst` & `sunpy-5.1.2/docs/dev_guide/contents/code_standards.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/conda_for_dependencies.rst` & `sunpy-5.1.2/docs/dev_guide/contents/conda_for_dependencies.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/dependencies.rst` & `sunpy-5.1.2/docs/dev_guide/contents/dependencies.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/documentation.rst` & `sunpy-5.1.2/docs/dev_guide/contents/documentation.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/example_gallery.rst` & `sunpy-5.1.2/docs/dev_guide/contents/example_gallery.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/funding.rst` & `sunpy-5.1.2/docs/dev_guide/contents/funding.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/images/actions_check_pr.png` & `sunpy-5.1.2/docs/dev_guide/contents/images/actions_check_pr.png`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/images/actions_summary_check.png` & `sunpy-5.1.2/docs/dev_guide/contents/images/actions_summary_check.png`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/images/checks.png` & `sunpy-5.1.2/docs/dev_guide/contents/images/checks.png`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/images/checks_pr.png` & `sunpy-5.1.2/docs/dev_guide/contents/images/checks_pr.png`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/logger.rst` & `sunpy-5.1.2/docs/dev_guide/contents/logger.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/maintainer_workflow.rst` & `sunpy-5.1.2/docs/dev_guide/contents/maintainer_workflow.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/newcomers.rst` & `sunpy-5.1.2/docs/dev_guide/contents/newcomers.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/pr_checklist.rst` & `sunpy-5.1.2/docs/dev_guide/contents/pr_checklist.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/pr_review_procedure.rst` & `sunpy-5.1.2/docs/dev_guide/contents/pr_review_procedure.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/public_api.rst` & `sunpy-5.1.2/docs/dev_guide/contents/public_api.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/remote_data_manager.rst` & `sunpy-5.1.2/docs/dev_guide/contents/remote_data_manager.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/tests.rst` & `sunpy-5.1.2/docs/dev_guide/contents/tests.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/contents/units_quantities.rst` & `sunpy-5.1.2/docs/dev_guide/contents/units_quantities.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/dev_guide/index.rst` & `sunpy-5.1.2/docs/dev_guide/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/coord_components.rst` & `sunpy-5.1.2/docs/how_to/coord_components.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/create_a_map.rst` & `sunpy-5.1.2/docs/how_to/create_a_map.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/create_coords.rst` & `sunpy-5.1.2/docs/how_to/create_coords.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/create_custom_map.rst` & `sunpy-5.1.2/docs/how_to/create_custom_map.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/create_custom_timeseries.rst` & `sunpy-5.1.2/docs/how_to/create_custom_timeseries.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/index.rst` & `sunpy-5.1.2/docs/how_to/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
    :maxdepth: 1
 
    coord_components
    create_a_map
    create_coords
    create_custom_map
    create_custom_timeseries
+   fix_map_metadata
    parse_time
    remote_data_manager
    search_multiple_wavelengths
    search_vso
    transform_coords
 
 **Quick Reference**
```

### Comparing `sunpy-5.1.1/docs/how_to/parse_time.rst` & `sunpy-5.1.2/docs/how_to/parse_time.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/remote_data_manager.rst` & `sunpy-5.1.2/docs/how_to/remote_data_manager.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/search_multiple_wavelengths.rst` & `sunpy-5.1.2/docs/how_to/search_multiple_wavelengths.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/search_vso.rst` & `sunpy-5.1.2/docs/how_to/search_vso.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/how_to/transform_coords.rst` & `sunpy-5.1.2/docs/how_to/transform_coords.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/index.rst` & `sunpy-5.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/make.bat` & `sunpy-5.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/nitpick-exceptions` & `sunpy-5.1.2/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/coordinates/index.rst` & `sunpy-5.1.2/docs/reference/coordinates/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/customization.rst` & `sunpy-5.1.2/docs/reference/customization.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/database.rst` & `sunpy-5.1.2/docs/reference/database.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/io.rst` & `sunpy-5.1.2/docs/reference/io.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/known_issues.rst` & `sunpy-5.1.2/docs/reference/known_issues.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/net.rst` & `sunpy-5.1.2/docs/reference/net.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/ssw.rst` & `sunpy-5.1.2/docs/reference/ssw.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/stability.rst` & `sunpy-5.1.2/docs/reference/stability.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/sunpy_stability.yaml` & `sunpy-5.1.2/docs/reference/sunpy_stability.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/timeseries.rst` & `sunpy-5.1.2/docs/reference/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/reference/troubleshooting.rst` & `sunpy-5.1.2/docs/reference/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/carrington.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/carrington.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/index.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/rotatedsunframe.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/rotatedsunframe.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/rsun.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/rsun.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/velocities.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/velocities.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/coordinates/wcs.rst` & `sunpy-5.1.2/docs/topic_guide/coordinates/wcs.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/custom_map_rotate.rst` & `sunpy-5.1.2/docs/topic_guide/custom_map_rotate.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/extending_fido.rst` & `sunpy-5.1.2/docs/topic_guide/extending_fido.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/helioviewer.rst` & `sunpy-5.1.2/docs/topic_guide/helioviewer.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/history_comments.rst` & `sunpy-5.1.2/docs/topic_guide/history_comments.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/index.rst` & `sunpy-5.1.2/docs/topic_guide/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/installation.rst` & `sunpy-5.1.2/docs/topic_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/logger.rst` & `sunpy-5.1.2/docs/topic_guide/logger.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/new_map_class.rst` & `sunpy-5.1.2/docs/topic_guide/new_map_class.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/rsun.rst` & `sunpy-5.1.2/docs/topic_guide/rsun.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/topic_guide/timeseries_metadata.rst` & `sunpy-5.1.2/docs/topic_guide/timeseries_metadata.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/acquiring_data/hek.rst` & `sunpy-5.1.2/docs/tutorial/acquiring_data/hek.rst`

 * *Files 1% similar despite different names*

```diff
@@ -150,18 +150,18 @@
    >>> help(a.hek.FRM) # doctest:+REMOTE_DATA
    Help on FRM in module sunpy.net.hek.attrs object:
    <BLANKLINE>
    class FRM(builtins.object)
     |  Data descriptors defined here:
     |
     |  __dict__
-    |      dictionary for instance variables (if defined)
+    |      dictionary for instance variables
     |
     |  __weakref__
-    |      list of weak references to the object (if defined)
+    |      list of weak references to the object
     |
     |  ----------------------------------------------------------------------
     |  Data and other attributes defined here:
     |
     |  Contact = <sunpy.net.hek.attrs._StringParamAttrWrapper object>
     |
     |  HumanFlag = <sunpy.net.hek.attrs._StringParamAttrWrapper object>
```

### Comparing `sunpy-5.1.1/docs/tutorial/acquiring_data/index.rst` & `sunpy-5.1.2/docs/tutorial/acquiring_data/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     2012-03-04 00:00:00.000 2012-03-04 23:59:59.999       LYRA ...      ESA     2
     2012-03-05 00:00:00.000 2012-03-05 23:59:59.999       LYRA ...      ESA     2
     2012-03-06 00:00:00.000 2012-03-06 23:59:59.999       LYRA ...      ESA     2
     <BLANKLINE>
     <BLANKLINE>
 
 Queries can be made more flexible or specific by adding more attrs objects to the `~sunpy.net.Fido` search.
-As an example, specific passbands can be searched for by supplying an `~astropy.units.Quantity` to the `a.Wavelength <sunpy.net.attrs.Wavelength>` attribute:
+As an example, specific passbands can be searched for by supplying a `~astropy.units.Quantity` to the `a.Wavelength <sunpy.net.attrs.Wavelength>` attribute:
 
 .. code-block:: python
 
     >>> import astropy.units as u
 
     >>> Fido.search(a.Time('2012/3/4', '2012/3/4'), a.Instrument.aia,
     ...             a.Wavelength(171*u.angstrom))  # doctest: +REMOTE_DATA
```

### Comparing `sunpy-5.1.1/docs/tutorial/acquiring_data/jsoc.rst` & `sunpy-5.1.2/docs/tutorial/acquiring_data/jsoc.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/coordinates.rst` & `sunpy-5.1.2/docs/tutorial/coordinates.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/index.rst` & `sunpy-5.1.2/docs/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/installation.rst` & `sunpy-5.1.2/docs/tutorial/installation.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/maps.rst` & `sunpy-5.1.2/docs/tutorial/maps.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/time.rst` & `sunpy-5.1.2/docs/tutorial/time.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/timeseries.rst` & `sunpy-5.1.2/docs/tutorial/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/tutorial/units.rst` & `sunpy-5.1.2/docs/tutorial/units.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/0.8.rst` & `sunpy-5.1.2/docs/whatsnew/0.8.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/0.9.rst` & `sunpy-5.1.2/docs/whatsnew/0.9.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/1.0.rst` & `sunpy-5.1.2/docs/whatsnew/1.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/1.1-wispr.png` & `sunpy-5.1.2/docs/whatsnew/1.1-wispr.png`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/1.1.rst` & `sunpy-5.1.2/docs/whatsnew/1.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/2.0.rst` & `sunpy-5.1.2/docs/whatsnew/2.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/2.1.rst` & `sunpy-5.1.2/docs/whatsnew/2.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/3.0.rst` & `sunpy-5.1.2/docs/whatsnew/3.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/3.1.rst` & `sunpy-5.1.2/docs/whatsnew/3.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/4.0.rst` & `sunpy-5.1.2/docs/whatsnew/4.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/4.1.rst` & `sunpy-5.1.2/docs/whatsnew/4.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/5.0.rst` & `sunpy-5.1.2/docs/whatsnew/5.0.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/5.1.rst` & `sunpy-5.1.2/docs/whatsnew/5.1.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/docs/whatsnew/index.rst` & `sunpy-5.1.2/docs/whatsnew/index.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/acquiring_data/downloading_cutouts.py` & `sunpy-5.1.2/examples/acquiring_data/downloading_cutouts.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/acquiring_data/fido_metadata_queries.py` & `sunpy-5.1.2/examples/acquiring_data/fido_metadata_queries.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/acquiring_data/querying_and_loading_SHARP_data.py` & `sunpy-5.1.2/examples/acquiring_data/querying_and_loading_SHARP_data.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/acquiring_data/querying_the_GOES_event_list.py` & `sunpy-5.1.2/examples/acquiring_data/querying_the_GOES_event_list.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/acquiring_data/search_cdaweb.py` & `sunpy-5.1.2/examples/acquiring_data/search_cdaweb.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/computer_vision_techniques/finding_masking_bright_pixels.py` & `sunpy-5.1.2/examples/computer_vision_techniques/finding_masking_bright_pixels.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/computer_vision_techniques/loop_edge_enhance.py` & `sunpy-5.1.2/examples/computer_vision_techniques/loop_edge_enhance.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/computer_vision_techniques/mask_disk.py` & `sunpy-5.1.2/examples/computer_vision_techniques/mask_disk.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/computer_vision_techniques/off_limb_enhance.py` & `sunpy-5.1.2/examples/computer_vision_techniques/off_limb_enhance.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/differential_rotation/comparing_rotation_models.py` & `sunpy-5.1.2/examples/differential_rotation/comparing_rotation_models.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/differential_rotation/differentially_rotated_coordinate.py` & `sunpy-5.1.2/examples/differential_rotation/differentially_rotated_coordinate.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/differential_rotation/differentially_rotated_gridlines.py` & `sunpy-5.1.2/examples/differential_rotation/differentially_rotated_gridlines.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/differential_rotation/reprojected_map.py` & `sunpy-5.1.2/examples/differential_rotation/reprojected_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/brightness_pixel_location.py` & `sunpy-5.1.2/examples/map/brightness_pixel_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/compare_rotation_results.py` & `sunpy-5.1.2/examples/map/compare_rotation_results.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/composite_map_AIA_HMI.py` & `sunpy-5.1.2/examples/map/composite_map_AIA_HMI.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/difference_images.py` & `sunpy-5.1.2/examples/map/difference_images.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/hmi_contours_wcsaxes.py` & `sunpy-5.1.2/examples/map/hmi_contours_wcsaxes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/image_bright_regions_gallery_example.py` & `sunpy-5.1.2/examples/map/image_bright_regions_gallery_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/lasco_mask.py` & `sunpy-5.1.2/examples/map/lasco_mask.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_contouring.py` & `sunpy-5.1.2/examples/map/map_contouring.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_data_histogram.py` & `sunpy-5.1.2/examples/map/map_data_histogram.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_from_numpy_array.py` & `sunpy-5.1.2/examples/map/map_from_numpy_array.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_metadata_modification.py` & `sunpy-5.1.2/examples/map/map_metadata_modification.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_resampling_and_superpixels.py` & `sunpy-5.1.2/examples/map/map_resampling_and_superpixels.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_rotation.py` & `sunpy-5.1.2/examples/map/map_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/map_segment.py` & `sunpy-5.1.2/examples/map/map_segment.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/masking_hmi.py` & `sunpy-5.1.2/examples/map/masking_hmi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/plot_frameless_image.py` & `sunpy-5.1.2/examples/map/plot_frameless_image.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map/submaps_and_cropping.py` & `sunpy-5.1.2/examples/map/submaps_and_cropping.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/autoalign_aia_hmi.py` & `sunpy-5.1.2/examples/map_transformations/autoalign_aia_hmi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/projection_custom_origin.py` & `sunpy-5.1.2/examples/map_transformations/projection_custom_origin.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/reprojection_aia_euvi_mosaic.py` & `sunpy-5.1.2/examples/map_transformations/reprojection_aia_euvi_mosaic.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/reprojection_align_aia_hmi.py` & `sunpy-5.1.2/examples/map_transformations/reprojection_align_aia_hmi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/reprojection_carrington.py` & `sunpy-5.1.2/examples/map_transformations/reprojection_carrington.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/reprojection_different_observers.py` & `sunpy-5.1.2/examples/map_transformations/reprojection_different_observers.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/reprojection_spherical_screen.py` & `sunpy-5.1.2/examples/map_transformations/reprojection_spherical_screen.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/map_transformations/upside_down_hmi.py` & `sunpy-5.1.2/examples/map_transformations/upside_down_hmi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/AIA_HMI_composite.py` & `sunpy-5.1.2/examples/plotting/AIA_HMI_composite.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/aia_example.py` & `sunpy-5.1.2/examples/plotting/aia_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/arrayanimatorwcs.py` & `sunpy-5.1.2/examples/plotting/arrayanimatorwcs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/fading_between_maps.py` & `sunpy-5.1.2/examples/plotting/fading_between_maps.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/finding_local_peaks_in_solar_data.py` & `sunpy-5.1.2/examples/plotting/finding_local_peaks_in_solar_data.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/finegrained_plot.py` & `sunpy-5.1.2/examples/plotting/finegrained_plot.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/great_arc_example.py` & `sunpy-5.1.2/examples/plotting/great_arc_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/grid_plotting.py` & `sunpy-5.1.2/examples/plotting/grid_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/hmi_synoptic_maps.py` & `sunpy-5.1.2/examples/plotting/hmi_synoptic_maps.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/lasco_overlay.py` & `sunpy-5.1.2/examples/plotting/lasco_overlay.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/lat_lon_lines.py` & `sunpy-5.1.2/examples/plotting/lat_lon_lines.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/limb_plotting.py` & `sunpy-5.1.2/examples/plotting/limb_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/lineAnimator_examples.py` & `sunpy-5.1.2/examples/plotting/lineAnimator_examples.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/magnetogram_active_regions.py` & `sunpy-5.1.2/examples/plotting/magnetogram_active_regions.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/map_editcolormap.py` & `sunpy-5.1.2/examples/plotting/map_editcolormap.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/masked_composite_plot.py` & `sunpy-5.1.2/examples/plotting/masked_composite_plot.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/mplcairo_plotting.py` & `sunpy-5.1.2/examples/plotting/mplcairo_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/overplot_hek_polygon.py` & `sunpy-5.1.2/examples/plotting/overplot_hek_polygon.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/plot_equator_prime_meridian.py` & `sunpy-5.1.2/examples/plotting/plot_equator_prime_meridian.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/plot_rectangle.py` & `sunpy-5.1.2/examples/plotting/plot_rectangle.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/plot_rotated_rectangle.py` & `sunpy-5.1.2/examples/plotting/plot_rotated_rectangle.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/plotting_blank_map.py` & `sunpy-5.1.2/examples/plotting/plotting_blank_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/quadrangle.py` & `sunpy-5.1.2/examples/plotting/quadrangle.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/simple_differential_rotation.py` & `sunpy-5.1.2/examples/plotting/simple_differential_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/solar_cycle_example.py` & `sunpy-5.1.2/examples/plotting/solar_cycle_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/sunpy_matplotlib_colormap.py` & `sunpy-5.1.2/examples/plotting/sunpy_matplotlib_colormap.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/three_map_composite.py` & `sunpy-5.1.2/examples/plotting/three_map_composite.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/wcsaxes_map_example.py` & `sunpy-5.1.2/examples/plotting/wcsaxes_map_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/wcsaxes_plotting_example.py` & `sunpy-5.1.2/examples/plotting/wcsaxes_plotting_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/plotting/xy_lims.py` & `sunpy-5.1.2/examples/plotting/xy_lims.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/saving_and_loading_data/coordinates_in_asdf.py` & `sunpy-5.1.2/examples/saving_and_loading_data/coordinates_in_asdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/saving_and_loading_data/genericmap_in_asdf.py` & `sunpy-5.1.2/examples/saving_and_loading_data/genericmap_in_asdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/saving_and_loading_data/genericmap_in_fits.py` & `sunpy-5.1.2/examples/saving_and_loading_data/genericmap_in_fits.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/showcase/eclipse_amount.py` & `sunpy-5.1.2/examples/showcase/eclipse_amount.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/showcase/hmi_cutout.py` & `sunpy-5.1.2/examples/showcase/hmi_cutout.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/showcase/stereoscopic_3d.py` & `sunpy-5.1.2/examples/showcase/stereoscopic_3d.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/showcase/where_is_stereo.py` & `sunpy-5.1.2/examples/showcase/where_is_stereo.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/goes_hek_m25.py` & `sunpy-5.1.2/examples/time_series/goes_hek_m25.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/goes_xrs_example.py` & `sunpy-5.1.2/examples/time_series/goes_xrs_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/goes_xrs_nrt_data.py` & `sunpy-5.1.2/examples/time_series/goes_xrs_nrt_data.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/power_spectra_example.py` & `sunpy-5.1.2/examples/time_series/power_spectra_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/timeseries_convolution_filter.py` & `sunpy-5.1.2/examples/time_series/timeseries_convolution_filter.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/timeseries_example.py` & `sunpy-5.1.2/examples/time_series/timeseries_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/timeseries_peak_finding.py` & `sunpy-5.1.2/examples/time_series/timeseries_peak_finding.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/time_series/timeseriesmetadata_example.py` & `sunpy-5.1.2/examples/time_series/timeseriesmetadata_example.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/AIA_limb_STEREO.py` & `sunpy-5.1.2/examples/units_and_coordinates/AIA_limb_STEREO.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/AltAz_Coordinate_transform.py` & `sunpy-5.1.2/examples/units_and_coordinates/AltAz_Coordinate_transform.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/ParkerSolarProbe_trajectory.py` & `sunpy-5.1.2/examples/units_and_coordinates/ParkerSolarProbe_trajectory.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py` & `sunpy-5.1.2/examples/units_and_coordinates/SDO_to_STEREO_Coordinate_Conversion.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/STEREO_SECCHI_starfield.py` & `sunpy-5.1.2/examples/units_and_coordinates/STEREO_SECCHI_starfield.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/getting_lasco_observer_location.py` & `sunpy-5.1.2/examples/units_and_coordinates/getting_lasco_observer_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/getting_observer_location.py` & `sunpy-5.1.2/examples/units_and_coordinates/getting_observer_location.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/map_slit_extraction.py` & `sunpy-5.1.2/examples/units_and_coordinates/map_slit_extraction.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/north_offset_frame.py` & `sunpy-5.1.2/examples/units_and_coordinates/north_offset_frame.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/planet_locations.py` & `sunpy-5.1.2/examples/units_and_coordinates/planet_locations.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/radec_to_hpc_map.py` & `sunpy-5.1.2/examples/units_and_coordinates/radec_to_hpc_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/spice.py` & `sunpy-5.1.2/examples/units_and_coordinates/spice.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/examples/units_and_coordinates/venus_transit.py` & `sunpy-5.1.2/examples/units_and_coordinates/venus_transit.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/licenses/ASTROPY.rst` & `sunpy-5.1.2/licenses/ASTROPY.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/licenses/GLUE.rst` & `sunpy-5.1.2/licenses/GLUE.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/licenses/SCIKIT-LEARN.rst` & `sunpy-5.1.2/licenses/SCIKIT-LEARN.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/licenses/TOWNCRIER.rst` & `sunpy-5.1.2/licenses/TOWNCRIER.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/pyproject.toml` & `sunpy-5.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/setup.cfg` & `sunpy-5.1.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	astropy>=5.0.6,!=5.1.0
 	numpy>=1.21.0
 	packaging>=19.0
 	parfive[ftp]>=2.0.0
+	pyerfa
 
 [options.extras_require]
 asdf = 
 	asdf-astropy>=0.1.1
 	asdf>=2.8.0
 dask = 
 	dask[array]>=2021.4.0
@@ -193,25 +194,26 @@
 	ignore:'cgi' is deprecated and slated for removal in Python 3.13:DeprecationWarning:zeep.utils
 	ignore:.*np.bool8.*is a deprecated alias.*:DeprecationWarning
 	ignore:Deprecated API features detected.*SQLAlchemy 2
 	ignore:`product` is deprecated as of NumPy 1.25.0:DeprecationWarning
 	ignore:.*module is deprecated, as it was designed for internal use
 	ignore::sunpy.util.exceptions.SunpyConnectionWarning
 	ignore:datetime.datetime.utcfromtimestamp():DeprecationWarning
+	ignore:\nPyarrow will become a required dependency of pandas in the next major release of pandas:DeprecationWarning
 
 [flake8]
 ignore = 
-	E225, # missing-whitespace-around-operator
-	E226, # missing-whitespace-around-arithmetic-operator
-	E501, # line-too-long
-	F401, # unused-import
-	F403, # undefined-local-with-import-star
-	F811, # redefined-while-unused
-	W503, # Line break occurred before a binary operator
-	W504, # Line break occurred after a binary operator
+	E225,
+	E226,
+	E501,
+	F401,
+	F403,
+	F811,
+	W503,
+	W504,
 max-line-length = 110
 exclude = 
 	.git,
 	__pycache__,
 	docs/conf.py,
 	build,
 	sunpy/data/sample.py,
```

### Comparing `sunpy-5.1.1/sunpy/CITATION.rst` & `sunpy-5.1.2/sunpy/CITATION.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/__init__.py` & `sunpy-5.1.2/sunpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/conftest.py` & `sunpy-5.1.2/sunpy/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/__init__.py` & `sunpy-5.1.2/sunpy/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/_transformations.py` & `sunpy-5.1.2/sunpy/coordinates/_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,16 @@
     """
     Return the matrix for the direct rotation from one representation to a second representation.
     The representations need not be normalized first, and can be arrays of representations.
     """
     A = start_representation.to_cartesian()
     B = end_representation.to_cartesian()
     rotation_axis = A.cross(B)
-    rotation_angle = -np.arccos(A.dot(B) / (A.norm() * B.norm()))  # negation is required
+    # Calculate the angle using both cross and dot products to minimize numerical-precision issues
+    rotation_angle = -np.arctan2(rotation_axis.norm(), A.dot(B))  # negation is required
 
     if rotation_angle.isscalar:
         # This line works around some input/output quirks of Astropy's rotation_matrix()
         matrix = np.array(rotation_matrix(rotation_angle, rotation_axis.xyz.value.tolist()))
     else:
         matrix_list = [np.array(rotation_matrix(angle, axis.xyz.value.tolist()))
                        for angle, axis in zip(rotation_angle, rotation_axis)]
@@ -1067,15 +1068,15 @@
     sun_earth_int = sun_earth.transform_to(int_frame).cartesian
 
     # Rotate from Earth equatorial to ecliptic
     rot_matrix = _rotation_matrix_obliquity(int_frame.equinox)
     earth_object_int = geicoord.cartesian.transform(rot_matrix)
 
     # Find the Sun-object vector in the intermediate frame
-    sun_object_int = sun_earth_int + earth_object_int
+    sun_object_int = earth_object_int + sun_earth_int  # add in this order to preserve the original units
     int_coord = int_frame.realize_frame(sun_object_int)
 
     # Convert to the final frame through HCRS
     return int_coord.transform_to(HCRS(obstime=int_coord.obstime)).transform_to(hmeframe)
 
 
 @frame_transform_graph.transform(FunctionTransformWithFiniteDifference,
```

### Comparing `sunpy-5.1.1/sunpy/coordinates/data/igrf13coeffs.txt` & `sunpy-5.1.2/sunpy/coordinates/data/igrf13coeffs.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/ephemeris.py` & `sunpy-5.1.2/sunpy/coordinates/ephemeris.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/frameattributes.py` & `sunpy-5.1.2/sunpy/coordinates/frameattributes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/frames.py` & `sunpy-5.1.2/sunpy/coordinates/frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/metaframes.py` & `sunpy-5.1.2/sunpy/coordinates/metaframes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/offset_frame.py` & `sunpy-5.1.2/sunpy/coordinates/offset_frame.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/spice.py` & `sunpy-5.1.2/sunpy/coordinates/spice.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/sun.py` & `sunpy-5.1.2/sunpy/coordinates/sun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Sun-specific coordinate calculations
 """
 from typing import Literal
 
+import erfa
 import numpy as np
 
 import astropy.units as u
 from astropy.constants import R_earth
 from astropy.constants import c as speed_of_light
 from astropy.coordinates import (
     ITRS,
@@ -19,16 +20,14 @@
     Latitude,
     Longitude,
     SkyCoord,
     get_body_barycentric,
 )
 from astropy.coordinates.builtin_frames.utils import get_jd12
 from astropy.coordinates.representation import CartesianRepresentation, SphericalRepresentation
-# Import erfa via astropy to make sure we are using the same ERFA library as Astropy
-from astropy.coordinates.sky_coordinate import erfa
 from astropy.time import Time
 
 from sunpy import log
 from sunpy.sun import constants
 from sunpy.time import parse_time
 from sunpy.time.time import _variables_for_parse_time_docstring
 from sunpy.util.decorators import add_common_docstring
```

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/strategies.py` & `sunpy-5.1.2/sunpy/coordinates/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_ephemeris.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_frameattributes.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_frameattributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,16 @@
     assert issubclass(result.representation_type, SphericalRepresentation)
     assert result.obstime == observer.obstime
     assert converted
 
 
 def test_coord_get():
 
-    # Test default (instance=None)
-    obs = Helioprojective.observer
+    # Test default observer is None
+    obs = Helioprojective().observer
     assert obs is None
 
     # Test get
     obstime = "2013-04-01"
     obs = Helioprojective(observer="earth", obstime=obstime).observer
     earth = get_earth(obstime)
     assert isinstance(obs, HeliographicStonyhurst)
```

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_frames.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_metaframes.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_metaframes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_offset_frame.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_offset_frame.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_spice.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_sun.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_sun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import warnings
 
 import numpy as np
 import pytest
+from erfa import ErfaWarning
 from numpy.testing import assert_allclose
 
 import astropy.units as u
 from astropy.coordinates import Angle, EarthLocation
 from astropy.tests.helper import assert_quantity_allclose
 from astropy.time import Time
-from astropy.utils.exceptions import ErfaWarning
 
 from sunpy.coordinates import sun
 from sunpy.sun.constants import radius
 from .helpers import assert_longitude_allclose
 
 # Ignore warnings that astropy throws when trying and failing to update ephemeris
 pytestmark = pytest.mark.filterwarnings("ignore:failed to download")
```

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_transformations.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -691,14 +691,21 @@
     new = old.transform_to(HeliocentricEarthEcliptic)
 
     assert_quantity_allclose(new.lon, Longitude(109.74535*u.deg), atol=0.05*u.arcsec, rtol=0)
     assert_quantity_allclose(new.lat, 10.000070*u.deg, atol=0.01*u.arcsec, rtol=0)
     assert_quantity_allclose(new.distance, old.distance)
 
 
+def test_hee_earth():
+    # The Earth in HEE should have negligible Z component
+    times = parse_time('2013-08-10 12:00') + np.arange(10) * u.s
+    earth_hee = get_earth(times).heliocentricearthecliptic
+    assert_quantity_allclose(0*u.m, earth_hee.cartesian.z, atol=1e-4*u.m)
+
+
 def test_hee_hee():
     # Test HEE loopback transformation
     obstime = Time('2001-01-01')
     old = SkyCoord(90*u.deg, 10*u.deg, 1*u.AU, frame=HeliocentricEarthEcliptic(obstime=obstime))
 
     new = old.transform_to(HeliocentricEarthEcliptic)
 
@@ -1044,14 +1051,44 @@
 
     for coord in coords_in:
         for frame in coords_in:
             out_coord = coord.transform_to(frame.replicate(**args_out))
             assert_quantity_allclose(out_coord.rsun, args_out['rsun'])
 
 
+_framepairs = [
+    ('hcrs', 'heliographic_stonyhurst'),
+    ('heliographic_stonyhurst', 'heliographic_carrington'),
+    ('heliographic_stonyhurst', 'heliocentricinertial'),
+    ('heliographic_stonyhurst', 'heliocentric'),
+    ('heliocentric', 'helioprojective'),
+    ('heliocentricmeanecliptic', 'heliocentricearthecliptic'),
+    ('heliocentricearthecliptic', 'geocentricsolarecliptic'),
+    ('heliocentricmeanecliptic', 'geocentricearthequatorial'),
+    ('itrs', 'geomagnetic'),
+    ('geomagnetic', 'solarmagnetic'),
+    ('solarmagnetic', 'geocentricsolarmagnetospheric'),
+]
+
+
+@pytest.mark.parametrize(("frame1", "frame2"), _framepairs)
+@pytest.mark.parametrize("unit", [u.m, u.AU])
+def test_unit_preservation(frame1, frame2, unit):
+    coord = SkyCoord(CartesianRepresentation(0, 0, 0) * unit,
+                     frame=frame1, obstime="2001-01-01", observer="earth")
+
+    # Transform one direction and verify the unit is preserved
+    result1 = coord.transform_to(frame2)
+    assert result1.cartesian.xyz.unit == unit
+
+    # Transform back and verify the unit is preserved
+    result2 = result1.transform_to(frame1)
+    assert result2.cartesian.xyz.unit == unit
+
+
 def test_propagate_with_solar_surface():
     # Test propagating the meridian by 6 days of solar rotation
     meridian = SkyCoord(0*u.deg, np.arange(0, 90, 10)*u.deg, 1*u.AU,
                         frame=HeliocentricInertial, obstime='2001-01-01')
     dt = 6*u.day
     end_frame = HeliocentricInertial(obstime=meridian.obstime + dt)
```

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_utils.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/tests/test_wcs_utils.py` & `sunpy-5.1.2/sunpy/coordinates/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/utils.py` & `sunpy-5.1.2/sunpy/coordinates/utils.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/coordinates/wcs_utils.py` & `sunpy-5.1.2/sunpy/coordinates/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/__init__.py` & `sunpy-5.1.2/sunpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/_sample.py` & `sunpy-5.1.2/sunpy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/cache.py` & `sunpy-5.1.2/sunpy/data/data_manager/cache.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/downloader.py` & `sunpy-5.1.2/sunpy/data/data_manager/downloader.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/manager.py` & `sunpy-5.1.2/sunpy/data/data_manager/manager.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/storage.py` & `sunpy-5.1.2/sunpy/data/data_manager/storage.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/conftest.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/mocks.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/test_cache.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/test_downloader.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/test_manager.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/data_manager/tests/test_storage.py` & `sunpy-5.1.2/sunpy/data/data_manager/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/sample.py` & `sunpy-5.1.2/sunpy/data/sample.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/sunpyrc` & `sunpy-5.1.2/sunpy/data/sunpyrc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2` & `sunpy-5.1.2/sunpy/data/test/2013_05_13__16_54_06_137__SOHO_LASCO_C3_white-light.jp2`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2` & `sunpy-5.1.2/sunpy/data/test/2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/20181209_180305_kcor_l2.header` & `sunpy-5.1.2/sunpy/data/test/20181209_180305_kcor_l2.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2` & `sunpy-5.1.2/sunpy/data/test/2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT/efz20040301.000010_s.fits` & `sunpy-5.1.2/sunpy/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT/efz20040301.010016_s.fits` & `sunpy-5.1.2/sunpy/data/test/EIT/efz20040301.010016_s.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.000010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.000010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.010016_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.010016_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.020010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.020010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.030011_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.030011_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.040010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.040010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.050010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.050010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.060010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.060010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.070014_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.070014_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.080010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.080010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.090010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.090010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.100010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.100010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.110010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.110010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EIT_header/efz20040301.120010_s.header` & `sunpy-5.1.2/sunpy/data/test/EIT_header/efz20040301.120010_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt` & `sunpy-5.1.2/sunpy/data/test/EVE_L0CS_DIODES_1m_truncated.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/FGMG4_20110214_030443.7.header` & `sunpy-5.1.2/sunpy/data/test/FGMG4_20110214_030443.7.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/HinodeSOT.header` & `sunpy-5.1.2/sunpy/data/test/HinodeSOT.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/HinodeXRT.header` & `sunpy-5.1.2/sunpy/data/test/HinodeXRT.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/19960106SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/19960106SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/19960430SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/19960430SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/19960513SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/19960513SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20000922SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20000922SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20000927SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20000927SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20001001SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20001001SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20020624SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20020624SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20020628SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20020628SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20100621SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20100621SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20150101SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20150101SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20150306SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20150306SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SRS/20150906SRS.txt` & `sunpy-5.1.2/sunpy/data/test/SRS/20150906SRS.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SWAP/resampled0_swap.header` & `sunpy-5.1.2/sunpy/data/test/SWAP/resampled0_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SWAP/resampled1_swap.header` & `sunpy-5.1.2/sunpy/data/test/SWAP/resampled1_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SWAP/resampled2_swap.header` & `sunpy-5.1.2/sunpy/data/test/SWAP/resampled2_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/SWAP/resampled3_swap.header` & `sunpy-5.1.2/sunpy/data/test/SWAP/resampled3_swap.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/YohkohSXT.header` & `sunpy-5.1.2/sunpy/data/test/YohkohSXT.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/__init__.py` & `sunpy-5.1.2/sunpy/data/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/_generate_asdf_test.py` & `sunpy-5.1.2/sunpy/data/test/_generate_asdf_test.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/aia_171_level1.fits` & `sunpy-5.1.2/sunpy/data/test/aia_171_level1.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/aiamap_genericmap_1.0.0.asdf` & `sunpy-5.1.2/sunpy/data/test/aiamap_genericmap_1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf` & `sunpy-5.1.2/sunpy/data/test/aiamap_shift_genericmap_1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/annotation_ppt.db` & `sunpy-5.1.2/sunpy/data/test/annotation_ppt.db`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/cor1_20090615_000500_s4c1A.header` & `sunpy-5.1.2/sunpy/data/test/cor1_20090615_000500_s4c1A.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header` & `sunpy-5.1.2/sunpy/data/test/dr_suvi-l2-ci195_g16_s20190403T093200Z_e20190403T093600Z_v1-0-0_rebinned.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/euvi_20090615_000900_n4euA_s.header` & `sunpy-5.1.2/sunpy/data/test/euvi_20090615_000900_n4euA_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve/eve_01.txt` & `sunpy-5.1.2/sunpy/data/test/eve/eve_01.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve/eve_02.txt` & `sunpy-5.1.2/sunpy/data/test/eve/eve_02.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve/eve_03.txt` & `sunpy-5.1.2/sunpy/data/test/eve/eve_03.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve/eve_04.txt` & `sunpy-5.1.2/sunpy/data/test/eve/eve_04.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve/eve_05.txt` & `sunpy-5.1.2/sunpy/data/test/eve/eve_05.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits` & `sunpy-5.1.2/sunpy/data/test/eve_l1_esp_2011046_00_truncated.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/gbm.fits` & `sunpy-5.1.2/sunpy/data/test/gbm.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/generated_sample.genx` & `sunpy-5.1.2/sunpy/data/test/generated_sample.genx`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/go1520110607.fits` & `sunpy-5.1.2/sunpy/data/test/go1520110607.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/go1520120601.fits.gz` & `sunpy-5.1.2/sunpy/data/test/go1520120601.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/goes_13_leap_second.nc` & `sunpy-5.1.2/sunpy/data/test/goes_13_leap_second.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/gong_synoptic.header` & `sunpy-5.1.2/sunpy/data/test/gong_synoptic.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/heliographic_phase_map.fits.gz` & `sunpy-5.1.2/sunpy/data/test/heliographic_phase_map.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/hi_20110910_114721_s7h2A.header` & `sunpy-5.1.2/sunpy/data/test/hi_20110910_114721_s7h2A.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/hmi_synoptic.header` & `sunpy-5.1.2/sunpy/data/test/hmi_synoptic.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/hsi_image_20101016_191218.fits` & `sunpy-5.1.2/sunpy/data/test/hsi_image_20101016_191218.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz` & `sunpy-5.1.2/sunpy/data/test/hsi_obssumm_20120601_018_truncated.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header` & `sunpy-5.1.2/sunpy/data/test/iris_l2_20130801_074720_4040000014_SJI_1400_t000.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/lasco_c2_25299383_s.header` & `sunpy-5.1.2/sunpy/data/test/lasco_c2_25299383_s.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/lasco_c3.header` & `sunpy-5.1.2/sunpy/data/test/lasco_c3.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz` & `sunpy-5.1.2/sunpy/data/test/lyra_20150101-000000_lev3_std_truncated.fits.gz`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header` & `sunpy-5.1.2/sunpy/data/test/mdi.fd_Ic.20101015_230100_TAI.data.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header` & `sunpy-5.1.2/sunpy/data/test/mdi.fd_M_96m_lev182.20101015_191200_TAI.data.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/mdi_synoptic.header` & `sunpy-5.1.2/sunpy/data/test/mdi_synoptic.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/not_actually_fits.fits` & `sunpy-5.1.2/sunpy/data/test/not_actually_fits.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/observed-solar-cycle-indices-truncated.json` & `sunpy-5.1.2/sunpy/data/test/observed-solar-cycle-indices-truncated.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/predicted-solar-cycle-truncated.json` & `sunpy-5.1.2/sunpy/data/test/predicted-solar-cycle-truncated.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf` & `sunpy-5.1.2/sunpy/data/test/psp_fld_l2_mag_rtn_1min_20200104_v02.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/resampled_hmi.fits` & `sunpy-5.1.2/sunpy/data/test/resampled_hmi.fits`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc` & `sunpy-5.1.2/sunpy/data/test/sci_gxrs-l2-irrad_g13_d20170901_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc` & `sunpy-5.1.2/sunpy/data/test/sci_gxrs-l2-irrad_g15_d20131028_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc` & `sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-avg1m_g15_d20190102_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc` & `sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-avg1m_g16_d20210101_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc` & `sunpy-5.1.2/sunpy/data/test/sci_xrsf-l2-flx1s_g17_d20201016_truncated.nc`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/seit_00171_fd_19961211_1900.header` & `sunpy-5.1.2/sunpy/data/test/seit_00171_fd_19961211_1900.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header` & `sunpy-5.1.2/sunpy/data/test/solo_L1_eui-fsi304-image_20201021T145510206_V03.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf` & `sunpy-5.1.2/sunpy/data/test/solo_L1_swa-pas-mom_20200706_V01.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf` & `sunpy-5.1.2/sunpy/data/test/solo_L2_epd-ept-north-hcad_20200713_V02.cdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/swap_lv1_20140606_000113.header` & `sunpy-5.1.2/sunpy/data/test/swap_lv1_20140606_000113.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/tca110810_truncated` & `sunpy-5.1.2/sunpy/data/test/tca110810_truncated`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/test_ana.fz` & `sunpy-5.1.2/sunpy/data/test/test_ana.fz`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/tsi20010130_025823_a2.header` & `sunpy-5.1.2/sunpy/data/test/tsi20010130_025823_a2.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header` & `sunpy-5.1.2/sunpy/data/test/waveunit/medn_halph_fl_20050501_074655.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/waveunit/mq130812.084253.header` & `sunpy-5.1.2/sunpy/data/test/waveunit/mq130812.084253.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/waveunit/na120701.091058.header` & `sunpy-5.1.2/sunpy/data/test/waveunit/na120701.091058.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header` & `sunpy-5.1.2/sunpy/data/test/waveunit/svsm_e3100_S2_20110625_1856.header`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/data/tests/test_sample.py` & `sunpy-5.1.2/sunpy/data/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/__init__.py` & `sunpy-5.1.2/sunpy/database/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/attrs.py` & `sunpy-5.1.2/sunpy/database/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/caching.py` & `sunpy-5.1.2/sunpy/database/caching.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/commands.py` & `sunpy-5.1.2/sunpy/database/commands.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/database.py` & `sunpy-5.1.2/sunpy/database/database.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tables.py` & `sunpy-5.1.2/sunpy/database/tables.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_attrs.py` & `sunpy-5.1.2/sunpy/database/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_caching.py` & `sunpy-5.1.2/sunpy/database/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_commands.py` & `sunpy-5.1.2/sunpy/database/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_database.py` & `sunpy-5.1.2/sunpy/database/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import configparser
 
 import pytest
 import sqlalchemy
 from parfive.results import Results
 
 from astropy import units
-from astropy.utils.exceptions import AstropyUserWarning
 
 import sunpy
 from sunpy.data.test import get_test_filepath
 from sunpy.database import (
     Database,
     EntryAlreadyAddedError,
     EntryAlreadyStarredError,
@@ -633,15 +632,15 @@
     database.redo()
     assert len(database) == 4
 
 
 def test_add_fom_path_duplicates(database, waveunit_fits_directory):
     database.add_from_dir(waveunit_fits_directory)
     assert len(database) == 4
-    with pytest.raises(EntryAlreadyAddedError), pytest.warns(AstropyUserWarning, match='File may have been truncated'):
+    with pytest.raises(EntryAlreadyAddedError):
         database.add_from_dir(waveunit_fits_directory)
 
 
 def test_add_fom_path_ignore_duplicates(database, waveunit_fits_directory):
     database.add_from_dir(waveunit_fits_directory)
     assert len(database) == 4
     database.add_from_dir(waveunit_fits_directory, ignore_already_added=True)
```

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_table.txt` & `sunpy-5.1.2/sunpy/database/tests/test_table.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/database/tests/test_tables.py` & `sunpy-5.1.2/sunpy/database/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/README.rst` & `sunpy-5.1.2/sunpy/extern/README.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/appdirs.py` & `sunpy-5.1.2/sunpy/extern/appdirs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/appdirs_license.txt` & `sunpy-5.1.2/sunpy/extern/appdirs_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/distro.py` & `sunpy-5.1.2/sunpy/extern/distro.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/distro_license.rst` & `sunpy-5.1.2/sunpy/extern/distro_license.rst`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/inflect.py` & `sunpy-5.1.2/sunpy/extern/inflect.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/inflect_license.txt` & `sunpy-5.1.2/sunpy/extern/inflect_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/parse.py` & `sunpy-5.1.2/sunpy/extern/parse.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/extern/parse_license.txt` & `sunpy-5.1.2/sunpy/extern/parse_license.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/image/resample.py` & `sunpy-5.1.2/sunpy/image/resample.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/image/tests/test_resample.py` & `sunpy-5.1.2/sunpy/image/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/image/tests/test_transform.py` & `sunpy-5.1.2/sunpy/image/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/image/transform.py` & `sunpy-5.1.2/sunpy/image/transform.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/_cdf.py` & `sunpy-5.1.2/sunpy/io/_cdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/_file_tools.py` & `sunpy-5.1.2/sunpy/io/_file_tools.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/_fits.py` & `sunpy-5.1.2/sunpy/io/_fits.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/_jp2.py` & `sunpy-5.1.2/sunpy/io/_jp2.py`

 * *Files 16% similar despite different names*

```diff
@@ -172,15 +172,19 @@
     Saving as a JPEG2000 will cast the data array to
     uint8 values to support the JPEG2000 format.
     """
     from glymur import Jp2k
 
     tmpname = fname + "tmp.jp2"
     jp2_data = np.uint8(data)
-    jp2 = Jp2k(tmpname, jp2_data, **kwargs)
+
+    # The jp2 data is flipped when read in, so we have to flip it back before
+    # saving. See https://github.com/sunpy/sunpy/pull/768 for context.
+    flipped = np.flip(jp2_data, 0)
+    jp2 = Jp2k(tmpname, flipped, **kwargs)
 
     # Append the XML data to the header information stored in jp2.box
     meta_boxes = jp2.box
     target_index = len(meta_boxes) - 1
     fits_box = generate_jp2_xmlbox(header)
     meta_boxes.insert(target_index, fits_box)
```

### Comparing `sunpy-5.1.1/sunpy/io/ana.py` & `sunpy-5.1.2/sunpy/io/ana.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/setup_package.py` & `sunpy-5.1.2/sunpy/io/setup_package.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/converters/frames.py` & `sunpy-5.1.2/sunpy/io/special/asdf/converters/frames.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/converters/generic_map.py` & `sunpy-5.1.2/sunpy/io/special/asdf/converters/generic_map.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/entry_points.py` & `sunpy-5.1.2/sunpy/io/special/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/manifests/sunpy-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/manifests/sunpy-1.1.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/manifests/sunpy-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/generic_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/generic_map-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricearthequatorial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricsolarecliptic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geocentricsolarmagnetospheric-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geocentricsolarmagnetospheric-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/geomagnetic-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/geomagnetic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentric-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentricearthecliptic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliocentricinertial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_carrington-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/heliographic_stonyhurst-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/helioprojective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/resources/schemas/solarmagnetic-1.0.0.yaml` & `sunpy-5.1.2/sunpy/io/special/asdf/resources/schemas/solarmagnetic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/tests/helpers.py` & `sunpy-5.1.2/sunpy/io/special/asdf/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/tests/hgc_100.asdf` & `sunpy-5.1.2/sunpy/io/special/asdf/tests/hgc_100.asdf`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/tests/test_coordinate_frames.py` & `sunpy-5.1.2/sunpy/io/special/asdf/tests/test_coordinate_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,45 +22,44 @@
     if new.has_data:
         assert new.data.components == old.data.components
         for comp in new.data.components:
             assert u.allclose(getattr(new.data, comp), getattr(old.data, comp))
 
 
 @pytest.fixture(params=sunpy_frames)
-@asdf_entry_points
 def coordframe_scalar(request):
     frame = request.param
 
     if frame._default_representation is CartesianRepresentation:
         data = np.random.random(3) * u.km
     else:
         data = np.random.random(2) * u.arcsec
 
     return frame(*data, obstime='2018-01-01T00:00:00')
 
 
 @pytest.fixture(params=sunpy_frames)
-@asdf_entry_points
 def coordframe_array(request):
     frame = request.param
 
     if frame._default_representation is CartesianRepresentation:
         data = np.random.random((3, 10)) * u.km
     else:
         data = np.random.random((2, 10)) * u.arcsec
 
     return frame(*data, obstime='2018-01-01T00:00:00')
 
 
-# Ignore warnings thrown when trying to load the ASDF in a different astropy
-# version to that with which it was created.
+# Ignore warnings thrown when trying to load the ASDF in a different
+# astropy version to that with which it was created.
 @pytest.mark.filterwarnings('ignore:.*was created with extension.*')
+@asdf_entry_points
 def test_hgc_100():
-    # Test that HeliographicCarrington is populated with Earth as the observer when loading a
-    # older schema (1.0.0)
+    # Test that HeliographicCarrington is populated with Earth as the
+    # observer when loading a older schema (1.0.0)
     test_file = os.path.join(os.path.dirname(__file__), "hgc_100.asdf")
     with asdf.open(test_file) as input_asdf:
         hgc = input_asdf['hgc']
         assert isinstance(hgc, frames.HeliographicCarrington)
         if hgc.obstime is None:
             assert hgc.observer == 'earth'
         else:
```

### Comparing `sunpy-5.1.1/sunpy/io/special/asdf/tests/test_genericmap.py` & `sunpy-5.1.2/sunpy/io/special/asdf/tests/test_genericmap.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     aia171_test_map._unit = u.m
     assert_roundtrip_map(aia171_test_map)
 
 
 @asdf_entry_points
 def test_load_100_file_with_shift():
     fname = get_test_filepath("aiamap_shift_genericmap_1.0.0.asdf")
-    with asdf.open(fname) as af:
+    with asdf.open(fname, copy_arrays=True) as af:
         aiamap = af['object']
         assert isinstance(aiamap, sunpy.map.sources.AIAMap)
         assert "crval1" in aiamap.meta.modified_items
         crval1 = aiamap.meta.modified_items["crval1"]
         assert crval1.current - crval1.original == 10
 
 
 @asdf_entry_points
 def test_load_100_file_with_no_shift():
     fname = get_test_filepath("aiamap_genericmap_1.0.0.asdf")
-    with asdf.open(fname) as af:
+    with asdf.open(fname, copy_arrays=True) as af:
         aiamap = af['object']
         assert isinstance(aiamap, sunpy.map.sources.AIAMap)
         assert "crval1" not in aiamap.meta.modified_items
         assert "crval2" not in aiamap.meta.modified_items
```

### Comparing `sunpy-5.1.1/sunpy/io/special/genx.py` & `sunpy-5.1.2/sunpy/io/special/genx.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/special/srs.py` & `sunpy-5.1.2/sunpy/io/special/srs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/_pyana.c` & `sunpy-5.1.2/sunpy/io/src/ana/_pyana.c`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anacompress.c` & `sunpy-5.1.2/sunpy/io/src/ana/anacompress.c`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anacompress.h` & `sunpy-5.1.2/sunpy/io/src/ana/anacompress.h`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anadecompress.c` & `sunpy-5.1.2/sunpy/io/src/ana/anadecompress.c`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anadecompress.h` & `sunpy-5.1.2/sunpy/io/src/ana/anadecompress.h`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anarw.c` & `sunpy-5.1.2/sunpy/io/src/ana/anarw.c`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/anarw.h` & `sunpy-5.1.2/sunpy/io/src/ana/anarw.h`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/src/ana/types.h` & `sunpy-5.1.2/sunpy/io/src/ana/types.h`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/generate_genx.pro` & `sunpy-5.1.2/sunpy/io/tests/generate_genx.pro`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_ana.py` & `sunpy-5.1.2/sunpy/io/tests/test_ana.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_cdf.py` & `sunpy-5.1.2/sunpy/io/tests/test_cdf.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_filetools.py` & `sunpy-5.1.2/sunpy/io/tests/test_filetools.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_fits.py` & `sunpy-5.1.2/sunpy/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_genx.py` & `sunpy-5.1.2/sunpy/io/tests/test_genx.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_jp2.py` & `sunpy-5.1.2/sunpy/io/tests/test_jp2.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,7 +40,12 @@
     outfile = tmpdir / "test.jp2"
     _jp2.write(str(outfile), data, header)
     assert outfile.exists()
 
     # Sanity check that reading back the jp2 returns coherent data
     jp2_readback = _jp2.read(outfile)
     assert header['DATE'] == jp2_readback[0].header['DATE']
+
+    # jp2 requires the data array to have type uint8, so cast the original
+    # data array to uint8 to compare it with the generated jp2 file.
+    original_data = np.uint8(data)
+    assert np.array_equal(original_data, jp2_readback[0].data)
```

### Comparing `sunpy-5.1.1/sunpy/io/tests/test_srs.py` & `sunpy-5.1.2/sunpy/io/tests/test_srs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/compositemap.py` & `sunpy-5.1.2/sunpy/map/compositemap.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/header_helper.py` & `sunpy-5.1.2/sunpy/map/header_helper.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/map_factory.py` & `sunpy-5.1.2/sunpy/map/map_factory.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/mapbase.py` & `sunpy-5.1.2/sunpy/map/mapbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,23 +50,23 @@
     add_common_docstring,
     cached_property_based_on,
     check_arithmetic_compatibility,
     deprecate_positional_args_since,
 )
 from sunpy.util.exceptions import warn_metadata, warn_user
 from sunpy.util.functools import seconddispatch
-from sunpy.util.util import _figure_to_base64
+from sunpy.util.util import _figure_to_base64, fix_duplicate_notes
 from sunpy.visualization import axis_labels_from_ctype, peek_show, wcsaxes_compat
 from sunpy.visualization.colormaps import cm as sunpy_cm
 
 TIME_FORMAT = config.get("general", "time_format")
 PixelPair = namedtuple('PixelPair', 'x y')
 SpatialPair = namedtuple('SpatialPair', 'axis1 axis2')
 
-_META_FIX_URL = 'https://docs.sunpy.org/en/stable/code_ref/map.html#fixing-map-metadata'
+_META_FIX_URL = 'https://docs.sunpy.org/en/stable/how_to/fix_map_metadata.html'
 
 # Manually specify the ``.meta`` docstring. This is assigned to the .meta
 # class attribute in GenericMap.__init__()
 _meta_doc = """
 The map metadata.
 
 This is used to interpret the map data. It may
@@ -190,15 +190,15 @@
         ``is_datasource_for`` attribute.
         This is then passed into the Map Factory so we can register them.
         """
         super().__init_subclass__(**kwargs)
         if cls.__doc__ is None:
             # Set an empty string, to prevent an error adding None to str in the next line
             cls.__doc__ = ''
-        cls.__doc__ += textwrap.indent(_notes_doc, "    ")
+        cls.__doc__ = fix_duplicate_notes(_notes_doc, cls.__doc__)
 
         if hasattr(cls, 'is_datasource_for'):
             # NOTE: This conditional is due to overlapping map sources in sunpy and pfsspy that
             # lead to a MultipleMatchError if sunpy.map and pfsspy.map are imported.
             # See https://github.com/sunpy/sunpy/issues/7294 for more information.
             if f'{cls.__module__}.{cls.__name__}' != "pfsspy.map.GongSynopticMap":
                 cls._registry[cls] = cls.is_datasource_for
@@ -1739,14 +1739,16 @@
             new_reference_pixel = np.array(new_reference_pixel).ravel()
 
         # Define the new reference_pixel
         new_meta['crval1'] = rotation_center[0].value
         new_meta['crval2'] = rotation_center[1].value
         new_meta['crpix1'] = new_reference_pixel[0] + 1  # FITS pixel origin is 1
         new_meta['crpix2'] = new_reference_pixel[1] + 1  # FITS pixel origin is 1
+        new_meta['NAXIS1'] = new_data.shape[1]
+        new_meta['NAXIS2'] = new_data.shape[0]
 
         # Unpad the array if necessary
         if unpad_x > 0:
             new_data = new_data[:, unpad_x:-unpad_x]
             new_meta['crpix1'] -= unpad_x
         if unpad_y > 0:
             new_data = new_data[unpad_y:-unpad_y, :]
```

### Comparing `sunpy-5.1.1/sunpy/map/mapsequence.py` & `sunpy-5.1.2/sunpy/map/mapsequence.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/maputils.py` & `sunpy-5.1.2/sunpy/map/maputils.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,33 +188,29 @@
     ----------
     smap : `~sunpy.map.GenericMap`
         A map in helioprojective Cartesian coordinates.
 
     Returns
     -------
     `~bool`
-        Returns `False` if any of the coordinates at the edge of the map
-         are less than one solar radius away from the center of the Sun.
+        Returns `True` if the map contains the full disk of the Sun,
+        otherwise `False`.
 
     Notes
     -----
     This function checks if the image coordinates include the solar disk.
     Therefore this function would return `True` for a coronagraph image
     such as from LASCO/C3 or STEREO/SECCHI COR1 since the solar disk is
     within the field of the view of the instrument (although no emission
     from the disk itself is present in the data.)
     """
     _verify_coordinate_helioprojective(smap.coordinate_frame)
     edge_of_world = _edge_coordinates(smap)
-    # Calculate the distance of the edge of the world in solar radii
-    coordinate_angles = np.sqrt(edge_of_world.Tx ** 2 + edge_of_world.Ty ** 2)
-
-    # Test if all the edge pixels are more than one solar radius distant
-    # and that the whole map is not all off disk.
-    return np.all(coordinate_angles > solar_angular_radius(edge_of_world)) and contains_solar_center(smap)
+    # Check that the edge pixels are all beyond the limb yet the Sun center is in the map
+    return np.all(~coordinate_is_on_solar_disk(edge_of_world)) and contains_solar_center(smap)
 
 
 def contains_solar_center(smap):
     """
     Returns `True` if smap contains the solar center.
 
     This is the case if and only if the solar center is inside or on the edges of the map.
@@ -251,51 +247,47 @@
 
     Returns
     -------
     `~bool`
         Returns `True` if the coordinate is on disk, `False` otherwise.
     """
     _verify_coordinate_helioprojective(coordinates)
-    # Calculate the angle of every pixel from the center of the Sun and compare it the angular
-    # radius of the Sun.
-    return np.sqrt(coordinates.Tx ** 2 + coordinates.Ty ** 2) < solar_angular_radius(coordinates)
+    # Calculate the radial angle from the center of the Sun (do not assume small angles)
+    # and compare it to the angular radius of the Sun
+    return np.arccos(np.cos(coordinates.Tx) * np.cos(coordinates.Ty)) <= solar_angular_radius(coordinates)
 
 
 def is_all_off_disk(smap):
     """
     Checks if none of the coordinates in the `~sunpy.map.GenericMap` are on the solar disk.
 
-    This is done by checking if the edges of the map do not contain the solar limb, and
+    This is done by checking if the edges of the map are all beyond the solar limb, and
     checking that the solar center is not in the map.
 
     Parameters
     ----------
     smap : `~sunpy.map.GenericMap`
         A map in helioprojective Cartesian coordinates.
 
     Returns
     -------
     `~bool`
-        Returns `True` if all map pixels have an angular radius greater than
-        the angular radius of the Sun.
+        Returns `True` if the map does not contain any part of the disk of the
+        Sun, otherwise `False`.
 
     Notes
     -----
     For coronagraph images such as those from LASCO C2 and C3 the full disk is
-    within the field of view of the instrument, but the solar disk itself is not imaged.
-    For such images this function will return `False`.
+    within the field of view of the instrument, even though the solar disk
+    itself is not imaged.  For such images this function will return `False`.
     """
     _verify_coordinate_helioprojective(smap.coordinate_frame)
     edge_of_world = _edge_coordinates(smap)
-    # Calculate the distance of the edge of the world in solar radii
-    coordinate_angles = np.sqrt(edge_of_world.Tx ** 2 + edge_of_world.Ty ** 2)
-
-    # Test if all the edge pixels are more than one solar radius distant
-    # and that the solar center is
-    return np.all(coordinate_angles > solar_angular_radius(edge_of_world)) and ~contains_solar_center(smap)
+    # Check that the edge pixels are all beyond the limb and the Sun center is not in the map
+    return np.all(~coordinate_is_on_solar_disk(edge_of_world)) and ~contains_solar_center(smap)
 
 
 def is_all_on_disk(smap):
     """
     Checks if all of the coordinates in the `~sunpy.map.GenericMap` are on the solar disk.
 
     The check is performed by calculating the angle of the edges of the map from
```

### Comparing `sunpy-5.1.1/sunpy/map/sources/__init__.py` & `sunpy-5.1.2/sunpy/map/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/gong.py` & `sunpy-5.1.2/sunpy/map/sources/gong.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/hinode.py` & `sunpy-5.1.2/sunpy/map/sources/hinode.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/iris.py` & `sunpy-5.1.2/sunpy/map/sources/iris.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/mlso.py` & `sunpy-5.1.2/sunpy/map/sources/mlso.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     and dynamics of coronal mass ejections and the evolution of the density structure of
     the low corona. The K-Cor records the polarization brightness (pB) formed by Thomson scattering
     of photospheric light by coronal free electrons. The National Center for Atmospheric
     Research (NCAR), via the National Science Foundation (NSF), provided full funding for the
     COSMO K-Cor, which was deployed to the Mauna Loa Solar Observatory (MLSO) in Hawaii in
     September 2013, replacing the aging MLSO Mk4 K-coronameter.
 
-    References
-    ----------
-    * `COSMO Mission Page <https://www2.hao.ucar.edu/cosmo>`_
-    * `KCOR Instrument Page <https://www2.hao.ucar.edu/mlso/instruments/mlso-kcor-coronagraph>`_
-
     Notes
     -----
     Observer location: The standard K-Cor metadata does not include the full 3D
     location of the observer.  There are 2D Carrington heliographic coordinates, but
     using them is not recommended because the calculation of Carrington longitude
     differs from ``sunpy`` (see :ref:`sunpy-topic-guide-coordinates-carrington`).
     Instead, we assume the default observer location to be the geographic location of MLSO.
+
+    References
+    ----------
+    * `COSMO Mission Page <https://www2.hao.ucar.edu/cosmo>`_
+    * `KCOR Instrument Page <https://www2.hao.ucar.edu/mlso/instruments/mlso-kcor-coronagraph>`_
     """
 
     # MLSO location per Wikipedia (https://en.wikipedia.org/wiki/Mauna_Loa_Solar_Observatory)
     _earth_location = EarthLocation(-155.576*u.deg, 19.536*u.deg, 3394*u.m)
 
     def __init__(self, data, header, **kwargs):
         super().__init__(data, header, **kwargs)
```

### Comparing `sunpy-5.1.1/sunpy/map/sources/proba2.py` & `sunpy-5.1.2/sunpy/map/sources/proba2.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/psp.py` & `sunpy-5.1.2/sunpy/map/sources/psp.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/rhessi.py` & `sunpy-5.1.2/sunpy/map/sources/rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/sdo.py` & `sunpy-5.1.2/sunpy/map/sources/sdo.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/soho.py` & `sunpy-5.1.2/sunpy/map/sources/soho.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/solo.py` & `sunpy-5.1.2/sunpy/map/sources/solo.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/source_type.py` & `sunpy-5.1.2/sunpy/map/sources/source_type.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/stereo.py` & `sunpy-5.1.2/sunpy/map/sources/stereo.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/suvi.py` & `sunpy-5.1.2/sunpy/map/sources/suvi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_aia_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_aia_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_cor_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_cor_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_eit_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_eit_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_eui_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_eui_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_euvi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_euvi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_gong_synoptic_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_gong_synoptic_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_hi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_hi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_hmi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_hmi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_hmi_synoptic_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_hmi_synoptic_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_iris_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_iris_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_kcor_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_kcor_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_lasco_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_lasco_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_mdi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_mdi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_rhessi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_rhessi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_sot_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_sot_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_source_type.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_source_type.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_suvi_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_suvi_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_swap_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_swap_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_sxt_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_sxt_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_trace_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_trace_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_wispr_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_wispr_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/tests/test_xrt_source.py` & `sunpy-5.1.2/sunpy/map/sources/tests/test_xrt_source.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/trace.py` & `sunpy-5.1.2/sunpy/map/sources/trace.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/sources/yohkoh.py` & `sunpy-5.1.2/sunpy/map/sources/yohkoh.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/conftest.py` & `sunpy-5.1.2/sunpy/map/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/strategies.py` & `sunpy-5.1.2/sunpy/map/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_compositemap.py` & `sunpy-5.1.2/sunpy/map/tests/test_compositemap.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_header.py` & `sunpy-5.1.2/sunpy/map/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_header_helper.py` & `sunpy-5.1.2/sunpy/map/tests/test_header_helper.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_map_factory.py` & `sunpy-5.1.2/sunpy/map/tests/test_map_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from astropy.io import fits
 from astropy.wcs import WCS
 
 import sunpy
 import sunpy.map
 from sunpy.data.test import get_dummy_map_from_header, get_test_data_filenames, get_test_filepath, rootdir
 from sunpy.tests.helpers import figure_test, skip_glymur
-from sunpy.util.exceptions import NoMapsInFileError, SunpyMetadataWarning, SunpyUserWarning
+from sunpy.util.exceptions import (
+    NoMapsInFileError,
+    SunpyDeprecationWarning,
+    SunpyMetadataWarning,
+    SunpyUserWarning,
+)
 
 a_list_of_many = [f for f in get_test_data_filenames() if 'efz' in f.name]
 
 AIA_171_IMAGE = get_test_filepath('aia_171_level1.fits')
 RHESSI_IMAGE = get_test_filepath('hsi_image_20101016_191218.fits')
 AIA_193_JP2 = get_test_filepath("2013_06_24__17_31_30_84__SDO_AIA_AIA_193.jp2")
 HMI_LOS_JP2 = get_test_filepath("2023_01_31__03_39_23_200__SDO_HMI_HMI_continuum.jp2")
@@ -150,26 +155,26 @@
     assert isinstance(pair_map, sunpy.map.GenericMap)
 
     # Custom Map
     data = np.arange(0, 100).reshape(10, 10)
     header = {'cdelt1': 10, 'cdelt2': 10,
               'telescop': 'sunpy',
               'cunit1': 'arcsec', 'cunit2': 'arcsec'}
-    with pytest.warns(SunpyMetadataWarning, match='Missing CTYPE1 from metadata, assuming CTYPE1 is HPLN-TAN'):
+    with pytest.warns(SunpyMetadataWarning, match='Missing CTYPE'):
         pair_map = sunpy.map.Map(data, header)
     assert isinstance(pair_map, sunpy.map.GenericMap)
 
     # Common keys not strings
     data = np.arange(0, 100).reshape(10, 10)
     header = {'cdelt1': 10, 'cdelt2': 10,
               'telescop': 100,
               'detector': 1,
               'instrume': 50,
               'cunit1': 'arcsec', 'cunit2': 'arcsec'}
-    with pytest.warns(SunpyMetadataWarning, match='Missing CTYPE1 from metadata, assuming CTYPE1 is HPLN-TAN'):
+    with pytest.warns(SunpyMetadataWarning, match='Missing CTYPE'):
         pair_map = sunpy.map.Map(data, header)
     assert isinstance(pair_map, sunpy.map.GenericMap)
 
 
 def test_errors(tmpdir):
     # If directory doesn't exist, make sure it's listed in the error msg
     nonexist_dir = 'nonexist'
@@ -272,32 +277,30 @@
     [RHESSI_IMAGE, sunpy.map.sources.RHESSIMap],
     ["FGMG4_20110214_030443.7.header", sunpy.map.sources.SOTMap],
     ["swap_lv1_20140606_000113.header", sunpy.map.sources.SWAPMap],
     ["HinodeXRT.header", sunpy.map.sources.XRTMap],
 ])
 def test_sources(file, mapcls):
     p = pathlib.Path(get_test_filepath(file))
-    if p.suffix == '.header':
-        m = get_dummy_map_from_header(p)
-    else:
-        m = sunpy.map.Map(p)
+    m = get_dummy_map_from_header(p) if p.suffix == '.header' else sunpy.map.Map(p)
     assert isinstance(m, mapcls)
 
-
+@pytest.mark.skipif(pytest.__version__ < "8.0.0", reason="pytest >= 8.0.0 raises a warning for this test")
 def test_no_2d_hdus(tmpdir):
     # Create a fake FITS file with a valid header but 1D data
     tmp_fpath = str(tmpdir / 'data.fits')
     with fits.open(AIA_171_IMAGE, ignore_blank=True) as hdul:
         fits.writeto(tmp_fpath, np.arange(100), hdul[0].header)
 
     with pytest.raises(NoMapsInFileError, match='Found no HDUs with >= 2D data'):
         sunpy.map.Map(tmp_fpath)
 
     with pytest.warns(SunpyUserWarning, match='One of the arguments failed to parse'):
-        sunpy.map.Map([tmp_fpath, AIA_171_IMAGE], silence_errors=True)
+        with pytest.warns(SunpyDeprecationWarning, match='"silence_errors" was deprecated in version 5.1 and will be removed in a future version'):
+            sunpy.map.Map([tmp_fpath, AIA_171_IMAGE], silence_errors=True)
 
 
 @skip_glymur
 def test_map_jp2_AIA():
     jp2_map = sunpy.map.Map(AIA_193_JP2, memmap=False)
     assert isinstance(jp2_map, sunpy.map.GenericMap)
     # The base of an array that owns its memory is None
```

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_mapbase.py` & `sunpy-5.1.2/sunpy/map/tests/test_mapbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,116 @@
 from sunpy.map.mapbase import GenericMap
 from sunpy.map.sources import AIAMap
 from sunpy.tests.helpers import figure_test
 from sunpy.time import parse_time
 from sunpy.util import SunpyUserWarning
 from sunpy.util.exceptions import SunpyMetadataWarning
 from sunpy.util.metadata import ModifiedItem
+from sunpy.util.util import fix_duplicate_notes
 from .conftest import make_simple_map
 from .strategies import matrix_meta
 
 
+def test_notes_combined():
+    map_documentation = """
+    Class Info.
+
+    Notes
+    -----
+    This is a note.
+
+    References
+    ----------
+    This is reference.
+    """
+    extra_note_section= """\nNotes\n-----\nThis should be combined."""
+    updated_documentation= fix_duplicate_notes(extra_note_section, map_documentation)
+    expected_result = """
+    Class Info.
+
+    Notes
+    -----
+    This is a note.
+
+    This should be combined.
+
+    References
+    ----------
+    This is reference.
+    """
+    assert updated_documentation == expected_result
+
+def test_notes_combined_no_references():
+    map_documentation = """
+    Class Info.
+
+    Notes
+    -----
+    This is a note.
+    """
+    extra_note_section= """\nNotes\n-----\nThis should be combined."""
+    updated_documentation= fix_duplicate_notes(extra_note_section, map_documentation)
+    updated_documentation2=updated_documentation.replace("\n    \n    ","\n\n    ")
+    expected_result = """
+    Class Info.
+
+    Notes
+    -----
+    This is a note.
+
+    This should be combined.
+    """
+    assert updated_documentation2.strip() == expected_result.strip()
+
+def test_notes_combined_no_existing_notes():
+    map_documentation = """
+    Class Info.
+
+    References
+    ----------
+    This is reference.
+    """
+    extra_note_section= """\nNotes\n-----\nThis should be combined."""
+    updated_documentation= fix_duplicate_notes(extra_note_section, map_documentation)
+    expected_result = """
+    Class Info.
+
+    Notes
+    -----
+    This should be combined.
+
+    References
+    ----------
+    This is reference.
+    """
+    assert updated_documentation == expected_result
+
+def test_notes_combined_no_notes_no_references():
+    map_documentation = """
+    Class Info.
+    """
+    extra_note_section= """\nNotes\n-----\nThis should be combined."""
+    updated_documentation= fix_duplicate_notes(extra_note_section, map_documentation)
+    updated_documentation2=updated_documentation.replace("\n    \n    ","\n\n    ")
+    expected_result = """
+    Class Info.
+
+    Notes
+    -----
+    This should be combined.
+    """
+    assert updated_documentation2.strip() == expected_result.strip()
+
+
 def test_fits_data_comparison(aia171_test_map):
     """Make sure the data is the same when read with astropy.io.fits and sunpy"""
     with pytest.warns(VerifyWarning, match="Invalid 'BLANK' keyword in header."):
-        data = fits.open(get_test_filepath('aia_171_level1.fits'))[0].data
-    np.testing.assert_allclose(aia171_test_map.data, data)
+        hdulist = fits.open(get_test_filepath('aia_171_level1.fits'))
+    np.testing.assert_allclose(aia171_test_map.data, hdulist[0].data)
+    hdulist.close()
 
 
 def test_header_fits_io():
     with pytest.warns(VerifyWarning, match="Invalid 'BLANK' keyword in header."):
         with fits.open(get_test_filepath('aia_171_level1.fits')) as hdu:
             AIAMap(hdu[0].data, hdu[0].header)
 
@@ -1177,17 +1270,14 @@
     generic_map.meta['cunit2'] = 'Angstrom'
     err_msg = ("Map only supports spherical coordinate systems with angular units "
                "(ie. equivalent to arcsec), but this map has units ['arcsec', 'Angstrom']")
     with pytest.raises(sunpy.map.MapMetaValidationError, match=re.escape(err_msg)):
         sunpy.map.Map(generic_map.data, generic_map.meta)
 
 
-# Heliographic Map Tests
-
-
 def test_hg_coord(heliographic_test_map):
     assert heliographic_test_map.coordinate_system[0] == "CRLN-CAR"
     assert heliographic_test_map.coordinate_system[1] == "CRLT-CAR"
     assert isinstance(heliographic_test_map.coordinate_frame,
                       sunpy.coordinates.HeliographicCarrington)
 
 
@@ -1202,42 +1292,45 @@
 def test_hg_data_to_pix(heliographic_test_map):
     out = heliographic_test_map.world_to_pixel(
         SkyCoord(
             0 * u.deg, 0 * u.deg, frame=heliographic_test_map.coordinate_frame))
     assert_quantity_allclose(out[0], 180 * u.pix)
     assert_quantity_allclose(out[1], 90 * u.pix)
 
-# Dimension testing
-
 
+@pytest.mark.skipif(pytest.__version__ < "8.0.0", reason="pytest >= 8.0.0 raises two warnings for this test")
 def test_more_than_two_dimensions():
-    """Checks to see if an appropriate error is raised when a FITS with more than two dimensions is
-    loaded.  We need to load a >2-dim dataset with a TELESCOP header"""
+    """
+    Checks to see if an appropriate error is raised when a FITS with more than two dimensions is
+    loaded.  We need to load a >2-dim dataset with a TELESCOP header
+    """
 
     # Data crudely represents 4 stokes, 4 wavelengths with Y,X of 3 and 5.
     bad_data = np.random.rand(4, 4, 3, 5)
     hdr = fits.Header()
     hdr['TELESCOP'] = 'XXX'
     hdr['cunit1'] = 'arcsec'
     hdr['cunit2'] = 'arcsec'
-    with pytest.warns(SunpyUserWarning, match='This file contains more than 2 dimensions.'):
-        bad_map = sunpy.map.Map(bad_data, hdr)
+    with pytest.warns(SunpyMetadataWarning, match='Missing CTYPE'):
+        with pytest.warns(SunpyUserWarning, match='This file contains more than 2 dimensions.'):
+            bad_map = sunpy.map.Map(bad_data, hdr)
     # Test fails if map.ndim > 2 and if the dimensions of the array are wrong.
     assert bad_map.ndim == 2
     assert_quantity_allclose(bad_map.dimensions, (5, 3) * u.pix)
 
 
 def test_missing_metadata_warnings():
     # Checks that warnings for missing metadata are only raised once
     with pytest.warns(Warning) as record:
-        header = {}
-        header['cunit1'] = 'arcsec'
-        header['cunit2'] = 'arcsec'
-        header['ctype1'] = 'HPLN-TAN'
-        header['ctype2'] = 'HPLT-TAN'
+        header = {
+            'cunit1': 'arcsec',
+            'cunit2': 'arcsec',
+            'ctype1': 'HPLN-TAN',
+            'ctype2': 'HPLT-TAN',
+        }
         array_map = sunpy.map.Map(np.random.rand(20, 15), header)
         array_map.peek()
     # There should be 2 warnings for missing metadata (obstime and observer location)
     assert len([w for w in record if w.category in (SunpyMetadataWarning, SunpyUserWarning)]) == 2
 
 
 def test_fits_header(aia171_test_map):
@@ -1257,14 +1350,21 @@
               'cunit2': 'arcsec',
               None: None,  # Cannot parse this into WCS
               }
     with pytest.raises(ValueError, match='All MetaDict keys must be strings'):
         sunpy.map.GenericMap(np.zeros((10, 10)), header)
 
 
+def test_updating_of_naxisi_on_rotate(aia171_test_map):
+    aia171_test_map_rotated = aia171_test_map.rotate(45 * u.deg, missing=0)
+    assert aia171_test_map.data.shape == (128, 128)
+    assert aia171_test_map_rotated.meta['NAXIS1'] == 182
+    assert aia171_test_map_rotated.meta['NAXIS2'] == 182
+
+
 def test_wcs_isot(aia171_test_map):
     # Check that a Map WCS returns the time as isot format
     assert aia171_test_map.wcs.to_header()['DATE-OBS'] == '2011-02-15T00:00:00.340'
 
 
 def test_repr_html(aia171_test_map):
     html_string = aia171_test_map._repr_html_()
@@ -1490,15 +1590,15 @@
     assert aiamap.meta.modified_items == {'cdelt1': ModifiedItem(old_cdelt1, 20)}
 
     # Check that rotate doesn't modify the original metadata
     aiamap_rot = aiamap.rotate(30 * u.deg)
     assert aiamap_rot.meta.original_meta == aiamap.meta.original_meta
     assert set(aiamap_rot.meta.added_items.keys()) == set(['pc1_1', 'pc1_2', 'pc2_1', 'pc2_2'])
     assert set(aiamap_rot.meta.removed_items.keys()) == set(['crota2'])
-    assert set(aiamap_rot.meta.modified_items) == set(['cdelt1', 'crpix1', 'crpix2', 'crval1'])
+    assert set(aiamap_rot.meta.modified_items) == set(['cdelt1', 'crpix1', 'crpix2', 'crval1', 'naxis1', 'naxis2'])
 
 
 def test_no_wcs_observer_info(heliographic_test_map):
     # Check that HeliographicCarrington WCS has observer info set
     assert isinstance(heliographic_test_map.coordinate_frame, HeliographicCarrington)
     wcs_aux = heliographic_test_map.wcs.wcs.aux
     assert wcs_aux.hgln_obs is not None
```

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_mapbase_dask.py` & `sunpy-5.1.2/sunpy/map/tests/test_mapbase_dask.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 import numpy as np
 import pytest
 
 import astropy.units as u
 import astropy.wcs
 from astropy.io import fits
 from astropy.io.fits.verify import VerifyWarning
+from astropy.wcs import FITSFixedWarning
 
 import sunpy.map
 from sunpy.data.test import get_test_filepath
 
 
 @pytest.fixture
 def aia171_test_dask_map(aia171_test_map):
     dask_array = pytest.importorskip('dask.array')
     return aia171_test_map._new_instance(
         dask_array.from_array(aia171_test_map.data),
         copy.deepcopy(aia171_test_map.meta)
     )
 
 
-def test_dask_array(aia171_test_dask_map):
+def test_dask_array_repr(aia171_test_dask_map):
     # Check that _repr_html_ functions for a dask array
     html_dask_repr = aia171_test_dask_map._repr_html_(compute_dask=False)
     html_computed_repr = aia171_test_dask_map._repr_html_(compute_dask=True)
     assert html_dask_repr != html_computed_repr
 
 
 # This is needed for the reproject_to function
 with pytest.warns(VerifyWarning, match="Invalid 'BLANK' keyword in header."):
     with fits.open(get_test_filepath('aia_171_level1.fits')) as hdu:
-        aia_wcs = astropy.wcs.WCS(header=hdu[0].header)
+        with pytest.warns(FITSFixedWarning, match="'datfix' made the change"):
+            aia_wcs = astropy.wcs.WCS(header=hdu[0].header)
 
 
 @pytest.mark.parametrize(("func", "args"), [
     ("max", {}),
     ("mean", {}),
     ("min", {}),
     pytest.param("reproject_to", {"wcs": aia_wcs}, marks=pytest.mark.xfail(reason="reproject is not dask aware")),
```

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_mapsequence.py` & `sunpy-5.1.2/sunpy/map/tests/test_mapsequence.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_maputils.py` & `sunpy-5.1.2/sunpy/map/tests/test_maputils.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_plotting.py` & `sunpy-5.1.2/sunpy/map/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/map/tests/test_reproject_to.py` & `sunpy-5.1.2/sunpy/map/tests/test_reproject_to.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/_attrs.py` & `sunpy-5.1.2/sunpy/net/_attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/attr.py` & `sunpy-5.1.2/sunpy/net/attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/attrs.py` & `sunpy-5.1.2/sunpy/net/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/base_client.py` & `sunpy-5.1.2/sunpy/net/base_client.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/cdaweb/cdaweb.py` & `sunpy-5.1.2/sunpy/net/cdaweb/cdaweb.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/cdaweb/data/attrs.json` & `sunpy-5.1.2/sunpy/net/cdaweb/data/attrs.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/cdaweb/helpers.py` & `sunpy-5.1.2/sunpy/net/cdaweb/helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/cdaweb/test/test_cdaweb.py` & `sunpy-5.1.2/sunpy/net/cdaweb/test/test_cdaweb.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/cdaweb/walker.py` & `sunpy-5.1.2/sunpy/net/cdaweb/walker.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/__init__.py` & `sunpy-5.1.2/sunpy/net/dataretriever/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/client.py` & `sunpy-5.1.2/sunpy/net/dataretriever/client.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/eve.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/fermi_gbm.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/goes.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/goes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/gong.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/gong.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/lyra.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/lyra.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/noaa.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/norh.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/rhessi.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_eve.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_goes_suvi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_goes_ud.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_goes_ud.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_gong_synoptic.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_lyra_ud.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_noaa.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_norh.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/sources/tests/test_rhessi.py` & `sunpy-5.1.2/sunpy/net/dataretriever/sources/tests/test_rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/dataretriever/tests/test_client.py` & `sunpy-5.1.2/sunpy/net/dataretriever/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/fido_factory.py` & `sunpy-5.1.2/sunpy/net/fido_factory.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/hek/attrs.py` & `sunpy-5.1.2/sunpy/net/hek/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/hek/hek.py` & `sunpy-5.1.2/sunpy/net/hek/hek.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/hek/tests/test_hek.py` & `sunpy-5.1.2/sunpy/net/hek/tests/test_hek.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/hek2vso/hek2vso.py` & `sunpy-5.1.2/sunpy/net/hek2vso/hek2vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/hek2vso/tests/test_hek2vso.py` & `sunpy-5.1.2/sunpy/net/hek2vso/tests/test_hek2vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/helio/chaincode.py` & `sunpy-5.1.2/sunpy/net/helio/chaincode.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/helio/hec.py` & `sunpy-5.1.2/sunpy/net/helio/hec.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 Access the Helio Event Catalogue
 """
 import io
 import os
 
 from lxml import etree
 from requests import Session
+from requests.exceptions import SSLError
 from zeep import Client
 from zeep.transports import Transport
 
 from astropy.io.votable.table import parse_single_table
 
+from sunpy import log
 from sunpy.net import attrs as a
 from sunpy.net.base_client import BaseClient, QueryResponseTable
 from sunpy.net.helio import attrs as ha
 from sunpy.net.helio import parser
 from sunpy.time import parse_time
 from sunpy.util.exceptions import warn_user
 
@@ -83,15 +85,20 @@
         if link is None:
             # The default wsdl file
             link = parser.wsdl_retriever()
         session = Session()
         # This is for use in our test suite.
         session.verify = not (bool(os.environ.get("NO_VERIFY_HELIO_SSL", 0)))
         transport = Transport(session=session)
-        self.hec_client = Client(link, transport=transport)
+        try:
+            self.hec_client = Client(link, transport=transport)
+        except SSLError:
+            log.warning('SSL verification error for HEC client.\n'
+                     'Set the \'NO_VERIFY_HELIO_SSL\' environment variable disable SSL verification for Helio.')
+            self.hec_client = None
 
     @classmethod
     def _can_handle_query(cls, *query):
         required = {a.Time}
         optional = {ha.MaxRecords, ha.TableName}
         return cls.check_attr_types_in_query(query, required, optional)
 
@@ -133,14 +140,17 @@
          31469 2005-01-03T08:27:56 2005-01-03T08:28:26 ...          6      5010334
          31470 2005-01-03T09:31:00 2005-01-03T09:33:34 ...          6      5010322
          31471 2005-01-03T09:34:52 2005-01-03T09:59:46 ...          6      5010336
          31472 2005-01-03T11:06:48 2005-01-03T11:07:18 ...         12      5010304
         <BLANKLINE>
         <BLANKLINE>
         """
+        if self.hec_client is None:
+            table = HECResponse([], client=self)
+            return table
         qrdict = {}
         for elem in args:
             if isinstance(elem, a.Time):
                 qrdict['Time'] = elem
             elif isinstance(elem, ha.MaxRecords):
                 qrdict['max_records'] = elem.value
             elif isinstance(elem, ha.TableName):
```

### Comparing `sunpy-5.1.1/sunpy/net/helio/parser.py` & `sunpy-5.1.2/sunpy/net/helio/parser.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/helio/tests/test_chaincode.py` & `sunpy-5.1.2/sunpy/net/helio/tests/test_chaincode.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/helio/tests/test_helio.py` & `sunpy-5.1.2/sunpy/net/helio/tests/test_helio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import urllib
 from unittest import mock
 
 import pytest
+from requests.exceptions import SSLError
 
 from sunpy.net import attrs as a
 from sunpy.net.helio.hec import HECClient
 from sunpy.net.helio.parser import (
     endpoint_parser,
     link_test,
     taverna_parser,
@@ -243,14 +244,24 @@
     """
     If `link_test` internally raises `URLError`, ensure it
     returns `None`
     """
     link_test('') is None
 
 
+@mock.patch('sunpy.net.helio.parser.webservice_parser', return_value=wsdl_urls())
+@mock.patch('sunpy.net.helio.parser.taverna_parser', return_value=some_taverna_urls())
+@mock.patch('sunpy.net.helio.parser.link_test', return_value='some text read')
+@mock.patch('sunpy.net.helio.hec.Client', side_effect=SSLError('SSL error'))
+def test_ssl_verify_error(mock_webservice, mock_taverna, mock_link, mock_zeep, caplog):
+    client = HECClient()
+    query = client.search(a.Time('2023/02/03', '2023/02/03'))
+    assert len(query) == 0
+    assert "Set the 'NO_VERIFY_HELIO_SSL' environment variable disable SSL verification for Helio." in caplog.text
+
 @pytest.fixture(scope="session")
 def client():
     try:
         client = HECClient()
         return client
     # If no links are found, the client should raise a ValueError
     except ValueError:
```

### Comparing `sunpy-5.1.1/sunpy/net/helioviewer.py` & `sunpy-5.1.2/sunpy/net/helioviewer.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/jsoc/attrs.py` & `sunpy-5.1.2/sunpy/net/jsoc/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/jsoc/data/attrs.json` & `sunpy-5.1.2/sunpy/net/jsoc/data/attrs.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/jsoc/jsoc.py` & `sunpy-5.1.2/sunpy/net/jsoc/jsoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,19 +296,20 @@
             2014-01-01T00:01:01Z  SDO/AIA    AIA_3      171    2145
 
         """
         return_results = JSOCResponse(client=self)
         query = and_(*query)
         blocks = []
         for block in walker.create(query):
-            iargs = kwargs.copy()
-            iargs.update(block)
-            # Update blocks with deep copy of iargs because in _make_recordset we use .pop() on element from iargs
-            blocks.append(copy.deepcopy(iargs))
-            return_results = astropy.table.vstack([return_results, self._lookup_records(iargs)])
+            extra_kwargs = kwargs.copy()
+            extra_kwargs |= block
+            # Update blocks with deep copy of extra_kwargs because in _make_recordset we use .pop() on
+            # element from extra_kwargs
+            blocks.append(copy.deepcopy(extra_kwargs))
+            return_results = astropy.table.vstack([return_results, self._lookup_records(extra_kwargs)])
         return_results.query_args = blocks
         return_results._original_num_rows = len(return_results)
         return return_results
 
     def request_data(self, jsoc_response, method='url', **kwargs):
         """
         Request that JSOC stages the data for download. This method will not
@@ -331,42 +332,38 @@
                    a list of  `~drms.client.ExportRequest` objects
             Request Id can be accessed by requests.id
             Request status can be accessed by requests.status
         """
 
         requests = []
         self.query_args = jsoc_response.query_args
-        supported_protocols = {'fits', 'as-is'}
-        supported_methods = {'url-tar', 'url', 'url-quick'}
+        supported_protocols = sorted(['fits', 'as-is'])
+        supported_methods = sorted(['url-tar', 'url', 'url-quick'])
         for block in jsoc_response.query_args:
 
             ds = self._make_recordset(**block)
             cd = drms.Client(email=block.get('notify', ''))
             protocol = block.get('protocol', 'fits')
             cutout = block.get('cutout')
 
             if protocol not in supported_protocols:
-                error_message = f"Protocols other than {','.join(supported_protocols)} "\
-                                "are not supported."
+                error_message = f"Protocols other than {','.join(supported_protocols)} are not supported."
                 raise TypeError(error_message)
             if method not in supported_methods:
-                error_message = f"Methods other than {','.join(supported_methods)} "\
-                                "are not supported."
+                error_message = f"Methods other than {','.join(supported_methods)}  are not supported."
                 raise TypeError(error_message)
             process = {'im_patch': cutout} if cutout is not None else None
 
             if method != 'url-tar':
                 method = 'url' if protocol == 'fits' else 'url_quick'
             r = cd.export(ds, method=method, protocol=protocol, process=process)
 
             requests.append(r)
 
-        if len(requests) == 1:
-            return requests[0]
-        return requests
+        return requests[0] if len(requests) == 1 else requests
 
     @convert_row_to_table
     def fetch(self, jsoc_response, path=None, progress=True, overwrite=False,
               downloader=None, wait=True, sleep=10, max_conn=default_max_conn, **kwargs):
         """
         Make the request for the data in a JSOC response and wait for it to be
         staged and then download the data.
@@ -422,23 +419,21 @@
             warn_user("Downloading of sliced JSOC results is not supported. "
                       "All the files present in the original response will "
                       "be downloaded when passed to fetch().")
 
         # Make staging request to JSOC
         responses = self.request_data(jsoc_response)
 
-        defaults = {'max_splits': 1}
-        defaults.update(kwargs)
-
+        defaults = {'max_splits': 1} | kwargs
         # Make response iterable
         if not isiterable(responses):
             responses = [responses]
 
         # Add them to the response for good measure
-        jsoc_response.requests = [r for r in responses]
+        jsoc_response.requests = list(responses)
         time.sleep(sleep/2.)
 
         for response in responses:
             response.wait(verbose=progress)
 
         return self.get_request(responses, path=path, overwrite=overwrite,
                                 progress=progress, downloader=downloader,
@@ -625,15 +620,15 @@
         if sample:
             sample = f'@{sample}s'
         # Populate primekeys dict with Time and Wavelength values
         if start_time and end_time:
             # Check whether any primekey listed in PRIMEKEY_LIST_TIME has been passed through
             # PrimeKey() attribute. If yes, raise an error, since Time can only be passed
             # either through PrimeKey() attribute or Time() attribute.
-            if not any(x in PRIMEKEY_LIST_TIME for x in primekey):
+            if all(x not in PRIMEKEY_LIST_TIME for x in primekey):
                 timestr = '{start}-{end}{sample}'.format(
                     start=start_time.tai.strftime("%Y.%m.%d_%H:%M:%S_TAI"),
                     end=end_time.tai.strftime("%Y.%m.%d_%H:%M:%S_TAI"),
                     sample=sample)
             else:
                 error_message = ("Time attribute has been passed both as a Time()"
                                  " and PrimeKey(). Please provide any one of them"
@@ -647,101 +642,87 @@
             # but it is a good idea to keep a check.
             match = set(primekey.keys()) & PRIMEKEY_LIST_TIME
             if len(match) > 1:
                 error_message = ("Querying of series, having more than 1 Time-type "
                                  "prime-keys is not yet supported. Alternative is to "
                                  "use only one of the primekey to query for series data.")
                 raise ValueError(error_message)
-            if match:
-                timestr = '{}'.format(primekey.pop(list(match)[0], ''))
-            else:
-                timestr = ''
-        if wavelength != '':
-            if not primekey.get('WAVELNTH', ''):
-                if isinstance(wavelength, list):
-                    wavelength = [int(np.ceil(wave.to(u.AA).value)) for wave in wavelength]
-                    wavelength = str(wavelength)
-                else:
-                    wavelength = f'{int(np.ceil(wavelength.to(u.AA).value))}'
-            else:
-                # This is executed when wavelength has been passed both through PrimeKey()
-                # and Wavelength().
-                error_message = ("Wavelength attribute has been passed both as a Wavelength()"
-                                 " and PrimeKey(). Please provide any one of them"
-                                 " or separate them by OR operator.")
-                raise ValueError(error_message)
-        else:
+            timestr = f"{primekey.pop(list(match)[0], '')}" if match else ''
+        if wavelength == '':
             # This is executed when wavelength has been passed through PrimeKey().
-            wavelength = '{}'.format(primekey.pop('WAVELNTH', ''))
+            wavelength = f"{primekey.pop('WAVELNTH', '')}"
+        elif not primekey.get('WAVELNTH'):
+            wavelength = f'{int(np.ceil(wavelength.to_value(u.AA)))}'
+        else:
+            # This is executed when wavelength has been passed both through PrimeKey()
+            # and Wavelength().
+            error_message = ("Wavelength attribute has been passed both as a Wavelength()"
+                             " and PrimeKey(). Please provide any one of them"
+                             " or separate them by OR operator.")
+            raise ValueError(error_message)
         # Populate primekey dict with formatted Time and Wavlength.
         if timestr:
             primekey['TIME'] = timestr
         if wavelength != '':
             primekey['WAVELNTH'] = wavelength
         # Extract and format primekeys
         primekey_string = ''
         c = drms.Client()
         si = c.info(series)
         primekeys_istime = si.keywords.loc[si.primekeys].is_time
         for pkey in primekeys_istime.index.values:
-            # The loop is iterating over the list of prime-keys existing for the given series.
-            if len(primekey) > 0:
-                if primekeys_istime[pkey]:
-                    primekey_string += '[{}]'.format(primekey.pop('TIME', ''))
-                else:
-                    primekey_string += '[{}]'.format(primekey.pop(pkey, ''))
-            else:
+            if len(primekey) <= 0:
                 break
-                # break because we can skip adding {} at the end of primekey_string, if the primekey
-                # dict is empty.
+            if primekeys_istime[pkey]:
+                primekey_string += f"[{primekey.pop('TIME', '')}]"
+            else:
+                primekey_string += f"[{primekey.pop(pkey, '')}]"
         if not primekey_string:
             # primekey_string cannot be totally empty
             #
             # Note that whilst it is technically possible to just search by series,
             # this is not allowed here, because some of these would be very large
-            # searches that would make JSOC sad
+            # searches that would make JSOC unhappy with sunpy
             raise ValueError("Time, Wavelength or an explicit PrimeKey must be specified.")
         keys = []
         keyword_info = c.keys(series)
         for key, value in keyword.items():
-            if key in keyword_info:
-                keys.append(f"{key}{value['operator']}{value['value']}")
-            else:
+            if key not in keyword_info:
                 raise ValueError(f"Keyword: '{key}' is not supported by series: {series}")
+            # We have to ensure that any input values that are strings are quoted
+            keys.append(f"{key}{value['operator']}'{value['value']}'")
         keyword_string = f"[? {' AND '.join(keys)} ?]" if keys else ""
         return f"{series}{primekey_string}{keyword_string}{segment}"
 
     def _lookup_records(self, iargs):
         """
         Do a LookData request to JSOC to workout what results the query returns.
         """
-        isMeta = iargs.get('meta', False)
+        is_meta = iargs.get('meta', False)
         keywords = iargs.get('keys', '**ALL**')
         client = drms.Client()
         if 'series' not in iargs:
             error_message = "Series must be specified for a JSOC Query"
             raise ValueError(error_message)
         if not isinstance(keywords, list) and not isinstance(keywords, str):
             error_message = "Keywords can only be passed as a list or comma-separated strings."
             raise TypeError(error_message)
         # Get a set of the PrimeKeys that exist for the given series, and check
         # whether the passed PrimeKeys is a subset of that.
         primekeys = client.pkeys(iargs['series'])
         primekeys_passed = iargs.get('primekey', None)  # primekeys_passes is a dict, with key-value pairs.
-        if primekeys_passed is not None:
-            if not set(list(primekeys_passed.keys())) <= set(primekeys):
-                error_message = f"Unexpected PrimeKeys were passed. The series {iargs['series']} supports the following Keywords: {primekeys}"
-                raise ValueError(error_message.format(series=iargs['series'], primekeys=primekeys))
+        if primekeys_passed is not None and not set(list(primekeys_passed.keys())) <= set(primekeys):
+            error_message = f"Unexpected PrimeKeys were passed. The series {iargs['series']} supports the following Keywords: {primekeys}"
+            raise ValueError(error_message.format(series=iargs['series'], primekeys=primekeys))
         # Raise special error for wavelength (even though the code would ignore it anyway)
         wavelength = iargs.get('wavelength', '')
-        if wavelength != '':
-            if 'WAVELNTH' not in primekeys:
-                error_message = (f"The series {iargs['series']} does not support wavelength attribute. "
-                                 f"The following primekeys are supported {primekeys}")
-                raise TypeError(error_message.format(series=iargs['series'], pkeys=primekeys))
+        if wavelength != '' and 'WAVELNTH' not in primekeys:
+            error_message = (f"The series {iargs['series']} does not support wavelength attribute. "
+                             f"The following primekeys are supported {primekeys}")
+            raise TypeError(error_message.format(series=iargs['series'], pkeys=primekeys))
         # Raise errors for segments
         # Get a set of the segments that exist for the given series, and check
         # whether the passed segments is a subset of that.
         series = client.info(iargs['series'])
         # Fetches all valid segment names
         segments = list(series.segments.index.values)
         segments_passed = iargs.get('segment', None)
@@ -761,15 +742,15 @@
         # Convert the list of keywords into comma-separated string.
         if isinstance(keywords, list):
             key = str(keywords)[1:-1].replace(' ', '').replace("'", '')
         else:
             key = keywords
         log.debug(f"Running following query: {ds}")
         log.debug(f"Requesting following keywords: {key}")
-        result = client.query(ds, key=key, rec_index=isMeta)
+        result = client.query(ds, key=key, rec_index=is_meta)
         if result is None or result.empty:
             return astropy.table.Table()
         else:
             return astropy.table.Table.from_pandas(result)
 
     @classmethod
     def _can_handle_query(cls, *query):
@@ -809,22 +790,22 @@
         for series in data_sources:
             info = client.series(rf'{series}\.')
             for item in info:
                 print(f'🛰 Getting info for {series}: {item}')
                 data = client.info(item)
                 series_store.append((data.name, data.note))
                 if not data.segments.empty:
-                    for row in data.segments.iterrows():
-                        segments.append((row[0], row[1][-1]))
+                    segments.extend((row[0], row[1][-1]) for row in data.segments.iterrows())
         series_store = list(set(series_store))
         segments = list(set(segments))
         with open(os.path.join(here, 'data', 'attrs.json'), 'w') as attrs_file:
-            keyword_info = {}
-            keyword_info["series_store"] = sorted(series_store)
-            keyword_info["segments"] = sorted(segments)
+            keyword_info = {
+                "series_store": sorted(series_store),
+                "segments": sorted(segments),
+            }
             json.dump(keyword_info, attrs_file, indent=2)
 
     @staticmethod
     def load_jsoc_values():
         """
         We take this list and register all the keywords as corresponding Attrs.
 
@@ -838,9 +819,9 @@
 
         here = os.path.dirname(os.path.realpath(__file__))
         with open(os.path.join(here, 'data', 'attrs.json')) as attrs_file:
             keyword_info = json.load(attrs_file)
         # Create attrs out of them.
         series_dict = {a.jsoc.Series: keyword_info["series_store"]}
         segments_dict = {a.jsoc.Segment: keyword_info["segments"]}
-        attrs = {**series_dict, **segments_dict}
+        attrs = series_dict | segments_dict
         return attrs
```

### Comparing `sunpy-5.1.1/sunpy/net/jsoc/tests/test_attr.py` & `sunpy-5.1.2/sunpy/net/jsoc/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/jsoc/tests/test_jsoc.py` & `sunpy-5.1.2/sunpy/net/jsoc/tests/test_jsoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import tempfile
 
 import pytest
 from parfive import Results
 
 import astropy.table
 import astropy.time
@@ -74,15 +75,15 @@
 
 
 @pytest.mark.remote_data
 def test_post_notify_fail(client):
     responses = client.search(
         a.Time('2020/1/1T00:00:00', '2020/1/1T00:00:45'),
         a.jsoc.Series('hmi.M_45s'))
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Email address is invalid or not registered"):
         client.request_data(responses)
 
 
 @pytest.mark.remote_data()
 def test_post_wave_series(client):
     with pytest.raises(TypeError, match="The series hmi.M_45s does not support wavelength attribute."):
         client.search(
@@ -122,98 +123,94 @@
     path = tempfile.mkdtemp()
     aa = client.get_request(bb, path=path)
     assert isinstance(aa, Results)
 
 
 @pytest.mark.remote_data
 def test_invalid_query(client):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Series must be specified for a JSOC Query"):
         client.search(a.Time('2020/1/1T01:00:00', '2020/1/1T01:00:45'))
 
 
 @pytest.mark.remote_data
 def test_lookup_records_errors(client):
     d1 = {'end_time': astropy.time.Time('2020-01-01 01:00:35'),
           'start_time': astropy.time.Time('2020-01-01 00:00:35')}
-    # Series must be specified for a JSOC Query
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Series must be specified for a JSOC Query"):
         client._lookup_records(d1)
 
-    d1.update({'series': 'aia.lev1_euv_12s'})
-    d1.update({'keys': 123})
-    # Keywords can only be passed as a list or comma-separated strings.
-    with pytest.raises(TypeError):
+    d1['series'] = 'aia.lev1_euv_12s'
+    d1['keys'] = 123
+    with pytest.raises(TypeError, match="Keywords can only be passed as a list or comma-separated strings."):
         client._lookup_records(d1)
-
     d1['keys'] = 'T_OBS'
-    d1.update({'primekey': {'foo': 'bar'}})
-    # Unexpected PrimeKeys were passed.
-    with pytest.raises(ValueError):
+    d1['primekey'] = {'foo': 'bar'}
+    with pytest.raises(ValueError, match=re.escape("Unexpected PrimeKeys were passed. The series aia.lev1_euv_12s supports the following Keywords: ['T_REC', 'WAVELNTH']")):
         client._lookup_records(d1)
 
     del d1['primekey']
-    d1.update({'segment': 123})
-    d1.update({'wavelength': 304*u.AA})
-    # Segments can only be passed as a comma-separated string or a list of strings.
-    with pytest.raises(TypeError):
+    d1['segment'] = 123
+    d1['wavelength'] = 304*u.AA
+    with pytest.raises(TypeError, match="Segments can only be passed as a comma-separated string or a list of strings."):
         client._lookup_records(d1)
 
-    # Unexpected Segments were passed.
-    d1.update({'segment': 'foo'})
-    with pytest.raises(ValueError):
+    d1['segment'] = 'foo'
+    with pytest.raises(ValueError, match=re.escape("Unexpected Segments were passed. The series aia.lev1_euv_12s contains the following Segments ['image', 'spikes']")):
         client._lookup_records(d1)
 
     del d1['segment']
-    d1.update({'series': 'hmi.m_45s'})
+    d1['series'] = 'hmi.m_45s'
     # The series does not support wavelength attribute.
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match=re.escape("The series hmi.m_45s does not support wavelength attribute. The following primekeys are supported ['T_REC', 'CAMERA']")):
         client._lookup_records(d1)
 
 
 @pytest.mark.remote_data
 def test_make_recordset_errors(client):
     d1 = {'series': 'aia.lev1_euv_12s'}
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Time, Wavelength or an explicit PrimeKey must be specified."):
         client._make_recordset(**d1)
 
-    d1.update({
+    d1 |= {
         'end_time': astropy.time.Time('2020-01-01 01:00:35', scale='tai'),
         'start_time': astropy.time.Time('2020-01-01 00:00:35', scale='tai'),
-        'primekey': {'T_REC': '2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI'}
-    })
+        'primekey': {
+            'T_REC': '2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI'
+        },
+    }
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=re.escape("Time attribute has been passed both as a Time() and PrimeKey(). Please provide any one of them or separate them by OR operator.")):
         client._make_recordset(**d1)
 
-    d1.update({
+    d1 |= {
         'end_time': astropy.time.Time('2020-01-01 01:00:35', scale='tai'),
         'start_time': astropy.time.Time('2020-01-01 00:00:35', scale='tai'),
         'wavelength': 604*u.AA,
-        'primekey': {'WAVELNTH': '604'}
-    })
+        'primekey': {'WAVELNTH': '604'},
+    }
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match=re.escape("Wavelength attribute has been passed both as a Wavelength() and PrimeKey(). Please provide any one of them or separate them by OR operator.")):
         client._make_recordset(**d1)
 
 
 @pytest.mark.remote_data
 def test_make_recordset(client):
     d1 = {'series': 'aia.lev1_euv_12s',
           'end_time': astropy.time.Time('2020-01-01 01:00:35', scale='tai'),
           'start_time': astropy.time.Time('2020-01-01 00:00:35', scale='tai')
           }
     exp = 'aia.lev1_euv_12s[2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI]'
     assert client._make_recordset(**d1) == exp
 
-    d1.update({'wavelength': 604*u.AA})
+    d1['wavelength'] = 604*u.AA
     exp = 'aia.lev1_euv_12s[2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI][604]'
     assert client._make_recordset(**d1) == exp
 
     del d1['wavelength']
-    d1.update({'primekey': {'WAVELNTH': '604'}})
+    d1['primekey'] = ({'WAVELNTH': '604'})
     assert client._make_recordset(**d1) == exp
 
     del d1['start_time'], d1['end_time']
     d1['primekey'].update({'T_REC': '2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI'})
     exp = 'aia.lev1_euv_12s[2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI]'
     assert client._make_recordset(**d1) == exp
 
@@ -230,31 +227,29 @@
 
     d1 = {'series': 'hmi.sharp_720s',
           'end_time': astropy.time.Time('2020-01-01 01:00:35', scale='tai'),
           'start_time': astropy.time.Time('2020-01-01 00:00:35', scale='tai'),
           'segment': ['continuum', 'magnetogram'],
           'primekey': {'HARPNUM': '4864'}
           }
-    exp = 'hmi.sharp_720s[4864][2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI]'\
-          '{continuum,magnetogram}'
+    exp = 'hmi.sharp_720s[4864][2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI]{continuum,magnetogram}'
     assert client._make_recordset(**d1) == exp
 
-    d1.update({'sample': 300.0})
-    exp = 'hmi.sharp_720s[][2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI@300.0s]'\
-          '{continuum,magnetogram}'
+    d1['sample'] = 300.0
+    exp = 'hmi.sharp_720s[][2020.01.01_00:00:35_TAI-2020.01.01_01:00:35_TAI@300.0s]{continuum,magnetogram}'
     assert client._make_recordset(**d1) == exp
 
 
 @pytest.mark.remote_data
 def test_request_data_error(client, jsoc_test_email):
     responses = client.search(
         a.Time('2020/1/1T1:00:36', '2020/1/1T01:00:38'),
         a.jsoc.Series('hmi.M_45s'), a.jsoc.Notify(jsoc_test_email),
         a.jsoc.Protocol('foo'))
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match="Protocols other than as-is,fits are not supported."):
         client.request_data(responses)
 
 
 @pytest.mark.remote_data
 def test_request_data_method(client, jsoc_test_email):
     responses = client.search(
         a.Time('2012/1/1T1:00:36', '2012/1/1T01:00:38'),
@@ -367,7 +362,18 @@
     #     a.Time('1990-12-12T00:00:00', '1990-12-12T0:01:00'),
     #    a.jsoc.Series.hmi_b_720s
     # )
     response = JSOCResponse()
     assert len(response) == 0
     result = client.fetch(response)
     assert len(result) == 0
+
+
+@pytest.mark.remote_data
+def test_string_keyword_is_converted_correctly(client):
+    # Bug reported here:
+    # https://community.openastronomy.org/t/how-to-select-only-fuv-iris-level-1-data-using-jsoc/900
+    responses = client.search(
+        a.Time("2014-01-01T00:00", "2014-01-01T00:05"),
+        a.jsoc.Series("iris.lev1"), a.jsoc.Keyword("INSTRUME") == "FUV"
+    )
+    assert len(responses) == 6
```

### Comparing `sunpy-5.1.1/sunpy/net/scraper.py` & `sunpy-5.1.2/sunpy/net/scraper.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/strategies.py` & `sunpy-5.1.2/sunpy/net/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_attr.py` & `sunpy-5.1.2/sunpy/net/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_attr_walker.py` & `sunpy-5.1.2/sunpy/net/tests/test_attr_walker.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_baseclient.py` & `sunpy-5.1.2/sunpy/net/tests/test_baseclient.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_fido.py` & `sunpy-5.1.2/sunpy/net/tests/test_fido.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_helioviewer.py` & `sunpy-5.1.2/sunpy/net/tests/test_helioviewer.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/tests/test_scraper.py` & `sunpy-5.1.2/sunpy/net/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/attrs.py` & `sunpy-5.1.2/sunpy/net/vso/attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/data/attrs.json` & `sunpy-5.1.2/sunpy/net/vso/data/attrs.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/legacy_response.py` & `sunpy-5.1.2/sunpy/net/vso/legacy_response.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/table_response.py` & `sunpy-5.1.2/sunpy/net/vso/table_response.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/tests/test_attrs.py` & `sunpy-5.1.2/sunpy/net/vso/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/tests/test_vso.py` & `sunpy-5.1.2/sunpy/net/vso/tests/test_vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/vso.py` & `sunpy-5.1.2/sunpy/net/vso/vso.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/net/vso/zeep_plugins.py` & `sunpy-5.1.2/sunpy/net/vso/zeep_plugins.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/physics/differential_rotation.py` & `sunpy-5.1.2/sunpy/physics/differential_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/physics/tests/reference/test_differential_rotation.txt` & `sunpy-5.1.2/sunpy/physics/tests/reference/test_differential_rotation.txt`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/physics/tests/test_differential_rotation.py` & `sunpy-5.1.2/sunpy/physics/tests/test_differential_rotation.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/sun/_constants.py` & `sunpy-5.1.2/sunpy/sun/_constants.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/sun/constants.py` & `sunpy-5.1.2/sunpy/sun/constants.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/sun/models.py` & `sunpy-5.1.2/sunpy/sun/models.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/sun/tests/test_constants.py` & `sunpy-5.1.2/sunpy/sun/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/figure_hashes_mpl_353_ft_261_astropy_511_animators_100.json` & `sunpy-5.1.2/sunpy/tests/figure_hashes_mpl_353_ft_261_astropy_511_animators_100.json`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json` & `sunpy-5.1.2/sunpy/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.644927536231884%*

 * *Differences: {"'sunpy.map.tests.test_compositemap.test_peek_composite_map'": "'601847a982ee4a372def1eede3a992921a33986735e6ec5b7ca1a92a7a056846'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map'": "'5776fedee0a8dd3f54d086af229a6af65f98c532e926315941ac82516654e6e5'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_colors'": "'c91039a3ede3c432fc040396c0ec318f6274e5eebc70e5de38be723bbf2a0a45'",*

 * * "'sunpy.map.tests.test_compositemap.test_plot_composite_map_contours'": "'b631946c2cab5be60009f68c8193 […]*

```diff
@@ -1,71 +1,71 @@
 {
     "sunpy.image.tests.test_transform.test_clipping": "f36c82068789b048d5855315f295e2404c85b0a63ec77de0e294d58b43c9acaf",
     "sunpy.image.tests.test_transform.test_nans": "776e5a2c12bbbff9f5f9de647052cd2ad1be03b39586b91502c8ebba08e87c1b",
-    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "a21143a11c499d95b3618d2f82a6d6e8a3cbad6291ab52b20b218b3f4a03c45b",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "41ee9a52dc0fb57edcecf307d3ae5ac110bcedf4542cd666977a482b859c088f",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "4e6310746beab7a9d866aab10d86878aa5797b2f20ae933f8cfdcdf1ce9d461e",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "28aa801517b26222b309e8296d5aac88d7964b6d39f3a418102f42e8c3bfb8e8",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "978a800d5c5dec799b1046e905e74a8f94567245f99aa93a0d33de4e98ec188b",
-    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "2e955b5da43296c9bc91950cca9e1dce2cbf3e49fed908f369c3446a8478d2b5",
-    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "2b2a157405dc296d5c06c74f7d8bc6e03b3cff4512cf9b0e66a773827497f37a",
-    "sunpy.map.tests.test_map_factory.test_map_jp2_HMI": "3b731f25ab5777f187def8296fbed88d27809867405e0e97d5e808ca1bb4b42c",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "cd86fb9c0ed0e26eaae00d816d0b5d3f381b2be22b8e99d45afe5a511ccd55e5",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "17748c119a97c112e77fcb368af595f2b5faada067a7188abe846c7b160f9ea8",
-    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "9168fca9a4e04def3da12624196b29ebe954004ad269faa4bab11276a85366af",
-    "sunpy.map.tests.test_mapbase.test_rotation_rect_pixelated_data": "5b37819c36a50a2a7a26944a2f1481027dd17390e73158f6b5510034102d35bb",
-    "sunpy.map.tests.test_mapsequence.test_map_sequence_plot": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
-    "sunpy.map.tests.test_mapsequence.test_map_sequence_plot_custom_cmap_norm": "c1276702147f4debaa14c17f6b0b2ab7f9e0b1ace309c72e767b2af071c4405e",
-    "sunpy.map.tests.test_mapsequence.test_norm_animator": "5a7217dd55ab3a593a27741fecfe0851208fd1d31baeca4cbd018d65aaf3f483",
-    "sunpy.map.tests.test_plotting.test_draw_contours_aia": "9b899f6ae244186a29f27b4167ea75b355428fbd69166cd55903e52b8f5fbf0b",
-    "sunpy.map.tests.test_plotting.test_draw_contours_different_wcs": "5f2abc715e899ad9b9425acfe1beb41a915423b93737781c348dfa0b99de8180",
-    "sunpy.map.tests.test_plotting.test_draw_grid_aia171": "51c9e572c5708a2112445426bfcaef25650e294b23f3ebd3aa3769d596e57dda",
-    "sunpy.map.tests.test_plotting.test_draw_limb_different_observer": "8802a9b36bb9679067b5c45d752f5cb9e6757a51c41d9809e0b3e131786ada02",
-    "sunpy.map.tests.test_plotting.test_draw_limb_heliographic_stonyhurst": "8fb7ab6239ddae9fb06c45b32a37cc14ef0c6d281bf6cd5ae567e8ad8cfd6ff5",
+    "sunpy.map.tests.test_compositemap.test_peek_composite_map": "601847a982ee4a372def1eede3a992921a33986735e6ec5b7ca1a92a7a056846",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map": "5776fedee0a8dd3f54d086af229a6af65f98c532e926315941ac82516654e6e5",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_colors": "c91039a3ede3c432fc040396c0ec318f6274e5eebc70e5de38be723bbf2a0a45",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_contours": "b631946c2cab5be60009f68c81938c35c23e6037a029df5213ec6067d140659f",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linestyles": "41c4f1b4463c65e6175a394a0795fde5e0943bce9ee7e5b6826967732cb91e59",
+    "sunpy.map.tests.test_compositemap.test_plot_composite_map_linewidths": "c911a7f8cb0fac3eb8caeaaa5e2d4086d5d6eea410bc4bcfa02105f5776ca367",
+    "sunpy.map.tests.test_compositemap.test_set_alpha_composite_map": "a0f312dfa68645b446a3a03a4adc2ce2e4452c30aae90348c6de0bf97b519a39",
+    "sunpy.map.tests.test_map_factory.test_map_jp2_HMI": "d54c99b975dc2e5805bfd39e00627ad92fba9fe2d38e510fc72b143cfbc28e4c",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[opencv]": "072505693731f65824dcaa7f0843087990f15f34b519285a2bc8965a1fa0ed37",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scikit-image]": "911a0442055922f0d31dd48d8f1ede3d1b8b4d11a55f00a3403e8124761c2346",
+    "sunpy.map.tests.test_mapbase.test_derotating_nonpurerotation_pcij[scipy]": "c15c6c707b3b0e707936988054aeb818eee7b39e2249db5309ca43585d325a51",
+    "sunpy.map.tests.test_mapbase.test_rotation_rect_pixelated_data": "356822787795278a4dab61bb8bbf5d62cc29d979ec1280653286a85b6188e944",
+    "sunpy.map.tests.test_mapsequence.test_map_sequence_plot": "86f2d19643fbeeaea8bd7097b9002a77da455eeeb46d4ac707bd3c55df15dc22",
+    "sunpy.map.tests.test_mapsequence.test_map_sequence_plot_custom_cmap_norm": "129afdbcb3de6893187f3bbe20e9107316ae5d04ceecb8a1969befe3bb3ff540",
+    "sunpy.map.tests.test_mapsequence.test_norm_animator": "2241b65ed7126250eb14ebbcd095ef4a1f696ad737a4e975ff8e66a007667487",
+    "sunpy.map.tests.test_plotting.test_draw_contours_aia": "90f83a5c24fdd88a1d14807034ba2b4ee1644d3f53745935eb8e537a2acc2b9a",
+    "sunpy.map.tests.test_plotting.test_draw_contours_different_wcs": "9cbb12775ed1da71226dcc500f434bdf0ece76d54894942fb34c1805d8d11de0",
+    "sunpy.map.tests.test_plotting.test_draw_grid_aia171": "a698bc5336276f695b06a7029dca0f7bc9565d2e86b33e4123582c77fb94596d",
+    "sunpy.map.tests.test_plotting.test_draw_limb_different_observer": "bba8a5d3d8e5e3e3a7d36060d9730e4545c5250367902cf97048c33049f330f3",
+    "sunpy.map.tests.test_plotting.test_draw_limb_heliographic_stonyhurst": "765a9da1806663c13acc8b5364d877892fa1dd46d3bfbc8f362b3ac7e4bd8fa2",
     "sunpy.map.tests.test_plotting.test_heliographic_grid_annotations": "c7c08b2b6dae1b96c303345b04682060da97a1b304e7f25bcfd40b2154751465",
     "sunpy.map.tests.test_plotting.test_heliographic_peek": "662a24f525b30ce89ba15b7668518f31d439fa8b0c5ba84da2a71bbda31edb9a",
     "sunpy.map.tests.test_plotting.test_heliographic_quadrangle_top_right": "40591e49e6b32ec3a27b6fc50b9e2fdfcaa9665eca70b6a515dfb9dc7c0b1724",
     "sunpy.map.tests.test_plotting.test_heliographic_quadrangle_width_height": "a52dca9100f3f96644e924f283c7ba9bd26db115be3a8e19b91898406d06f9ba",
-    "sunpy.map.tests.test_plotting.test_peek_aia171": "4448f1b15f721ba8a63cdbed738d11fb8fc90b3d517ad62742db9adb184d1fb2",
-    "sunpy.map.tests.test_plotting.test_peek_grid_aia171": "d27ca38c6f529a415a14624dd43ff6a9436b6972d1d82faa4a9884fd601eb106",
-    "sunpy.map.tests.test_plotting.test_peek_grid_limb_aia171": "6abc117f65bd55acceaed9ddeddaef34e4f1bf920f86cc4f701f9c87d7bb1845",
-    "sunpy.map.tests.test_plotting.test_peek_grid_spacing_aia171": "e2629577592c46e2baa1658fcf1f92ac1e5e6985a08c7aa6d2df3869f4654924",
-    "sunpy.map.tests.test_plotting.test_peek_limb_aia171": "2d5a36e6b8873ded8a6141b60caddd9aa697344c8df59852e80c4dcda7fd67be",
-    "sunpy.map.tests.test_plotting.test_plot_aia171": "3cdc53f41914028a4e9f23112d7e616ce8a423ef5670c8365fdadbc0e59780ca",
-    "sunpy.map.tests.test_plotting.test_plot_aia171_clip": "920852d09b1b0af6ed406312e8e54ce2b327d38061a0652d95df03b41e1c552d",
-    "sunpy.map.tests.test_plotting.test_plot_aia171_superpixel": "1c133f41c740f4974b8dd27477a247a64c7f8e387d1d8d8c9b4f42ca0387b2ac",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign": "352a8c7ece7f3439750a199cfa345d1ef23e6c14d545a94f67a6eb2e2257e898",
-    "sunpy.map.tests.test_plotting.test_plot_autoalign_pixel_alignment": "03e6e20d752c9de9f45022ea1819ca9bbd95950b0852f9138b28448636d533b6",
-    "sunpy.map.tests.test_plotting.test_plot_masked_aia171": "8acfaf714eca9295e1d4ecd17e6eec62c8fc991cba45eeb0ba6d2efaa492d29b",
-    "sunpy.map.tests.test_plotting.test_plot_masked_aia171_superpixel": "ffabe0ca544b93c8084af36edb5b293cdce613d13b73ddeaa906ddf2617da34b",
-    "sunpy.map.tests.test_plotting.test_plot_resample": "351baa39339b9f7d206232b9c2fb777d7edf965e1554040171ac40e3a1f5ec62",
-    "sunpy.map.tests.test_plotting.test_plot_rotated_aia171": "9df0409afa257ebe481aa5170321072ddca349fe596f3d662208e127f39a938e",
-    "sunpy.map.tests.test_plotting.test_plot_superpixel": "4fcd7af5690bbb5a1ae65ab2bf80db31aa41f240456cddaf49c6132fd459b973",
-    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right": "e55f63d480032009779aa5c1742aff30694587f8bee2f8201c7c64192880cecb",
-    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right_different_axes": "893064c44b850aea39b24b2a94af10af340745c0e32b867033b0f14684bf337f",
-    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_width_height": "68f0ac032a79416bd0287e393ea98ed5ac54a22a068db08131885046c39b8cbc",
-    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_top_right": "9a2d796c365b5280464ecfdb01f62d27ddeee127e6aee4f243a98ec98f923df7",
-    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_width_height": "89f18bf54f0ebeb6ce36522620f6551457bfd1dd1da1634edb50cbea5adc2939",
-    "sunpy.map.tests.test_plotting.test_rectangle_aia171_top_right": "643d623d94d9390a94266e1088dacb03bd62668815a3b04e1bda51afa701d8a4",
-    "sunpy.map.tests.test_plotting.test_rectangle_aia171_width_height": "d6afbac82891ed231d8bcbe5a66fe0098856dba4aca684073ddee2ec3b10a289",
-    "sunpy.map.tests.test_reproject_to.test_reproject_to_hgs": "c1dc26bedf3d24690364637e1a7d6fde165445049e633e8407ad2ccf42416fcb",
-    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_adaptive": "40cb43b7431941e8977449f5ed5d1439e7dddf9f0ec0aa21d0c18f09a25e259c",
-    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_exact": "93171456dfac771f53bc0465922cf5811048df0b56100d329a55f71b36bdc8f5",
-    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_interpolation": "b82e6462d4ccb8c188b5f6deac3258326ba6840ef624c18f044a9d4cadce3cf2",
+    "sunpy.map.tests.test_plotting.test_peek_aia171": "5029c815df9b406ac04e2fa221ae57e7f12dfce1d90888f4878ec58c948a3f1f",
+    "sunpy.map.tests.test_plotting.test_peek_grid_aia171": "6e13b565c19a9dd20f1cabdcb0044923a2b960de57a117aa337c2e259547163e",
+    "sunpy.map.tests.test_plotting.test_peek_grid_limb_aia171": "b00af72714cf4788e6593022a8531446a45238785ea0d87512c303ec087e217b",
+    "sunpy.map.tests.test_plotting.test_peek_grid_spacing_aia171": "37642547c98d3dd1fd21a7d57d1017c0f455542110f375614c6feb38a10a927b",
+    "sunpy.map.tests.test_plotting.test_peek_limb_aia171": "abb4faffa1a291e08c72953e73b453b3c0073331b4e14dde0a40f0e17174f20c",
+    "sunpy.map.tests.test_plotting.test_plot_aia171": "86f2d19643fbeeaea8bd7097b9002a77da455eeeb46d4ac707bd3c55df15dc22",
+    "sunpy.map.tests.test_plotting.test_plot_aia171_clip": "29b93bbe004670248aed9ddde8c5f8e6eda2d975d6c046f05a9c4a5f144caf2c",
+    "sunpy.map.tests.test_plotting.test_plot_aia171_superpixel": "02f8b342f79e2395052ee851cb785fc0f208c10a26bb6a6547e71e4da12d9a6c",
+    "sunpy.map.tests.test_plotting.test_plot_autoalign": "dc61f7444a64f9c5c8830dbad0efed15812fd4f55b237cb9cc4cd2f7b2a05975",
+    "sunpy.map.tests.test_plotting.test_plot_autoalign_pixel_alignment": "dd407fa27c34d512e5a98f811a2533868b0dab67895c4d4f2b53b4bc52f781b0",
+    "sunpy.map.tests.test_plotting.test_plot_masked_aia171": "738b6d265e9a6c534204f44912048566289c59f89aa8d98345969db835f7e834",
+    "sunpy.map.tests.test_plotting.test_plot_masked_aia171_superpixel": "854f60a854e0f3166762c94831445b83f5402a8aa70e34013616f7e4074476fe",
+    "sunpy.map.tests.test_plotting.test_plot_resample": "df6313df2fbf65d1f9aaf018677772c05750dcbd3e0098f34ca41cc40e5d8815",
+    "sunpy.map.tests.test_plotting.test_plot_rotated_aia171": "982363a267e12a380c48c02ab73a98bbadae4ce54f4b621898f815aac2daf040",
+    "sunpy.map.tests.test_plotting.test_plot_superpixel": "45ebdec700a7699f7aaea6e86b22c049c65ed3c457aa2e0f5b53d135b9f54c79",
+    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right": "586d82cd41587965becb6793956d2855d96da84a4791acc7de5e52b6f77e6ad0",
+    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_top_right_different_axes": "47f6153e288bcc952fc5e0e8600d180550f3f20ef69d7b6090208b511b81eed6",
+    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_pix_width_height": "ab094f1c23b454913db9e31c1a8faf6fc69fd196688c1b569bb22d261b127f55",
+    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_top_right": "4c7026849d4ccf1a9b38eb669de3ecf83523e20a6e784bea4fad5feb57f37d3d",
+    "sunpy.map.tests.test_plotting.test_quadrangle_aia17_width_height": "545e2056688bd4903fe93cbe8e81a33d0020690f7842d4237f75438381c4a5b6",
+    "sunpy.map.tests.test_plotting.test_rectangle_aia171_top_right": "c691c8232a7b775c43c955153e8b79b3022bbc1d8f0ccc9607da635279b0bb43",
+    "sunpy.map.tests.test_plotting.test_rectangle_aia171_width_height": "2d92a7b78edea18f6e14d62dcaff46448137270eb31a1552c80b570092fb3dc3",
+    "sunpy.map.tests.test_reproject_to.test_reproject_to_hgs": "90452e9e8f248f8798a794ba70e157bf0eb87a083bda55a8ffc846c2024b1363",
+    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_adaptive": "ee2cc06c8ed27369e1b2cd6b5d16688663ee061e3d84a3ccee09923bae10b16c",
+    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_exact": "a772b4ba8deeb611c683d86911bf0b5acb90a3b307b1064c1d04511050810eed",
+    "sunpy.map.tests.test_reproject_to.test_reproject_to_hpc_interpolation": "adca79ed26b0139f29c5c0bec63d1a818fe8ba0cd718923d952210e6e8ca801c",
     "sunpy.timeseries.sources.tests.test_eve.test_esp_peek": "28b1e7af0e1894d22fd9db90d9e2bc5eb76e291c9e41fa1bb1d33d95bd13cce3",
     "sunpy.timeseries.sources.tests.test_eve.test_eve_peek": "2a22f93af44971411800e4fcd0d93d2128fe2b9e6b97e576e8372c2cd12d7d78",
     "sunpy.timeseries.sources.tests.test_fermi_gbm.test_fermi_gbm_peek": "83f0b53ca6f1cd809bd03e4aff80b3c02c8078e552b0c3e90b2cb3cf26932a51",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_peek": "4fc2d89d3ce2727a75a9feee13c0671e4bd570fe87af2d1706d13a2799db3ee3",
     "sunpy.timeseries.sources.tests.test_goes.test_goes_ylim": "432cd4458eed29764d6bfaae2bee0820706fc293d7b23972fc587eae590bcd72",
     "sunpy.timeseries.sources.tests.test_lyra.test_lyra_peek": "48924d42773a4d834342cdce5ad1e005db9980bf6db6525d97a141a08f411aba",
     "sunpy.timeseries.sources.tests.test_noaa.test_noaa_json_ind_peek": "a61ea2eb004d89f16b6ea4b6c56b2eedbb456ecc301d2c710eb3312f70c6a6f7",
     "sunpy.timeseries.sources.tests.test_noaa.test_noaa_json_pre_peek": "2673bf752a5f4133239a4b96308de5159e1202ce55efa5a590deba213788af74",
     "sunpy.timeseries.sources.tests.test_norh.test_norh_peek": "a403f6ec3064a1dbcf4c190a9724d3b893b4608ca5d0a0cae8a400378f0c8f9e",
     "sunpy.timeseries.sources.tests.test_rhessi.test_rhessi_peek": "f7783ff9d1b00a03cebfdc173057f67a44de00621eff3bb22d23355c3ba7c85b",
     "sunpy.timeseries.tests.test_timeseriesbase.test_column_subset_peek": "0c1ac6714d9bc505db3ee449fa9a8ba6842b0d756a8c8f02a2133547123c2a92",
     "sunpy.timeseries.tests.test_timeseriesbase.test_generic_ts_peek": "ba0469ba921c3367384c04de4e64d16cacd1499277a14f1809c087d8f21ee041",
-    "sunpy.visualization.animator.tests.test_mapsequenceanimator.test_map_sequence_animator_wcs_simple_plot": "5f52fb6efb00e04e4de394ec8d5edb940d5690602ff249998631eacef3b9f2f1",
+    "sunpy.visualization.animator.tests.test_mapsequenceanimator.test_map_sequence_animator_wcs_simple_plot": "07683c79407f568ce977ba2560e33da8668d06937f74732d2f375d6605f3c58e",
     "sunpy.visualization.colormaps.tests.test_cm.test_cmap_visual": "fbbd93e66471a92f042543226f7e091f3c3b7f6079bbf418863019e63aaa4db9",
-    "sunpy.visualization.tests.test_drawing.test_draw_equator_aia171": "abc52d5e8254b32ed42942926a4ee92d7b0aaf441bfe8c54cdcd98d6a7a62eba",
-    "sunpy.visualization.tests.test_drawing.test_draw_prime_meridian_aia171": "6602b10b71759a5dae32691cfdab8762de61409a433c97b151de663f3515eb66",
+    "sunpy.visualization.tests.test_drawing.test_draw_equator_aia171": "e10ed71a0bb1ebd65020723e97c290e9ef22fa303af545529117ef808d8d8c80",
+    "sunpy.visualization.tests.test_drawing.test_draw_prime_meridian_aia171": "2f2d22110f97212e459b018ccd39470a94b8eaf7de9949458c946195506ba106",
     "sunpy.visualization.tests.test_drawing.test_heliographic_equator_prime_meridian": "3cb195a44e899ef46de7365bd0a0c580b7ea69662bdc560a1bbb1686c2ad48cf"
 }
```

### Comparing `sunpy-5.1.1/sunpy/tests/helpers.py` & `sunpy-5.1.2/sunpy/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/mocks.py` & `sunpy-5.1.2/sunpy/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/self_test.py` & `sunpy-5.1.2/sunpy/tests/self_test.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/tests/test_mocks.py` & `sunpy-5.1.2/sunpy/tests/tests/test_mocks.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/tests/test_self_test.py` & `sunpy-5.1.2/sunpy/tests/tests/test_self_test.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/tests/tests/test_sunpy_data_filenames.py` & `sunpy-5.1.2/sunpy/tests/tests/test_sunpy_data_filenames.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/time/tests/test_taiseconds.py` & `sunpy-5.1.2/sunpy/time/tests/test_taiseconds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import erfa
 import pytest
 
 from astropy.time import Time
-from astropy.time.formats import erfa
 
 # This registers the TimeTaiSeconds format with astropy
 from sunpy.time import *  # NOQA
 
 
 def test_time_t0():
     """
```

### Comparing `sunpy-5.1.1/sunpy/time/tests/test_time.py` & `sunpy-5.1.2/sunpy/time/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/time/tests/test_timerange.py` & `sunpy-5.1.2/sunpy/time/tests/test_timerange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timedelta
 
 import pytest
+from erfa import ErfaWarning
 
 import astropy.units as u
 from astropy.time import Time, TimeDelta
-from astropy.utils.exceptions import ErfaWarning
 
 import sunpy.time
 from sunpy.time import is_time_equal
 
 tbegin_str = '2012/1/1'
 tfin_str = '2012/1/2'
 dt = u.Quantity(24 * 60 * 60, 's')
```

### Comparing `sunpy-5.1.1/sunpy/time/time.py` & `sunpy-5.1.2/sunpy/time/time.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/time/timeformats.py` & `sunpy-5.1.2/sunpy/time/timeformats.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/time/timerange.py` & `sunpy-5.1.2/sunpy/time/timerange.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/conftest.py` & `sunpy-5.1.2/sunpy/timeseries/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from collections import OrderedDict
 
 import numpy as np
 import pytest
-from erfa.core import ErfaWarning
+from erfa import ErfaWarning
 from pandas import DataFrame
 
 import astropy.units as u
 from astropy.table import Table
 from astropy.time import TimeDelta
 
 import sunpy
```

### Comparing `sunpy-5.1.1/sunpy/timeseries/metadata.py` & `sunpy-5.1.2/sunpy/timeseries/metadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/__init__.py` & `sunpy-5.1.2/sunpy/timeseries/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/eve.py` & `sunpy-5.1.2/sunpy/timeseries/sources/eve.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/fermi_gbm.py` & `sunpy-5.1.2/sunpy/timeseries/sources/fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/goes.py` & `sunpy-5.1.2/sunpy/timeseries/sources/goes.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         """
         if columns is None:
             columns = ["xrsa", "xrsb"]
         axes, columns = self._setup_axes_columns(axes, columns)
         plot_settings = {"xrsa": ["blue", r"0.5--4.0 $\AA$"], "xrsb": ["red", r"1.0--8.0 $\AA$"]}
         data = self.to_dataframe()
         for channel in columns:
-            axes.plot_date(
+            axes.plot(
                 data.index, data[channel], "-", label=plot_settings[channel][1], color=plot_settings[channel][0], lw=2, **kwargs
             )
         axes.set_yscale("log")
         axes.set_ylim(1e-9, 1e-2)
         axes.set_ylabel("Watts m$^{-2}$")
         self._setup_x_axis(axes)
```

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/lyra.py` & `sunpy-5.1.2/sunpy/timeseries/sources/lyra.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/noaa.py` & `sunpy-5.1.2/sunpy/timeseries/sources/noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/norh.py` & `sunpy-5.1.2/sunpy/timeseries/sources/norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/rhessi.py` & `sunpy-5.1.2/sunpy/timeseries/sources/rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_eve.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_eve.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from sunpy.tests.helpers import figure_test
 from sunpy.util.exceptions import SunpyDeprecationWarning, SunpyUserWarning
 
 esp_filepath = get_test_filepath('eve_l1_esp_2011046_00_truncated.fits')
 eve_filepath = get_test_filepath('EVE_L0CS_DIODES_1m_truncated.txt')
 
 
+@pytest.mark.skipif(pytest.__version__ < "8.0.0", reason="pytest >= 8.0.0 raises an extra warning for this test")
 def test_eve():
-    # Test an EVE TimeSeries
-    with pytest.warns(SunpyUserWarning, match='Unknown units for x_cool proxy'):
-        ts_eve = sunpy.timeseries.TimeSeries(eve_filepath, source='EVE')
+    with pytest.warns(SunpyUserWarning, match='Unknown units for oldXRSB proxy'):
+        with pytest.warns(SunpyUserWarning, match='Unknown units for x_cool'):
+            ts_eve = sunpy.timeseries.TimeSeries(eve_filepath, source='EVE')
     assert isinstance(ts_eve, sunpy.timeseries.sources.eve.EVESpWxTimeSeries)
 
 
 def test_implicit_esp():
     # Test an ESP TimeSeries
     ts_esp = sunpy.timeseries.TimeSeries(esp_filepath)
     assert isinstance(ts_esp, sunpy.timeseries.sources.eve.ESPTimeSeries)
```

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_fermi_gbm.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_fermi_gbm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_goes.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_goes.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_lyra.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_lyra.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_noaa.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_noaa.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_norh.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_norh.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/sources/tests/test_rhessi.py` & `sunpy-5.1.2/sunpy/timeseries/sources/tests/test_rhessi.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/tests/test_timeseries_factory.py` & `sunpy-5.1.2/sunpy/timeseries/tests/test_timeseries_factory.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/tests/test_timeseriesbase.py` & `sunpy-5.1.2/sunpy/timeseries/tests/test_timeseriesbase.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/tests/test_timeseriesmetadata.py` & `sunpy-5.1.2/sunpy/timeseries/tests/test_timeseriesmetadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/timeseries_factory.py` & `sunpy-5.1.2/sunpy/timeseries/timeseries_factory.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/timeseries/timeseriesbase.py` & `sunpy-5.1.2/sunpy/timeseries/timeseriesbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,15 +853,15 @@
     def to_array(self, **kwargs):
         """
         Return a `numpy.array` of the given `~sunpy.timeseries.TimeSeries`.
 
         Parameters
         ----------
         **kwargs : `dict`
-            All keyword arguments are passed to `pandas.DataFrame.to_numpy`.
+            All keyword arguments are passed to ``pandas.DataFrame.to_numpy``.
 
         Returns
         -------
         `~numpy.ndarray`
             If the data is heterogeneous and contains booleans or objects, the result will be of ``dtype=object``.
         """
         if hasattr(self._data, "to_numpy"):
```

### Comparing `sunpy-5.1.1/sunpy/util/config.py` & `sunpy-5.1.2/sunpy/util/config.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/datatype_factory_base.py` & `sunpy-5.1.2/sunpy/util/datatype_factory_base.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/decorators.py` & `sunpy-5.1.2/sunpy/util/decorators.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/exceptions.py` & `sunpy-5.1.2/sunpy/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/functools.py` & `sunpy-5.1.2/sunpy/util/functools.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/io.py` & `sunpy-5.1.2/sunpy/util/io.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/logger.py` & `sunpy-5.1.2/sunpy/util/logger.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/metadata.py` & `sunpy-5.1.2/sunpy/util/metadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/net.py` & `sunpy-5.1.2/sunpy/util/net.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/parfive_helpers.py` & `sunpy-5.1.2/sunpy/util/parfive_helpers.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/sphinx/__init__.py` & `sunpy-5.1.2/sunpy/util/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/sphinx/doctest.py` & `sunpy-5.1.2/sunpy/util/sphinx/doctest.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/sphinx/generate.py` & `sunpy-5.1.2/sunpy/util/sphinx/generate.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/sysinfo.py` & `sunpy-5.1.2/sunpy/util/sysinfo.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_config.py` & `sunpy-5.1.2/sunpy/util/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_datatype_factory_base.py` & `sunpy-5.1.2/sunpy/util/tests/test_datatype_factory_base.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_decorators.py` & `sunpy-5.1.2/sunpy/util/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_functools.py` & `sunpy-5.1.2/sunpy/util/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_logger.py` & `sunpy-5.1.2/sunpy/util/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_metadata.py` & `sunpy-5.1.2/sunpy/util/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_net.py` & `sunpy-5.1.2/sunpy/util/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_sysinfo.py` & `sunpy-5.1.2/sunpy/util/tests/test_sysinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     system_info,
 )
 
 
 def test_find_dependencies():
     missing, installed = find_dependencies()
     assert missing == {}
-    assert sorted(list(installed.keys())) == sorted(["astropy", "numpy", "packaging", "parfive"])
+    assert sorted(list(installed.keys())) == sorted(["astropy", "numpy", "packaging", "parfive", 'pyerfa'])
 
     missing, installed = find_dependencies(package="sunpy", extras=["required", "all"])
     assert missing == {}
     assert sorted(list(installed.keys())) == sorted(['asdf',
                                                      'asdf-astropy',
                                                      'astropy',
                                                      'numpy',
@@ -33,14 +33,15 @@
                                                      'reproject',
                                                      'beautifulsoup4',
                                                      'drms',
                                                      'python-dateutil',
                                                      'tqdm',
                                                      'zeep',
                                                      'cdflib',
+                                                     'pyerfa',
                                                      'h5netcdf',
                                                      'h5py',
                                                      'pandas'])
 
 
 def test_missing_dependencies_by_extra():
     missing = missing_dependencies_by_extra()
```

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_util.py` & `sunpy-5.1.2/sunpy/util/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/tests/test_xml.py` & `sunpy-5.1.2/sunpy/util/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/util/util.py` & `sunpy-5.1.2/sunpy/util/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 This module provides general utility functions.
 """
 import os
 import hashlib
 import inspect
+import textwrap
 from io import BytesIO
 from base64 import b64encode
 from shutil import get_terminal_size
 from itertools import chain, count
 from collections import UserList
 
 __all__ = ['unique', 'replacement_filename', 'expand_list',
            'expand_list_generator', 'dict_keys_same', 'hash_file', 'get_width',
-           'get_keywords', 'get_set_methods']
-
+           'get_keywords', 'get_set_methods', 'fix_duplicate_notes']
 
 def unique(itr, key=None):
     """
     Return only unique elements of a sequence.
 
     Parameters
     ----------
@@ -276,7 +276,44 @@
 
 
 def _figure_to_base64(fig):
     # Converts a matplotlib Figure to a base64 UTF-8 string
     buf = BytesIO()
     fig.savefig(buf, format='png', facecolor='none')  # works better than transparent=True
     return b64encode(buf.getvalue()).decode('utf-8')
+
+
+def fix_duplicate_notes(subclass_doc, cls_doc):
+    """
+    Returns a new documentation string such that there are notes section duplication in in `~sunpy.map.Map` subclasses.
+
+    Parameters
+    ----------
+    subclass_doc : str
+        The documentation that needs to be appended.
+    cls_doc
+        The original class's documentation.
+
+    Returns
+    -------
+    str
+        Updated documentation that contains no note section duplication.
+    """
+    existing_notes_pos = cls_doc.find('Notes\n    -----')
+    subclass_notes_pos = subclass_doc.find('Notes\n-----')
+    subclass_notes_data = textwrap.indent(subclass_doc[subclass_notes_pos + len('Notes\n-----'):].strip(), "    ")
+    references_pattern = "References\n    ----------"
+    examples_pattern = "Examples\n   -------"
+    start_index = cls_doc.find(references_pattern if references_pattern in cls_doc else examples_pattern)
+    if start_index!=-1:
+        next_pattern_pos = min(pos for pos in [cls_doc.find(references_pattern, start_index), cls_doc.find(examples_pattern, start_index)] if pos != -1)
+        other_patterns = cls_doc[:next_pattern_pos]
+        if existing_notes_pos!=-1:
+            cls_doc = other_patterns + subclass_notes_data.lstrip() + '\n\n    ' + cls_doc[next_pattern_pos:]
+        else:
+            cls_doc = other_patterns + 'Notes\n    -----\n' + subclass_notes_data + '\n\n    ' + cls_doc[next_pattern_pos:]
+    elif existing_notes_pos != -1:
+        cls_doc +="\n"+subclass_notes_data
+    else:
+        cls_doc += textwrap.indent(subclass_doc, "    ")
+
+    return cls_doc
```

### Comparing `sunpy-5.1.1/sunpy/util/xml.py` & `sunpy-5.1.2/sunpy/util/xml.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/version.py` & `sunpy-5.1.2/sunpy/version.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/animator/mapsequenceanimator.py` & `sunpy-5.1.2/sunpy/visualization/animator/mapsequenceanimator.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/animator/tests/test_mapsequenceanimator.py` & `sunpy-5.1.2/sunpy/visualization/animator/tests/test_mapsequenceanimator.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/cm.py` & `sunpy-5.1.2/sunpy/visualization/colormaps/cm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/color_tables.py` & `sunpy-5.1.2/sunpy/visualization/colormaps/color_tables.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_blue.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_blue.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_green.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_green.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_dark_red.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_dark_red.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/eit_yellow.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/eit_yellow.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_171.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_171.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_195.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_195.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_284.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_284.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/euvi_304.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/euvi_304.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/grayscale.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/grayscale.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/hi1.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/hi1.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/hi2.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/hi2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/hmi_mag.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/hmi_mag.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/idl_3.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/idl_3.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/lasco_c2.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/lasco_c2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/lasco_c3.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/lasco_c3.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/rhessi.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/rhessi.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/std_gamma_2.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/std_gamma_2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/stereo_cor1.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/stereo_cor1.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/stereo_cor2.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/stereo_cor2.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1216.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1216.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1550.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1550.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1600.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1600.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_1700.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_1700.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_171.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_171.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_195.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_195.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/data/trace_284.csv` & `sunpy-5.1.2/sunpy/visualization/colormaps/data/trace_284.csv`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/colormaps/tests/test_cm.py` & `sunpy-5.1.2/sunpy/visualization/colormaps/tests/test_cm.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/drawing.py` & `sunpy-5.1.2/sunpy/visualization/drawing.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/tests/test_drawing.py` & `sunpy-5.1.2/sunpy/visualization/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/visualization.py` & `sunpy-5.1.2/sunpy/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy/visualization/wcsaxes_compat.py` & `sunpy-5.1.2/sunpy/visualization/wcsaxes_compat.py`

 * *Files identical despite different names*

### Comparing `sunpy-5.1.1/sunpy.egg-info/PKG-INFO` & `sunpy-5.1.2/sunpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy
-Version: 5.1.1
+Version: 5.1.2
 Summary: SunPy core package: Python for Solar Physics
 Home-page: https://sunpy.org
 Download-URL: https://pypi.org/project/sunpy/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/sunpy/
@@ -29,14 +29,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: astropy!=5.1.0,>=5.0.6
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: packaging>=19.0
 Requires-Dist: parfive[ftp]>=2.0.0
+Requires-Dist: pyerfa
 Provides-Extra: asdf
 Requires-Dist: asdf-astropy>=0.1.1; extra == "asdf"
 Requires-Dist: asdf>=2.8.0; extra == "asdf"
 Provides-Extra: dask
 Requires-Dist: dask[array]>=2021.4.0; extra == "dask"
 Provides-Extra: database
 Requires-Dist: sqlalchemy>=1.3.4; extra == "database"
@@ -272,65 +273,62 @@
 Requires-Dist: spiceypy; extra == "dev"
 Requires-Dist: sunpy-sphinx-theme>=2.0.0rc1; extra == "dev"
 Requires-Dist: sphinx-hoverxref; extra == "dev"
 
 *********
 ``sunpy``
 *********
-
 |SunPy Logo|
 
-+----------------------+----------------------+----------------------+
-| Release              | Development          | Community            |
-+======================+======================+======================+
-| |Latest PyPi         | |Python Versions|    | |Matrix Chat Room|   |
-| Version|             |                      |                      |
-+----------------------+----------------------+----------------------+
-| |Latest Conda        | |Project Status:     | |OpenAstronomy       |
-| Version|             | Active - The project | Discourse community| |
-|                      | has reached a        |                      |
-|                      | stable, usable state |                      |
-|                      | and is being         |                      |
-|                      | actively developed.| |                      |
-+----------------------+----------------------+----------------------+
-| |Zenodo - Latest     | |Continuous          | |Google Groups       |
-| DOI|                 | Integration Status|  | Mailing List|        |
-+----------------------+----------------------+----------------------+
-| |sunpy Stable        | |CodeCov Code        | |Powered by          |
-| Documentation|       | Coverage|            | NumFOCUS|            |
-+----------------------+----------------------+----------------------+
++-----------------------------------+-----------------------------------+-----------------------------------+
+|           Release                 |           Development             |           Community               |
++===================================+===================================+===================================+
+|       |Latest PyPi Version|       |        |Python Versions|          |         |Matrix Chat Room|        |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|     |Latest Conda Version|        |     |Project Status: Active|      |     |OpenAstronomy Discourse|     |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|      |Zenodo - Latest DOI|        |  |Continuous Integration Status|  |    |Google Groups Mailing List|   |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|    |sunpy stable documentation|   |     |CodeCov Code Coverage|       |       |Powered by NumFOCUS|       |
++-----------------------------------+-----------------------------------+-----------------------------------+
+|         |sunpy citation|          |                                   |            |pyOpenSci|            |
++-----------------------------------+-----------------------------------+-----------------------------------+
 
-.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/sunpy_logo_landscape.svg
+.. |SunPy Logo| image:: https://raw.githubusercontent.com/sunpy/sunpy-logo/master/generated/sunpy_logo_landscape.png
    :width: 200px
 .. |Latest PyPi Version| image:: https://img.shields.io/pypi/v/sunpy.svg
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/sunpy
    :target: https://pypi.python.org/pypi/sunpy/
 .. |Matrix Chat Room| image:: https://img.shields.io/matrix/sunpy:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=matrix.org
    :target: https://app.element.io/#/room/#sunpy:openastronomy.org
 .. |Latest Conda Version| image:: https://anaconda.org/conda-forge/sunpy/badges/version.svg
    :target: https://anaconda.org/conda-forge/sunpy
-.. |Project Status: Active - The project has reached a stable, usable state and is being actively developed.| image:: https://www.repostatus.org/badges/latest/active.svg
+.. |Project Status: Active| image:: https://www.repostatus.org/badges/latest/active.svg
    :target: https://www.repostatus.org/#active
-.. |OpenAstronomy Discourse community| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
+.. |OpenAstronomy Discourse| image:: https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/try2/original/1X/5e1e3b3cada2d7fbae4734d4bc53999933d71c95.svg
    :height: 20px
    :target: https://community.openastronomy.org/
 .. |Zenodo - Latest DOI| image:: https://zenodo.org/badge/2165383.svg
    :target: https://zenodo.org/badge/latestdoi/2165383
 .. |Continuous Integration Status| image:: https://github.com/sunpy/sunpy/actions/workflows/ci.yml/badge.svg?branch=main
    :target: https://github.com/sunpy/sunpy/actions/workflows/ci.yml
-.. |Google Groups Mailing List| image:: https://fonts.gstatic.com/s/i/productlogos/groups/v9/web-48dp/logo_groups_color_1x_web_48dp.png
+.. |Google Groups Mailing List| image:: https://upload.wikimedia.org/wikipedia/commons/2/27/Google_Groups_logo.gif
    :height: 20px
    :target: https://groups.google.com/g/sunpy
-.. |sunpy Stable Documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
+.. |sunpy stable documentation| image:: https://readthedocs.org/projects/sunpy/badge/?version=stable
    :target: https://docs.sunpy.org/
 .. |CodeCov Code Coverage| image:: https://codecov.io/gh/sunpy/sunpy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
+.. |sunpy citation| image:: https://img.shields.io/badge/cite-sunpy-orange
+   :target: https://docs.sunpy.org/en/stable/citation.html
+.. |pyOpenSci| image:: https://tinyurl.com/y22nb8up
+   :target: https://github.com/pyOpenSci/software-submission/issues/147
 
 ``sunpy`` is a Python software package that provides fundamental tools for accessing, loading and interacting with solar physics data in Python.
 It includes an interface for searching and downloading data from multiple data providers, data containers for image and time series data, commonly used solar coordinate frames and associated transformations, as well as other functionality needed for solar data analysis.
 
 Installation
 ============
```

### Comparing `sunpy-5.1.1/sunpy.egg-info/SOURCES.txt` & `sunpy-5.1.2/sunpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 docs/dev_guide/contents/images/checks.png
 docs/dev_guide/contents/images/checks_pr.png
 docs/how_to/coord_components.rst
 docs/how_to/create_a_map.rst
 docs/how_to/create_coords.rst
 docs/how_to/create_custom_map.rst
 docs/how_to/create_custom_timeseries.rst
+docs/how_to/fix_map_metadata.rst
 docs/how_to/index.rst
 docs/how_to/parse_time.rst
 docs/how_to/remote_data_manager.rst
 docs/how_to/search_multiple_wavelengths.rst
 docs/how_to/search_vso.rst
 docs/how_to/transform_coords.rst
 docs/reference/customization.rst
```

### Comparing `sunpy-5.1.1/sunpy.egg-info/requires.txt` & `sunpy-5.1.2/sunpy.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 astropy!=5.1.0,>=5.0.6
 numpy>=1.21.0
 packaging>=19.0
 parfive[ftp]>=2.0.0
+pyerfa
 
 [all]
 asdf-astropy>=0.1.1
 asdf>=2.8.0
 dask[array]>=2021.4.0
 sqlalchemy>=1.3.4
 scikit-image>=0.18.0
```

