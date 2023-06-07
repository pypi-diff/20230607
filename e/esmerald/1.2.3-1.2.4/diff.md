# Comparing `tmp/esmerald-1.2.3.tar.gz` & `tmp/esmerald-1.2.4.tar.gz`

## Comparing `esmerald-1.2.3.tar` & `esmerald-1.2.4.tar`

### file list

```diff
@@ -1,188 +1,189 @@
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/__init__.py
--rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/testclient.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/base.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/events.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.3/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.3/LICENSE
--rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.3/README.md
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 esmerald-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 esmerald-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/__init__.py
+-rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/enums.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/injector.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/params.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/py.typed
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/testclient.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/websockets.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/session.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/crypto.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/base_user.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/databases/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/databases/tortoise/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/router.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/urls/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/urls/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/pydantic.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/sync.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/timezone.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/url.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.4/LICENSE
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.2.4/README.md
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 esmerald-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    20202 2020-02-02 00:00:00.000000 esmerald-1.2.4/PKG-INFO
```

### Comparing `esmerald-1.2.3/esmerald/__init__.py` & `esmerald-1.2.4/esmerald/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-Esmerald: Highly scalable, performant, easy to learn and for every application.
-"""
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.2.3/esmerald/applications.py` & `esmerald-1.2.4/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/backgound.py` & `esmerald-1.2.4/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/enums.py` & `esmerald-1.2.4/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/exception_handlers.py` & `esmerald-1.2.4/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/exceptions.py` & `esmerald-1.2.4/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/injector.py` & `esmerald-1.2.4/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/logging.py` & `esmerald-1.2.4/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/params.py` & `esmerald-1.2.4/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/parsers.py` & `esmerald-1.2.4/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/requests.py` & `esmerald-1.2.4/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/testclient.py` & `esmerald-1.2.4/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/types.py` & `esmerald-1.2.4/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/websockets.py` & `esmerald-1.2.4/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/__init__.py` & `esmerald-1.2.4/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/global_settings.py` & `esmerald-1.2.4/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/config/jwt.py` & `esmerald-1.2.4/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/config/openapi.py` & `esmerald-1.2.4/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/config/session.py` & `esmerald-1.2.4/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/config/static_files.py` & `esmerald-1.2.4/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/encoding.py` & `esmerald-1.2.4/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/hashers.py` & `esmerald-1.2.4/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.2.4/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.2.4/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.2.4/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/tortoise/base_user.py` & `esmerald-1.2.4/esmerald/contrib/auth/tortoise/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/auth/tortoise/middleware.py` & `esmerald-1.2.4/esmerald/contrib/auth/tortoise/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/contrib/databases/tortoise/__init__.py` & `esmerald-1.2.4/esmerald/contrib/databases/tortoise/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/base.py` & `esmerald-1.2.4/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/cli.py` & `esmerald-1.2.4/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/env.py` & `esmerald-1.2.4/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/templates.py` & `esmerald-1.2.4/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/utils.py` & `esmerald-1.2.4/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/createapp.py` & `esmerald-1.2.4/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/createproject.py` & `esmerald-1.2.4/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/list.py` & `esmerald-1.2.4/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/run.py` & `esmerald-1.2.4/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/runserver.py` & `esmerald-1.2.4/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/directives/operations/show_urls.py` & `esmerald-1.2.4/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/terminal/base.py` & `esmerald-1.2.4/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/terminal/print.py` & `esmerald-1.2.4/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/core/terminal/terminal.py` & `esmerald-1.2.4/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/__init__.py` & `esmerald-1.2.4/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/base.py` & `esmerald-1.2.4/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/encoders.py` & `esmerald-1.2.4/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/file.py` & `esmerald-1.2.4/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/json.py` & `esmerald-1.2.4/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/redirect.py` & `esmerald-1.2.4/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/stream.py` & `esmerald-1.2.4/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/datastructures/template.py` & `esmerald-1.2.4/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/interceptors/interceptor.py` & `esmerald-1.2.4/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/__init__.py` & `esmerald-1.2.4/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/asyncexitstack.py` & `esmerald-1.2.4/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/authentication.py` & `esmerald-1.2.4/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/basic.py` & `esmerald-1.2.4/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/csrf.py` & `esmerald-1.2.4/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/errors.py` & `esmerald-1.2.4/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/middleware/exceptions.py` & `esmerald-1.2.4/esmerald/middleware/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import inspect
 from inspect import getmro
 from typing import Any, Callable, Dict, List, Mapping, Optional, Type, Union, cast
 
 from pydantic import BaseModel
 from starlette import status
-from starlette._utils import is_async_callable
-from starlette.concurrency import run_in_threadpool
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.middleware.errors import ServerErrorMiddleware
 from starlette.middleware.exceptions import ExceptionMiddleware as StarletteExceptionMiddleware
 from starlette.responses import Response as StarletteResponse
-from starlette.types import ASGIApp, Message, Receive, Scope, Send
+from starlette.types import ASGIApp, Receive, Scope, Send
 
 from esmerald.enums import MediaType, ScopeType
 from esmerald.exception_handlers import http_exception_handler
 from esmerald.exceptions import HTTPException, WebSocketException
+from esmerald.middleware._exception_handlers import wrap_app_handling_exceptions
 from esmerald.requests import Request
 from esmerald.responses import Response
 from esmerald.types import ExceptionHandler, ExceptionHandlers
 from esmerald.websockets import WebSocket
 
 
 class ExceptionMiddleware(StarletteExceptionMiddleware):
@@ -45,57 +43,26 @@
                 self.add_exception_handler(key, value)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if scope["type"] not in ("http", "websocket"):
             await self.app(scope, receive, send)
             return
 
-        response_started = False
+        scope["starlette.exception_handlers"] = (
+            self._exception_handlers,
+            self._status_handlers,
+        )
+
+        conn: Union[Request, WebSocket]
+        if scope["type"] == "http":
+            conn = Request(scope, receive, send)
+        else:
+            conn = WebSocket(scope, receive, send)
 
-        async def sender(message: Message) -> None:
-            nonlocal response_started
-
-            if message["type"] == "http.response.start":
-                response_started = True
-            await send(message)
-
-        try:
-            await self.app(scope=scope, receive=receive, send=send)
-        except Exception as exc:
-            handler = None
-
-            if isinstance(exc, StarletteHTTPException):
-                handler = self._status_handlers.get(exc.status_code)
-
-            if handler is None:
-                handler = self._lookup_exception_handler(exc)
-
-            if handler is None:
-                raise exc
-
-            if response_started:
-                msg = "Caught handled exception, but response already started."
-                raise RuntimeError(msg) from exc
-
-            if scope["type"] == "http":
-                request = Request(scope, receive=receive)
-                if is_async_callable(handler):
-                    response = await handler(request, exc)
-                else:
-                    response = await run_in_threadpool(handler, request, exc)
-                await response(scope, receive, sender)
-            elif scope["type"] == "websocket":
-                websocket = WebSocket(scope, receive=receive, send=send)
-                if is_async_callable(handler):
-                    if inspect.isfunction(handler):
-                        await self.app(scope, receive, send)
-                    else:
-                        await handler(websocket, exc)
-                else:
-                    await run_in_threadpool(handler, websocket, exc)
+        await wrap_app_handling_exceptions(self.app, conn)(scope, receive, send)
 
 
 class ResponseContent(BaseModel):
     detail: Optional[str]
     extra: Optional[Union[Dict[str, Any], List[Any]]] = None
     headers: Optional[Dict[str, str]] = None
     status_code: int = status.HTTP_500_INTERNAL_SERVER_ERROR
```

### Comparing `esmerald-1.2.3/esmerald/middleware/settings_middleware.py` & `esmerald-1.2.4/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/apiview.py` & `esmerald-1.2.4/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/enums.py` & `esmerald-1.2.4/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/parameters.py` & `esmerald-1.2.4/esmerald/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/path_item.py` & `esmerald-1.2.4/esmerald/openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/request_body.py` & `esmerald-1.2.4/esmerald/openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/responses.py` & `esmerald-1.2.4/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/schema.py` & `esmerald-1.2.4/esmerald/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/openapi/utils.py` & `esmerald-1.2.4/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/permissions/base.py` & `esmerald-1.2.4/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/permissions/utils.py` & `esmerald-1.2.4/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/pluggables/base.py` & `esmerald-1.2.4/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/protocols/asyncdao.py` & `esmerald-1.2.4/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/protocols/dao.py` & `esmerald-1.2.4/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/protocols/interceptor.py` & `esmerald-1.2.4/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/protocols/template.py` & `esmerald-1.2.4/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/responses/base.py` & `esmerald-1.2.4/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/responses/encoders.py` & `esmerald-1.2.4/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/responses/json.py` & `esmerald-1.2.4/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/responses/template.py` & `esmerald-1.2.4/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/base.py` & `esmerald-1.2.4/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/events.py` & `esmerald-1.2.4/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/gateways.py` & `esmerald-1.2.4/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/handlers.py` & `esmerald-1.2.4/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/router.py` & `esmerald-1.2.4/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/routing/views.py` & `esmerald-1.2.4/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/security/jwt/token.py` & `esmerald-1.2.4/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/template/jinja.py` & `esmerald-1.2.4/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/template/mako.py` & `esmerald-1.2.4/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/datastructures.py` & `esmerald-1.2.4/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/helpers.py` & `esmerald-1.2.4/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/model.py` & `esmerald-1.2.4/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/signature.py` & `esmerald-1.2.4/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/types.py` & `esmerald-1.2.4/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/transformers/utils.py` & `esmerald-1.2.4/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/urls/base.py` & `esmerald-1.2.4/esmerald/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/constants.py` & `esmerald-1.2.4/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/crypto.py` & `esmerald-1.2.4/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/functional.py` & `esmerald-1.2.4/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/helpers.py` & `esmerald-1.2.4/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/model.py` & `esmerald-1.2.4/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/module_loading.py` & `esmerald-1.2.4/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/pydantic.py` & `esmerald-1.2.4/esmerald/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/sync.py` & `esmerald-1.2.4/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/esmerald/utils/timezone.py` & `esmerald-1.2.4/esmerald/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/LICENSE` & `esmerald-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.3/README.md` & `esmerald-1.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 * **Middleware**: Apply middlewares on the application level or API level.
 * **Exception Handlers**: Apply exception handlers on any desired level.
 * **Permissions**: Apply specific rules and permissions on each API.
 * **Interceptors**: Intercept requests and add logic before reaching the endpoint.
 * **Pluggables**: Create plugins for Esmerald and hook them into any application and/or
 distribute them.
 * **DAO and AsyncDAO**: Avoid database calls directly from the APIs. Use business objects instead.
-* **Tortoise ORM**: Native support for [Tortoise ORM](https://tortoise.github.io/).
+* **Saffier ORM**: Native support for [Saffier ORM](./databases/saffier/motivation.md).
 * **APIView**: Class Based endpoints for your beloved OOP design.
 * **JSON serialization/deserialization**: Both UJSON and ORJON support.
 * **Lifespan**: Support for the newly lifespan and on_start/on_shutdown events.
 * **Scheduler**: Yes, that's right, it comes with a scheduler for those automated tasks.
 * **Dependency Injection**: Like any other great framework out there.
 * **Simplicity from settings**: Yes, we have a way to make the code even cleaner by introducing settings
 based systems.
```

#### html2text {}

```diff
@@ -52,21 +52,21 @@
 **Async and Sync**: Do you prefer sync or async? You can have both. *
 **Middleware**: Apply middlewares on the application level or API level. *
 **Exception Handlers**: Apply exception handlers on any desired level. *
 **Permissions**: Apply specific rules and permissions on each API. *
 **Interceptors**: Intercept requests and add logic before reaching the
 endpoint. * **Pluggables**: Create plugins for Esmerald and hook them into any
 application and/or distribute them. * **DAO and AsyncDAO**: Avoid database
-calls directly from the APIs. Use business objects instead. * **Tortoise ORM**:
-Native support for [Tortoise ORM](https://tortoise.github.io/). * **APIView**:
-Class Based endpoints for your beloved OOP design. * **JSON serialization/
-deserialization**: Both UJSON and ORJON support. * **Lifespan**: Support for
-the newly lifespan and on_start/on_shutdown events. * **Scheduler**: Yes,
-that's right, it comes with a scheduler for those automated tasks. *
-**Dependency Injection**: Like any other great framework out there. *
+calls directly from the APIs. Use business objects instead. * **Saffier ORM**:
+Native support for [Saffier ORM](./databases/saffier/motivation.md). *
+**APIView**: Class Based endpoints for your beloved OOP design. * **JSON
+serialization/deserialization**: Both UJSON and ORJON support. * **Lifespan**:
+Support for the newly lifespan and on_start/on_shutdown events. *
+**Scheduler**: Yes, that's right, it comes with a scheduler for those automated
+tasks. * **Dependency Injection**: Like any other great framework out there. *
 **Simplicity from settings**: Yes, we have a way to make the code even cleaner
 by introducing settings based systems. * **Database**: Out of the box support
 for async databases. ## Relation to Starlette and other frameworks Esmerald
 uses Starlette under the hood. The reason behind this decison comes with the
 fact that performance is there and no issues with routing. Once the application
 is up, all the routes are mounted and therefore the url paths are defined.
 Esmerald encourages standard practices and design in mind which means that any
```

### Comparing `esmerald-1.2.3/pyproject.toml` & `esmerald-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,41 @@
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.6.0,<0.7.0",
     "pydantic>=1.10.7,<2.0.0",
     "pydantic-factories==1.17.2",
     "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=1.1.0",
     "rich>=13.3.1,<14.0.0",
-    "starlette>=0.27.0,<0.30.0",
+    "starlette>=0.28.0,<1.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
     "starlette",
-    "fastapi",
     "framework",
     "websocket",
     "openapi",
     "ml",
     "machine learning",
+    "python",
+    "security",
+    "web",
+    "rest",
+    "openapi",
+    "web-framework",
+    "swagger",
+    "python3",
+    "asyncio",
+    "redoc",
+    "openapi3",
+    "python-types",
+    "uvicorn",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dymmond/esmerald"
 Documentation = "https://esmerald.dymmond.com/"
 Changelog = "https://esmerald.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
@@ -100,15 +112,15 @@
     "orjson>=3.8.5,<4.0.0",
     "saffier[postgres]>=0.7.4",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
-    "types-ujson==5.7.0.1",
+    "types-ujson==5.7.0.5",
     "types-orjson==3.6.2",
 ]
 
 dev = [
     "autoflake>=1.4.0",
     "flake8>=3.8.3,<6.0.0",
     "uvicorn[standard]>=0.19.0",
```

### Comparing `esmerald-1.2.3/PKG-INFO` & `esmerald-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.2.3
+Version: 1.2.4
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: api,asgi,fastapi,framework,http,machine learning,ml,openapi,pydantic,rest,starlette,websocket
+Keywords: api,asgi,asyncio,framework,http,machine learning,ml,openapi,openapi3,pydantic,python,python-types,python3,redoc,rest,security,starlette,swagger,uvicorn,web,web-framework,websocket
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -46,15 +46,15 @@
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: openapi-schemas-pydantic>=1.1.0
 Requires-Dist: pydantic-factories==1.17.2
 Requires-Dist: pydantic<2.0.0,>=1.10.7
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: starlette<0.30.0,>=0.27.0
+Requires-Dist: starlette<1.0,>=0.28.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
@@ -96,15 +96,15 @@
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Requires-Dist: saffier[postgres]>=0.7.4; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
-Requires-Dist: types-ujson==5.7.0.1; extra == 'test'
+Requires-Dist: types-ujson==5.7.0.5; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
 
 <p align="center">
   <a href="https://esmerald.dymmond.com"><img src="https://res.cloudinary.com/dymmond/image/upload/v1673619342/esmerald/img/logo-gr_z1ot8o.png" alt='Esmerald'></a>
@@ -246,15 +246,15 @@
 * **Middleware**: Apply middlewares on the application level or API level.
 * **Exception Handlers**: Apply exception handlers on any desired level.
 * **Permissions**: Apply specific rules and permissions on each API.
 * **Interceptors**: Intercept requests and add logic before reaching the endpoint.
 * **Pluggables**: Create plugins for Esmerald and hook them into any application and/or
 distribute them.
 * **DAO and AsyncDAO**: Avoid database calls directly from the APIs. Use business objects instead.
-* **Tortoise ORM**: Native support for [Tortoise ORM](https://tortoise.github.io/).
+* **Saffier ORM**: Native support for [Saffier ORM](./databases/saffier/motivation.md).
 * **APIView**: Class Based endpoints for your beloved OOP design.
 * **JSON serialization/deserialization**: Both UJSON and ORJON support.
 * **Lifespan**: Support for the newly lifespan and on_start/on_shutdown events.
 * **Scheduler**: Yes, that's right, it comes with a scheduler for those automated tasks.
 * **Dependency Injection**: Like any other great framework out there.
 * **Simplicity from settings**: Yes, we have a way to make the code even cleaner by introducing settings
 based systems.
```

