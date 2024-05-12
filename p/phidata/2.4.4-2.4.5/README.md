# Comparing `tmp/phidata-2.4.4.tar.gz` & `tmp/phidata-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.4.4.tar", last modified: Thu May  9 22:24:31 2024, max compression
+gzip compressed data, was "phidata-2.4.5.tar", last modified: Sun May 12 10:29:15 2024, max compression
```

## Comparing `phidata-2.4.4.tar` & `phidata-2.4.5.tar`

### file list

```diff
@@ -1,634 +1,636 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.029963 phidata-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-09 22:24:17.000000 phidata-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-09 22:24:31.029963 phidata-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-09 22:24:17.000000 phidata-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.953962 phidata-2.4.4/phi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.953962 phidata-2.4.4/phi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.957962 phidata-2.4.4/phi/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/schemas/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.957962 phidata-2.4.4/phi/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/app/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/app/db_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.957962 phidata-2.4.4/phi/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67323 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.957962 phidata-2.4.4/phi/assistant/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/assistant/openai/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/file/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/file/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/file/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/row.py
--rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/assistant/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.961962 phidata-2.4.4/phi/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.965962 phidata-2.4.4/phi/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/glue/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/s3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/cli/k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/k/k_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.969962 phidata-2.4.4/phi/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/cli/ws/ws_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/ollama/ollama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.973962 phidata-2.4.4/phi/docker/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/app/whoami/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/whoami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/app/whoami/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resource/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/docker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.977962 phidata-2.4.4/phi/document/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/document/reader/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/firecrawl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/document/reader/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/document/reader/website.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/anyscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/fireworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/together.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/embedder/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/file/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/file/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/file/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/file/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/file/local/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.981962 phidata-2.4.4/phi/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/infra/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/infra/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.985962 phidata-2.4.4/phi/k8s/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/app/traefik/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.989962 phidata-2.4.4/phi/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/crb/eks_admin_crb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.993962 phidata-2.4.4/phi/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/enums/volume_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/helm/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/helm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:30.997962 phidata-2.4.4/phi/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.001963 phidata-2.4.4/phi/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resource/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/llamaindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/knowledge/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/s3/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/website.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/knowledge/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/llm/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/anthropic/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/llm/anyscale/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/anyscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/anyscale/anyscale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.005962 phidata-2.4.4/phi/llm/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/aws/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/aws/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/azure/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/cohere/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/cohere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/cohere/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/fireworks/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/fireworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/fireworks/fireworks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/gemini/gemini.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/groq/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/groq/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/mistral/mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20162 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/ollama/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/ollama/hermes.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/ollama/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/ollama/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/openai/like.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/openrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/openrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/openrouter/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/llm/together/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/together/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/llm/together/together.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.009963 phidata-2.4.4/phi/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/memory/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/prompt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/prompt/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/prompt/template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/storage/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/assistant/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/assistant/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/assistant/singlestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/storage/assistant/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/table/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/table/sql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.013963 phidata-2.4.4/phi/task/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.017963 phidata-2.4.4/phi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/apify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/arxiv_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/exa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.017963 phidata-2.4.4/phi/tools/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/fastapi/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/newspaper4k.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/newspaper_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/openbb_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/phi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/resend_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/serpapi_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.017963 phidata-2.4.4/phi/tools/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/streamlit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/tavily.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/tool_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/yfinance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/youtube_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/tools/zendesk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.021963 phidata-2.4.4/phi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/format_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/py_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/response_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/lancedb/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/lancedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/lancedb/lancedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/pgvector/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pgvector/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pgvector/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pgvector/pgvector2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/pineconedb/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pineconedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/pineconedb/pineconedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/vectordb/singlestore/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/singlestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/singlestore/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/vectordb/singlestore/s2vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.025963 phidata-2.4.4/phi/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-09 22:24:17.000000 phidata-2.4.4/phi/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.029963 phidata-2.4.4/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 22:24:30.000000 phidata-2.4.4/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-09 22:24:17.000000 phidata-2.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:24:31.029963 phidata-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-09 22:24:17.000000 phidata-2.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:24:31.029963 phidata-2.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 22:24:17.000000 phidata-2.4.4/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.319842 phidata-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-12 10:29:02.000000 phidata-2.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-12 10:29:15.319842 phidata-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-12 10:29:02.000000 phidata-2.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.239843 phidata-2.4.5/phi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.239843 phidata-2.4.5/phi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.239843 phidata-2.4.5/phi/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/schemas/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.243843 phidata-2.4.5/phi/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/app/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/app/db_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.243843 phidata-2.4.5/phi/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67323 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.243843 phidata-2.4.5/phi/assistant/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.243843 phidata-2.4.5/phi/assistant/openai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/file/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/file/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/assistant/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.243843 phidata-2.4.5/phi/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.247843 phidata-2.4.5/phi/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.251843 phidata-2.4.5/phi/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/glue/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/s3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/aws/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.255843 phidata-2.4.5/phi/cli/k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/k/k_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.259843 phidata-2.4.5/phi/docker/app/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/ollama/ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/app/whoami/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/whoami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/app/whoami/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.263843 phidata-2.4.5/phi/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resource/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/docker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.267843 phidata-2.4.5/phi/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.267843 phidata-2.4.5/phi/document/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/firecrawl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.267843 phidata-2.4.5/phi/document/reader/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/document/reader/website.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.267843 phidata-2.4.5/phi/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/anyscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/fireworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/embedder/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.267843 phidata-2.4.5/phi/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/file/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/file/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/file/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/file/local/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/infra/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/infra/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/k8s/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/k8s/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/k8s/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.271843 phidata-2.4.5/phi/k8s/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/app/traefik/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.275843 phidata-2.4.5/phi/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/crb/eks_admin_crb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.279843 phidata-2.4.5/phi/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/enums/volume_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/helm/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/helm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.283843 phidata-2.4.5/phi/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.287843 phidata-2.4.5/phi/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.287843 phidata-2.4.5/phi/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.287843 phidata-2.4.5/phi/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.291843 phidata-2.4.5/phi/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resource/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/llamaindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/knowledge/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/knowledge/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/anthropic/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/anyscale/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/anyscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/anyscale/anyscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/aws/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/aws/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/azure/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/cohere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/cohere/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.295843 phidata-2.4.5/phi/llm/fireworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/fireworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/fireworks/fireworks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/gemini/gemini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/groq/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/mistral/mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20162 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/ollama/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/ollama/hermes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/ollama/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/ollama/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/openai/like.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/openrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/openrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/openrouter/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/llm/together/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/together/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/llm/together/together.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/memory/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.299842 phidata-2.4.5/phi/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/prompt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/prompt/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/prompt/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/storage/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/assistant/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/assistant/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/assistant/singlestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/storage/assistant/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/table/sql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.303842 phidata-2.4.5/phi/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.307842 phidata-2.4.5/phi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/apify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/arxiv_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/exa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.307842 phidata-2.4.5/phi/tools/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/fastapi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/hackernews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/newspaper4k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/newspaper_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/openbb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/phi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/resend_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/serpapi_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.307842 phidata-2.4.5/phi/tools/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/streamlit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/tavily.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/tool_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/yfinance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/youtube_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/tools/zendesk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.311842 phidata-2.4.5/phi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/format_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/py_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/response_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/lancedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/lancedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/lancedb/lancedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pgvector/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pgvector/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pgvector/pgvector2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/pineconedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pineconedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/pineconedb/pineconedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/vectordb/singlestore/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/singlestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/singlestore/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/vectordb/singlestore/s2vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.315842 phidata-2.4.5/phi/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-12 10:29:02.000000 phidata-2.4.5/phi/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.319842 phidata-2.4.5/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 10:29:15.000000 phidata-2.4.5/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-12 10:29:02.000000 phidata-2.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 10:29:15.319842 phidata-2.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-12 10:29:02.000000 phidata-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:29:15.319842 phidata-2.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 10:29:02.000000 phidata-2.4.5/tests/test_placeholder.py
```

### Comparing `phidata-2.4.4/LICENSE` & `phidata-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/PKG-INFO` & `phidata-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.4.4
+Version: 2.4.5
 Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phidata-2.4.4/README.md` & `phidata-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/api.py` & `phidata-2.4.5/phi/api/api.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/assistant.py` & `phidata-2.4.5/phi/api/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/prompt.py` & `phidata-2.4.5/phi/api/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/routes.py` & `phidata-2.4.5/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/schemas/prompt.py` & `phidata-2.4.5/phi/api/schemas/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/schemas/workspace.py` & `phidata-2.4.5/phi/api/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/user.py` & `phidata-2.4.5/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/api/workspace.py` & `phidata-2.4.5/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/app/base.py` & `phidata-2.4.5/phi/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/app/context.py` & `phidata-2.4.5/phi/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/app/db_app.py` & `phidata-2.4.5/phi/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/app/group.py` & `phidata-2.4.5/phi/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/assistant.py` & `phidata-2.4.5/phi/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/duckdb.py` & `phidata-2.4.5/phi/assistant/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/assistant.py` & `phidata-2.4.5/phi/assistant/openai/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/file/file.py` & `phidata-2.4.5/phi/assistant/openai/file/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/file/local.py` & `phidata-2.4.5/phi/assistant/openai/file/local.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/file/url.py` & `phidata-2.4.5/phi/assistant/openai/file/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/message.py` & `phidata-2.4.5/phi/assistant/openai/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/row.py` & `phidata-2.4.5/phi/assistant/openai/row.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/run.py` & `phidata-2.4.5/phi/assistant/openai/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/openai/thread.py` & `phidata-2.4.5/phi/assistant/openai/thread.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/python.py` & `phidata-2.4.5/phi/assistant/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/assistant/run.py` & `phidata-2.4.5/phi/assistant/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/api_client.py` & `phidata-2.4.5/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/base.py` & `phidata-2.4.5/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/django/django.py` & `phidata-2.4.5/phi/aws/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/fastapi/fastapi.py` & `phidata-2.4.5/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/jupyter/jupyter.py` & `phidata-2.4.5/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/qdrant/qdrant.py` & `phidata-2.4.5/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/app/streamlit/streamlit.py` & `phidata-2.4.5/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/acm/certificate.py` & `phidata-2.4.5/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/base.py` & `phidata-2.4.5/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/cloudformation/stack.py` & `phidata-2.4.5/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ec2/security_group.py` & `phidata-2.4.5/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ec2/subnet.py` & `phidata-2.4.5/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ec2/volume.py` & `phidata-2.4.5/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ecs/cluster.py` & `phidata-2.4.5/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ecs/container.py` & `phidata-2.4.5/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ecs/service.py` & `phidata-2.4.5/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ecs/task_definition.py` & `phidata-2.4.5/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/ecs/volume.py` & `phidata-2.4.5/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/eks/addon.py` & `phidata-2.4.5/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/eks/cluster.py` & `phidata-2.4.5/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.4.5/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.4.5/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/eks/node_group.py` & `phidata-2.4.5/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/elasticache/cluster.py` & `phidata-2.4.5/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.4.5/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/elb/listener.py` & `phidata-2.4.5/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/elb/load_balancer.py` & `phidata-2.4.5/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/elb/target_group.py` & `phidata-2.4.5/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/emr/cluster.py` & `phidata-2.4.5/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/glue/crawler.py` & `phidata-2.4.5/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/iam/policy.py` & `phidata-2.4.5/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/iam/role.py` & `phidata-2.4.5/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/rds/db_cluster.py` & `phidata-2.4.5/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/rds/db_instance.py` & `phidata-2.4.5/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.4.5/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/s3/bucket.py` & `phidata-2.4.5/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/s3/object.py` & `phidata-2.4.5/phi/aws/resource/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/secret/manager.py` & `phidata-2.4.5/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/secret/reader.py` & `phidata-2.4.5/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resource/types.py` & `phidata-2.4.5/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/aws/resources.py` & `phidata-2.4.5/phi/aws/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/base.py` & `phidata-2.4.5/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/auth_server.py` & `phidata-2.4.5/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/config.py` & `phidata-2.4.5/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/console.py` & `phidata-2.4.5/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/credentials.py` & `phidata-2.4.5/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/entrypoint.py` & `phidata-2.4.5/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/k/k_cli.py` & `phidata-2.4.5/phi/cli/k/k_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/operator.py` & `phidata-2.4.5/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/settings.py` & `phidata-2.4.5/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/cli/ws/ws_cli.py` & `phidata-2.4.5/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/constants.py` & `phidata-2.4.5/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/api_client.py` & `phidata-2.4.5/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/airflow/base.py` & `phidata-2.4.5/phi/docker/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/airflow/worker.py` & `phidata-2.4.5/phi/docker/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/base.py` & `phidata-2.4.5/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/django/django.py` & `phidata-2.4.5/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/fastapi/fastapi.py` & `phidata-2.4.5/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/jupyter/jupyter.py` & `phidata-2.4.5/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/mysql/mysql.py` & `phidata-2.4.5/phi/docker/app/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/postgres/postgres.py` & `phidata-2.4.5/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/qdrant/qdrant.py` & `phidata-2.4.5/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/redis/redis.py` & `phidata-2.4.5/phi/docker/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/streamlit/streamlit.py` & `phidata-2.4.5/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/superset/base.py` & `phidata-2.4.5/phi/docker/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/app/traefik/router.py` & `phidata-2.4.5/phi/docker/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/base.py` & `phidata-2.4.5/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/container.py` & `phidata-2.4.5/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/image.py` & `phidata-2.4.5/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/network.py` & `phidata-2.4.5/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/types.py` & `phidata-2.4.5/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resource/volume.py` & `phidata-2.4.5/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/docker/resources.py` & `phidata-2.4.5/phi/docker/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/base.py` & `phidata-2.4.5/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/arxiv.py` & `phidata-2.4.5/phi/document/reader/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/base.py` & `phidata-2.4.5/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/docx.py` & `phidata-2.4.5/phi/document/reader/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/firecrawl_reader.py` & `phidata-2.4.5/phi/document/reader/firecrawl_reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/json.py` & `phidata-2.4.5/phi/document/reader/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/pdf.py` & `phidata-2.4.5/phi/document/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/s3/pdf.py` & `phidata-2.4.5/phi/document/reader/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/s3/text.py` & `phidata-2.4.5/phi/document/reader/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/text.py` & `phidata-2.4.5/phi/document/reader/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/document/reader/website.py` & `phidata-2.4.5/phi/document/reader/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/embedder/mistral.py` & `phidata-2.4.5/phi/embedder/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/embedder/ollama.py` & `phidata-2.4.5/phi/embedder/ollama.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/embedder/openai.py` & `phidata-2.4.5/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/embedder/voyageai.py` & `phidata-2.4.5/phi/embedder/voyageai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/file/local/csv.py` & `phidata-2.4.5/phi/file/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/infra/resources.py` & `phidata-2.4.5/phi/infra/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/api_client.py` & `phidata-2.4.5/phi/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/airflow/base.py` & `phidata-2.4.5/phi/k8s/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/airflow/worker.py` & `phidata-2.4.5/phi/k8s/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/base.py` & `phidata-2.4.5/phi/k8s/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/fastapi/fastapi.py` & `phidata-2.4.5/phi/k8s/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/jupyter/jupyter.py` & `phidata-2.4.5/phi/k8s/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/postgres/postgres.py` & `phidata-2.4.5/phi/k8s/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/redis/redis.py` & `phidata-2.4.5/phi/k8s/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/streamlit/streamlit.py` & `phidata-2.4.5/phi/k8s/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/superset/base.py` & `phidata-2.4.5/phi/k8s/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/traefik/crds.py` & `phidata-2.4.5/phi/k8s/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/app/traefik/router.py` & `phidata-2.4.5/phi/k8s/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.5/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/apps/v1/deployment.py` & `phidata-2.4.5/phi/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/base.py` & `phidata-2.4.5/phi/k8s/create/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/common/port.py` & `phidata-2.4.5/phi/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/config_map.py` & `phidata-2.4.5/phi/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/container.py` & `phidata-2.4.5/phi/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/namespace.py` & `phidata-2.4.5/phi/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/persistent_volume.py` & `phidata-2.4.5/phi/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.4.5/phi/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/secret.py` & `phidata-2.4.5/phi/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/service.py` & `phidata-2.4.5/phi/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/service_account.py` & `phidata-2.4.5/phi/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/core/v1/volume.py` & `phidata-2.4.5/phi/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/crb/eks_admin_crb.py` & `phidata-2.4.5/phi/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.4.5/phi/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.5/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.5/phi/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/enums/api_version.py` & `phidata-2.4.5/phi/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/enums/kind.py` & `phidata-2.4.5/phi/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/enums/pv.py` & `phidata-2.4.5/phi/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/helm/chart.py` & `phidata-2.4.5/phi/k8s/helm/chart.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/helm/cli.py` & `phidata-2.4.5/phi/k8s/helm/cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/operator.py` & `phidata-2.4.5/phi/k8s/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.5/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/apps/v1/deployment.py` & `phidata-2.4.5/phi/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.4.5/phi/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/base.py` & `phidata-2.4.5/phi/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/config_map.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/container.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/namespace.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/node_selector.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/object_reference.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/pod.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/pod_spec.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/secret.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/service.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/service_account.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/toleration.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/volume.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/core/v1/volume_source.py` & `phidata-2.4.5/phi/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/kubeconfig.py` & `phidata-2.4.5/phi/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/meta/v1/label_selector.py` & `phidata-2.4.5/phi/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/meta/v1/object_meta.py` & `phidata-2.4.5/phi/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.4.5/phi/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.5/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.5/phi/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/types.py` & `phidata-2.4.5/phi/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resource/yaml.py` & `phidata-2.4.5/phi/k8s/resource/yaml.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/k8s/resources.py` & `phidata-2.4.5/phi/k8s/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/arxiv.py` & `phidata-2.4.5/phi/knowledge/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/base.py` & `phidata-2.4.5/phi/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/combined.py` & `phidata-2.4.5/phi/knowledge/combined.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/document.py` & `phidata-2.4.5/phi/knowledge/document.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/docx.py` & `phidata-2.4.5/phi/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/json.py` & `phidata-2.4.5/phi/knowledge/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/langchain.py` & `phidata-2.4.5/phi/knowledge/langchain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/llamaindex.py` & `phidata-2.4.5/phi/knowledge/llamaindex.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/pdf.py` & `phidata-2.4.5/phi/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/s3/base.py` & `phidata-2.4.5/phi/knowledge/s3/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/s3/pdf.py` & `phidata-2.4.5/phi/knowledge/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/s3/text.py` & `phidata-2.4.5/phi/knowledge/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/text.py` & `phidata-2.4.5/phi/knowledge/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/website.py` & `phidata-2.4.5/phi/knowledge/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/knowledge/wikipedia.py` & `phidata-2.4.5/phi/knowledge/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/anthropic/claude.py` & `phidata-2.4.5/phi/llm/anthropic/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/aws/bedrock.py` & `phidata-2.4.5/phi/llm/aws/bedrock.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/aws/claude.py` & `phidata-2.4.5/phi/llm/aws/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/azure/openai_chat.py` & `phidata-2.4.5/phi/llm/azure/openai_chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/base.py` & `phidata-2.4.5/phi/llm/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/cohere/chat.py` & `phidata-2.4.5/phi/llm/cohere/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/gemini/gemini.py` & `phidata-2.4.5/phi/llm/gemini/gemini.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/groq/groq.py` & `phidata-2.4.5/phi/llm/groq/groq.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/message.py` & `phidata-2.4.5/phi/llm/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/mistral/mistral.py` & `phidata-2.4.5/phi/llm/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/ollama/chat.py` & `phidata-2.4.5/phi/llm/ollama/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/ollama/hermes.py` & `phidata-2.4.5/phi/llm/ollama/hermes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/ollama/tools.py` & `phidata-2.4.5/phi/llm/ollama/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/openai/chat.py` & `phidata-2.4.5/phi/llm/openai/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/llm/together/together.py` & `phidata-2.4.5/phi/llm/together/together.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/memory/assistant.py` & `phidata-2.4.5/phi/memory/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/prompt/registry.py` & `phidata-2.4.5/phi/prompt/registry.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/prompt/template.py` & `phidata-2.4.5/phi/prompt/template.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/resource/base.py` & `phidata-2.4.5/phi/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/resource/group.py` & `phidata-2.4.5/phi/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/storage/assistant/base.py` & `phidata-2.4.5/phi/storage/assistant/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/storage/assistant/postgres.py` & `phidata-2.4.5/phi/storage/assistant/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/storage/assistant/singlestore.py` & `phidata-2.4.5/phi/storage/assistant/singlestore.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/storage/assistant/sqllite.py` & `phidata-2.4.5/phi/storage/assistant/sqllite.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/task/task.py` & `phidata-2.4.5/phi/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/airflow.py` & `phidata-2.4.5/phi/tools/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/apify.py` & `phidata-2.4.5/phi/tools/apify.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/arxiv_toolkit.py` & `phidata-2.4.5/phi/tools/arxiv_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/csv_tools.py` & `phidata-2.4.5/phi/tools/csv_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/duckdb.py` & `phidata-2.4.5/phi/tools/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/duckduckgo.py` & `phidata-2.4.5/phi/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/email.py` & `phidata-2.4.5/phi/tools/email.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/exa.py` & `phidata-2.4.5/phi/tools/exa.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/file.py` & `phidata-2.4.5/phi/tools/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/function.py` & `phidata-2.4.5/phi/tools/function.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/google.py` & `phidata-2.4.5/phi/tools/google.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/newspaper4k.py` & `phidata-2.4.5/phi/tools/newspaper4k.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/newspaper_toolkit.py` & `phidata-2.4.5/phi/tools/newspaper_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/openbb_tools.py` & `phidata-2.4.5/phi/tools/openbb_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/pandas.py` & `phidata-2.4.5/phi/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/phi.py` & `phidata-2.4.5/phi/tools/phi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/pubmed.py` & `phidata-2.4.5/phi/tools/pubmed.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/python.py` & `phidata-2.4.5/phi/tools/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/resend_toolkit.py` & `phidata-2.4.5/phi/tools/resend_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/serpapi_toolkit.py` & `phidata-2.4.5/phi/tools/serpapi_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/shell.py` & `phidata-2.4.5/phi/tools/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/sql.py` & `phidata-2.4.5/phi/tools/sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/streamlit/components.py` & `phidata-2.4.5/phi/tools/streamlit/components.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/tavily.py` & `phidata-2.4.5/phi/tools/tavily.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/toolkit.py` & `phidata-2.4.5/phi/tools/toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/website.py` & `phidata-2.4.5/phi/tools/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/wikipedia.py` & `phidata-2.4.5/phi/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/yfinance.py` & `phidata-2.4.5/phi/tools/yfinance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/youtube_toolkit.py` & `phidata-2.4.5/phi/tools/youtube_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/tools/zendesk.py` & `phidata-2.4.5/phi/tools/zendesk.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/common.py` & `phidata-2.4.5/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/defaults.py` & `phidata-2.4.5/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/enum.py` & `phidata-2.4.5/phi/utils/enum.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/filesystem.py` & `phidata-2.4.5/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/functions.py` & `phidata-2.4.5/phi/utils/functions.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/git.py` & `phidata-2.4.5/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/json_io.py` & `phidata-2.4.5/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/json_schema.py` & `phidata-2.4.5/phi/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/load_env.py` & `phidata-2.4.5/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/log.py` & `phidata-2.4.5/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/merge_dict.py` & `phidata-2.4.5/phi/utils/merge_dict.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/message.py` & `phidata-2.4.5/phi/utils/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/pickle.py` & `phidata-2.4.5/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/py_io.py` & `phidata-2.4.5/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/pyproject.py` & `phidata-2.4.5/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/resource_filter.py` & `phidata-2.4.5/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/shell.py` & `phidata-2.4.5/phi/utils/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/timer.py` & `phidata-2.4.5/phi/utils/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/tools.py` & `phidata-2.4.5/phi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/utils/yaml_io.py` & `phidata-2.4.5/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/base.py` & `phidata-2.4.5/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/lancedb/lancedb.py` & `phidata-2.4.5/phi/vectordb/lancedb/lancedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/pgvector/pgvector.py` & `phidata-2.4.5/phi/vectordb/pgvector/pgvector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/pgvector/pgvector2.py` & `phidata-2.4.5/phi/vectordb/pgvector/pgvector2.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/pineconedb/pineconedb.py` & `phidata-2.4.5/phi/vectordb/pineconedb/pineconedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/qdrant/qdrant.py` & `phidata-2.4.5/phi/vectordb/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/singlestore/index.py` & `phidata-2.4.5/phi/vectordb/singlestore/index.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/vectordb/singlestore/s2vectordb.py` & `phidata-2.4.5/phi/vectordb/singlestore/s2vectordb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/workflow/workflow.py` & `phidata-2.4.5/phi/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/workspace/config.py` & `phidata-2.4.5/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/workspace/helpers.py` & `phidata-2.4.5/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/workspace/operator.py` & `phidata-2.4.5/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phi/workspace/settings.py` & `phidata-2.4.5/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.4.4/phidata.egg-info/PKG-INFO` & `phidata-2.4.5/phidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.4.4
+Version: 2.4.5
 Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phidata-2.4.4/phidata.egg-info/SOURCES.txt` & `phidata-2.4.5/phidata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -403,22 +403,24 @@
 phi/table/sql/base.py
 phi/task/__init__.py
 phi/task/task.py
 phi/tools/__init__.py
 phi/tools/airflow.py
 phi/tools/apify.py
 phi/tools/arxiv_toolkit.py
+phi/tools/calculator.py
 phi/tools/csv_tools.py
 phi/tools/duckdb.py
 phi/tools/duckduckgo.py
 phi/tools/email.py
 phi/tools/exa.py
 phi/tools/file.py
 phi/tools/function.py
 phi/tools/google.py
+phi/tools/hackernews.py
 phi/tools/newspaper4k.py
 phi/tools/newspaper_toolkit.py
 phi/tools/openbb_tools.py
 phi/tools/pandas.py
 phi/tools/phi.py
 phi/tools/pubmed.py
 phi/tools/python.py
```

### Comparing `phidata-2.4.4/pyproject.toml` & `phidata-2.4.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.4.4"
+version = "2.4.5"
 description = "Memory, knowledge and tools for LLMs."
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```

