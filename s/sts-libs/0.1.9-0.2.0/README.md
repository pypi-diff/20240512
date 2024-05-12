# Comparing `tmp/sts_libs-0.1.9.tar.gz` & `tmp/sts_libs-0.2.0.tar.gz`

## Comparing `sts_libs-0.1.9.tar` & `sts_libs-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 sts_libs-0.1.9/.gitlab-ci.yml
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 sts_libs-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 sts_libs-0.1.9/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.1.9/noxfile.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.1.9/.fmf/version
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 sts_libs-0.1.9/docs/contributing.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/main.fmf
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/be2iscsi.fmf
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/bnx2i.fmf
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/cxgb4i.fmf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/local.fmf
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/qedi.fmf
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/tier0.fmf
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/iscsi/libiscsi/main.fmf
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/rdma/main.fmf
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/rdma/regression.fmf
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sts_libs-0.1.9/plans/rdma/test_case_vars.yaml
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 sts_libs-0.1.9/scripts/install-python.sh
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/blockdevice.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    52263 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    73709 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    41772 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/nvme.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/rdma.py
--rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fixtures/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fixtures/common_fixtures.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fixtures/iscsi_fixtures.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fixtures/rdma_fixtures.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/fixtures/stratis_fixtures.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/log.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/conftest.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/pytest.ini
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/main.fmf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/_vars/be2iscsi.yaml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/_vars/bnx2i.yaml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/_vars/cxgb4i.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/_vars/qedi.yaml
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/_vars/template_iscsi_host.yaml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/libiscsi/main.fmf
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/libiscsi/local/libiscsi-local.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/libiscsi/local/main.fmf
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/login-logout-stress/login-logout-stress.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/login-logout-stress/main.fmf
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/many-luns/main.fmf
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/many-luns/many-luns-local.py
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/parameters/iscsi_params.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/iscsi/parameters/main.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/main.fmf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/main.fmf
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/customers/main.fmf
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/customers/customer_1/issue_23967_verify_speed.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/customers/customer_1/main.fmf
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/others/main.fmf
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/bugs/others/reproducers.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/pyverbs-tests/core/main.fmf
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/pyverbs-tests/core/pyverbs-tests.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/sriov/core/main.fmf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/rdma/sriov/core/sriov.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/stratis/main.fmf
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/stratis/pool_create_destroy/main.fmf
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 sts_libs-0.1.9/tests/stratis/pool_create_destroy/test_pool.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.1.9/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.1.9/LICENSE
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 sts_libs-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 sts_libs-0.1.9/sts_libs/README.md
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 sts_libs-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 sts_libs-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 sts_libs-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 sts_libs-0.2.0/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.2.0/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.2.0/.fmf/version
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 sts_libs-0.2.0/docs/contributing.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/main.fmf
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/be2iscsi.fmf
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/bnx2i.fmf
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/cxgb4i.fmf
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/intel.fmf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/local.fmf
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/qedi.fmf
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/tier0.fmf
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/rdma/main.fmf
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/rdma/regression.fmf
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sts_libs-0.2.0/plans/rdma/test_case_vars.yaml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/blockdevice.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    52298 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    38862 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    73709 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    41772 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/nvme.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/rdma.py
+-rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fixtures/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fixtures/common_fixtures.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fixtures/iscsi_fixtures.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fixtures/rdma_fixtures.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/fixtures/stratis_fixtures.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/pytest.ini
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/main.fmf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/be2iscsi.yaml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/bnx2i.yaml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/cxgb4i.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/intel.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/qedi.yaml
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/_vars/template_iscsi_host.yaml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/libiscsi/local/libiscsi-local.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/libiscsi/local/main.fmf
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/login-logout-stress/login-logout-stress.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/login-logout-stress/main.fmf
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/many-luns/main.fmf
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/many-luns/many-luns-local.py
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/parameters/iscsi_params.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/iscsi/parameters/main.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/main.fmf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/main.fmf
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/customers/main.fmf
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/customers/customer_1/issue_23967_verify_speed.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/customers/customer_1/main.fmf
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/others/main.fmf
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/bugs/others/reproducers.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/pyverbs-tests/core/main.fmf
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/pyverbs-tests/core/pyverbs-tests.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/sriov/core/main.fmf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/rdma/sriov/core/sriov.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/stratis/main.fmf
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/stratis/pool_create_destroy/main.fmf
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 sts_libs-0.2.0/tests/stratis/pool_create_destroy/test_pool.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 sts_libs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 sts_libs-0.2.0/sts_libs/README.md
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 sts_libs-0.2.0/PKG-INFO
```

### Comparing `sts_libs-0.1.9/.gitlab-ci.yml` & `sts_libs-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/.pre-commit-config.yaml` & `sts_libs-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/README.md` & `sts_libs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/noxfile.py` & `sts_libs-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/docs/contributing.md` & `sts_libs-0.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/plans/rdma/regression.fmf` & `sts_libs-0.2.0/plans/rdma/regression.fmf`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/blockdevice.py` & `sts_libs-0.2.0/sts_libs/src/sts/blockdevice.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/dm.py` & `sts_libs-0.2.0/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/dmpd.py` & `sts_libs-0.2.0/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/fc.py` & `sts_libs-0.2.0/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/fio.py` & `sts_libs-0.2.0/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/iscsi.py` & `sts_libs-0.2.0/sts_libs/src/sts/iscsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1483,22 +1483,22 @@
     if not iface_name:
         logging.error('create_iscsi_iface() - requires iface name as parameter')
         return False
 
     if iface_name in get_iscsi_iface_names():
         logging.info(f'iSCSI interface {iface_name} already exists')
         return True
+
     iscsiadm = IscsiAdm()
-    retcode, output = iscsiadm.iface(op='new', iface=iface_name)
-    if retcode != 0:
+    if not iscsiadm.iface(op='new', iface=iface_name).succeeded:
         logging.error('Could not create iSCSI interface')
-        print(output)
         return False
 
-    if mac is not None and not iscsiadm.iface_update(iface=iface_name, name='iface.hwaddress', value=mac):
+    if mac and not iscsiadm.iface_update(iface=iface_name, name='iface.hwaddress', value=mac).succeeded:
+        logging.error('Unable to assign mac to newly created iSCSI interface')
         return False
 
     return True
 
 
 def clone_iscsi_iface(new_iface_name, base_iface):  # noqa: ANN001, ANN201
     print(f'Cloning iface: {base_iface} to {new_iface_name}')
```

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/linux.py` & `sts_libs-0.2.0/sts_libs/src/sts/linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1023,17 +1023,23 @@
         return False
 
     return True
 
 
 def in_container() -> bool:
     """Check if we are running inside container."""
-    if run('cat /proc/1/attr/current | grep container_t').rc == 0:
-        return True
-    if run('cat /proc/self/cgroup | grep docker').rc == 0:
+    try:
+        proc_current = Path('/proc/1/attr/current').read_text()
+        # Check for unconfined, which can be found in gitlab ci
+        if 'container_t' in proc_current or 'unconfined' in proc_current:
+            return True
+        if 'docker' in Path('/proc/self/cgroup').read_text():
+            return True
+    except PermissionError:
+        logging.info('Assuming containerized environment')
         return True
     return False
 
 
 def get_memory(units='m', total=False):  # noqa: ANN001, ANN201
     """Returns data from 'free' as a dict."""
     possible_units = 'b bytes k kilo m mega  g giga tera peta'.split()
```

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/lio.py` & `sts_libs-0.2.0/sts_libs/src/sts/lio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/loopdev.py` & `sts_libs-0.2.0/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/lsm.py` & `sts_libs-0.2.0/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/lvm.py` & `sts_libs-0.2.0/sts_libs/src/sts/lvm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/md.py` & `sts_libs-0.2.0/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/mp.py` & `sts_libs-0.2.0/sts_libs/src/sts/mp.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/net.py` & `sts_libs-0.2.0/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/nvme.py` & `sts_libs-0.2.0/sts_libs/src/sts/nvme.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.2.0/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/rdma.py` & `sts_libs-0.2.0/sts_libs/src/sts/rdma.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/scsi.py` & `sts_libs-0.2.0/sts_libs/src/sts/scsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.2.0/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/stratis.py` & `sts_libs-0.2.0/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/vdo.py` & `sts_libs-0.2.0/sts_libs/src/sts/vdo.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/fixtures/iscsi_fixtures.py` & `sts_libs-0.2.0/sts_libs/src/sts/fixtures/iscsi_fixtures.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/fixtures/rdma_fixtures.py` & `sts_libs-0.2.0/sts_libs/src/sts/fixtures/rdma_fixtures.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/fixtures/stratis_fixtures.py` & `sts_libs-0.2.0/sts_libs/src/sts/fixtures/stratis_fixtures.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/logchecker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/size.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.2.0/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/cmdline_test.py` & `sts_libs-0.2.0/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/fio_test.py` & `sts_libs-0.2.0/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/iscsi_test.py` & `sts_libs-0.2.0/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/linux_test.py` & `sts_libs-0.2.0/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/logchecker_test.py` & `sts_libs-0.2.0/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/lvm_test.py` & `sts_libs-0.2.0/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/md_test.py` & `sts_libs-0.2.0/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/net_test.py` & `sts_libs-0.2.0/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.2.0/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/sts_libs/tests/scsi_test.py` & `sts_libs-0.2.0/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/_vars/template_iscsi_host.yaml` & `sts_libs-0.2.0/tests/iscsi/_vars/template_iscsi_host.yaml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/libiscsi/local/libiscsi-local.py` & `sts_libs-0.2.0/tests/iscsi/libiscsi/local/libiscsi-local.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/login-logout-stress/login-logout-stress.py` & `sts_libs-0.2.0/tests/iscsi/login-logout-stress/login-logout-stress.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/many-luns/many-luns-local.py` & `sts_libs-0.2.0/tests/iscsi/many-luns/many-luns-local.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/parameters/iscsi_params.py` & `sts_libs-0.2.0/tests/iscsi/parameters/iscsi_params.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/iscsi/parameters/main.fmf` & `sts_libs-0.2.0/tests/iscsi/parameters/main.fmf`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/rdma/bugs/others/reproducers.py` & `sts_libs-0.2.0/tests/rdma/bugs/others/reproducers.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     def test_23034_warnings_speed_unknown() -> None:
         """Verify no unexpected warning message is shown.
 
         When a multiple port adapter has one port connected and one not connected,
         running ibv_devinfo will trigger a similar message:<port> speed is unknown, defaulting to 1000.
         """
         warning_msg = '"speed is unknown, defaulting to 1000"'
-        assert run(f'dmesg | grep {warning_msg}').exit_status == 1
+        assert run(f'dmesg -c | grep {warning_msg}').exit_status == 1
         run('ibv_devinfo')
-        assert run(f'dmesg | grep {warning_msg}').exit_status == 1
+        assert run(f'dmesg -c | grep {warning_msg}').exit_status == 1
```

### Comparing `sts_libs-0.1.9/tests/rdma/pyverbs-tests/core/pyverbs-tests.py` & `sts_libs-0.2.0/tests/rdma/pyverbs-tests/core/pyverbs-tests.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/rdma/sriov/core/sriov.py` & `sts_libs-0.2.0/tests/rdma/sriov/core/sriov.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/tests/stratis/pool_create_destroy/test_pool.py` & `sts_libs-0.2.0/tests/stratis/pool_create_destroy/test_pool.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/.gitignore` & `sts_libs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/LICENSE` & `sts_libs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/pyproject.toml` & `sts_libs-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,22 @@
   "ruff",
   "mypy",
   "pre-commit",
 ]
 
 [tool.hatch.envs.default.scripts]
 # TODO use pytest-container
-container-prep = 'buildah from --name fedora-sts fedora && buildah run fedora-sts dnf install -y python3-pip'
-tests = 'buildah copy fedora-sts ../sts sts && buildah run fedora-sts pip install sts/ && buildah run fedora-sts pytest sts/sts_libs/tests/'
+container-prep = """\
+  buildah from --name fedora-sts fedora &&\
+  buildah run fedora-sts dnf install -y python3-pip &&\
+  buildah config --env SETUPTOOLS_SCM_PRETEND_VERSION="0.0.1" fedora-sts &&\
+  buildah copy fedora-sts ../sts sts &&\
+  buildah run fedora-sts python3 -m pip install -e sts\
+  """
+tests = 'buildah copy fedora-sts ../sts sts && buildah run fedora-sts pytest sts/sts_libs/tests/'
 format = ['ruff check --fix', 'ruff format']
 lint = ['ruff check', 'ruff format --check']
 check = 'mypy {args:.}'
 all = ['format', 'lint', 'check', 'tests']
 
 [tool.ruff]
 line-length = 120
```

### Comparing `sts_libs-0.1.9/sts_libs/README.md` & `sts_libs-0.2.0/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.9/PKG-INFO` & `sts_libs-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sts-libs
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library for pytest-based Linux storage tests
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Zhaojuan Guo <zguo@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>, Jakub Krysl <jkrysl@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
```

