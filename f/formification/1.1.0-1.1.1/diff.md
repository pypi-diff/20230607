# Comparing `tmp/formification-1.1.0.tar.gz` & `tmp/formification-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formification-1.1.0.tar", last modified: Wed Jun  7 10:41:59 2023, max compression
+gzip compressed data, was "formification-1.1.1.tar", last modified: Wed Jun  7 10:56:37 2023, max compression
```

## Comparing `formification-1.1.0.tar` & `formification-1.1.1.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.291314 formification-1.1.0/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1066 2023-06-07 09:38:32.000000 formification-1.1.0/LICENSE
--rw-rw-r--   0 levimoore   (501) staff       (20)      111 2023-06-05 06:46:49.000000 formification-1.1.0/MANIFEST.in
--rw-r--r--   0 levimoore   (501) staff       (20)     5692 2023-06-07 10:41:59.291392 formification-1.1.0/PKG-INFO
--rw-rw-r--   0 levimoore   (501) staff       (20)     4635 2023-06-05 06:46:49.000000 formification-1.1.0/README.md
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.207741 formification-1.1.0/formification.egg-info/
--rw-r--r--   0 levimoore   (501) staff       (20)     5692 2023-06-07 10:41:59.000000 formification-1.1.0/formification.egg-info/PKG-INFO
--rw-r--r--   0 levimoore   (501) staff       (20)    17720 2023-06-07 10:41:59.000000 formification-1.1.0/formification.egg-info/SOURCES.txt
--rw-r--r--   0 levimoore   (501) staff       (20)        1 2023-06-07 10:41:59.000000 formification-1.1.0/formification.egg-info/dependency_links.txt
--rw-r--r--   0 levimoore   (501) staff       (20)      237 2023-06-07 10:41:59.000000 formification-1.1.0/formification.egg-info/requires.txt
--rw-r--r--   0 levimoore   (501) staff       (20)       10 2023-06-07 10:41:59.000000 formification-1.1.0/formification.egg-info/top_level.txt
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.213361 formification-1.1.0/formulaic/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/__init__.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     3461 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/admin.py
--rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/apps.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     2043 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/auto_populate.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      768 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/beanstalk_jobs.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1337 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/csv_export.py
--rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/exceptions.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     3809 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/fields.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     3415 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/forms.py
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.214250 formification-1.1.0/formulaic/migrations/
--rw-rw-r--   0 levimoore   (501) staff       (20)    11960 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/migrations/0001_initial.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      379 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/migrations/0002_add_default_to_field_enabled.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      624 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/migrations/0003_auto_20201230_1406.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      486 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/migrations/0004_submission_promo_source.py
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/migrations/__init__.py
--rw-rw-r--   0 levimoore   (501) staff       (20)    31413 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/models.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     4640 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/rules.py
--rw-rw-r--   0 levimoore   (501) staff       (20)    11002 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/serializers.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      193 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/settings.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      186 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/signals.py
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205299 formification-1.1.0/formulaic/static/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.200965 formification-1.1.0/formulaic/static/admin/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205202 formification-1.1.0/formulaic/static/admin/formulaic/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.214596 formification-1.1.0/formulaic/static/admin/formulaic/css/
--rw-rw-r--   0 levimoore   (501) staff       (20)     3714 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/css/edit_fields.css
--rw-rw-r--   0 levimoore   (501) staff       (20)      837 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/css/form.css
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.219554 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/
--rw-rw-r--   0 levimoore   (501) staff       (20)       60 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.bowerrc
--rw-rw-r--   0 levimoore   (501) staff       (20)      368 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.editorconfig
--rw-rw-r--   0 levimoore   (501) staff       (20)      298 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.ember-cli
--rw-rw-r--   0 levimoore   (501) staff       (20)      185 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.eslintrc.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      243 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.gitignore
--rw-rw-r--   0 levimoore   (501) staff       (20)        7 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.nvmrc
--rw-rw-r--   0 levimoore   (501) staff       (20)      336 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.travis.yml
--rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/.watchmanconfig
--rw-rw-r--   0 levimoore   (501) staff       (20)     1832 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/README.md
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.220553 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.220974 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/
--rw-rw-r--   0 levimoore   (501) staff       (20)      943 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      445 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/app.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.226045 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/.gitkeep
--rw-rw-r--   0 levimoore   (501) staff       (20)     1191 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox-select-multiple.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-email.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-full-name.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-hidden.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-integer.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-phone-number.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-radio-select.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select-multiple.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-text.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-textarea.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     4268 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2809 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2463 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      163 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-fields.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     1344 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      321 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rules.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.226435 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/.gitkeep
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.227541 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.229637 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1837 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/booleanfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2862 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      313 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/hiddenfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/index.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/textfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     6031 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      597 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2011 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     3030 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       94 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.229850 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/.gitkeep
--rw-rw-r--   0 levimoore   (501) staff       (20)      902 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.229988 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/
--rw-rw-r--   0 levimoore   (501) staff       (20)      333 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/cookie-initializer.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.233166 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/.gitkeep
--rw-rw-r--   0 levimoore   (501) staff       (20)      463 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/basefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      376 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/booleanfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      719 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      387 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/field.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      229 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/form.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      362 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/hiddenfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      195 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/option.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      200 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optiongroup.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      199 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optionlist.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      124 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/privacypolicy.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      263 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rule.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      458 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rulecondition.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      419 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/ruleresult.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      253 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submission.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      155 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submissionsource.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      326 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/textfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       65 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/resolver.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      991 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.233497 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/.gitkeep
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.234298 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/
--rw-rw-r--   0 levimoore   (501) staff       (20)     9006 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2120 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     6219 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     2040 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      221 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.235543 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/
--rw-rw-r--   0 levimoore   (501) staff       (20)      329 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/field.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      191 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optiongroup.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      190 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optionlist.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      235 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/rule.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      103 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/submissionsource.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.235726 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/
--rw-rw-r--   0 levimoore   (501) staff       (20)     6320 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.236125 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/
--rw-rw-r--   0 levimoore   (501) staff       (20)      114 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/application.hbs
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.239775 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/.gitkeep
--rw-rw-r--   0 levimoore   (501) staff       (20)       28 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/base-sortable.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      378 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox-select-multiple.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      259 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-email.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)       70 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-full-name.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      101 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-hidden.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)       61 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-integer.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)       69 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-phone-number.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      743 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      176 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select-multiple.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      339 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-text.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      213 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-textarea.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1559 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1427 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      803 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      556 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1711 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      619 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.240484 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.241471 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1786 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     4565 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     3599 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1497 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1663 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      970 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     4350 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     1014 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)     2677 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs
--rw-rw-r--   0 levimoore   (501) staff       (20)      159 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form.hbs
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.241650 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/
--rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/json.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.241977 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/
--rw-rw-r--   0 levimoore   (501) staff       (20)      922 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/slug.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.242140 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/
--rw-rw-r--   0 levimoore   (501) staff       (20)     2394 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.242949 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1124 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/booleanfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      522 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/hiddenfield.js
--rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/textfield.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.243508 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/
--rw-rw-r--   0 levimoore   (501) staff       (20)     2129 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      622 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     1668 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      231 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/bower.json
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.243702 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1308 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.244842 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.255987 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/
--rw-rw-r--   0 levimoore   (501) staff       (20)   201293 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css
--rw-rw-r--   0 levimoore   (501) staff       (20)    96917 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map
--rw-rw-r--   0 levimoore   (501) staff       (20)   197827 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js
--rw-rw-r--   0 levimoore   (501) staff       (20)   244408 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map
--rw-rw-r--   0 levimoore   (501) staff       (20)    26702 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.266817 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/
--rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/bg-stripes.png
--rw-rw-r--   0 levimoore   (501) staff       (20)    16445 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png
--rw-rw-r--   0 levimoore   (501) staff       (20)     8424 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css
--rw-rw-r--   0 levimoore   (501) staff       (20)   221524 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js
--rw-rw-r--   0 levimoore   (501) staff       (20)   276278 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map
--rw-rw-r--   0 levimoore   (501) staff       (20)    38972 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js
--rw-rw-r--   0 levimoore   (501) staff       (20)    47670 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map
--rw-rw-r--   0 levimoore   (501) staff       (20)     9760 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css
--rw-rw-r--   0 levimoore   (501) staff       (20)  3564382 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js
--rw-rw-r--   0 levimoore   (501) staff       (20)  4324732 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map
--rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.203732 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.267183 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/
--rw-rw-r--   0 levimoore   (501) staff       (20)    91113 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.272481 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/
--rw-rw-r--   0 levimoore   (501) staff       (20)    20127 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 levimoore   (501) staff       (20)   108738 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 levimoore   (501) staff       (20)    45404 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 levimoore   (501) staff       (20)    23424 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 levimoore   (501) staff       (20)    18028 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2
--rw-rw-r--   0 levimoore   (501) staff       (20)     1508 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html
--rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/robots.txt
--rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.272753 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/
--rw-rw-r--   0 levimoore   (501) staff       (20)     2051 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html
--rw-rw-r--   0 levimoore   (501) staff       (20)     1645 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js
--rw-rw-r--   0 levimoore   (501) staff       (20)   234080 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json
--rw-rw-r--   0 levimoore   (501) staff       (20)     1381 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/package.json
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.273223 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.204178 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.273439 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/
--rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/bg-stripes.png
--rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml
--rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/robots.txt
--rw-rw-r--   0 levimoore   (501) staff       (20)      214 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/testem.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.274046 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/
--rw-rw-r--   0 levimoore   (501) staff       (20)       55 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/.eslintrc.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.275096 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/
--rw-rw-r--   0 levimoore   (501) staff       (20)      117 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/destroy-app.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      617 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      255 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/resolver.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      474 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/start-app.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     1074 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.275288 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/.gitkeep
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.278802 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/
--rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      671 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      711 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      656 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/test-helper.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.279000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/.gitkeep
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.279135 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/
--rw-rw-r--   0 levimoore   (501) staff       (20)      627 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.279427 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/
--rw-rw-r--   0 levimoore   (501) staff       (20)      286 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/form-test.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.279727 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/.gitkeep
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.282045 formification-1.1.0/formulaic/static/admin/formulaic/images/
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1629 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-090.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1658 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-270.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1845 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-move.png
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.283087 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/
--rwxr-xr-x   0 levimoore   (501) staff       (20)      663 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)      224 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/minus.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1548 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/pencil.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)      482 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/plus.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/backup/tick.png
--rw-rw-r--   0 levimoore   (501) staff       (20)     9159 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/icons-grappelli.png
--rw-rw-r--   0 levimoore   (501) staff       (20)      934 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/label-bg.png
--rw-rw-r--   0 levimoore   (501) staff       (20)     2545 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/loading.gif
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1105 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/minus.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1905 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/pencil.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)     1541 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/plus.png
--rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/images/tick.png
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.283765 formification-1.1.0/formulaic/static/admin/formulaic/js/
--rw-rw-r--   0 levimoore   (501) staff       (20)    28628 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/js/edit_fields.js
--rw-rw-r--   0 levimoore   (501) staff       (20)      794 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/js/form.js
--rw-rw-r--   0 levimoore   (501) staff       (20)    93107 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205554 formification-1.1.0/formulaic/static/formulaic/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.286484 formification-1.1.0/formulaic/static/formulaic/css/
--rw-rw-r--   0 levimoore   (501) staff       (20)   219801 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/css/bootstrap.css
--rw-rw-r--   0 levimoore   (501) staff       (20)   194385 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/css/bootstrap.min.css
--rw-rw-r--   0 levimoore   (501) staff       (20)      239 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/css/custom_form.css
--rw-rw-r--   0 levimoore   (501) staff       (20)     1407 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/css/gate-form.css
--rw-rw-r--   0 levimoore   (501) staff       (20)    25253 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/css/intlTelInput.css
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.287226 formification-1.1.0/formulaic/static/formulaic/img/
--rw-rw-r--   0 levimoore   (501) staff       (20)    70857 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/img/flags.png
--rw-rw-r--   0 levimoore   (501) staff       (20)   174369 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/img/flags@2x.png
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.288857 formification-1.1.0/formulaic/static/formulaic/js/
--rw-rw-r--   0 levimoore   (501) staff       (20)    20880 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/js/custom_form.js
--rw-rw-r--   0 levimoore   (501) staff       (20)   246620 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/js/intTelInput_utils.js
--rw-rw-r--   0 levimoore   (501) staff       (20)    29401 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/js/intlTelInput.min.js
--rw-rw-r--   0 levimoore   (501) staff       (20)     1982 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/static/formulaic/js/phoneNumber.js
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205949 formification-1.1.0/formulaic/templates/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205800 formification-1.1.0/formulaic/templates/admin/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.205860 formification-1.1.0/formulaic/templates/admin/formulaic/
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.289361 formification-1.1.0/formulaic/templates/admin/formulaic/form/
--rw-rw-r--   0 levimoore   (501) staff       (20)     1652 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templates/admin/formulaic/form/change_form.html
--rw-rw-r--   0 levimoore   (501) staff       (20)      545 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templates/admin/formulaic/form/change_list.html
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.289832 formification-1.1.0/formulaic/templates/formulaic/
--rw-rw-r--   0 levimoore   (501) staff       (20)     3052 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templates/formulaic/bootstrap-form.html
--rw-rw-r--   0 levimoore   (501) staff       (20)     1181 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templates/formulaic/form.html
--rw-rw-r--   0 levimoore   (501) staff       (20)     3114 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templates/formulaic/gate-form.html
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.290268 formification-1.1.0/formulaic/templatetags/
--rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templatetags/__init__.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     2309 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templatetags/form.py
--rw-rw-r--   0 levimoore   (501) staff       (20)      217 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/templatetags/setting_tags.py
-drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:41:59.291174 formification-1.1.0/formulaic/tests/
--rw-rw-r--   0 levimoore   (501) staff       (20)      110 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/__init__.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1876 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/test_csv_export.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     5023 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/test_forms.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1978 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/test_models.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1533 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/test_validators.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     7798 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/tests/test_views.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1127 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/urls.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     2058 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/utils.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1246 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/validators.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     8838 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/views.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     2099 2023-06-05 06:46:49.000000 formification-1.1.0/formulaic/widgets.py
--rw-rw-r--   0 levimoore   (501) staff       (20)     1287 2023-06-07 10:41:59.291781 formification-1.1.0/setup.cfg
--rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 formification-1.1.0/setup.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.611362 formification-1.1.1/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1066 2023-06-07 09:38:32.000000 formification-1.1.1/LICENSE
+-rw-rw-r--   0 levimoore   (501) staff       (20)      111 2023-06-05 06:46:49.000000 formification-1.1.1/MANIFEST.in
+-rw-r--r--   0 levimoore   (501) staff       (20)     5446 2023-06-07 10:56:37.611440 formification-1.1.1/PKG-INFO
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4635 2023-06-05 06:46:49.000000 formification-1.1.1/README.md
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.535688 formification-1.1.1/formification.egg-info/
+-rw-r--r--   0 levimoore   (501) staff       (20)     5446 2023-06-07 10:56:37.000000 formification-1.1.1/formification.egg-info/PKG-INFO
+-rw-r--r--   0 levimoore   (501) staff       (20)    17720 2023-06-07 10:56:37.000000 formification-1.1.1/formification.egg-info/SOURCES.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)        1 2023-06-07 10:56:37.000000 formification-1.1.1/formification.egg-info/dependency_links.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)      237 2023-06-07 10:56:37.000000 formification-1.1.1/formification.egg-info/requires.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)       10 2023-06-07 10:56:37.000000 formification-1.1.1/formification.egg-info/top_level.txt
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.539760 formification-1.1.1/formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3461 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/admin.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/apps.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2043 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/auto_populate.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      768 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/beanstalk_jobs.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1337 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/csv_export.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/exceptions.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3809 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/fields.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3415 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/forms.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.540576 formification-1.1.1/formulaic/migrations/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    11960 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/migrations/0001_initial.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      379 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/migrations/0002_add_default_to_field_enabled.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      624 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/migrations/0003_auto_20201230_1406.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      486 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/migrations/0004_submission_promo_source.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/migrations/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)    31413 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/models.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4640 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/rules.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)    11002 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/serializers.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      193 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/settings.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      186 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/signals.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533405 formification-1.1.1/formulaic/static/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.529452 formification-1.1.1/formulaic/static/admin/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533321 formification-1.1.1/formulaic/static/admin/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.540854 formification-1.1.1/formulaic/static/admin/formulaic/css/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3714 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/css/edit_fields.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)      837 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/css/form.css
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.544085 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)       60 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.bowerrc
+-rw-rw-r--   0 levimoore   (501) staff       (20)      368 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.editorconfig
+-rw-rw-r--   0 levimoore   (501) staff       (20)      298 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.ember-cli
+-rw-rw-r--   0 levimoore   (501) staff       (20)      185 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.eslintrc.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      243 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.gitignore
+-rw-rw-r--   0 levimoore   (501) staff       (20)        7 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.nvmrc
+-rw-rw-r--   0 levimoore   (501) staff       (20)      336 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.travis.yml
+-rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/.watchmanconfig
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1832 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/README.md
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.544896 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.545292 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      943 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      445 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/app.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.548544 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1191 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox-select-multiple.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-email.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-full-name.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-hidden.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-integer.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-phone-number.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-radio-select.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select-multiple.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-text.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-textarea.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4268 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2809 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2463 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      163 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1344 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      321 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rules.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.548813 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.549474 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.550493 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1837 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2862 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      313 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/textfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6031 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      597 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2011 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3030 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       94 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.550658 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)      902 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/index.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.550774 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      333 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/cookie-initializer.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.553381 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)      463 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      376 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      719 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      387 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      229 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      362 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      195 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/option.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      200 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/optiongroup.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      199 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/optionlist.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      124 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/privacypolicy.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      263 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      458 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/rulecondition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      419 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/ruleresult.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      253 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/submission.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      155 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/submissionsource.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      326 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/textfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       65 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/resolver.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      991 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/router.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.553650 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.554271 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9006 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2120 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6219 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2040 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      221 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.555059 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      329 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      191 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optiongroup.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      190 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optionlist.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      235 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      103 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/submissionsource.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.555220 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/styles/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6320 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.555533 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      114 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/application.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.558761 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)       28 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/base-sortable.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      378 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox-select-multiple.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      259 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-email.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       70 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-full-name.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      101 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-hidden.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       61 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-integer.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       69 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-phone-number.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      743 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      176 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select-multiple.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      339 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-text.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      213 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-textarea.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1559 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1427 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      803 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      556 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1711 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      619 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.559382 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.560331 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1786 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4565 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3599 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1497 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1663 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      970 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4350 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1014 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2677 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      159 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.560487 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/json.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.560795 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/utils/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      922 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/utils/slug.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.560952 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2394 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.561746 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1124 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      522 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/textfield.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.562273 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2129 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      622 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1668 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      231 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/bower.json
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.562453 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/config/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1308 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.563507 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.574717 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/
+-rw-rw-r--   0 levimoore   (501) staff       (20)   201293 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)    96917 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)   197827 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   244408 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)    26702 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.586531 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/bg-stripes.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)    16445 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     8424 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)   221524 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   276278 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)    38972 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    47670 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9760 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)  3564382 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)  4324732 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.531958 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.586942 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    91113 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.593147 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    20127 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 levimoore   (501) staff       (20)   108738 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 levimoore   (501) staff       (20)    45404 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 levimoore   (501) staff       (20)    23424 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 levimoore   (501) staff       (20)    18028 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1508 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/robots.txt
+-rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.593444 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2051 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1645 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   234080 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1381 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/package.json
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.593883 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.532411 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/assets/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.594092 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/bg-stripes.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml
+-rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/robots.txt
+-rw-rw-r--   0 levimoore   (501) staff       (20)      214 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/testem.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.595009 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)       55 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/.eslintrc.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.595902 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      117 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/destroy-app.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      617 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      255 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/resolver.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      474 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/start-app.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1074 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.596104 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.598907 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      671 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      711 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      656 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/test-helper.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.599099 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.599234 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      627 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.599496 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      286 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/form-test.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.599814 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/vendor/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/vendor/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.602027 formification-1.1.1/formulaic/static/admin/formulaic/images/
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1629 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-090.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1658 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-270.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1845 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-move.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.602964 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      663 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/arrow-move.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      224 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/minus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1548 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/pencil.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      482 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/plus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/backup/tick.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9159 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/icons-grappelli.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)      934 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/label-bg.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2545 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/loading.gif
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1105 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/minus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1905 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/pencil.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1541 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/plus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/images/tick.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.603639 formification-1.1.1/formulaic/static/admin/formulaic/js/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    28628 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/js/edit_fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      794 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/js/form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    93107 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533614 formification-1.1.1/formulaic/static/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.605728 formification-1.1.1/formulaic/static/formulaic/css/
+-rw-rw-r--   0 levimoore   (501) staff       (20)   219801 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/css/bootstrap.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)   194385 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/css/bootstrap.min.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)      239 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/css/custom_form.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1407 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/css/gate-form.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)    25253 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/css/intlTelInput.css
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.606470 formification-1.1.1/formulaic/static/formulaic/img/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    70857 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/img/flags.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)   174369 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/img/flags@2x.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.608182 formification-1.1.1/formulaic/static/formulaic/js/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    20880 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/js/custom_form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   246620 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/js/intTelInput_utils.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    29401 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/js/intlTelInput.min.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1982 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/static/formulaic/js/phoneNumber.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533946 formification-1.1.1/formulaic/templates/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533816 formification-1.1.1/formulaic/templates/admin/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.533870 formification-1.1.1/formulaic/templates/admin/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.608728 formification-1.1.1/formulaic/templates/admin/formulaic/form/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1652 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templates/admin/formulaic/form/change_form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)      545 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templates/admin/formulaic/form/change_list.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.609283 formification-1.1.1/formulaic/templates/formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3052 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templates/formulaic/bootstrap-form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1181 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templates/formulaic/form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3114 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templates/formulaic/gate-form.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.609784 formification-1.1.1/formulaic/templatetags/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templatetags/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2309 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templatetags/form.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      217 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/templatetags/setting_tags.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:56:37.611190 formification-1.1.1/formulaic/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      110 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1876 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/test_csv_export.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     5023 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/test_forms.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1978 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/test_models.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1533 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/test_validators.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     7798 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/tests/test_views.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1127 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/urls.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2058 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/utils.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1246 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/validators.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     8838 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/views.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2099 2023-06-05 06:46:49.000000 formification-1.1.1/formulaic/widgets.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1096 2023-06-07 10:56:37.612072 formification-1.1.1/setup.cfg
+-rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 formification-1.1.1/setup.py
```

### Comparing `formification-1.1.0/LICENSE` & `formification-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/PKG-INFO` & `formification-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: formification
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Django app for building custom web forms and collecting submissions.
 Home-page: https://github.com/levimoore1992/formification
 Author: Levi Moore
 Author-email: levimoore1992@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Formulaic
```

### Comparing `formification-1.1.0/README.md` & `formification-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formification.egg-info/PKG-INFO` & `formification-1.1.1/formification.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: formification
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Django app for building custom web forms and collecting submissions.
 Home-page: https://github.com/levimoore1992/formification
 Author: Levi Moore
 Author-email: levimoore1992@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Formulaic
```

### Comparing `formification-1.1.0/formification.egg-info/SOURCES.txt` & `formification-1.1.1/formification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/admin.py` & `formification-1.1.1/formulaic/admin.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/auto_populate.py` & `formification-1.1.1/formulaic/auto_populate.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/beanstalk_jobs.py` & `formification-1.1.1/formulaic/beanstalk_jobs.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/csv_export.py` & `formification-1.1.1/formulaic/csv_export.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/fields.py` & `formification-1.1.1/formulaic/fields.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/forms.py` & `formification-1.1.1/formulaic/forms.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/migrations/0001_initial.py` & `formification-1.1.1/formulaic/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/migrations/0003_auto_20201230_1406.py` & `formification-1.1.1/formulaic/migrations/0003_auto_20201230_1406.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/models.py` & `formification-1.1.1/formulaic/models.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/rules.py` & `formification-1.1.1/formulaic/rules.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/serializers.py` & `formification-1.1.1/formulaic/serializers.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/css/edit_fields.css` & `formification-1.1.1/formulaic/static/admin/formulaic/css/edit_fields.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/css/form.css` & `formification-1.1.1/formulaic/static/admin/formulaic/css/form.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/README.md` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/README.md`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/index.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/router.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/package.json` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/package.json`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js` & `formification-1.1.1/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-090.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-090.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-270.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-270.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/arrow-move.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/arrow-move.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/backup/arrow-move.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/backup/pencil.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/backup/pencil.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/backup/tick.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/backup/tick.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/icons-grappelli.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/icons-grappelli.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/label-bg.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/label-bg.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/loading.gif` & `formification-1.1.1/formulaic/static/admin/formulaic/images/loading.gif`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/minus.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/minus.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/pencil.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/pencil.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/plus.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/plus.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/images/tick.png` & `formification-1.1.1/formulaic/static/admin/formulaic/images/tick.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/js/edit_fields.js` & `formification-1.1.1/formulaic/static/admin/formulaic/js/edit_fields.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/js/form.js` & `formification-1.1.1/formulaic/static/admin/formulaic/js/form.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js` & `formification-1.1.1/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/css/bootstrap.css` & `formification-1.1.1/formulaic/static/formulaic/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/css/bootstrap.min.css` & `formification-1.1.1/formulaic/static/formulaic/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/css/gate-form.css` & `formification-1.1.1/formulaic/static/formulaic/css/gate-form.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/css/intlTelInput.css` & `formification-1.1.1/formulaic/static/formulaic/css/intlTelInput.css`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/img/flags.png` & `formification-1.1.1/formulaic/static/formulaic/img/flags.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/img/flags@2x.png` & `formification-1.1.1/formulaic/static/formulaic/img/flags@2x.png`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/js/custom_form.js` & `formification-1.1.1/formulaic/static/formulaic/js/custom_form.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/js/intTelInput_utils.js` & `formification-1.1.1/formulaic/static/formulaic/js/intTelInput_utils.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/js/intlTelInput.min.js` & `formification-1.1.1/formulaic/static/formulaic/js/intlTelInput.min.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/static/formulaic/js/phoneNumber.js` & `formification-1.1.1/formulaic/static/formulaic/js/phoneNumber.js`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templates/admin/formulaic/form/change_form.html` & `formification-1.1.1/formulaic/templates/admin/formulaic/form/change_form.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templates/admin/formulaic/form/change_list.html` & `formification-1.1.1/formulaic/templates/admin/formulaic/form/change_list.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templates/formulaic/bootstrap-form.html` & `formification-1.1.1/formulaic/templates/formulaic/bootstrap-form.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templates/formulaic/form.html` & `formification-1.1.1/formulaic/templates/formulaic/form.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templates/formulaic/gate-form.html` & `formification-1.1.1/formulaic/templates/formulaic/gate-form.html`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/templatetags/form.py` & `formification-1.1.1/formulaic/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/tests/test_csv_export.py` & `formification-1.1.1/formulaic/tests/test_csv_export.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/tests/test_forms.py` & `formification-1.1.1/formulaic/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/tests/test_models.py` & `formification-1.1.1/formulaic/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/tests/test_validators.py` & `formification-1.1.1/formulaic/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/tests/test_views.py` & `formification-1.1.1/formulaic/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/urls.py` & `formification-1.1.1/formulaic/urls.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/utils.py` & `formification-1.1.1/formulaic/utils.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/validators.py` & `formification-1.1.1/formulaic/validators.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/views.py` & `formification-1.1.1/formulaic/views.py`

 * *Files identical despite different names*

### Comparing `formification-1.1.0/formulaic/widgets.py` & `formification-1.1.1/formulaic/widgets.py`

 * *Files identical despite different names*

