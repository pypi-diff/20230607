# Comparing `tmp/django-formulaic-0.1.0.tar.gz` & `tmp/django-formulaic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formulaic-0.1.0.tar", last modified: Sat Apr  8 03:15:53 2023, max compression
+gzip compressed data, was "django-formulaic-1.0.0.tar", last modified: Wed Jun  7 10:19:35 2023, max compression
```

## Comparing `django-formulaic-0.1.0.tar` & `django-formulaic-1.0.0.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.760174 django-formulaic-0.1.0/
--rw-r--r--   0 lmoore     (503) staff       (20)     1072 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/LICENSE
--rw-r--r--   0 lmoore     (503) staff       (20)      111 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/MANIFEST.in
--rw-r--r--   0 lmoore     (503) staff       (20)     7176 2023-04-08 03:15:53.760535 django-formulaic-0.1.0/PKG-INFO
--rw-r--r--   0 lmoore     (503) staff       (20)     4635 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/README.md
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.000775 django-formulaic-0.1.0/django_formulaic.egg-info/
--rw-r--r--   0 lmoore     (503) staff       (20)     7176 2023-04-08 03:15:52.000000 django-formulaic-0.1.0/django_formulaic.egg-info/PKG-INFO
--rw-r--r--   0 lmoore     (503) staff       (20)    17735 2023-04-08 03:15:52.000000 django-formulaic-0.1.0/django_formulaic.egg-info/SOURCES.txt
--rw-r--r--   0 lmoore     (503) staff       (20)        1 2023-04-08 03:15:52.000000 django-formulaic-0.1.0/django_formulaic.egg-info/dependency_links.txt
--rw-r--r--   0 lmoore     (503) staff       (20)      237 2023-04-08 03:15:52.000000 django-formulaic-0.1.0/django_formulaic.egg-info/requires.txt
--rw-r--r--   0 lmoore     (503) staff       (20)       10 2023-04-08 03:15:52.000000 django-formulaic-0.1.0/django_formulaic.egg-info/top_level.txt
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.039232 django-formulaic-0.1.0/formulaic/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/__init__.py
--rw-r--r--   0 lmoore     (503) staff       (20)     3461 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/admin.py
--rw-r--r--   0 lmoore     (503) staff       (20)       93 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/apps.py
--rw-r--r--   0 lmoore     (503) staff       (20)     2043 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/auto_populate.py
--rw-r--r--   0 lmoore     (503) staff       (20)      768 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/beanstalk_jobs.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1337 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/csv_export.py
--rw-r--r--   0 lmoore     (503) staff       (20)       93 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/exceptions.py
--rw-r--r--   0 lmoore     (503) staff       (20)     3809 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/fields.py
--rw-r--r--   0 lmoore     (503) staff       (20)     3415 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/forms.py
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.050840 django-formulaic-0.1.0/formulaic/migrations/
--rw-r--r--   0 lmoore     (503) staff       (20)    11960 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/migrations/0001_initial.py
--rw-r--r--   0 lmoore     (503) staff       (20)      379 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/migrations/0002_add_default_to_field_enabled.py
--rw-r--r--   0 lmoore     (503) staff       (20)      624 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/migrations/0003_auto_20201230_1406.py
--rw-r--r--   0 lmoore     (503) staff       (20)      486 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/migrations/0004_submission_promo_source.py
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/migrations/__init__.py
--rw-r--r--   0 lmoore     (503) staff       (20)    31405 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/models.py
--rw-r--r--   0 lmoore     (503) staff       (20)     4640 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/rules.py
--rw-r--r--   0 lmoore     (503) staff       (20)    11002 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/serializers.py
--rw-r--r--   0 lmoore     (503) staff       (20)      193 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/settings.py
--rw-r--r--   0 lmoore     (503) staff       (20)      186 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/signals.py
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.964483 django-formulaic-0.1.0/formulaic/static/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.923958 django-formulaic-0.1.0/formulaic/static/admin/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.963649 django-formulaic-0.1.0/formulaic/static/admin/formulaic/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.057093 django-formulaic-0.1.0/formulaic/static/admin/formulaic/css/
--rw-r--r--   0 lmoore     (503) staff       (20)     3714 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/css/edit_fields.css
--rw-r--r--   0 lmoore     (503) staff       (20)      837 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/css/form.css
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.105938 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/
--rw-r--r--   0 lmoore     (503) staff       (20)       60 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.bowerrc
--rw-r--r--   0 lmoore     (503) staff       (20)      368 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.editorconfig
--rw-r--r--   0 lmoore     (503) staff       (20)      298 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.ember-cli
--rw-r--r--   0 lmoore     (503) staff       (20)      185 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.eslintrc.js
--rw-r--r--   0 lmoore     (503) staff       (20)      243 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.gitignore
--rw-r--r--   0 lmoore     (503) staff       (20)        7 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.nvmrc
--rw-r--r--   0 lmoore     (503) staff       (20)      336 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.travis.yml
--rw-r--r--   0 lmoore     (503) staff       (20)       37 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/.watchmanconfig
--rw-r--r--   0 lmoore     (503) staff       (20)     1832 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/README.md
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.121841 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.125009 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/
--rw-r--r--   0 lmoore     (503) staff       (20)      943 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js
--rw-r--r--   0 lmoore     (503) staff       (20)      445 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/app.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.185556 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/.gitkeep
--rw-r--r--   0 lmoore     (503) staff       (20)     1191 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox-select-multiple.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-email.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-full-name.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-hidden.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-integer.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-phone-number.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-radio-select.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select-multiple.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-text.js
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-textarea.js
--rw-r--r--   0 lmoore     (503) staff       (20)     4268 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2809 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2463 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js
--rw-r--r--   0 lmoore     (503) staff       (20)      163 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-fields.js
--rw-r--r--   0 lmoore     (503) staff       (20)     1344 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js
--rw-r--r--   0 lmoore     (503) staff       (20)      321 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rules.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.192238 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/.gitkeep
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.203788 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.222764 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/
--rw-r--r--   0 lmoore     (503) staff       (20)     1837 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)       73 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/booleanfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2862 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      313 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/hiddenfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      112 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/index.js
--rw-r--r--   0 lmoore     (503) staff       (20)       73 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/textfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)     6031 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js
--rw-r--r--   0 lmoore     (503) staff       (20)      597 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2011 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js
--rw-r--r--   0 lmoore     (503) staff       (20)     3030 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js
--rw-r--r--   0 lmoore     (503) staff       (20)       94 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.225528 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/.gitkeep
--rw-r--r--   0 lmoore     (503) staff       (20)      902 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.227818 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/
--rw-r--r--   0 lmoore     (503) staff       (20)      333 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/cookie-initializer.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.276197 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/.gitkeep
--rw-r--r--   0 lmoore     (503) staff       (20)      463 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/basefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      376 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/booleanfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      719 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      387 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/field.js
--rw-r--r--   0 lmoore     (503) staff       (20)      229 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/form.js
--rw-r--r--   0 lmoore     (503) staff       (20)      362 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/hiddenfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      195 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/option.js
--rw-r--r--   0 lmoore     (503) staff       (20)      200 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optiongroup.js
--rw-r--r--   0 lmoore     (503) staff       (20)      199 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optionlist.js
--rw-r--r--   0 lmoore     (503) staff       (20)      124 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/privacypolicy.js
--rw-r--r--   0 lmoore     (503) staff       (20)      263 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rule.js
--rw-r--r--   0 lmoore     (503) staff       (20)      458 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rulecondition.js
--rw-r--r--   0 lmoore     (503) staff       (20)      419 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/ruleresult.js
--rw-r--r--   0 lmoore     (503) staff       (20)      253 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submission.js
--rw-r--r--   0 lmoore     (503) staff       (20)      155 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submissionsource.js
--rw-r--r--   0 lmoore     (503) staff       (20)      326 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/textfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)       65 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/resolver.js
--rw-r--r--   0 lmoore     (503) staff       (20)      991 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.281414 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/.gitkeep
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.292953 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/
--rw-r--r--   0 lmoore     (503) staff       (20)     9006 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2120 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js
--rw-r--r--   0 lmoore     (503) staff       (20)     6219 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js
--rw-r--r--   0 lmoore     (503) staff       (20)     2040 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js
--rw-r--r--   0 lmoore     (503) staff       (20)      221 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.306810 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/
--rw-r--r--   0 lmoore     (503) staff       (20)      329 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/field.js
--rw-r--r--   0 lmoore     (503) staff       (20)      191 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optiongroup.js
--rw-r--r--   0 lmoore     (503) staff       (20)      190 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optionlist.js
--rw-r--r--   0 lmoore     (503) staff       (20)      235 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/rule.js
--rw-r--r--   0 lmoore     (503) staff       (20)      103 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/submissionsource.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.309285 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/
--rw-r--r--   0 lmoore     (503) staff       (20)     6320 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.315174 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/
--rw-r--r--   0 lmoore     (503) staff       (20)      114 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/application.hbs
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.370585 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/.gitkeep
--rw-r--r--   0 lmoore     (503) staff       (20)       28 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/base-sortable.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      378 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox-select-multiple.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      259 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)       72 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-email.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)       70 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-full-name.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      101 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-hidden.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)       61 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-integer.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)       69 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-phone-number.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      743 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      176 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select-multiple.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      339 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)       73 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-text.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      213 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-textarea.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1559 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1427 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      803 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      556 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1711 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      619 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.383199 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.400543 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/
--rw-r--r--   0 lmoore     (503) staff       (20)     1786 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     4565 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     3599 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      756 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1497 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1663 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      970 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     4350 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     1014 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)     2677 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs
--rw-r--r--   0 lmoore     (503) staff       (20)      159 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form.hbs
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.403333 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/
--rw-r--r--   0 lmoore     (503) staff       (20)      220 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/json.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.409476 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/
--rw-r--r--   0 lmoore     (503) staff       (20)      922 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js
--rw-r--r--   0 lmoore     (503) staff       (20)      220 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/slug.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.412131 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/
--rw-r--r--   0 lmoore     (503) staff       (20)     2394 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.426820 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/
--rw-r--r--   0 lmoore     (503) staff       (20)     1124 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)       74 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/booleanfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)      522 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js
--rw-r--r--   0 lmoore     (503) staff       (20)       74 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/hiddenfield.js
--rw-r--r--   0 lmoore     (503) staff       (20)       74 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/textfield.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.435454 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/
--rw-r--r--   0 lmoore     (503) staff       (20)     2129 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js
--rw-r--r--   0 lmoore     (503) staff       (20)      622 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js
--rw-r--r--   0 lmoore     (503) staff       (20)     1668 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js
--rw-r--r--   0 lmoore     (503) staff       (20)      231 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/bower.json
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.438266 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/
--rw-r--r--   0 lmoore     (503) staff       (20)     1308 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.449705 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.515092 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/
--rw-r--r--   0 lmoore     (503) staff       (20)   201293 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css
--rw-r--r--   0 lmoore     (503) staff       (20)    96917 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map
--rw-r--r--   0 lmoore     (503) staff       (20)   197827 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js
--rw-r--r--   0 lmoore     (503) staff       (20)   244408 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map
--rw-r--r--   0 lmoore     (503) staff       (20)    26702 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.536168 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/
--rw-r--r--   0 lmoore     (503) staff       (20)      218 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/bg-stripes.png
--rw-r--r--   0 lmoore     (503) staff       (20)    16445 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png
--rw-r--r--   0 lmoore     (503) staff       (20)     8424 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css
--rw-r--r--   0 lmoore     (503) staff       (20)   221524 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js
--rw-r--r--   0 lmoore     (503) staff       (20)   276278 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map
--rw-r--r--   0 lmoore     (503) staff       (20)    38972 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js
--rw-r--r--   0 lmoore     (503) staff       (20)    47670 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map
--rw-r--r--   0 lmoore     (503) staff       (20)     9760 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css
--rw-r--r--   0 lmoore     (503) staff       (20)  3564382 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js
--rw-r--r--   0 lmoore     (503) staff       (20)  4324732 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map
--rw-r--r--   0 lmoore     (503) staff       (20)      585 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.947709 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.539109 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/
--rw-r--r--   0 lmoore     (503) staff       (20)    91113 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.554322 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/
--rw-r--r--   0 lmoore     (503) staff       (20)    20127 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 lmoore     (503) staff       (20)   108738 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 lmoore     (503) staff       (20)    45404 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 lmoore     (503) staff       (20)    23424 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 lmoore     (503) staff       (20)    18028 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 lmoore     (503) staff       (20)     1508 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html
--rw-r--r--   0 lmoore     (503) staff       (20)       51 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/robots.txt
--rw-r--r--   0 lmoore     (503) staff       (20)      681 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.556903 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/
--rw-r--r--   0 lmoore     (503) staff       (20)     2051 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html
--rw-r--r--   0 lmoore     (503) staff       (20)     1645 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js
--rw-r--r--   0 lmoore     (503) staff       (20)   234080 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json
--rw-r--r--   0 lmoore     (503) staff       (20)     1381 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/package.json
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.562010 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.952548 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.564338 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/
--rw-r--r--   0 lmoore     (503) staff       (20)      218 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/bg-stripes.png
--rw-r--r--   0 lmoore     (503) staff       (20)      585 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml
--rw-r--r--   0 lmoore     (503) staff       (20)       51 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/robots.txt
--rw-r--r--   0 lmoore     (503) staff       (20)      214 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/testem.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.571130 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/
--rw-r--r--   0 lmoore     (503) staff       (20)       55 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/.eslintrc.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.581210 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/
--rw-r--r--   0 lmoore     (503) staff       (20)      117 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/destroy-app.js
--rw-r--r--   0 lmoore     (503) staff       (20)      617 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js
--rw-r--r--   0 lmoore     (503) staff       (20)      255 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/resolver.js
--rw-r--r--   0 lmoore     (503) staff       (20)      474 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/start-app.js
--rw-r--r--   0 lmoore     (503) staff       (20)     1074 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.583698 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/.gitkeep
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.617791 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/
--rw-r--r--   0 lmoore     (503) staff       (20)      661 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      756 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      676 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      661 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      681 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      666 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      671 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      696 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      696 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      711 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      666 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      656 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      676 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      666 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js
--rw-r--r--   0 lmoore     (503) staff       (20)      112 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/test-helper.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.620769 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/.gitkeep
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.623587 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/
--rw-r--r--   0 lmoore     (503) staff       (20)      627 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.626422 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/
--rw-r--r--   0 lmoore     (503) staff       (20)      286 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/form-test.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.629113 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/.gitkeep
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.657550 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1629 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-090.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1658 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-270.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1845 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-move.png
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.672989 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/
--rwxr-xr-x   0 lmoore     (503) staff       (20)      663 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)      224 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/minus.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1548 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/pencil.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)      482 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/plus.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)      582 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/tick.png
--rw-r--r--   0 lmoore     (503) staff       (20)     9159 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/icons-grappelli.png
--rw-r--r--   0 lmoore     (503) staff       (20)      934 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/label-bg.png
--rw-r--r--   0 lmoore     (503) staff       (20)     2545 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/loading.gif
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1105 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/minus.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1905 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/pencil.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)     1541 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/plus.png
--rwxr-xr-x   0 lmoore     (503) staff       (20)      582 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/tick.png
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.682608 django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/
--rw-r--r--   0 lmoore     (503) staff       (20)    28628 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/edit_fields.js
--rw-r--r--   0 lmoore     (503) staff       (20)      794 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/form.js
--rw-r--r--   0 lmoore     (503) staff       (20)    93107 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.967866 django-formulaic-0.1.0/formulaic/static/formulaic/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.701542 django-formulaic-0.1.0/formulaic/static/formulaic/css/
--rw-r--r--   0 lmoore     (503) staff       (20)   219801 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/css/bootstrap.css
--rw-r--r--   0 lmoore     (503) staff       (20)   194385 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/css/bootstrap.min.css
--rw-r--r--   0 lmoore     (503) staff       (20)      239 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/css/custom_form.css
--rw-r--r--   0 lmoore     (503) staff       (20)     1407 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/css/gate-form.css
--rw-r--r--   0 lmoore     (503) staff       (20)    25253 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/css/intlTelInput.css
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.709218 django-formulaic-0.1.0/formulaic/static/formulaic/img/
--rw-r--r--   0 lmoore     (503) staff       (20)    70857 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/img/flags.png
--rw-r--r--   0 lmoore     (503) staff       (20)   174369 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/img/flags@2x.png
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.724163 django-formulaic-0.1.0/formulaic/static/formulaic/js/
--rw-r--r--   0 lmoore     (503) staff       (20)    20880 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/js/custom_form.js
--rw-r--r--   0 lmoore     (503) staff       (20)   246620 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/js/intTelInput_utils.js
--rw-r--r--   0 lmoore     (503) staff       (20)    29401 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/js/intlTelInput.min.js
--rw-r--r--   0 lmoore     (503) staff       (20)     1982 2023-04-07 05:41:47.000000 django-formulaic-0.1.0/formulaic/static/formulaic/js/phoneNumber.js
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.971739 django-formulaic-0.1.0/formulaic/templates/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.970201 django-formulaic-0.1.0/formulaic/templates/admin/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:52.971029 django-formulaic-0.1.0/formulaic/templates/admin/formulaic/
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.730000 django-formulaic-0.1.0/formulaic/templates/admin/formulaic/form/
--rw-r--r--   0 lmoore     (503) staff       (20)     1652 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templates/admin/formulaic/form/change_form.html
--rw-r--r--   0 lmoore     (503) staff       (20)      545 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templates/admin/formulaic/form/change_list.html
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.737070 django-formulaic-0.1.0/formulaic/templates/formulaic/
--rw-r--r--   0 lmoore     (503) staff       (20)     3052 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templates/formulaic/bootstrap-form.html
--rw-r--r--   0 lmoore     (503) staff       (20)     1181 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templates/formulaic/form.html
--rw-r--r--   0 lmoore     (503) staff       (20)     3114 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templates/formulaic/gate-form.html
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.743871 django-formulaic-0.1.0/formulaic/templatetags/
--rw-r--r--   0 lmoore     (503) staff       (20)        0 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templatetags/__init__.py
--rw-r--r--   0 lmoore     (503) staff       (20)     2309 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templatetags/form.py
--rw-r--r--   0 lmoore     (503) staff       (20)      217 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/templatetags/setting_tags.py
-drwxr-xr-x   0 lmoore     (503) staff       (20)        0 2023-04-08 03:15:53.758735 django-formulaic-0.1.0/formulaic/tests/
--rw-r--r--   0 lmoore     (503) staff       (20)      110 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/__init__.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1876 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/test_csv_export.py
--rw-r--r--   0 lmoore     (503) staff       (20)     5023 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/test_forms.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1978 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/test_models.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1533 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/test_validators.py
--rw-r--r--   0 lmoore     (503) staff       (20)     7798 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/tests/test_views.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1127 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/urls.py
--rw-r--r--   0 lmoore     (503) staff       (20)     2058 2023-04-08 03:08:13.000000 django-formulaic-0.1.0/formulaic/utils.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1246 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/validators.py
--rw-r--r--   0 lmoore     (503) staff       (20)     8838 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/views.py
--rw-r--r--   0 lmoore     (503) staff       (20)     2099 2023-04-07 05:41:48.000000 django-formulaic-0.1.0/formulaic/widgets.py
--rw-r--r--   0 lmoore     (503) staff       (20)     1282 2023-04-08 03:15:53.764375 django-formulaic-0.1.0/setup.cfg
--rw-r--r--   0 lmoore     (503) staff       (20)       37 2023-04-08 03:14:48.000000 django-formulaic-0.1.0/setup.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.792911 django-formulaic-1.0.0/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1066 2023-06-07 09:38:32.000000 django-formulaic-1.0.0/LICENSE
+-rw-rw-r--   0 levimoore   (501) staff       (20)      111 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/MANIFEST.in
+-rw-r--r--   0 levimoore   (501) staff       (20)     5695 2023-06-07 10:19:35.793013 django-formulaic-1.0.0/PKG-INFO
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4635 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/README.md
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.719102 django-formulaic-1.0.0/django_formulaic.egg-info/
+-rw-r--r--   0 levimoore   (501) staff       (20)     5695 2023-06-07 10:19:35.000000 django-formulaic-1.0.0/django_formulaic.egg-info/PKG-INFO
+-rw-r--r--   0 levimoore   (501) staff       (20)    17735 2023-06-07 10:19:35.000000 django-formulaic-1.0.0/django_formulaic.egg-info/SOURCES.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)        1 2023-06-07 10:19:35.000000 django-formulaic-1.0.0/django_formulaic.egg-info/dependency_links.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)      237 2023-06-07 10:19:35.000000 django-formulaic-1.0.0/django_formulaic.egg-info/requires.txt
+-rw-r--r--   0 levimoore   (501) staff       (20)       10 2023-06-07 10:19:35.000000 django-formulaic-1.0.0/django_formulaic.egg-info/top_level.txt
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.725332 django-formulaic-1.0.0/formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3461 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/admin.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/apps.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2043 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/auto_populate.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      768 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/beanstalk_jobs.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1337 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/csv_export.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)       93 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/exceptions.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3809 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/fields.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3415 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/forms.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.726212 django-formulaic-1.0.0/formulaic/migrations/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    11960 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/migrations/0001_initial.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      379 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/migrations/0002_add_default_to_field_enabled.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      624 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/migrations/0003_auto_20201230_1406.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      486 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/migrations/0004_submission_promo_source.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/migrations/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)    31413 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/models.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4640 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/rules.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)    11002 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/serializers.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      193 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/settings.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      186 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/signals.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.716398 django-formulaic-1.0.0/formulaic/static/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.652437 django-formulaic-1.0.0/formulaic/static/admin/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.716304 django-formulaic-1.0.0/formulaic/static/admin/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.726536 django-formulaic-1.0.0/formulaic/static/admin/formulaic/css/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3714 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/css/edit_fields.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)      837 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/css/form.css
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.730268 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)       60 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.bowerrc
+-rw-rw-r--   0 levimoore   (501) staff       (20)      368 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.editorconfig
+-rw-rw-r--   0 levimoore   (501) staff       (20)      298 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.ember-cli
+-rw-rw-r--   0 levimoore   (501) staff       (20)      185 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.eslintrc.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      243 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.gitignore
+-rw-rw-r--   0 levimoore   (501) staff       (20)        7 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.nvmrc
+-rw-rw-r--   0 levimoore   (501) staff       (20)      336 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.travis.yml
+-rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/.watchmanconfig
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1832 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/README.md
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.731153 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.731651 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      943 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      445 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/app.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.735876 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1191 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox-select-multiple.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-checkbox.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-email.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-full-name.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-hidden.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-integer.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-phone-number.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-radio-select.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select-multiple.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-select.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-text.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/preview-textarea.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4268 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2809 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2463 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      163 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1344 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      321 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rules.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.736296 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.737372 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.738511 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1837 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2862 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      313 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/textfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6031 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      597 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2011 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3030 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       94 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.738692 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/helpers/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)      902 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.738829 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      333 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/initializers/cookie-initializer.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.741871 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)      463 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      376 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      719 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      387 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      229 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      362 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      195 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/option.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      200 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optiongroup.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      199 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/optionlist.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      124 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/privacypolicy.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      263 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      458 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/rulecondition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      419 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/ruleresult.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      253 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submission.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      155 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/submissionsource.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      326 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/textfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       65 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/resolver.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      991 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.742149 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.742813 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9006 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2120 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6219 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2040 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      221 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.743638 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      329 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/field.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      191 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optiongroup.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      190 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/optionlist.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      235 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      103 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/serializers/submissionsource.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.743804 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     6320 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.744154 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      114 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/application.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.747671 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/.gitkeep
+-rw-rw-r--   0 levimoore   (501) staff       (20)       28 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/base-sortable.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      378 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox-select-multiple.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      259 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-checkbox.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       72 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-email.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       70 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-full-name.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      101 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-hidden.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       61 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-integer.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       69 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-phone-number.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      743 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      176 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select-multiple.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      339 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-select.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)       73 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-text.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      213 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-textarea.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1559 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1427 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      803 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      556 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1711 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      619 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.748432 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.749579 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1786 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4565 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3599 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1497 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1663 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      970 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     4350 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1014 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2677 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs
+-rw-rw-r--   0 levimoore   (501) staff       (20)      159 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form.hbs
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.749768 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/transforms/json.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.750166 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      922 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      220 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/slug.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.750343 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2394 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.751266 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1124 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/booleanfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      522 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/hiddenfield.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)       74 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/textfield.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.751757 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2129 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      622 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1668 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      231 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/bower.json
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.751928 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/config/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1308 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.752752 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.763128 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/
+-rw-rw-r--   0 levimoore   (501) staff       (20)   201293 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)    96917 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)   197827 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   244408 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)    26702 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.770672 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/images/bg-stripes.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)    16445 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     8424 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)   221524 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   276278 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)    38972 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    47670 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9760 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)  3564382 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)  4324732 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map
+-rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.654951 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.770973 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    91113 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.775726 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    20127 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 levimoore   (501) staff       (20)   108738 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 levimoore   (501) staff       (20)    45404 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 levimoore   (501) staff       (20)    23424 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 levimoore   (501) staff       (20)    18028 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1508 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/robots.txt
+-rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.776006 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2051 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1645 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   234080 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1381 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/package.json
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.776350 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.655384 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.776774 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      218 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/assets/images/bg-stripes.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)      585 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml
+-rw-rw-r--   0 levimoore   (501) staff       (20)       51 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/robots.txt
+-rw-rw-r--   0 levimoore   (501) staff       (20)      214 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/testem.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.777558 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)       55 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/.eslintrc.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.778584 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      117 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/destroy-app.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      617 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      255 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/resolver.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      474 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/start-app.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1074 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.778761 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.781795 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      756 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      661 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      681 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      671 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      696 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      711 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      656 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      676 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      666 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      112 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/test-helper.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.781967 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.782093 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      627 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.782483 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      286 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/routes/form-test.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.782693 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/vendor/.gitkeep
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.784685 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1629 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-090.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1658 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-270.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1845 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-move.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.785656 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      663 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      224 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/minus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1548 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/pencil.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      482 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/plus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/tick.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     9159 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/icons-grappelli.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)      934 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/label-bg.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2545 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/loading.gif
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1105 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/minus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1905 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/pencil.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)     1541 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/plus.png
+-rwxr-xr-x   0 levimoore   (501) staff       (20)      582 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/tick.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.786271 django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    28628 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/edit_fields.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)      794 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    93107 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.716633 django-formulaic-1.0.0/formulaic/static/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.788207 django-formulaic-1.0.0/formulaic/static/formulaic/css/
+-rw-rw-r--   0 levimoore   (501) staff       (20)   219801 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/css/bootstrap.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)   194385 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/css/bootstrap.min.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)      239 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/css/custom_form.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1407 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/css/gate-form.css
+-rw-rw-r--   0 levimoore   (501) staff       (20)    25253 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/css/intlTelInput.css
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.788957 django-formulaic-1.0.0/formulaic/static/formulaic/img/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    70857 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/img/flags.png
+-rw-rw-r--   0 levimoore   (501) staff       (20)   174369 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/img/flags@2x.png
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.790575 django-formulaic-1.0.0/formulaic/static/formulaic/js/
+-rw-rw-r--   0 levimoore   (501) staff       (20)    20880 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/js/custom_form.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)   246620 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/js/intTelInput_utils.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)    29401 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/js/intlTelInput.min.js
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1982 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/static/formulaic/js/phoneNumber.js
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.717007 django-formulaic-1.0.0/formulaic/templates/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.716849 django-formulaic-1.0.0/formulaic/templates/admin/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.716920 django-formulaic-1.0.0/formulaic/templates/admin/formulaic/
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.790922 django-formulaic-1.0.0/formulaic/templates/admin/formulaic/form/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1652 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templates/admin/formulaic/form/change_form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)      545 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templates/admin/formulaic/form/change_list.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.791392 django-formulaic-1.0.0/formulaic/templates/formulaic/
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3052 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templates/formulaic/bootstrap-form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1181 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templates/formulaic/form.html
+-rw-rw-r--   0 levimoore   (501) staff       (20)     3114 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templates/formulaic/gate-form.html
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.791857 django-formulaic-1.0.0/formulaic/templatetags/
+-rw-rw-r--   0 levimoore   (501) staff       (20)        0 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templatetags/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2309 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templatetags/form.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)      217 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/templatetags/setting_tags.py
+drwxr-xr-x   0 levimoore   (501) staff       (20)        0 2023-06-07 10:19:35.792766 django-formulaic-1.0.0/formulaic/tests/
+-rw-rw-r--   0 levimoore   (501) staff       (20)      110 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/__init__.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1876 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/test_csv_export.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     5023 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/test_forms.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1978 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/test_models.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1533 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/test_validators.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     7798 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/tests/test_views.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1127 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/urls.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2058 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/utils.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1246 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/validators.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     8838 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/views.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     2099 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/formulaic/widgets.py
+-rw-rw-r--   0 levimoore   (501) staff       (20)     1290 2023-06-07 10:19:35.793466 django-formulaic-1.0.0/setup.cfg
+-rw-rw-r--   0 levimoore   (501) staff       (20)       37 2023-06-05 06:46:49.000000 django-formulaic-1.0.0/setup.py
```

### Comparing `django-formulaic-0.1.0/PKG-INFO` & `django-formulaic-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,212 +1,212 @@
 Metadata-Version: 2.1
 Name: django-formulaic
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Django app for building custom web forms and collecting submissions.
-Home-page: https://github.com/Govexec/django-formulaic
-Author: Bryan Scott
-Author-email: bscott@govexec.com
+Home-page: https://github.com/levimoore1992/formification
+Author: Levi Moore
+Author-email: levimoore1992@gmail.com
 License: MIT
-Description: # Django Formulaic
-        
-        Django Formulaic allows Django Admin users to create custom forms.  The generated forms
-        are rendered using an extension of Django's Form class.  Form submission data is
-        collected by the app and accessible via its admin interface.
-        
-        _The app was originally developed for internal use.  We hope others will find it useful,
-        but it definitely lacks polish at this point in its development._
-        
-        ## Implementation
-        
-        ### Configuration
-        
-        ```python
-        # settings.py
-        INSTALLED_APPS = [
-            # ...
-            'django_filters',
-            'rest_framework',
-            'formulaic',
-            'admin_ordering',
-            # ...
-        ]
-        ```
-        
-        ```python
-        # urls.py
-        urlpatterns = [
-            # ...
-        
-            path('formulaic/', include('formulaic.urls')),
-            path('admin/', admin.site.urls),
-        ]
-        ```
-        
-        ```python
-        # settings.py
-        FORMULAIC_EXPORT_STORAGE_LOCATION = '/data/shared/assets/formulaic_exports'
-        ```
-        
-        ### Example Usage
-        
-        The `CustomForm` class extends Django's `forms.Form` class, so you can expect a lot of the same behavior you see in Django's documentation.
-        
-        ```python
-        # urls.py
-        from django.contrib import admin
-        from django.urls import path, include
-        
-        from formulaic_demo import views as fd_views
-        
-        urlpatterns = [
-            path('form-test/', fd_views.test_formulaic_form),
-            path(
-                'form-test/completed/',
-                fd_views.test_formulaic_form_complete,
-                name='form-complete'
-            ),
-        
-            path('formulaic/', include('formulaic.urls')),
-            path('admin/', admin.site.urls),
-        ]
-        ```
-        
-        ```python
-        # formulaic_demo/views.py
-        from django.shortcuts import redirect, render
-        
-        from formulaic.forms import CustomForm
-        from formulaic.models import Form
-        
-        
-        def test_formulaic_form(request):
-            formulaic_form = Form.objects.get(slug='robot-form')
-        
-            if request.method == 'POST':
-                form = CustomForm(
-                    request.POST,
-                    request=request,
-                    # page-specific name for form. will be stored with each submission in the
-                    # `source` field.
-                    instance_id='form-page-a',
-                    form=formulaic_form
-                )
-        
-                if form.is_valid():
-                    formulaic_form.create_submission(
-                        form.cleaned_data,
-                        source=form.instance_id,
-                        metadata={
-                            'extra-data-1': 'some data',
-                            'extra-data-2': 'more data',
-                        }
-                    )
-        
-                    return redirect('form-complete')
-        
-                elif not form.is_valid():
-                    errors = form.errors
-                    # raise Exception('Not valid {}'.format(form.errors))
-                    return render(request, 'formulaic_demo/formulaic-form.html', {
-                        'form': form
-                    })
-            else:
-                form = CustomForm(
-                    request=request,
-                    # page-specific name for form. will be stored with each submission in the
-                    # `source` field.
-                    instance_id='form-page-a',
-                    form=formulaic_form
-                )
-        
-            return render(request, 'formulaic_demo/formulaic-form.html', {
-                'form': form
-            })
-        
-        
-        def test_formulaic_form_complete(request):
-            formulaic_form = Form.objects.get(slug='robot-form')
-        
-            return render(request, 'formulaic_demo/formulaic-form-complete.html', {
-                'message': formulaic_form.success_message,
-            })
-        
-        ```
-        
-        ```html
-        <!-- templates/formulaic_demo/formulaic-form.html -->
-        <!DOCTYPE html>
-        <html lang="en">
-          <head>
-            <meta charset="utf-8">
-            <title>Test Formulaic Form</title>
-            <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
-          </head>
-          <body>
-            {{ form }}
-          </body>
-        </html>
-        
-        ```
-        
-        ```html
-        <!-- templates/formulaic_demoformulaic-form-complete.html -->
-        <!DOCTYPE html>
-        <html lang="en">
-          <head>
-            <meta charset="utf-8">
-            <title>Test Formulaic Form</title>
-          </head>
-          <body>
-            <p>{{ message }}</p>
-          </body>
-        </html>
-        
-        
-        ```
-        
-        ## Dependencies
-        
-        ### Python
-        
-        - Django 3.1 [wip: expanding to a wider range]
-        - Python 3.8 [wip: expanding to a wider range]
-        - django-rest-framework 3.11.2 [wip: any breaking changes in 4.x?]
-        - django-filter 0.9.2
-        - nameparser 0.3.16
-        - pyzipcode 2.0.0
-        - us 0.9.1
-        - tzlocal 1.2.2
-        
-        We would like to phase these out or make them optional
-        
-        - beautifulsoup4 4.4.1
-        - raven 6.10.0
-        - django-ckeditor 5.9.0
-        
-        ### JavaScript
-        
-        - **jQuery** must be included (for now) for the public-facing forms.
-        - The admin interface was built mostly using **EmberJS**.  You'll find setup instructions in the `README.md` at the root of that project: `/formulaic/static/admin/ember-formulaic`. This should only be important if you wish to make changes to the admin.
-        
-        ## License
-        
-        Formulaic is licensed under the MIT License.  View the `LICENSE` file in the root directory for more information.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >3.9
+Requires-Python: <=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Formulaic
+
+Django Formulaic allows Django Admin users to create custom forms.  The generated forms
+are rendered using an extension of Django's Form class.  Form submission data is
+collected by the app and accessible via its admin interface.
+
+_The app was originally developed for internal use.  We hope others will find it useful,
+but it definitely lacks polish at this point in its development._
+
+## Implementation
+
+### Configuration
+
+```python
+# settings.py
+INSTALLED_APPS = [
+    # ...
+    'django_filters',
+    'rest_framework',
+    'formulaic',
+    'admin_ordering',
+    # ...
+]
+```
+
+```python
+# urls.py
+urlpatterns = [
+    # ...
+
+    path('formulaic/', include('formulaic.urls')),
+    path('admin/', admin.site.urls),
+]
+```
+
+```python
+# settings.py
+FORMULAIC_EXPORT_STORAGE_LOCATION = '/data/shared/assets/formulaic_exports'
+```
+
+### Example Usage
+
+The `CustomForm` class extends Django's `forms.Form` class, so you can expect a lot of the same behavior you see in Django's documentation.
+
+```python
+# urls.py
+from django.contrib import admin
+from django.urls import path, include
+
+from formulaic_demo import views as fd_views
+
+urlpatterns = [
+    path('form-test/', fd_views.test_formulaic_form),
+    path(
+        'form-test/completed/',
+        fd_views.test_formulaic_form_complete,
+        name='form-complete'
+    ),
+
+    path('formulaic/', include('formulaic.urls')),
+    path('admin/', admin.site.urls),
+]
+```
+
+```python
+# formulaic_demo/views.py
+from django.shortcuts import redirect, render
+
+from formulaic.forms import CustomForm
+from formulaic.models import Form
+
+
+def test_formulaic_form(request):
+    formulaic_form = Form.objects.get(slug='robot-form')
+
+    if request.method == 'POST':
+        form = CustomForm(
+            request.POST,
+            request=request,
+            # page-specific name for form. will be stored with each submission in the
+            # `source` field.
+            instance_id='form-page-a',
+            form=formulaic_form
+        )
+
+        if form.is_valid():
+            formulaic_form.create_submission(
+                form.cleaned_data,
+                source=form.instance_id,
+                metadata={
+                    'extra-data-1': 'some data',
+                    'extra-data-2': 'more data',
+                }
+            )
+
+            return redirect('form-complete')
+
+        elif not form.is_valid():
+            errors = form.errors
+            # raise Exception('Not valid {}'.format(form.errors))
+            return render(request, 'formulaic_demo/formulaic-form.html', {
+                'form': form
+            })
+    else:
+        form = CustomForm(
+            request=request,
+            # page-specific name for form. will be stored with each submission in the
+            # `source` field.
+            instance_id='form-page-a',
+            form=formulaic_form
+        )
+
+    return render(request, 'formulaic_demo/formulaic-form.html', {
+        'form': form
+    })
+
+
+def test_formulaic_form_complete(request):
+    formulaic_form = Form.objects.get(slug='robot-form')
+
+    return render(request, 'formulaic_demo/formulaic-form-complete.html', {
+        'message': formulaic_form.success_message,
+    })
+
+```
+
+```html
+<!-- templates/formulaic_demo/formulaic-form.html -->
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+    <title>Test Formulaic Form</title>
+    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
+  </head>
+  <body>
+    {{ form }}
+  </body>
+</html>
+
+```
+
+```html
+<!-- templates/formulaic_demoformulaic-form-complete.html -->
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+    <title>Test Formulaic Form</title>
+  </head>
+  <body>
+    <p>{{ message }}</p>
+  </body>
+</html>
+
+
+```
+
+## Dependencies
+
+### Python
+
+- Django 3.1 [wip: expanding to a wider range]
+- Python 3.8 [wip: expanding to a wider range]
+- django-rest-framework 3.11.2 [wip: any breaking changes in 4.x?]
+- django-filter 0.9.2
+- nameparser 0.3.16
+- pyzipcode 2.0.0
+- us 0.9.1
+- tzlocal 1.2.2
+
+We would like to phase these out or make them optional
+
+- beautifulsoup4 4.4.1
+- raven 6.10.0
+- django-ckeditor 5.9.0
+
+### JavaScript
+
+- **jQuery** must be included (for now) for the public-facing forms.
+- The admin interface was built mostly using **EmberJS**.  You'll find setup instructions in the `README.md` at the root of that project: `/formulaic/static/admin/ember-formulaic`. This should only be important if you wish to make changes to the admin.
+
+## License
+
+Formulaic is licensed under the MIT License.  View the `LICENSE` file in the root directory for more information.
```

### Comparing `django-formulaic-0.1.0/README.md` & `django-formulaic-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/django_formulaic.egg-info/PKG-INFO` & `django-formulaic-1.0.0/django_formulaic.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,212 +1,212 @@
 Metadata-Version: 2.1
 Name: django-formulaic
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Django app for building custom web forms and collecting submissions.
-Home-page: https://github.com/Govexec/django-formulaic
-Author: Bryan Scott
-Author-email: bscott@govexec.com
+Home-page: https://github.com/levimoore1992/formification
+Author: Levi Moore
+Author-email: levimoore1992@gmail.com
 License: MIT
-Description: # Django Formulaic
-        
-        Django Formulaic allows Django Admin users to create custom forms.  The generated forms
-        are rendered using an extension of Django's Form class.  Form submission data is
-        collected by the app and accessible via its admin interface.
-        
-        _The app was originally developed for internal use.  We hope others will find it useful,
-        but it definitely lacks polish at this point in its development._
-        
-        ## Implementation
-        
-        ### Configuration
-        
-        ```python
-        # settings.py
-        INSTALLED_APPS = [
-            # ...
-            'django_filters',
-            'rest_framework',
-            'formulaic',
-            'admin_ordering',
-            # ...
-        ]
-        ```
-        
-        ```python
-        # urls.py
-        urlpatterns = [
-            # ...
-        
-            path('formulaic/', include('formulaic.urls')),
-            path('admin/', admin.site.urls),
-        ]
-        ```
-        
-        ```python
-        # settings.py
-        FORMULAIC_EXPORT_STORAGE_LOCATION = '/data/shared/assets/formulaic_exports'
-        ```
-        
-        ### Example Usage
-        
-        The `CustomForm` class extends Django's `forms.Form` class, so you can expect a lot of the same behavior you see in Django's documentation.
-        
-        ```python
-        # urls.py
-        from django.contrib import admin
-        from django.urls import path, include
-        
-        from formulaic_demo import views as fd_views
-        
-        urlpatterns = [
-            path('form-test/', fd_views.test_formulaic_form),
-            path(
-                'form-test/completed/',
-                fd_views.test_formulaic_form_complete,
-                name='form-complete'
-            ),
-        
-            path('formulaic/', include('formulaic.urls')),
-            path('admin/', admin.site.urls),
-        ]
-        ```
-        
-        ```python
-        # formulaic_demo/views.py
-        from django.shortcuts import redirect, render
-        
-        from formulaic.forms import CustomForm
-        from formulaic.models import Form
-        
-        
-        def test_formulaic_form(request):
-            formulaic_form = Form.objects.get(slug='robot-form')
-        
-            if request.method == 'POST':
-                form = CustomForm(
-                    request.POST,
-                    request=request,
-                    # page-specific name for form. will be stored with each submission in the
-                    # `source` field.
-                    instance_id='form-page-a',
-                    form=formulaic_form
-                )
-        
-                if form.is_valid():
-                    formulaic_form.create_submission(
-                        form.cleaned_data,
-                        source=form.instance_id,
-                        metadata={
-                            'extra-data-1': 'some data',
-                            'extra-data-2': 'more data',
-                        }
-                    )
-        
-                    return redirect('form-complete')
-        
-                elif not form.is_valid():
-                    errors = form.errors
-                    # raise Exception('Not valid {}'.format(form.errors))
-                    return render(request, 'formulaic_demo/formulaic-form.html', {
-                        'form': form
-                    })
-            else:
-                form = CustomForm(
-                    request=request,
-                    # page-specific name for form. will be stored with each submission in the
-                    # `source` field.
-                    instance_id='form-page-a',
-                    form=formulaic_form
-                )
-        
-            return render(request, 'formulaic_demo/formulaic-form.html', {
-                'form': form
-            })
-        
-        
-        def test_formulaic_form_complete(request):
-            formulaic_form = Form.objects.get(slug='robot-form')
-        
-            return render(request, 'formulaic_demo/formulaic-form-complete.html', {
-                'message': formulaic_form.success_message,
-            })
-        
-        ```
-        
-        ```html
-        <!-- templates/formulaic_demo/formulaic-form.html -->
-        <!DOCTYPE html>
-        <html lang="en">
-          <head>
-            <meta charset="utf-8">
-            <title>Test Formulaic Form</title>
-            <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
-          </head>
-          <body>
-            {{ form }}
-          </body>
-        </html>
-        
-        ```
-        
-        ```html
-        <!-- templates/formulaic_demoformulaic-form-complete.html -->
-        <!DOCTYPE html>
-        <html lang="en">
-          <head>
-            <meta charset="utf-8">
-            <title>Test Formulaic Form</title>
-          </head>
-          <body>
-            <p>{{ message }}</p>
-          </body>
-        </html>
-        
-        
-        ```
-        
-        ## Dependencies
-        
-        ### Python
-        
-        - Django 3.1 [wip: expanding to a wider range]
-        - Python 3.8 [wip: expanding to a wider range]
-        - django-rest-framework 3.11.2 [wip: any breaking changes in 4.x?]
-        - django-filter 0.9.2
-        - nameparser 0.3.16
-        - pyzipcode 2.0.0
-        - us 0.9.1
-        - tzlocal 1.2.2
-        
-        We would like to phase these out or make them optional
-        
-        - beautifulsoup4 4.4.1
-        - raven 6.10.0
-        - django-ckeditor 5.9.0
-        
-        ### JavaScript
-        
-        - **jQuery** must be included (for now) for the public-facing forms.
-        - The admin interface was built mostly using **EmberJS**.  You'll find setup instructions in the `README.md` at the root of that project: `/formulaic/static/admin/ember-formulaic`. This should only be important if you wish to make changes to the admin.
-        
-        ## License
-        
-        Formulaic is licensed under the MIT License.  View the `LICENSE` file in the root directory for more information.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >3.9
+Requires-Python: <=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Formulaic
+
+Django Formulaic allows Django Admin users to create custom forms.  The generated forms
+are rendered using an extension of Django's Form class.  Form submission data is
+collected by the app and accessible via its admin interface.
+
+_The app was originally developed for internal use.  We hope others will find it useful,
+but it definitely lacks polish at this point in its development._
+
+## Implementation
+
+### Configuration
+
+```python
+# settings.py
+INSTALLED_APPS = [
+    # ...
+    'django_filters',
+    'rest_framework',
+    'formulaic',
+    'admin_ordering',
+    # ...
+]
+```
+
+```python
+# urls.py
+urlpatterns = [
+    # ...
+
+    path('formulaic/', include('formulaic.urls')),
+    path('admin/', admin.site.urls),
+]
+```
+
+```python
+# settings.py
+FORMULAIC_EXPORT_STORAGE_LOCATION = '/data/shared/assets/formulaic_exports'
+```
+
+### Example Usage
+
+The `CustomForm` class extends Django's `forms.Form` class, so you can expect a lot of the same behavior you see in Django's documentation.
+
+```python
+# urls.py
+from django.contrib import admin
+from django.urls import path, include
+
+from formulaic_demo import views as fd_views
+
+urlpatterns = [
+    path('form-test/', fd_views.test_formulaic_form),
+    path(
+        'form-test/completed/',
+        fd_views.test_formulaic_form_complete,
+        name='form-complete'
+    ),
+
+    path('formulaic/', include('formulaic.urls')),
+    path('admin/', admin.site.urls),
+]
+```
+
+```python
+# formulaic_demo/views.py
+from django.shortcuts import redirect, render
+
+from formulaic.forms import CustomForm
+from formulaic.models import Form
+
+
+def test_formulaic_form(request):
+    formulaic_form = Form.objects.get(slug='robot-form')
+
+    if request.method == 'POST':
+        form = CustomForm(
+            request.POST,
+            request=request,
+            # page-specific name for form. will be stored with each submission in the
+            # `source` field.
+            instance_id='form-page-a',
+            form=formulaic_form
+        )
+
+        if form.is_valid():
+            formulaic_form.create_submission(
+                form.cleaned_data,
+                source=form.instance_id,
+                metadata={
+                    'extra-data-1': 'some data',
+                    'extra-data-2': 'more data',
+                }
+            )
+
+            return redirect('form-complete')
+
+        elif not form.is_valid():
+            errors = form.errors
+            # raise Exception('Not valid {}'.format(form.errors))
+            return render(request, 'formulaic_demo/formulaic-form.html', {
+                'form': form
+            })
+    else:
+        form = CustomForm(
+            request=request,
+            # page-specific name for form. will be stored with each submission in the
+            # `source` field.
+            instance_id='form-page-a',
+            form=formulaic_form
+        )
+
+    return render(request, 'formulaic_demo/formulaic-form.html', {
+        'form': form
+    })
+
+
+def test_formulaic_form_complete(request):
+    formulaic_form = Form.objects.get(slug='robot-form')
+
+    return render(request, 'formulaic_demo/formulaic-form-complete.html', {
+        'message': formulaic_form.success_message,
+    })
+
+```
+
+```html
+<!-- templates/formulaic_demo/formulaic-form.html -->
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+    <title>Test Formulaic Form</title>
+    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
+  </head>
+  <body>
+    {{ form }}
+  </body>
+</html>
+
+```
+
+```html
+<!-- templates/formulaic_demoformulaic-form-complete.html -->
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+    <title>Test Formulaic Form</title>
+  </head>
+  <body>
+    <p>{{ message }}</p>
+  </body>
+</html>
+
+
+```
+
+## Dependencies
+
+### Python
+
+- Django 3.1 [wip: expanding to a wider range]
+- Python 3.8 [wip: expanding to a wider range]
+- django-rest-framework 3.11.2 [wip: any breaking changes in 4.x?]
+- django-filter 0.9.2
+- nameparser 0.3.16
+- pyzipcode 2.0.0
+- us 0.9.1
+- tzlocal 1.2.2
+
+We would like to phase these out or make them optional
+
+- beautifulsoup4 4.4.1
+- raven 6.10.0
+- django-ckeditor 5.9.0
+
+### JavaScript
+
+- **jQuery** must be included (for now) for the public-facing forms.
+- The admin interface was built mostly using **EmberJS**.  You'll find setup instructions in the `README.md` at the root of that project: `/formulaic/static/admin/ember-formulaic`. This should only be important if you wish to make changes to the admin.
+
+## License
+
+Formulaic is licensed under the MIT License.  View the `LICENSE` file in the root directory for more information.
```

### Comparing `django-formulaic-0.1.0/django_formulaic.egg-info/SOURCES.txt` & `django-formulaic-1.0.0/django_formulaic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/admin.py` & `django-formulaic-1.0.0/formulaic/admin.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/auto_populate.py` & `django-formulaic-1.0.0/formulaic/auto_populate.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/beanstalk_jobs.py` & `django-formulaic-1.0.0/formulaic/beanstalk_jobs.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/csv_export.py` & `django-formulaic-1.0.0/formulaic/csv_export.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/fields.py` & `django-formulaic-1.0.0/formulaic/fields.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/forms.py` & `django-formulaic-1.0.0/formulaic/forms.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/migrations/0001_initial.py` & `django-formulaic-1.0.0/formulaic/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/migrations/0003_auto_20201230_1406.py` & `django-formulaic-1.0.0/formulaic/migrations/0003_auto_20201230_1406.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/models.py` & `django-formulaic-1.0.0/formulaic/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -949,14 +949,14 @@
 
         # replace ids with text values
         if value and self.field and self.field.subtype_in(ChoiceField.SUBTYPES.keys()):
             # convert to list for query
             if not isinstance(value, list):
                 value = [value]
 
-            selected_options = [options_lookup.get(json.loads(v)) for v in value]
+            selected_options = [options_lookup.get(json.loads(v), str(v)) for v in value]
             return ",".join(selected_options)
 
         return self.output_value
 
     def __str__(self):
         return "{}:{}".format(self.key, self.value)
```

### Comparing `django-formulaic-0.1.0/formulaic/rules.py` & `django-formulaic-1.0.0/formulaic/rules.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/serializers.py` & `django-formulaic-1.0.0/formulaic/serializers.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/css/edit_fields.css` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/css/edit_fields.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/css/form.css` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/css/form.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/README.md` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/README.md`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/adapters/application.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/base-sortable.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-condition.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/rule-result.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-field.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/components/sortable-rule.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/basefield.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields/choicefield.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/fields.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/index.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/rules.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/controllers/form/submissions.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/index.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/models/choicefield.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/router.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/fields.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/index.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/rules.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/routes/form/submissions.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/styles/app.less`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/preview-radio-select.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-condition.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/rule-result.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-field.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-fields.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rule.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/components/sortable-rules.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/booleanfield.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/choicefield.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/field.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/hiddenfield.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/index.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields/textfield.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/fields.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/index.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/rules.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/templates/form/submissions.hbs`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/utils/fields.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/factories.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/basefield.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/fields/choicefield.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rule.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/rulecondition.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/app/validators/rules/ruleresult.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/config/environment.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.css.map`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/ember-formulaic.map`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/failed.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/passed.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/test-support.map`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/tests.map`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/assets/vendor.map`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/crossdomain.xml`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/ember-welcome-page/images/construction.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/index.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/testem.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/dist/tests/index.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/ember-cli-build.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/npm-shrinkwrap.json`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/package.json` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/package.json`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/public/crossdomain.xml`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/helpers/module-for-acceptance.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/index.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/base-sortable-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-select-multiple-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-checkbox-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-email-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-full-name-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-hidden-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-integer-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-phone-number-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-radio-select-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-multiple-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-select-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-text-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/preview-textarea-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/integration/components/sortable-rules-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/ember-formulaic/tests/unit/initializers/cookie-test.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-090.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-090.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-270.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-270.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/arrow-move.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/arrow-move.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/arrow-move.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/pencil.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/pencil.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/backup/tick.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/backup/tick.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/icons-grappelli.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/icons-grappelli.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/label-bg.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/label-bg.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/loading.gif` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/loading.gif`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/minus.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/minus.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/pencil.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/pencil.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/plus.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/plus.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/images/tick.png` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/images/tick.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/edit_fields.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/edit_fields.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/form.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/form.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js` & `django-formulaic-1.0.0/formulaic/static/admin/formulaic/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/css/bootstrap.css` & `django-formulaic-1.0.0/formulaic/static/formulaic/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/css/bootstrap.min.css` & `django-formulaic-1.0.0/formulaic/static/formulaic/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/css/gate-form.css` & `django-formulaic-1.0.0/formulaic/static/formulaic/css/gate-form.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/css/intlTelInput.css` & `django-formulaic-1.0.0/formulaic/static/formulaic/css/intlTelInput.css`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/img/flags.png` & `django-formulaic-1.0.0/formulaic/static/formulaic/img/flags.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/img/flags@2x.png` & `django-formulaic-1.0.0/formulaic/static/formulaic/img/flags@2x.png`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/js/custom_form.js` & `django-formulaic-1.0.0/formulaic/static/formulaic/js/custom_form.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/js/intTelInput_utils.js` & `django-formulaic-1.0.0/formulaic/static/formulaic/js/intTelInput_utils.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/js/intlTelInput.min.js` & `django-formulaic-1.0.0/formulaic/static/formulaic/js/intlTelInput.min.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/static/formulaic/js/phoneNumber.js` & `django-formulaic-1.0.0/formulaic/static/formulaic/js/phoneNumber.js`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templates/admin/formulaic/form/change_form.html` & `django-formulaic-1.0.0/formulaic/templates/admin/formulaic/form/change_form.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templates/admin/formulaic/form/change_list.html` & `django-formulaic-1.0.0/formulaic/templates/admin/formulaic/form/change_list.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templates/formulaic/bootstrap-form.html` & `django-formulaic-1.0.0/formulaic/templates/formulaic/bootstrap-form.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templates/formulaic/form.html` & `django-formulaic-1.0.0/formulaic/templates/formulaic/form.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templates/formulaic/gate-form.html` & `django-formulaic-1.0.0/formulaic/templates/formulaic/gate-form.html`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/templatetags/form.py` & `django-formulaic-1.0.0/formulaic/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/tests/test_csv_export.py` & `django-formulaic-1.0.0/formulaic/tests/test_csv_export.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/tests/test_forms.py` & `django-formulaic-1.0.0/formulaic/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/tests/test_models.py` & `django-formulaic-1.0.0/formulaic/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/tests/test_validators.py` & `django-formulaic-1.0.0/formulaic/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/tests/test_views.py` & `django-formulaic-1.0.0/formulaic/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/urls.py` & `django-formulaic-1.0.0/formulaic/urls.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/utils.py` & `django-formulaic-1.0.0/formulaic/utils.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/validators.py` & `django-formulaic-1.0.0/formulaic/validators.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/views.py` & `django-formulaic-1.0.0/formulaic/views.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/formulaic/widgets.py` & `django-formulaic-1.0.0/formulaic/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formulaic-0.1.0/setup.cfg` & `django-formulaic-1.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = django-formulaic
-version = 0.1.0
+version = 1.0.0
 description = A Django app for building custom web forms and collecting submissions.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/Govexec/django-formulaic
-author = Bryan Scott
-author_email = bscott@govexec.com
+url = https://github.com/levimoore1992/formification
+author = Levi Moore
+author_email = levimoore1992@gmail.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.1
+	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
@@ -24,15 +24,15 @@
 	Programming Language :: Python :: 3.9
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
-python_requires = >3.9
+python_requires = <=3.9
 install_requires = 
 	Django >= 1.8
 	django-admin-ordering==0.13.1
 	django-ckeditor>=5.9.0
 	django-filter>=1.1.0
 	djangorestframework>=3.11.2
 	nameparser==0.3.16
```

