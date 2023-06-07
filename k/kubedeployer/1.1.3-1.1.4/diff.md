# Comparing `tmp/kubedeployer-1.1.3.tar.gz` & `tmp/kubedeployer-1.1.4.tar.gz`

## Comparing `kubedeployer-1.1.3.tar` & `kubedeployer-1.1.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/.dockerignore
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/.pylintrc
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/Dockerfile
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeploy
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/pytest.ini
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/requirements.txt
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/docs/ru.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/__main__.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deploy.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/docker.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/files.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/kubectl.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/kustomize.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/manifests.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/text.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/types.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/console/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/console/wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deployer/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deployer/abstract_deployer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deployer/kustomize_deployer.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deployer/orthodox_deployer.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/deployer/smart_deployer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/__init__.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/environment_variables.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/exceptions.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/specification.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/variable_reader.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/gitlab_ci/variable_types.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/k8s/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/k8s/annotations.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/k8s/deserialize.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/k8s/models.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/k8s/specifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/data.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/errors.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/formatters.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/report.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/kubesec/scanner.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/data.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/errors.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/formatters.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/report.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/security/trivy/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/utils/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/utils/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/vault/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/vault/client.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/vault/factory.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/kubedeployer/vault/service.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/scripts/run_e2e_tests.sh
--rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/scripts/run_tests.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/mocks.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/Dockerfile
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/docker-compose.yaml
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/entrypoint.sh
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/e2e_tests/e2e_entrypoint.sh
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/integration_tests/docker-compose.yaml
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/integration_tests/integration_entrypoint.sh
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/kind/config.yaml
--rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/kind/prepare-kind.sh
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/containers/manifests/rbac.yaml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/envs/base
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/envs/override
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/env-manifest.yaml
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/manifests.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/env-app/manifest.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/env-app/production/ingress.yaml
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/conftest.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_deployer.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_k8s.py
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_kubedeployer.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_kustomize.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_security_kubesec.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/test_security_trivy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/vault/__init__.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/integration/vault/mocks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_console.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_console_wrap.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_deployer.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_files.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_manifests.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_text.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_utils_convert.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/tests/unit/test_vault.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/LICENSE
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    22349 2020-02-02 00:00:00.000000 kubedeployer-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.dockerignore
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.pylintrc
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/Dockerfile
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeploy
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/pytest.ini
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/requirements.txt
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/docs/ru.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/__main__.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deploy.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/docker.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/files.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/kubectl.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/kustomize.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/manifests.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/text.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/types.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/console/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/console/wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/abstract_deployer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/kustomize_deployer.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/orthodox_deployer.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/deployer/smart_deployer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/__init__.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/environment_variables.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/exceptions.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/specification.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_reader.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_types.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/annotations.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/deserialize.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/models.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/k8s/specifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/data.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/errors.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/formatters.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/report.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/kubesec/scanner.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/data.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/errors.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/formatters.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/report.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/security/trivy/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/utils/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/utils/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/client.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/factory.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/kubedeployer/vault/service.py
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/scripts/run_e2e_tests.sh
+-rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/scripts/run_tests.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/mocks.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/Dockerfile
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/docker-compose.yaml
+-rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/entrypoint.sh
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/e2e_tests/e2e_entrypoint.sh
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/integration_tests/docker-compose.yaml
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/integration_tests/integration_entrypoint.sh
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/kind/config.yaml
+-rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/kind/prepare-kind.sh
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/containers/manifests/rbac.yaml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/envs/base
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/envs/override
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/env-manifest.yaml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/manifests.yaml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/env-app/manifest.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/env-app/production/ingress.yaml
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/kustomization.yaml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/service.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/configmap.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/overlays/stage/kustomization.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/stage/configmap.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/service.yaml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/stage/configmap.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_deployer.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_k8s.py
+-rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_kubedeployer.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_kustomize.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_security_kubesec.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/test_security_trivy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/vault/__init__.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/integration/vault/mocks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_console.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_console_wrap.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_deployer.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_files.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_manifests.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_text.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_utils_convert.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/tests/unit/test_vault.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/LICENSE
+-rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    22349 2020-02-02 00:00:00.000000 kubedeployer-1.1.4/PKG-INFO
```

### Comparing `kubedeployer-1.1.3/.pylintrc` & `kubedeployer-1.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/Dockerfile` & `kubedeployer-1.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/.github/workflows/ci.yml` & `kubedeployer-1.1.4/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
       - name: Build and push Docker image
         uses: docker/build-push-action@ad44023a93711e3deb337508980b4b5e9bcdc5dc
         with:
           context: .
           target: release
           build-args: |
-            LIB_VERSION: ${{ steps.get_version.outputs.version-without-v }}
+            LIB_VERSION=${{ steps.get_version.outputs.version-without-v }}
           push: true
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
 
   trigger-pipeline:
     name: Trigger Gitlab pipeline
     runs-on: ubuntu-latest
```

### Comparing `kubedeployer-1.1.3/docs/ru.md` & `kubedeployer-1.1.4/docs/ru.md`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/__init__.py` & `kubedeployer-1.1.4/kubedeployer/__init__.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/deploy.py` & `kubedeployer-1.1.4/kubedeployer/deploy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/docker.py` & `kubedeployer-1.1.4/kubedeployer/docker.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/files.py` & `kubedeployer-1.1.4/kubedeployer/files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/kubectl.py` & `kubedeployer-1.1.4/kubedeployer/kubectl.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/kustomize.py` & `kubedeployer-1.1.4/kubedeployer/kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/manifests.py` & `kubedeployer-1.1.4/kubedeployer/manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/text.py` & `kubedeployer-1.1.4/kubedeployer/text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/console/__init__.py` & `kubedeployer-1.1.4/kubedeployer/console/__init__.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/console/wrap.py` & `kubedeployer-1.1.4/kubedeployer/console/wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/deployer/kustomize_deployer.py` & `kubedeployer-1.1.4/kubedeployer/deployer/kustomize_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/deployer/orthodox_deployer.py` & `kubedeployer-1.1.4/kubedeployer/deployer/orthodox_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/deployer/smart_deployer.py` & `kubedeployer-1.1.4/kubedeployer/deployer/smart_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/gitlab_ci/environment_variables.py` & `kubedeployer-1.1.4/kubedeployer/gitlab_ci/environment_variables.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/gitlab_ci/specification.py` & `kubedeployer-1.1.4/kubedeployer/gitlab_ci/specification.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/gitlab_ci/variable_reader.py` & `kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_reader.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/gitlab_ci/variable_types.py` & `kubedeployer-1.1.4/kubedeployer/gitlab_ci/variable_types.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/k8s/annotations.py` & `kubedeployer-1.1.4/kubedeployer/k8s/annotations.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/k8s/models.py` & `kubedeployer-1.1.4/kubedeployer/k8s/models.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/kubesec/data.py` & `kubedeployer-1.1.4/kubedeployer/security/kubesec/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/kubesec/formatters.py` & `kubedeployer-1.1.4/kubedeployer/security/kubesec/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/kubesec/report.py` & `kubedeployer-1.1.4/kubedeployer/security/kubesec/report.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/kubesec/scanner.py` & `kubedeployer-1.1.4/kubedeployer/security/kubesec/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/trivy/data.py` & `kubedeployer-1.1.4/kubedeployer/security/trivy/data.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/trivy/formatters.py` & `kubedeployer-1.1.4/kubedeployer/security/trivy/formatters.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/security/trivy/scanner.py` & `kubedeployer-1.1.4/kubedeployer/security/trivy/scanner.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/vault/client.py` & `kubedeployer-1.1.4/kubedeployer/vault/client.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/vault/factory.py` & `kubedeployer-1.1.4/kubedeployer/vault/factory.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/kubedeployer/vault/service.py` & `kubedeployer-1.1.4/kubedeployer/vault/service.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/scripts/run_e2e_tests.sh` & `kubedeployer-1.1.4/scripts/run_e2e_tests.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/conftest.py` & `kubedeployer-1.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/mocks.py` & `kubedeployer-1.1.4/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/Dockerfile` & `kubedeployer-1.1.4/tests/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/entrypoint.sh` & `kubedeployer-1.1.4/tests/containers/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/e2e_tests/e2e_entrypoint.sh` & `kubedeployer-1.1.4/tests/containers/e2e_tests/e2e_entrypoint.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/kind/config.yaml` & `kubedeployer-1.1.4/tests/containers/kind/config.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/kind/prepare-kind.sh` & `kubedeployer-1.1.4/tests/containers/kind/prepare-kind.sh`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/containers/manifests/rbac.yaml` & `kubedeployer-1.1.4/tests/containers/manifests/rbac.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/env-manifest.yaml` & `kubedeployer-1.1.4/tests/data/manifests/env-manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/manifests.yaml` & `kubedeployer-1.1.4/tests/data/manifests/manifests.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/env-app/manifest.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/env-app/manifest.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/env-app/production/ingress.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/env-app/production/ingress.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app/base/deployment.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/kustomize-app-with-env/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app/deployment.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml` & `kubedeployer-1.1.4/tests/data/manifests/apps/non-kustomize-app-with-env/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_deployer.py` & `kubedeployer-1.1.4/tests/integration/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_k8s.py` & `kubedeployer-1.1.4/tests/integration/test_k8s.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_kubedeployer.py` & `kubedeployer-1.1.4/tests/integration/test_kubedeployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_kustomize.py` & `kubedeployer-1.1.4/tests/integration/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_security_kubesec.py` & `kubedeployer-1.1.4/tests/integration/test_security_kubesec.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/integration/test_security_trivy.py` & `kubedeployer-1.1.4/tests/integration/test_security_trivy.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_console_wrap.py` & `kubedeployer-1.1.4/tests/unit/test_console_wrap.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_deployer.py` & `kubedeployer-1.1.4/tests/unit/test_deployer.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_files.py` & `kubedeployer-1.1.4/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_manifests.py` & `kubedeployer-1.1.4/tests/unit/test_manifests.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_text.py` & `kubedeployer-1.1.4/tests/unit/test_text.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_utils_convert.py` & `kubedeployer-1.1.4/tests/unit/test_utils_convert.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/tests/unit/test_vault.py` & `kubedeployer-1.1.4/tests/unit/test_vault.py`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/.gitignore` & `kubedeployer-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/LICENSE` & `kubedeployer-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/README.md` & `kubedeployer-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/pyproject.toml` & `kubedeployer-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kubedeployer-1.1.3/PKG-INFO` & `kubedeployer-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubedeployer
-Version: 1.1.3
+Version: 1.1.4
 Summary: package to deploy application on kubernetes
 Project-URL: Homepage, https://github.com/itlabsio/kubedeployer
 Project-URL: Bug Tracker, https://github.com/itlabsio/kubedeployer/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

