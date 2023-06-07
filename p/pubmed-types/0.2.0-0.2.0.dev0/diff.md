# Comparing `tmp/pubmed_types-0.2.0.tar.gz` & `tmp/pubmed_types-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_types-0.2.0.tar", max compression
+gzip compressed data, was "pubmed_types-0.2.0.dev0.tar", max compression
```

## Comparing `pubmed_types-0.2.0.tar` & `pubmed_types-0.2.0.dev0.tar`

### file list

```diff
@@ -1,665 +1,665 @@
--rw-r--r--   0        0        0     1072 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/LICENSE
--rw-r--r--   0        0        0     4736 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/README.md
--rw-r--r--   0        0        0     1534 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      547 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/src/pubmed_types/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/src/pubmed_types/models/__init__.py
--rw-r--r--   0        0        0    16884 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/src/pubmed_types/models/jats/__init__.py
--rw-r--r--   0        0        0     7420 2023-06-07 14:20:36.044921 pubmed_types-0.2.0/src/pubmed_types/models/jats/abbrev_journal_title.py
--rw-r--r--   0        0        0  1063860 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/access_date.py
--rw-r--r--   0        0        0     1373 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/alt_text.py
--rw-r--r--   0        0        0     8829 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/app.py
--rw-r--r--   0        0        0     8782 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/app_group.py
--rw-r--r--   0        0        0      108 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/array_orientation.py
--rw-r--r--   0        0        0     2648 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article.py
--rw-r--r--   0        0        0     1202 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_categories.py
--rw-r--r--   0        0        0      369 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_dtd_version.py
--rw-r--r--   0        0        0     1423 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_id.py
--rw-r--r--   0        0        0     9505 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_meta.py
--rw-r--r--   0        0        0     3813 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_version.py
--rw-r--r--   0        0        0      827 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/article_version_alternatives.py
--rw-r--r--   0        0        0     1720 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/author_notes.py
--rw-r--r--   0        0        0     2439 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/award_desc.py
--rw-r--r--   0        0        0     4305 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/award_group.py
--rw-r--r--   0        0        0     2432 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/award_name.py
--rw-r--r--   0        0        0     2079 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/back.py
--rw-r--r--   0        0        0     7354 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/body.py
--rw-r--r--   0        0        0       78 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/bold_toggle.py
--rw-r--r--   0        0        0      112 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/boxed_text_orientation.py
--rw-r--r--   0        0        0      149 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/boxed_text_position.py
--rw-r--r--   0        0        0      529 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/break_mod.py
--rw-r--r--   0        0        0      117 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/chem_struct_wrap_orientation.py
--rw-r--r--   0        0        0      154 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/chem_struct_wrap_position.py
--rw-r--r--   0        0        0     1344 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/city.py
--rw-r--r--   0        0        0       82 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/code_executable.py
--rw-r--r--   0        0        0      107 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/code_orientation.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/code_position.py
--rw-r--r--   0        0        0     1574 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/col.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/col_align.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/col_valign.py
--rw-r--r--   0        0        0     1765 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/colgroup.py
--rw-r--r--   0        0        0      153 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/colgroup_align.py
--rw-r--r--   0        0        0      138 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/colgroup_valign.py
--rw-r--r--   0        0        0     7391 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/conf_num.py
--rw-r--r--   0        0        0     7394 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/conf_theme.py
--rw-r--r--   0        0        0     4282 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/conference.py
--rw-r--r--   0        0        0       82 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_corresp.py
--rw-r--r--   0        0        0       83 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_deceased.py
--rw-r--r--   0        0        0       87 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_equal_contrib.py
--rw-r--r--   0        0        0     1940 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_id.py
--rw-r--r--   0        0        0       98 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_id_authenticated.py
--rw-r--r--   0        0        0     1889 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/contributed_resource_group.py
--rw-r--r--   0        0        0     1083 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/copyright_year.py
--rw-r--r--   0        0        0     8856 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/corresp.py
--rw-r--r--   0        0        0      871 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/count.py
--rw-r--r--   0        0        0     1907 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/counts.py
--rw-r--r--   0        0        0     3692 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/custom_meta.py
--rw-r--r--   0        0        0     1389 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/custom_meta_group.py
--rw-r--r--   0        0        0     1328 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/day.py
--rw-r--r--   0        0        0     1217 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/elocation_id.py
--rw-r--r--   0        0        0      704 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/equation_count.py
--rw-r--r--   0        0        0     1328 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/era.py
--rw-r--r--   0        0        0     3812 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/event.py
--rw-r--r--   0        0        0     3112 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/event_desc.py
--rw-r--r--   0        0        0     3121 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/extended_by.py
--rw-r--r--   0        0        0      692 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_count.py
--rw-r--r--   0        0        0      111 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_group_orientation.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_group_position.py
--rw-r--r--   0        0        0      106 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_orientation.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_position.py
--rw-r--r--   0        0        0     2865 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/floats_group.py
--rw-r--r--   0        0        0     1461 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/fpage.py
--rw-r--r--   0        0        0     2105 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/front.py
--rw-r--r--   0        0        0     9504 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/front_stub.py
--rw-r--r--   0        0        0     1657 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/funding_group.py
--rw-r--r--   0        0        0     9222 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/funding_statement.py
--rw-r--r--   0        0        0     1866 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/glyph_data.py
--rw-r--r--   0        0        0      728 2023-06-07 14:20:36.048920 pubmed_types-0.2.0/src/pubmed_types/models/jats/glyph_ref.py
--rw-r--r--   0        0        0      110 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/graphic_orientation.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/graphic_position.py
--rw-r--r--   0        0        0     7176 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/history.py
--rw-r--r--   0        0        0      528 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/hr.py
--rw-r--r--   0        0        0      718 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/index_term_range_end.py
--rw-r--r--   0        0        0     2029 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/institution_id.py
--rw-r--r--   0        0        0     3114 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_id.py
--rw-r--r--   0        0        0     7395 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_sponsor.py
--rw-r--r--   0        0        0     7400 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_subtitle.py
--rw-r--r--   0        0        0     1874 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_title_group.py
--rw-r--r--   0        0        0       80 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/italic_toggle.py
--rw-r--r--   0        0        0     1543 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_id.py
--rw-r--r--   0        0        0     2748 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_meta.py
--rw-r--r--   0        0        0     7406 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_subtitle.py
--rw-r--r--   0        0        0     7404 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_title.py
--rw-r--r--   0        0        0     1683 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_title_group.py
--rw-r--r--   0        0        0     1338 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/lpage.py
--rw-r--r--   0        0        0      108 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/media_orientation.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/media_position.py
--rw-r--r--   0        0        0     6803 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/meta_name.py
--rw-r--r--   0        0        0     6806 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/meta_value.py
--rw-r--r--   0        0        0     1408 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/milestone_end.py
--rw-r--r--   0        0        0     1414 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/milestone_start.py
--rw-r--r--   0        0        0       83 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/monospace_toggle.py
--rw-r--r--   0        0        0     1334 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/month.py
--rw-r--r--   0        0        0      153 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/name_name_style.py
--rw-r--r--   0        0        0     1422 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/object_id.py
--rw-r--r--   0        0        0       81 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/option_correct.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/__init__.py
--rw-r--r--   0        0        0      124 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/__init__.py
--rw-r--r--   0        0        0     1259 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/free_to_read.py
--rw-r--r--   0        0        0     1335 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/license_ref.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/__init__.py
--rw-r--r--   0        0        0    18862 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/abs.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/and_mod.py
--rw-r--r--   0        0        0     2149 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation.py
--rw-r--r--   0        0        0     2036 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml.py
--rw-r--r--   0        0        0      415 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml_model.py
--rw-r--r--   0        0        0     1582 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/approx.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccos.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccosh.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccot.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccoth.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccsc.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccsch.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsec.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsech.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsin.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsinh.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arctan.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arctanh.py
--rw-r--r--   0        0        0     1576 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arg.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/card.py
--rw-r--r--   0        0        0      466 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
--rw-r--r--   0        0        0     1737 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cbytes.py
--rw-r--r--   0        0        0     1584 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ceiling.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/codomain.py
--rw-r--r--   0        0        0      168 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/complexes.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.052920 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/compose.py
--rw-r--r--   0        0        0  1482653 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/condition.py
--rw-r--r--   0        0        0     1588 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/conjugate.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cos.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cosh.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cot.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/coth.py
--rw-r--r--   0        0        0     1767 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cs.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/csc.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/csch.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/curl.py
--rw-r--r--   0        0        0      189 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
--rw-r--r--   0        0        0      456 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/determinant.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/diff.py
--rw-r--r--   0        0        0      454 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divergence.py
--rw-r--r--   0        0        0     1582 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divide.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/domain.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/emptyset.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/eq.py
--rw-r--r--   0        0        0      454 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/equivalent.py
--rw-r--r--   0        0        0      454 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/eulergamma.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exists.py
--rw-r--r--   0        0        0     1576 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exp.py
--rw-r--r--   0        0        0      458 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exponentiale.py
--rw-r--r--   0        0        0     1588 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorial.py
--rw-r--r--   0        0        0     1586 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorof.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/false.py
--rw-r--r--   0        0        0     1580 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/floor.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/forall.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/gcd.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/geq.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/grad.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/gt.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ident.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/image.py
--rw-r--r--   0        0        0     1588 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginary.py
--rw-r--r--   0        0        0      454 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginaryi.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/implies.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/in_mod.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/infinity.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/int_mod.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/integers.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/intersect.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/interval.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/inverse.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lambda_mod.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/laplacian.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lcm.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/leq.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/limit.py
--rw-r--r--   0        0        0      161 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/linestyle.py
--rw-r--r--   0        0        0      161 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/list_order.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ln.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/log.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lt.py
--rw-r--r--   0        0        0      136 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maction_value.py
--rw-r--r--   0        0        0     2637 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup.py
--rw-r--r--   0        0        0      207 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
--rw-r--r--   0        0        0     2605 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
--rw-r--r--   0        0        0      139 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark_value.py
--rw-r--r--   0        0        0    74911 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.056921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_accent.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_accentunder.py
--rw-r--r--   0        0        0      161 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_align.py
--rw-r--r--   0        0        0      142 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_bevelled.py
--rw-r--r--   0        0        0      165 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_charalign.py
--rw-r--r--   0        0        0      166 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_denomalign.py
--rw-r--r--   0        0        0      131 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_dir.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_display.py
--rw-r--r--   0        0        0      146 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
--rw-r--r--   0        0        0      138 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_edge.py
--rw-r--r--   0        0        0      146 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_equalrows.py
--rw-r--r--   0        0        0      139 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_fence.py
--rw-r--r--   0        0        0      166 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_form.py
--rw-r--r--   0        0        0      199 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalign.py
--rw-r--r--   0        0        0      236 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
--rw-r--r--   0        0        0      235 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
--rw-r--r--   0        0        0      185 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_largeop.py
--rw-r--r--   0        0        0      225 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_linebreak.py
--rw-r--r--   0        0        0      228 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
--rw-r--r--   0        0        0      208 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_location.py
--rw-r--r--   0        0        0      495 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
--rw-r--r--   0        0        0      641 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
--rw-r--r--   0        0        0      164 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_numalign.py
--rw-r--r--   0        0        0      220 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_overflow.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_separator.py
--rw-r--r--   0        0        0      204 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_side.py
--rw-r--r--   0        0        0      200 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_stackalign.py
--rw-r--r--   0        0        0      142 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_stretchy.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_symmetric.py
--rw-r--r--   0        0        0      117 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_value.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/matrix.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/matrixrow.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/max.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mean.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/median.py
--rw-r--r--   0        0        0      137 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/menclose_value.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/merror_value.py
--rw-r--r--   0        0        0      136 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfenced_value.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
--rw-r--r--   0        0        0      165 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
--rw-r--r--   0        0        0      120 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_value.py
--rw-r--r--   0        0        0     5927 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph.py
--rw-r--r--   0        0        0      151 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
--rw-r--r--   0        0        0      643 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_value.py
--rw-r--r--   0        0        0     5355 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_dir.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_value.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/min.py
--rw-r--r--   0        0        0     1580 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/minus.py
--rw-r--r--   0        0        0     3231 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
--rw-r--r--   0        0        0      214 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
--rw-r--r--   0        0        0      139 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
--rw-r--r--   0        0        0      499 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
--rw-r--r--   0        0        0      137 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
--rw-r--r--   0        0        0      142 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
--rw-r--r--   0        0        0     5355 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_dir.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_value.py
--rw-r--r--   0        0        0    10173 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo.py
--rw-r--r--   0        0        0      138 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_accent.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_dir.py
--rw-r--r--   0        0        0      137 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fence.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
--rw-r--r--   0        0        0      164 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_form.py
--rw-r--r--   0        0        0      197 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
--rw-r--r--   0        0        0      234 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
--rw-r--r--   0        0        0      233 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
--rw-r--r--   0        0        0      139 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_largeop.py
--rw-r--r--   0        0        0      223 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
--rw-r--r--   0        0        0      226 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
--rw-r--r--   0        0        0      639 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_separator.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
--rw-r--r--   0        0        0      125 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_value.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mode.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/moment.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_accent.py
--rw-r--r--   0        0        0      162 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_align.py
--rw-r--r--   0        0        0      134 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_value.py
--rw-r--r--   0        0        0      136 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mpadded_value.py
--rw-r--r--   0        0        0      137 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mphantom_value.py
--rw-r--r--   0        0        0     2432 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
--rw-r--r--   0        0        0      134 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mroot_value.py
--rw-r--r--   0        0        0      131 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mrow_dir.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mrow_value.py
--rw-r--r--   0        0        0     5611 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_dir.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_value.py
--rw-r--r--   0        0        0      213 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarries_location.py
--rw-r--r--   0        0        0      292 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarries_value.py
--rw-r--r--   0        0        0      211 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarry_location.py
--rw-r--r--   0        0        0      290 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarry_value.py
--rw-r--r--   0        0        0      136 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msgroup_value.py
--rw-r--r--   0        0        0     3514 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline.py
--rw-r--r--   0        0        0      121 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline_value.py
--rw-r--r--   0        0        0     7532 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_dir.py
--rw-r--r--   0        0        0      151 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
--rw-r--r--   0        0        0      201 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalign.py
--rw-r--r--   0        0        0      238 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalignfirst.py
--rw-r--r--   0        0        0      237 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalignlast.py
--rw-r--r--   0        0        0      269 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
--rw-r--r--   0        0        0      643 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_value.py
--rw-r--r--   0        0        0      134 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msqrt_value.py
--rw-r--r--   0        0        0      134 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msrow_value.py
--rw-r--r--   0        0        0      167 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
--rw-r--r--   0        0        0      202 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
--rw-r--r--   0        0        0      123 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_value.py
--rw-r--r--   0        0        0      142 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_align.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
--rw-r--r--   0        0        0      168 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
--rw-r--r--   0        0        0      151 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
--rw-r--r--   0        0        0      168 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_form.py
--rw-r--r--   0        0        0      201 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
--rw-r--r--   0        0        0      238 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
--rw-r--r--   0        0        0      237 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
--rw-r--r--   0        0        0      187 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
--rw-r--r--   0        0        0      143 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
--rw-r--r--   0        0        0      227 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
--rw-r--r--   0        0        0      230 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
--rw-r--r--   0        0        0      210 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_location.py
--rw-r--r--   0        0        0      497 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
--rw-r--r--   0        0        0      643 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
--rw-r--r--   0        0        0      149 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
--rw-r--r--   0        0        0      166 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
--rw-r--r--   0        0        0      206 2023-06-07 14:20:36.060921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_side.py
--rw-r--r--   0        0        0      202 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
--rw-r--r--   0        0        0      144 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_value.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msub_value.py
--rw-r--r--   0        0        0      136 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msubsup_value.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msup_value.py
--rw-r--r--   0        0        0     6570 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
--rw-r--r--   0        0        0      206 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_side.py
--rw-r--r--   0        0        0      141 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_value.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtd.py
--rw-r--r--   0        0        0     5412 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext.py
--rw-r--r--   0        0        0      132 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_dir.py
--rw-r--r--   0        0        0      150 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
--rw-r--r--   0        0        0      642 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
--rw-r--r--   0        0        0      134 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_value.py
--rw-r--r--   0        0        0     3175 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr.py
--rw-r--r--   0        0        0      207 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
--rw-r--r--   0        0        0      132 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr_value.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_align.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_value.py
--rw-r--r--   0        0        0      146 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_accent.py
--rw-r--r--   0        0        0      151 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
--rw-r--r--   0        0        0      167 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_align.py
--rw-r--r--   0        0        0      139 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_value.py
--rw-r--r--   0        0        0      462 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
--rw-r--r--   0        0        0     1576 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/neq.py
--rw-r--r--   0        0        0     2401 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none.py
--rw-r--r--   0        0        0      133 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none_value.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/not_mod.py
--rw-r--r--   0        0        0      454 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notanumber.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notin.py
--rw-r--r--   0        0        0      456 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notprsubset.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notsubset.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/or_mod.py
--rw-r--r--   0        0        0      458 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/outerproduct.py
--rw-r--r--   0        0        0      456 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/partialdiff.py
--rw-r--r--   0        0        0      438 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/pi.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/plus.py
--rw-r--r--   0        0        0     1580 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/power.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/primes.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/product.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/prsubset.py
--rw-r--r--   0        0        0     1586 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/quotient.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rationals.py
--rw-r--r--   0        0        0     1578 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/real.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/reals.py
--rw-r--r--   0        0        0     1576 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rem.py
--rw-r--r--   0        0        0     1578 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/root.py
--rw-r--r--   0        0        0      460 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/scalarproduct.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sdev.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sec.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sech.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/selector.py
--rw-r--r--   0        0        0      215 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sep.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/setdiff.py
--rw-r--r--   0        0        0     1405 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/share.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sin.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sinh.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/subset.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sum.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tan.py
--rw-r--r--   0        0        0      442 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tanh.py
--rw-r--r--   0        0        0     1710 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tendsto.py
--rw-r--r--   0        0        0      444 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/times.py
--rw-r--r--   0        0        0      452 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/transpose.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/true.py
--rw-r--r--   0        0        0      448 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/union.py
--rw-r--r--   0        0        0      450 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/variance.py
--rw-r--r--   0        0        0      446 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/vector.py
--rw-r--r--   0        0        0      460 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/vectorproduct.py
--rw-r--r--   0        0        0      209 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/verticalalign.py
--rw-r--r--   0        0        0      440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/xor.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/__init__.py
--rw-r--r--   0        0        0      479 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/__init__.py
--rw-r--r--   0        0        0      187 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/actuate_type.py
--rw-r--r--   0        0        0     1883 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/arc_type.py
--rw-r--r--   0        0        0     1165 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/extended.py
--rw-r--r--   0        0        0     1449 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/locator_type.py
--rw-r--r--   0        0        0     1240 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/resource_type.py
--rw-r--r--   0        0        0      192 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/show_type.py
--rw-r--r--   0        0        0     1930 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/simple.py
--rw-r--r--   0        0        0     1199 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/title_elt_type.py
--rw-r--r--   0        0        0      228 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/type_type.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/xml/__init__.py
--rw-r--r--   0        0        0       15 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/__init__.py
--rw-r--r--   0        0        0      120 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/__init__.py
--rw-r--r--   0        0        0      118 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/lang_value.py
--rw-r--r--   0        0        0      154 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/space_value.py
--rw-r--r--   0        0        0      863 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/overline_end.py
--rw-r--r--   0        0        0      747 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/overline_start.py
--rw-r--r--   0        0        0       82 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/overline_toggle.py
--rw-r--r--   0        0        0      692 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/page_count.py
--rw-r--r--   0        0        0     1349 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/page_range.py
--rw-r--r--   0        0        0     1366 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/postal_code.py
--rw-r--r--   0        0        0      112 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/preformat_orientation.py
--rw-r--r--   0        0        0      149 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/preformat_position.py
--rw-r--r--   0        0        0     2142 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/principal_award_recipient.py
--rw-r--r--   0        0        0     1855 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/principal_investigator.py
--rw-r--r--   0        0        0     2483 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta.py
--rw-r--r--   0        0        0      148 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta_base_tagset.py
--rw-r--r--   0        0        0      109 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta_mathml_version.py
--rw-r--r--   0        0        0      138 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta_table_model.py
--rw-r--r--   0        0        0      116 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta_tagset_family.py
--rw-r--r--   0        0        0     2894 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_date.py
--rw-r--r--   0        0        0      740 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_date_not_available.py
--rw-r--r--   0        0        0      708 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_history.py
--rw-r--r--   0        0        0     2861 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_id.py
--rw-r--r--   0        0        0     1192 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/publisher.py
--rw-r--r--   0        0        0      268 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/question_question_response_type.py
--rw-r--r--   0        0        0      695 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/ref_count.py
--rw-r--r--   0        0        0     1440 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_group.py
--rw-r--r--   0        0        0     2014 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_id.py
--rw-r--r--   0        0        0     4989 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_name.py
--rw-r--r--   0        0        0     1009 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_wrap.py
--rw-r--r--   0        0        0     2223 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/response.py
--rw-r--r--   0        0        0     3127 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/restricted_by.py
--rw-r--r--   0        0        0       79 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/roman_toggle.py
--rw-r--r--   0        0        0      728 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/rp.py
--rw-r--r--   0        0        0     1346 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/rt.py
--rw-r--r--   0        0        0       83 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sans_serif_toggle.py
--rw-r--r--   0        0        0       76 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sc_toggle.py
--rw-r--r--   0        0        0     1337 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/season.py
--rw-r--r--   0        0        0     9005 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/self_uri.py
--rw-r--r--   0        0        0     7416 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/series_text.py
--rw-r--r--   0        0        0     7394 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/series_title.py
--rw-r--r--   0        0        0     7912 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sig.py
--rw-r--r--   0        0        0     8403 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sig_block.py
--rw-r--r--   0        0        0     1361 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/state.py
--rw-r--r--   0        0        0       80 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/strike_toggle.py
--rw-r--r--   0        0        0     8497 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/string_conf.py
--rw-r--r--   0        0        0      159 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/string_name_name_style.py
--rw-r--r--   0        0        0       87 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/styled_content_toggle.py
--rw-r--r--   0        0        0       92 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sub_arrange.py
--rw-r--r--   0        0        0     2576 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sub_article.py
--rw-r--r--   0        0        0       92 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/sup_arrange.py
--rw-r--r--   0        0        0      124 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/supplementary_material_orientation.py
--rw-r--r--   0        0        0      161 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/supplementary_material_position.py
--rw-r--r--   0        0        0     1316 2023-06-07 14:20:36.064921 pubmed_types-0.2.0/src/pubmed_types/models/jats/support_description.py
--rw-r--r--   0        0        0     1500 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/support_group.py
--rw-r--r--   0        0        0     9387 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/support_source.py
--rw-r--r--   0        0        0      695 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_count.py
--rw-r--r--   0        0        0      220 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_frame.py
--rw-r--r--   0        0        0      140 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_rules.py
--rw-r--r--   0        0        0      117 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_wrap_group_orientation.py
--rw-r--r--   0        0        0      154 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_wrap_group_position.py
--rw-r--r--   0        0        0      112 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_wrap_orientation.py
--rw-r--r--   0        0        0      149 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/table_wrap_position.py
--rw-r--r--   0        0        0      150 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tbody_align.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tbody_valign.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/td_align.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/td_scope.py
--rw-r--r--   0        0        0      132 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/td_valign.py
--rw-r--r--   0        0        0     1386 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tex_math.py
--rw-r--r--   0        0        0      128 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tex_math_notation.py
--rw-r--r--   0        0        0      150 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tfoot_align.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tfoot_valign.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/th_align.py
--rw-r--r--   0        0        0      129 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/th_scope.py
--rw-r--r--   0        0        0      132 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/th_valign.py
--rw-r--r--   0        0        0      150 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/thead_align.py
--rw-r--r--   0        0        0      135 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/thead_valign.py
--rw-r--r--   0        0        0     1542 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/title_group.py
--rw-r--r--   0        0        0      147 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tr_align.py
--rw-r--r--   0        0        0      132 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/tr_valign.py
--rw-r--r--   0        0        0     8910 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_abstract.py
--rw-r--r--   0        0        0     7376 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_subtitle.py
--rw-r--r--   0        0        0     1641 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_title_group.py
--rw-r--r--   0        0        0      866 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/underline_end.py
--rw-r--r--   0        0        0      750 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/underline_start.py
--rw-r--r--   0        0        0       83 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/underline_toggle.py
--rw-r--r--   0        0        0     2893 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/volume_issue_group.py
--rw-r--r--   0        0        0      692 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/word_count.py
--rw-r--r--   0        0        0     1627 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/jats/year.py
--rw-r--r--   0        0        0     7746 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/__init__.py
--rw-r--r--   0        0        0      566 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/abstract.py
--rw-r--r--   0        0        0     1612 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/abstract_text.py
--rw-r--r--   0        0        0      229 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/abstract_text_nlm_category.py
--rw-r--r--   0        0        0      342 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/accession_number_list.py
--rw-r--r--   0        0        0      933 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/affiliation.py
--rw-r--r--   0        0        0      588 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/affiliation_info.py
--rw-r--r--   0        0        0     3024 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article.py
--rw-r--r--   0        0        0      878 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_date.py
--rw-r--r--   0        0        0      466 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_id.py
--rw-r--r--   0        0        0      303 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_id_id_type.py
--rw-r--r--   0        0        0      364 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_id_list.py
--rw-r--r--   0        0        0      242 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_pub_model.py
--rw-r--r--   0        0        0     1418 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_title.py
--rw-r--r--   0        0        0     1934 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author.py
--rw-r--r--   0        0        0       80 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_equal_contrib.py
--rw-r--r--   0        0        0      838 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_list.py
--rw-r--r--   0        0        0       82 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_list_complete_yn.py
--rw-r--r--   0        0        0      100 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_list_type.py
--rw-r--r--   0        0        0       75 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_valid_yn.py
--rw-r--r--   0        0        0      765 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/beginning_date.py
--rw-r--r--   0        0        0     3113 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book.py
--rw-r--r--   0        0        0     4177 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_document.py
--rw-r--r--   0        0        0      587 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_document_set.py
--rw-r--r--   0        0        0     1415 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_title.py
--rw-r--r--   0        0        0      592 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/chemical.py
--rw-r--r--   0        0        0      356 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/chemical_list.py
--rw-r--r--   0        0        0     1036 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/citation.py
--rw-r--r--   0        0        0      936 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/citation_string.py
--rw-r--r--   0        0        0      934 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/coi_statement.py
--rw-r--r--   0        0        0     1421 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/collection_title.py
--rw-r--r--   0        0        0      936 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/collective_name.py
--rw-r--r--   0        0        0      934 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/comments_corrections.py
--rw-r--r--   0        0        0      424 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/comments_corrections_list.py
--rw-r--r--   0        0        0     1025 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/comments_corrections_ref_type.py
--rw-r--r--   0        0        0      768 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/contribution_date.py
--rw-r--r--   0        0        0      579 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/data_bank.py
--rw-r--r--   0        0        0      644 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/data_bank_list.py
--rw-r--r--   0        0        0       84 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/data_bank_list_complete_yn.py
--rw-r--r--   0        0        0      672 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/date_completed.py
--rw-r--r--   0        0        0      670 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/date_revised.py
--rw-r--r--   0        0        0      338 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/delete_citation.py
--rw-r--r--   0        0        0      309 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/delete_document.py
--rw-r--r--   0        0        0      948 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/descriptor_name.py
--rw-r--r--   0        0        0       88 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/descriptor_name_major_topic_yn.py
--rw-r--r--   0        0        0       86 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/descriptor_name_type.py
--rw-r--r--   0        0        0      397 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/disp_formula.py
--rw-r--r--   0        0        0      808 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/elocation_id.py
--rw-r--r--   0        0        0       88 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/elocation_id_eid_type.py
--rw-r--r--   0        0        0       80 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/elocation_id_valid_yn.py
--rw-r--r--   0        0        0      762 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/ending_date.py
--rw-r--r--   0        0        0      327 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/gene_symbol_list.py
--rw-r--r--   0        0        0      465 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/general_note.py
--rw-r--r--   0        0        0      152 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/general_note_owner.py
--rw-r--r--   0        0        0      806 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/grant.py
--rw-r--r--   0        0        0      611 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/grant_list.py
--rw-r--r--   0        0        0       81 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/grant_list_complete_yn.py
--rw-r--r--   0        0        0      382 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/history.py
--rw-r--r--   0        0        0      426 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/identifier.py
--rw-r--r--   0        0        0     1533 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/investigator.py
--rw-r--r--   0        0        0      380 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/investigator_list.py
--rw-r--r--   0        0        0       81 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/investigator_valid_yn.py
--rw-r--r--   0        0        0      514 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/issn.py
--rw-r--r--   0        0        0      100 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/issn_issn_type.py
--rw-r--r--   0        0        0      508 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/item_list.py
--rw-r--r--   0        0        0      869 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/journal.py
--rw-r--r--   0        0        0      938 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/journal_issue.py
--rw-r--r--   0        0        0      107 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/journal_issue_cited_medium.py
--rw-r--r--   0        0        0     1313 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword.py
--rw-r--r--   0        0        0      601 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword_list.py
--rw-r--r--   0        0        0      184 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword_list_owner.py
--rw-r--r--   0        0        0       81 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword_major_topic_yn.py
--rw-r--r--   0        0        0      460 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/location_label.py
--rw-r--r--   0        0        0      205 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/location_label_type.py
--rw-r--r--   0        0        0     5574 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_citation.py
--rw-r--r--   0        0        0      178 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_citation_owner.py
--rw-r--r--   0        0        0      284 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_citation_status.py
--rw-r--r--   0        0        0      813 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_journal_info.py
--rw-r--r--   0        0        0      618 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/mesh_heading.py
--rw-r--r--   0        0        0      376 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/mesh_heading_list.py
--rw-r--r--   0        0        0      423 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/name_of_substance.py
--rw-r--r--   0        0        0      354 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/object_list.py
--rw-r--r--   0        0        0      497 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/object_mod.py
--rw-r--r--   0        0        0      997 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_abstract.py
--rw-r--r--   0        0        0      223 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_abstract_type.py
--rw-r--r--   0        0        0      518 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_id.py
--rw-r--r--   0        0        0      257 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_id_source.py
--rw-r--r--   0        0        0      649 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pagination.py
--rw-r--r--   0        0        0     1118 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/param.py
--rw-r--r--   0        0        0      827 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/personal_name_subject.py
--rw-r--r--   0        0        0      426 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/personal_name_subject_list.py
--rw-r--r--   0        0        0      461 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pmid.py
--rw-r--r--   0        0        0      893 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pub_date.py
--rw-r--r--   0        0        0     1462 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pub_med_pub_date.py
--rw-r--r--   0        0        0      496 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pub_med_pub_date_pub_status.py
--rw-r--r--   0        0        0      423 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publication_type.py
--rw-r--r--   0        0        0      400 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publication_type_list.py
--rw-r--r--   0        0        0      557 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publisher.py
--rw-r--r--   0        0        0      935 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publisher_name.py
--rw-r--r--   0        0        0      600 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_article.py
--rw-r--r--   0        0        0      839 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_article_set.py
--rw-r--r--   0        0        0      611 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_book_article.py
--rw-r--r--   0        0        0      384 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_book_article_set.py
--rw-r--r--   0        0        0      987 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_book_data.py
--rw-r--r--   0        0        0     1213 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_data.py
--rw-r--r--   0        0        0      724 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/qualifier_name.py
--rw-r--r--   0        0        0       87 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/qualifier_name_major_topic_yn.py
--rw-r--r--   0        0        0      576 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/reference.py
--rw-r--r--   0        0        0      678 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/reference_list.py
--rw-r--r--   0        0        0      765 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/section.py
--rw-r--r--   0        0        0     1312 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/section_title.py
--rw-r--r--   0        0        0      347 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/sections.py
--rw-r--r--   0        0        0      928 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suffix.py
--rw-r--r--   0        0        0      386 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suppl_mesh_list.py
--rw-r--r--   0        0        0      668 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suppl_mesh_name.py
--rw-r--r--   0        0        0      185 2023-06-07 14:20:36.068921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suppl_mesh_name_type.py
--rw-r--r--   0        0        0     4251 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/u.py
--rw-r--r--   0        0        0      614 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/url.py
--rw-r--r--   0        0        0      661 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/url_lang.py
--rw-r--r--   0        0        0      150 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/url_type.py
--rw-r--r--   0        0        0     1043 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/vernacular_title.py
--rw-r--r--   0        0        0      933 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/models/pubmed/volume_title.py
--rw-r--r--   0        0        0        0 2023-06-07 14:20:36.072921 pubmed_types-0.2.0/src/pubmed_types/py.typed
--rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 pubmed_types-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/LICENSE
+-rw-r--r--   0        0        0     4808 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/README.md
+-rw-r--r--   0        0        0     1523 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/src/pubmed_types/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/src/pubmed_types/models/__init__.py
+-rw-r--r--   0        0        0    16884 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/__init__.py
+-rw-r--r--   0        0        0     7420 2023-06-07 01:53:13.336301 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/abbrev_journal_title.py
+-rw-r--r--   0        0        0  1063860 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/access_date.py
+-rw-r--r--   0        0        0     1373 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/alt_text.py
+-rw-r--r--   0        0        0     8829 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app.py
+-rw-r--r--   0        0        0     8782 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app_group.py
+-rw-r--r--   0        0        0      108 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/array_orientation.py
+-rw-r--r--   0        0        0     2648 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article.py
+-rw-r--r--   0        0        0     1202 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_categories.py
+-rw-r--r--   0        0        0      369 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_dtd_version.py
+-rw-r--r--   0        0        0     1423 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_id.py
+-rw-r--r--   0        0        0     9505 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_meta.py
+-rw-r--r--   0        0        0     3813 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version.py
+-rw-r--r--   0        0        0      827 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version_alternatives.py
+-rw-r--r--   0        0        0     1720 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/author_notes.py
+-rw-r--r--   0        0        0     2439 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_desc.py
+-rw-r--r--   0        0        0     4305 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_group.py
+-rw-r--r--   0        0        0     2432 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_name.py
+-rw-r--r--   0        0        0     2079 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/back.py
+-rw-r--r--   0        0        0     7354 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/body.py
+-rw-r--r--   0        0        0       78 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/bold_toggle.py
+-rw-r--r--   0        0        0      112 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/boxed_text_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/boxed_text_position.py
+-rw-r--r--   0        0        0      529 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/break_mod.py
+-rw-r--r--   0        0        0      117 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/chem_struct_wrap_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/chem_struct_wrap_position.py
+-rw-r--r--   0        0        0     1344 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/city.py
+-rw-r--r--   0        0        0       82 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/code_executable.py
+-rw-r--r--   0        0        0      107 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/code_orientation.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/code_position.py
+-rw-r--r--   0        0        0     1574 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/col.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/col_align.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/col_valign.py
+-rw-r--r--   0        0        0     1765 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/colgroup.py
+-rw-r--r--   0        0        0      153 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/colgroup_align.py
+-rw-r--r--   0        0        0      138 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/colgroup_valign.py
+-rw-r--r--   0        0        0     7391 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_num.py
+-rw-r--r--   0        0        0     7394 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_theme.py
+-rw-r--r--   0        0        0     4282 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conference.py
+-rw-r--r--   0        0        0       82 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_corresp.py
+-rw-r--r--   0        0        0       83 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_deceased.py
+-rw-r--r--   0        0        0       87 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_equal_contrib.py
+-rw-r--r--   0        0        0     1940 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_id.py
+-rw-r--r--   0        0        0       98 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_id_authenticated.py
+-rw-r--r--   0        0        0     1889 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contributed_resource_group.py
+-rw-r--r--   0        0        0     1083 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/copyright_year.py
+-rw-r--r--   0        0        0     8856 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/corresp.py
+-rw-r--r--   0        0        0      871 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/count.py
+-rw-r--r--   0        0        0     1907 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/counts.py
+-rw-r--r--   0        0        0     3692 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta.py
+-rw-r--r--   0        0        0     1389 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta_group.py
+-rw-r--r--   0        0        0     1328 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/day.py
+-rw-r--r--   0        0        0     1217 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/elocation_id.py
+-rw-r--r--   0        0        0      704 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/equation_count.py
+-rw-r--r--   0        0        0     1328 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/era.py
+-rw-r--r--   0        0        0     3812 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event.py
+-rw-r--r--   0        0        0     3112 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event_desc.py
+-rw-r--r--   0        0        0     3121 2023-06-07 01:53:13.340302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/extended_by.py
+-rw-r--r--   0        0        0      692 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_count.py
+-rw-r--r--   0        0        0      111 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_group_orientation.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_group_position.py
+-rw-r--r--   0        0        0      106 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_orientation.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_position.py
+-rw-r--r--   0        0        0     2865 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/floats_group.py
+-rw-r--r--   0        0        0     1461 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fpage.py
+-rw-r--r--   0        0        0     2105 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front.py
+-rw-r--r--   0        0        0     9504 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front_stub.py
+-rw-r--r--   0        0        0     1657 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_group.py
+-rw-r--r--   0        0        0     9222 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_statement.py
+-rw-r--r--   0        0        0     1866 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_data.py
+-rw-r--r--   0        0        0      728 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_ref.py
+-rw-r--r--   0        0        0      110 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/graphic_orientation.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/graphic_position.py
+-rw-r--r--   0        0        0     7176 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/history.py
+-rw-r--r--   0        0        0      528 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/hr.py
+-rw-r--r--   0        0        0      718 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/index_term_range_end.py
+-rw-r--r--   0        0        0     2029 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/institution_id.py
+-rw-r--r--   0        0        0     3114 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_id.py
+-rw-r--r--   0        0        0     7395 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_sponsor.py
+-rw-r--r--   0        0        0     7400 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_subtitle.py
+-rw-r--r--   0        0        0     1874 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_title_group.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/italic_toggle.py
+-rw-r--r--   0        0        0     1543 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_id.py
+-rw-r--r--   0        0        0     2748 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_meta.py
+-rw-r--r--   0        0        0     7406 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_subtitle.py
+-rw-r--r--   0        0        0     7404 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title.py
+-rw-r--r--   0        0        0     1683 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title_group.py
+-rw-r--r--   0        0        0     1338 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/lpage.py
+-rw-r--r--   0        0        0      108 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/media_orientation.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/media_position.py
+-rw-r--r--   0        0        0     6803 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_name.py
+-rw-r--r--   0        0        0     6806 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_value.py
+-rw-r--r--   0        0        0     1408 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_end.py
+-rw-r--r--   0        0        0     1414 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_start.py
+-rw-r--r--   0        0        0       83 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/monospace_toggle.py
+-rw-r--r--   0        0        0     1334 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/month.py
+-rw-r--r--   0        0        0      153 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/name_name_style.py
+-rw-r--r--   0        0        0     1422 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/object_id.py
+-rw-r--r--   0        0        0       81 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/option_correct.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/__init__.py
+-rw-r--r--   0        0        0     1259 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/free_to_read.py
+-rw-r--r--   0        0        0     1335 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/license_ref.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/__init__.py
+-rw-r--r--   0        0        0    18862 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/abs.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/and_mod.py
+-rw-r--r--   0        0        0     2149 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation.py
+-rw-r--r--   0        0        0     2036 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml.py
+-rw-r--r--   0        0        0      415 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml_model.py
+-rw-r--r--   0        0        0     1582 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/approx.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccos.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccosh.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccot.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccoth.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccsc.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arccsch.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsec.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsech.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsin.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arcsinh.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arctan.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arctanh.py
+-rw-r--r--   0        0        0     1576 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arg.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/card.py
+-rw-r--r--   0        0        0      466 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
+-rw-r--r--   0        0        0     1737 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cbytes.py
+-rw-r--r--   0        0        0     1584 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ceiling.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/codomain.py
+-rw-r--r--   0        0        0      168 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/complexes.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.344302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/compose.py
+-rw-r--r--   0        0        0  1482653 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/condition.py
+-rw-r--r--   0        0        0     1588 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/conjugate.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cos.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cosh.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cot.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/coth.py
+-rw-r--r--   0        0        0     1767 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cs.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/csc.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.348302 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/csch.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/curl.py
+-rw-r--r--   0        0        0      189 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
+-rw-r--r--   0        0        0      456 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/determinant.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/diff.py
+-rw-r--r--   0        0        0      454 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divergence.py
+-rw-r--r--   0        0        0     1582 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divide.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/domain.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/emptyset.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/eq.py
+-rw-r--r--   0        0        0      454 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/equivalent.py
+-rw-r--r--   0        0        0      454 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/eulergamma.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exists.py
+-rw-r--r--   0        0        0     1576 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exp.py
+-rw-r--r--   0        0        0      458 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exponentiale.py
+-rw-r--r--   0        0        0     1588 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorial.py
+-rw-r--r--   0        0        0     1586 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorof.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/false.py
+-rw-r--r--   0        0        0     1580 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/floor.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/forall.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/gcd.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/geq.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/grad.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/gt.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ident.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/image.py
+-rw-r--r--   0        0        0     1588 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginary.py
+-rw-r--r--   0        0        0      454 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginaryi.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/implies.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/in_mod.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/infinity.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/int_mod.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/integers.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/intersect.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/interval.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/inverse.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lambda_mod.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/laplacian.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lcm.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/leq.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/limit.py
+-rw-r--r--   0        0        0      161 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/linestyle.py
+-rw-r--r--   0        0        0      161 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/list_order.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ln.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/log.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/lt.py
+-rw-r--r--   0        0        0      136 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maction_value.py
+-rw-r--r--   0        0        0     2637 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup.py
+-rw-r--r--   0        0        0      207 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
+-rw-r--r--   0        0        0     2605 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
+-rw-r--r--   0        0        0      139 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark_value.py
+-rw-r--r--   0        0        0    74911 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_accent.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_accentunder.py
+-rw-r--r--   0        0        0      161 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_align.py
+-rw-r--r--   0        0        0      142 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_bevelled.py
+-rw-r--r--   0        0        0      165 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_charalign.py
+-rw-r--r--   0        0        0      166 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_denomalign.py
+-rw-r--r--   0        0        0      131 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_dir.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_display.py
+-rw-r--r--   0        0        0      146 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
+-rw-r--r--   0        0        0      138 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_edge.py
+-rw-r--r--   0        0        0      146 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_equalrows.py
+-rw-r--r--   0        0        0      139 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_fence.py
+-rw-r--r--   0        0        0      166 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_form.py
+-rw-r--r--   0        0        0      199 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalign.py
+-rw-r--r--   0        0        0      236 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
+-rw-r--r--   0        0        0      235 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
+-rw-r--r--   0        0        0      185 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_largeop.py
+-rw-r--r--   0        0        0      225 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_linebreak.py
+-rw-r--r--   0        0        0      228 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
+-rw-r--r--   0        0        0      208 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_location.py
+-rw-r--r--   0        0        0      495 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
+-rw-r--r--   0        0        0      641 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
+-rw-r--r--   0        0        0      164 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_numalign.py
+-rw-r--r--   0        0        0      220 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_overflow.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_separator.py
+-rw-r--r--   0        0        0      204 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_side.py
+-rw-r--r--   0        0        0      200 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_stackalign.py
+-rw-r--r--   0        0        0      142 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_stretchy.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_symmetric.py
+-rw-r--r--   0        0        0      117 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_value.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/matrix.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/matrixrow.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/max.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mean.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/median.py
+-rw-r--r--   0        0        0      137 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/menclose_value.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/merror_value.py
+-rw-r--r--   0        0        0      136 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfenced_value.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
+-rw-r--r--   0        0        0      165 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
+-rw-r--r--   0        0        0      120 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mfrac_value.py
+-rw-r--r--   0        0        0     5927 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph.py
+-rw-r--r--   0        0        0      151 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
+-rw-r--r--   0        0        0      643 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_value.py
+-rw-r--r--   0        0        0     5355 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_dir.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_value.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/min.py
+-rw-r--r--   0        0        0     1580 2023-06-07 01:53:13.352303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/minus.py
+-rw-r--r--   0        0        0     3231 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
+-rw-r--r--   0        0        0      214 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
+-rw-r--r--   0        0        0      139 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
+-rw-r--r--   0        0        0      499 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
+-rw-r--r--   0        0        0      137 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
+-rw-r--r--   0        0        0      142 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
+-rw-r--r--   0        0        0     5355 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_dir.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_value.py
+-rw-r--r--   0        0        0    10173 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo.py
+-rw-r--r--   0        0        0      138 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_accent.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_dir.py
+-rw-r--r--   0        0        0      137 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fence.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
+-rw-r--r--   0        0        0      164 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_form.py
+-rw-r--r--   0        0        0      197 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
+-rw-r--r--   0        0        0      234 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
+-rw-r--r--   0        0        0      233 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
+-rw-r--r--   0        0        0      139 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_largeop.py
+-rw-r--r--   0        0        0      223 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
+-rw-r--r--   0        0        0      226 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
+-rw-r--r--   0        0        0      639 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_separator.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
+-rw-r--r--   0        0        0      125 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_value.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mode.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/moment.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_accent.py
+-rw-r--r--   0        0        0      162 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_align.py
+-rw-r--r--   0        0        0      134 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mover_value.py
+-rw-r--r--   0        0        0      136 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mpadded_value.py
+-rw-r--r--   0        0        0      137 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mphantom_value.py
+-rw-r--r--   0        0        0     2432 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
+-rw-r--r--   0        0        0      134 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mroot_value.py
+-rw-r--r--   0        0        0      131 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mrow_dir.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mrow_value.py
+-rw-r--r--   0        0        0     5611 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_dir.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
+-rw-r--r--   0        0        0      639 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
+-rw-r--r--   0        0        0      131 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_value.py
+-rw-r--r--   0        0        0      213 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarries_location.py
+-rw-r--r--   0        0        0      292 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarries_value.py
+-rw-r--r--   0        0        0      211 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarry_location.py
+-rw-r--r--   0        0        0      290 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mscarry_value.py
+-rw-r--r--   0        0        0      136 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msgroup_value.py
+-rw-r--r--   0        0        0     3514 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline.py
+-rw-r--r--   0        0        0      121 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline_value.py
+-rw-r--r--   0        0        0     7532 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_dir.py
+-rw-r--r--   0        0        0      151 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
+-rw-r--r--   0        0        0      201 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalign.py
+-rw-r--r--   0        0        0      238 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalignfirst.py
+-rw-r--r--   0        0        0      237 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_indentalignlast.py
+-rw-r--r--   0        0        0      269 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
+-rw-r--r--   0        0        0      643 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_value.py
+-rw-r--r--   0        0        0      134 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msqrt_value.py
+-rw-r--r--   0        0        0      134 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msrow_value.py
+-rw-r--r--   0        0        0      167 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
+-rw-r--r--   0        0        0      202 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
+-rw-r--r--   0        0        0      123 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstack_value.py
+-rw-r--r--   0        0        0      142 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_align.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
+-rw-r--r--   0        0        0      167 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
+-rw-r--r--   0        0        0      168 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
+-rw-r--r--   0        0        0      151 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
+-rw-r--r--   0        0        0      168 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_form.py
+-rw-r--r--   0        0        0      201 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
+-rw-r--r--   0        0        0      238 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
+-rw-r--r--   0        0        0      237 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
+-rw-r--r--   0        0        0      187 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
+-rw-r--r--   0        0        0      143 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
+-rw-r--r--   0        0        0      227 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
+-rw-r--r--   0        0        0      230 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
+-rw-r--r--   0        0        0      210 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_location.py
+-rw-r--r--   0        0        0      497 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
+-rw-r--r--   0        0        0      643 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
+-rw-r--r--   0        0        0      149 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
+-rw-r--r--   0        0        0      166 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
+-rw-r--r--   0        0        0      206 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_side.py
+-rw-r--r--   0        0        0      202 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
+-rw-r--r--   0        0        0      144 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_value.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msub_value.py
+-rw-r--r--   0        0        0      136 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msubsup_value.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msup_value.py
+-rw-r--r--   0        0        0     6570 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
+-rw-r--r--   0        0        0      206 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_side.py
+-rw-r--r--   0        0        0      141 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable_value.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtd.py
+-rw-r--r--   0        0        0     5412 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext.py
+-rw-r--r--   0        0        0      132 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_dir.py
+-rw-r--r--   0        0        0      150 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
+-rw-r--r--   0        0        0      642 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
+-rw-r--r--   0        0        0      134 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_value.py
+-rw-r--r--   0        0        0     3175 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr.py
+-rw-r--r--   0        0        0      207 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
+-rw-r--r--   0        0        0      132 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr_value.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
+-rw-r--r--   0        0        0      163 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_align.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munder_value.py
+-rw-r--r--   0        0        0      146 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_accent.py
+-rw-r--r--   0        0        0      151 2023-06-07 01:53:13.356303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
+-rw-r--r--   0        0        0      167 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_align.py
+-rw-r--r--   0        0        0      139 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/munderover_value.py
+-rw-r--r--   0        0        0      462 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
+-rw-r--r--   0        0        0     1576 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/neq.py
+-rw-r--r--   0        0        0     2401 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none.py
+-rw-r--r--   0        0        0      133 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none_value.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/not_mod.py
+-rw-r--r--   0        0        0      454 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notanumber.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notin.py
+-rw-r--r--   0        0        0      456 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notprsubset.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/notsubset.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/or_mod.py
+-rw-r--r--   0        0        0      458 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/outerproduct.py
+-rw-r--r--   0        0        0      456 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/partialdiff.py
+-rw-r--r--   0        0        0      438 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/pi.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/plus.py
+-rw-r--r--   0        0        0     1580 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/power.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/primes.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/product.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/prsubset.py
+-rw-r--r--   0        0        0     1586 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/quotient.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rationals.py
+-rw-r--r--   0        0        0     1578 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/real.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/reals.py
+-rw-r--r--   0        0        0     1576 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rem.py
+-rw-r--r--   0        0        0     1578 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/root.py
+-rw-r--r--   0        0        0      460 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/scalarproduct.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sdev.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sec.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sech.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/selector.py
+-rw-r--r--   0        0        0      215 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sep.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/setdiff.py
+-rw-r--r--   0        0        0     1405 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/share.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sin.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sinh.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/subset.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/sum.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tan.py
+-rw-r--r--   0        0        0      442 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tanh.py
+-rw-r--r--   0        0        0     1710 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tendsto.py
+-rw-r--r--   0        0        0      444 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/times.py
+-rw-r--r--   0        0        0      452 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/transpose.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/true.py
+-rw-r--r--   0        0        0      448 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/union.py
+-rw-r--r--   0        0        0      450 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/variance.py
+-rw-r--r--   0        0        0      446 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/vector.py
+-rw-r--r--   0        0        0      460 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/vectorproduct.py
+-rw-r--r--   0        0        0      209 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/verticalalign.py
+-rw-r--r--   0        0        0      440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/xor.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/actuate_type.py
+-rw-r--r--   0        0        0     1883 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/arc_type.py
+-rw-r--r--   0        0        0     1165 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/extended.py
+-rw-r--r--   0        0        0     1449 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/locator_type.py
+-rw-r--r--   0        0        0     1240 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/resource_type.py
+-rw-r--r--   0        0        0      192 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/show_type.py
+-rw-r--r--   0        0        0     1930 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/simple.py
+-rw-r--r--   0        0        0     1199 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/title_elt_type.py
+-rw-r--r--   0        0        0      228 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/type_type.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/xml/__init__.py
+-rw-r--r--   0        0        0       15 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/__init__.py
+-rw-r--r--   0        0        0      118 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/lang_value.py
+-rw-r--r--   0        0        0      154 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/xml/pkg_1998/namespace/space_value.py
+-rw-r--r--   0        0        0      863 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_end.py
+-rw-r--r--   0        0        0      747 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_start.py
+-rw-r--r--   0        0        0       82 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_toggle.py
+-rw-r--r--   0        0        0      692 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_count.py
+-rw-r--r--   0        0        0     1349 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_range.py
+-rw-r--r--   0        0        0     1366 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/postal_code.py
+-rw-r--r--   0        0        0      112 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/preformat_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/preformat_position.py
+-rw-r--r--   0        0        0     2142 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_award_recipient.py
+-rw-r--r--   0        0        0     1855 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_investigator.py
+-rw-r--r--   0        0        0     2483 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta.py
+-rw-r--r--   0        0        0      148 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta_base_tagset.py
+-rw-r--r--   0        0        0      109 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta_mathml_version.py
+-rw-r--r--   0        0        0      138 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta_table_model.py
+-rw-r--r--   0        0        0      116 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta_tagset_family.py
+-rw-r--r--   0        0        0     2894 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date.py
+-rw-r--r--   0        0        0      740 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date_not_available.py
+-rw-r--r--   0        0        0      708 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_history.py
+-rw-r--r--   0        0        0     2861 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_id.py
+-rw-r--r--   0        0        0     1192 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/publisher.py
+-rw-r--r--   0        0        0      268 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/question_question_response_type.py
+-rw-r--r--   0        0        0      695 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/ref_count.py
+-rw-r--r--   0        0        0     1440 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_group.py
+-rw-r--r--   0        0        0     2014 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_id.py
+-rw-r--r--   0        0        0     4989 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_name.py
+-rw-r--r--   0        0        0     1009 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_wrap.py
+-rw-r--r--   0        0        0     2223 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/response.py
+-rw-r--r--   0        0        0     3127 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/restricted_by.py
+-rw-r--r--   0        0        0       79 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/roman_toggle.py
+-rw-r--r--   0        0        0      728 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rp.py
+-rw-r--r--   0        0        0     1346 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rt.py
+-rw-r--r--   0        0        0       83 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sans_serif_toggle.py
+-rw-r--r--   0        0        0       76 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sc_toggle.py
+-rw-r--r--   0        0        0     1337 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/season.py
+-rw-r--r--   0        0        0     9005 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/self_uri.py
+-rw-r--r--   0        0        0     7416 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_text.py
+-rw-r--r--   0        0        0     7394 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_title.py
+-rw-r--r--   0        0        0     7912 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig.py
+-rw-r--r--   0        0        0     8403 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig_block.py
+-rw-r--r--   0        0        0     1361 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/state.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/strike_toggle.py
+-rw-r--r--   0        0        0     8497 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/string_conf.py
+-rw-r--r--   0        0        0      159 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/string_name_name_style.py
+-rw-r--r--   0        0        0       87 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/styled_content_toggle.py
+-rw-r--r--   0        0        0       92 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sub_arrange.py
+-rw-r--r--   0        0        0     2576 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sub_article.py
+-rw-r--r--   0        0        0       92 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sup_arrange.py
+-rw-r--r--   0        0        0      124 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/supplementary_material_orientation.py
+-rw-r--r--   0        0        0      161 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/supplementary_material_position.py
+-rw-r--r--   0        0        0     1316 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_description.py
+-rw-r--r--   0        0        0     1500 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_group.py
+-rw-r--r--   0        0        0     9387 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_source.py
+-rw-r--r--   0        0        0      695 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_count.py
+-rw-r--r--   0        0        0      220 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_frame.py
+-rw-r--r--   0        0        0      140 2023-06-07 01:53:13.360303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_rules.py
+-rw-r--r--   0        0        0      117 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_wrap_group_orientation.py
+-rw-r--r--   0        0        0      154 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_wrap_group_position.py
+-rw-r--r--   0        0        0      112 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_wrap_orientation.py
+-rw-r--r--   0        0        0      149 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_wrap_position.py
+-rw-r--r--   0        0        0      150 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tbody_align.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tbody_valign.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/td_align.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/td_scope.py
+-rw-r--r--   0        0        0      132 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/td_valign.py
+-rw-r--r--   0        0        0     1386 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tex_math.py
+-rw-r--r--   0        0        0      128 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tex_math_notation.py
+-rw-r--r--   0        0        0      150 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tfoot_align.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tfoot_valign.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/th_align.py
+-rw-r--r--   0        0        0      129 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/th_scope.py
+-rw-r--r--   0        0        0      132 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/th_valign.py
+-rw-r--r--   0        0        0      150 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/thead_align.py
+-rw-r--r--   0        0        0      135 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/thead_valign.py
+-rw-r--r--   0        0        0     1542 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/title_group.py
+-rw-r--r--   0        0        0      147 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tr_align.py
+-rw-r--r--   0        0        0      132 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tr_valign.py
+-rw-r--r--   0        0        0     8910 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_abstract.py
+-rw-r--r--   0        0        0     7376 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_subtitle.py
+-rw-r--r--   0        0        0     1641 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_title_group.py
+-rw-r--r--   0        0        0      866 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_end.py
+-rw-r--r--   0        0        0      750 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_start.py
+-rw-r--r--   0        0        0       83 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_toggle.py
+-rw-r--r--   0        0        0     2893 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/volume_issue_group.py
+-rw-r--r--   0        0        0      692 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/word_count.py
+-rw-r--r--   0        0        0     1627 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/year.py
+-rw-r--r--   0        0        0     7746 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/__init__.py
+-rw-r--r--   0        0        0      566 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract.py
+-rw-r--r--   0        0        0     1612 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract_text.py
+-rw-r--r--   0        0        0      229 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract_text_nlm_category.py
+-rw-r--r--   0        0        0      342 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/accession_number_list.py
+-rw-r--r--   0        0        0      933 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation.py
+-rw-r--r--   0        0        0      588 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation_info.py
+-rw-r--r--   0        0        0     3024 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article.py
+-rw-r--r--   0        0        0      878 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_date.py
+-rw-r--r--   0        0        0      466 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_id.py
+-rw-r--r--   0        0        0      303 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_id_id_type.py
+-rw-r--r--   0        0        0      364 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_id_list.py
+-rw-r--r--   0        0        0      242 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_pub_model.py
+-rw-r--r--   0        0        0     1418 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_title.py
+-rw-r--r--   0        0        0     1934 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_equal_contrib.py
+-rw-r--r--   0        0        0      838 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_list.py
+-rw-r--r--   0        0        0       82 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_list_complete_yn.py
+-rw-r--r--   0        0        0      100 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_list_type.py
+-rw-r--r--   0        0        0       75 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_valid_yn.py
+-rw-r--r--   0        0        0      765 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/beginning_date.py
+-rw-r--r--   0        0        0     3113 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book.py
+-rw-r--r--   0        0        0     4177 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document.py
+-rw-r--r--   0        0        0      587 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document_set.py
+-rw-r--r--   0        0        0     1415 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_title.py
+-rw-r--r--   0        0        0      592 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/chemical.py
+-rw-r--r--   0        0        0      356 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/chemical_list.py
+-rw-r--r--   0        0        0     1036 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/citation.py
+-rw-r--r--   0        0        0      936 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/citation_string.py
+-rw-r--r--   0        0        0      934 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/coi_statement.py
+-rw-r--r--   0        0        0     1421 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/collection_title.py
+-rw-r--r--   0        0        0      936 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/collective_name.py
+-rw-r--r--   0        0        0      934 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections.py
+-rw-r--r--   0        0        0      424 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections_list.py
+-rw-r--r--   0        0        0     1025 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections_ref_type.py
+-rw-r--r--   0        0        0      768 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/contribution_date.py
+-rw-r--r--   0        0        0      579 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank.py
+-rw-r--r--   0        0        0      644 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank_list.py
+-rw-r--r--   0        0        0       84 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank_list_complete_yn.py
+-rw-r--r--   0        0        0      672 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_completed.py
+-rw-r--r--   0        0        0      670 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_revised.py
+-rw-r--r--   0        0        0      338 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/delete_citation.py
+-rw-r--r--   0        0        0      309 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/delete_document.py
+-rw-r--r--   0        0        0      948 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/descriptor_name.py
+-rw-r--r--   0        0        0       88 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/descriptor_name_major_topic_yn.py
+-rw-r--r--   0        0        0       86 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/descriptor_name_type.py
+-rw-r--r--   0        0        0      397 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/disp_formula.py
+-rw-r--r--   0        0        0      808 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/elocation_id.py
+-rw-r--r--   0        0        0       88 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/elocation_id_eid_type.py
+-rw-r--r--   0        0        0       80 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/elocation_id_valid_yn.py
+-rw-r--r--   0        0        0      762 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/ending_date.py
+-rw-r--r--   0        0        0      327 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/gene_symbol_list.py
+-rw-r--r--   0        0        0      465 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/general_note.py
+-rw-r--r--   0        0        0      152 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/general_note_owner.py
+-rw-r--r--   0        0        0      806 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant.py
+-rw-r--r--   0        0        0      611 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant_list.py
+-rw-r--r--   0        0        0       81 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant_list_complete_yn.py
+-rw-r--r--   0        0        0      382 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/history.py
+-rw-r--r--   0        0        0      426 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/identifier.py
+-rw-r--r--   0        0        0     1533 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/investigator.py
+-rw-r--r--   0        0        0      380 2023-06-07 01:53:13.364303 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/investigator_list.py
+-rw-r--r--   0        0        0       81 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/investigator_valid_yn.py
+-rw-r--r--   0        0        0      514 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/issn.py
+-rw-r--r--   0        0        0      100 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/issn_issn_type.py
+-rw-r--r--   0        0        0      508 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/item_list.py
+-rw-r--r--   0        0        0      869 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal.py
+-rw-r--r--   0        0        0      938 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal_issue.py
+-rw-r--r--   0        0        0      107 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal_issue_cited_medium.py
+-rw-r--r--   0        0        0     1313 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword.py
+-rw-r--r--   0        0        0      601 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword_list.py
+-rw-r--r--   0        0        0      184 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword_list_owner.py
+-rw-r--r--   0        0        0       81 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword_major_topic_yn.py
+-rw-r--r--   0        0        0      460 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/location_label.py
+-rw-r--r--   0        0        0      205 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/location_label_type.py
+-rw-r--r--   0        0        0     5574 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_citation.py
+-rw-r--r--   0        0        0      178 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_citation_owner.py
+-rw-r--r--   0        0        0      284 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_citation_status.py
+-rw-r--r--   0        0        0      813 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_journal_info.py
+-rw-r--r--   0        0        0      618 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/mesh_heading.py
+-rw-r--r--   0        0        0      376 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/mesh_heading_list.py
+-rw-r--r--   0        0        0      423 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/name_of_substance.py
+-rw-r--r--   0        0        0      354 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/object_list.py
+-rw-r--r--   0        0        0      497 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/object_mod.py
+-rw-r--r--   0        0        0      997 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_abstract.py
+-rw-r--r--   0        0        0      223 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_abstract_type.py
+-rw-r--r--   0        0        0      518 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_id.py
+-rw-r--r--   0        0        0      257 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_id_source.py
+-rw-r--r--   0        0        0      649 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pagination.py
+-rw-r--r--   0        0        0     1118 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/param.py
+-rw-r--r--   0        0        0      827 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/personal_name_subject.py
+-rw-r--r--   0        0        0      426 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/personal_name_subject_list.py
+-rw-r--r--   0        0        0      461 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pmid.py
+-rw-r--r--   0        0        0      893 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_date.py
+-rw-r--r--   0        0        0     1462 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_med_pub_date.py
+-rw-r--r--   0        0        0      496 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_med_pub_date_pub_status.py
+-rw-r--r--   0        0        0      423 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publication_type.py
+-rw-r--r--   0        0        0      400 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publication_type_list.py
+-rw-r--r--   0        0        0      557 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publisher.py
+-rw-r--r--   0        0        0      935 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publisher_name.py
+-rw-r--r--   0        0        0      600 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article.py
+-rw-r--r--   0        0        0      839 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article_set.py
+-rw-r--r--   0        0        0      611 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_article.py
+-rw-r--r--   0        0        0      384 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_article_set.py
+-rw-r--r--   0        0        0      987 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_data.py
+-rw-r--r--   0        0        0     1213 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_data.py
+-rw-r--r--   0        0        0      724 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/qualifier_name.py
+-rw-r--r--   0        0        0       87 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/qualifier_name_major_topic_yn.py
+-rw-r--r--   0        0        0      576 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference.py
+-rw-r--r--   0        0        0      678 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference_list.py
+-rw-r--r--   0        0        0      765 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section.py
+-rw-r--r--   0        0        0     1312 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section_title.py
+-rw-r--r--   0        0        0      347 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/sections.py
+-rw-r--r--   0        0        0      928 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suffix.py
+-rw-r--r--   0        0        0      386 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suppl_mesh_list.py
+-rw-r--r--   0        0        0      668 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suppl_mesh_name.py
+-rw-r--r--   0        0        0      185 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suppl_mesh_name_type.py
+-rw-r--r--   0        0        0     4251 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/u.py
+-rw-r--r--   0        0        0      614 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url.py
+-rw-r--r--   0        0        0      661 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url_lang.py
+-rw-r--r--   0        0        0      150 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url_type.py
+-rw-r--r--   0        0        0     1043 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/vernacular_title.py
+-rw-r--r--   0        0        0      933 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/volume_title.py
+-rw-r--r--   0        0        0        0 2023-06-07 01:53:13.368304 pubmed_types-0.2.0.dev0/src/pubmed_types/py.typed
+-rw-r--r--   0        0        0     5965 1970-01-01 00:00:00.000000 pubmed_types-0.2.0.dev0/PKG-INFO
```

### Comparing `pubmed_types-0.2.0/LICENSE` & `pubmed_types-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/README.md` & `pubmed_types-0.2.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pubmed-types (v0.2.0)
+# pubmed-types (v0.2.0-dev0)
 
 <p align="center">
     <img src="https://img.shields.io/pypi/dm/pubmed-types?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/pubmed-types?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/pubmed-types?style=flat-square"/>
     <a href="https://github.com/tefra/xsdata-pydantic">
         <img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/Built%20with-xsdata--pydantic-blue">
@@ -54,15 +54,15 @@
 
 ```python
 import tarfile
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
-from pubmed_types import pmc_article
+from pubmed_types import parse_pubmed_xml
 
 # Input file source and output file destination
 source = (
     "ftp://ftp.ncbi.nlm.nih.gov"
     + "/pub/pmc/oa_bulk/oa_comm/xml"
     + "/oa_comm_xml.incr.2023-03-21.tar.gz"
 )
@@ -72,15 +72,15 @@
 # 1. Get an open access article dataset from the FTP server
 with closing(request.urlopen(source)) as url:
     with tarfile.open(fileobj=url, mode="r:gz") as fr:
         fr.extractall(destination)
 
 # 2. Parse the file
 file_path = destination.joinpath("PMC009xxxxxx").joinpath("PMC9970662.xml")
-full_text = pmc_article(file_path)
+full_text = parse_pubmed_xml(file_path)
 
 # 3. Print out the article title
 print(f"Title: {full_text.front.article_meta.title_group.article_title.content[0]}")
 ```
 
 Output:
 
@@ -92,35 +92,34 @@
 
 ```python
 import gzip
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
-from pubmed_types import pubmed_article_set
+from pubmed_types import parse_pubmed_xml, PubmedArticleSet
 
 # Input file source and output file destination
 source = "ftp://ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
 destination = Path("downloads").joinpath("pubmed23n1168.xml")
 destination.parent.mkdir(exist_ok=True)
 
 # 1. Get a pubmed citation daily update file from the FTP server
 with closing(request.urlopen(source)) as url:
     with gzip.GzipFile(fileobj=url, mode="rb") as fr:
         with open(destination, mode="wb") as fw:
             fw.write(fr.read())
 
 # 2. Parse the file
-article_set = pubmed_article_set(destination)
+article_set = parse_pubmed_xml(destination)
+assert isinstance(article_set, PubmedArticleSet)
 
 # 3. Get the number of citations in the file
 print(f"Number of citations: {len(article_set.pubmed_article)}")
-print(
-    f"{article_set.pubmed_article[0].medline_citation.article.article_title.content[0]}"
-)
+print(f"{article_set.pubmed_article[0].medline_citation.article.article_title.content[0]}")
 ```
 
 Output:
 
 ```bash
 Number of citations: 2543
 A Patent and Pattern Mother.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# pubmed-types (v0.2.0)
+# pubmed-types (v0.2.0-dev0)
    [https://img.shields.io/pypi/dm/pubmed-types?style=flat-square] [https://
 img.shields.io/pypi/l/pubmed-types?style=flat-square] [https://img.shields.io/
 pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic] [./images/
                                  coverage.svg]
 ## Introduction A complete implementation of the XML schema for PMC Open Access
 articles and Pubmed article sets (citations). This package helps to parse
 PubMed XML data into Pydantic models. This validates the input xml data and
@@ -23,38 +23,39 @@
 classes have the benefit of providing type hints with tab completion for IDEs,
 making it easier to navigate the complex structure of the citation data. ## How
 do I use it? It is possible to use `xsdata-pydantic` and the autogenerated
 classes directly to parse an XML file, but we provide a convenience function to
 easily open PubMed XMl citations and PMC open access articles. ### Example 1: A
 PMC Open Access Article ```python import tarfile import urllib.request as
 request from contextlib import closing from pathlib import Path from
-pubmed_types import pmc_article # Input file source and output file destination
-source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/oa_comm/xml" + "/
-oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path("downloads")
-destination.mkdir(exist_ok=True) # 1. Get an open access article dataset from
-the FTP server with closing(request.urlopen(source)) as url: with tarfile.open
-(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2. Parse the
-file file_path = destination.joinpath("PMC009xxxxxx").joinpath
-("PMC9970662.xml") full_text = pmc_article(file_path) # 3. Print out the
+pubmed_types import parse_pubmed_xml # Input file source and output file
+destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/
+oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path
+("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access article
+dataset from the FTP server with closing(request.urlopen(source)) as url: with
+tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2.
+Parse the file file_path = destination.joinpath("PMC009xxxxxx").joinpath
+("PMC9970662.xml") full_text = parse_pubmed_xml(file_path) # 3. Print out the
 article title print(f"Title:
 {full_text.front.article_meta.title_group.article_title.content[0]}") ```
 Output: ```bash Title: Lactate as a myokine and exerkine: drivers and signals
 of physiology and metabolism ``` ### Example 2: A Pubmed baseline citation file
 ```python import gzip import urllib.request as request from contextlib import
-closing from pathlib import Path from pubmed_types import pubmed_article_set #
-Input file source and output file destination source = "ftp://
-ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
+closing from pathlib import Path from pubmed_types import parse_pubmed_xml,
+PubmedArticleSet # Input file source and output file destination source = "ftp:
+//ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
 destination = Path("downloads").joinpath("pubmed23n1168.xml")
 destination.parent.mkdir(exist_ok=True) # 1. Get a pubmed citation daily update
 file from the FTP server with closing(request.urlopen(source)) as url: with
 gzip.GzipFile(fileobj=url, mode="rb") as fr: with open(destination, mode="wb")
-as fw: fw.write(fr.read()) # 2. Parse the file article_set = pubmed_article_set
-(destination) # 3. Get the number of citations in the file print(f"Number of
-citations: {len(article_set.pubmed_article)}") print( f"
-{article_set.pubmed_article[0].medline_citation.article.article_title.content
-[0]}" ) ``` Output: ```bash Number of citations: 2543 A Patent and Pattern
-Mother. ``` ## FAQ ### Why does it take so long to parse a pubmed citation set
-There is a lot of data, and the schema is deep and complex. ### Why are the
-return structures so complicated? The return structures are a direct reflection
-of the XML format defined by the NLM. In the future some utility classes might
-be made for common components (title, authors, etc), but for now this is
-intended to be an unbiased way of parsing the XML.
+as fw: fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
+(destination) assert isinstance(article_set, PubmedArticleSet) # 3. Get the
+number of citations in the file print(f"Number of citations: {len
+(article_set.pubmed_article)}") print(f"{article_set.pubmed_article
+[0].medline_citation.article.article_title.content[0]}") ``` Output: ```bash
+Number of citations: 2543 A Patent and Pattern Mother. ``` ## FAQ ### Why does
+it take so long to parse a pubmed citation set There is a lot of data, and the
+schema is deep and complex. ### Why are the return structures so complicated?
+The return structures are a direct reflection of the XML format defined by the
+NLM. In the future some utility classes might be made for common components
+(title, authors, etc), but for now this is intended to be an unbiased way of
+parsing the XML.
```

### Comparing `pubmed_types-0.2.0/pyproject.toml` & `pubmed_types-0.2.0.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pubmed-types"
-version = "0.2.0"
+version = "0.2.0-dev0"
 authors = ["Nick Schaub <nick.schaub@nih.gov>"]
 description = "Pubmed XML parsing and typehints."
 readme = "README.md"
 license = "MIT"
 packages = [{include = "pubmed_types", from = "src"}]
 homepage = "https://github.com/nicholas-schaub/pubmed-types"
 repository = "https://github.com/nicholas-schaub/pubmed-types"
@@ -37,12 +37,11 @@
 nox = "^2023.4.22"
 requests = "^2.31.0"
 pytest = "^7.3.1"
 bump2version = "^1.0.1"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.3.1"
 coverage-badge = "^1.1.0"
-mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pubmed_types-0.2.0/src/pubmed_types/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.0-dev0"
 
 from pathlib import Path
 from typing import Union
 
 from xsdata_pydantic.bindings import XmlParser
 
 from .models.jats.article import Article as PMCArticle
```

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/abbrev_journal_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/abbrev_journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/access_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/access_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/alt_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/alt_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/app.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/app_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article_categories.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_categories.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article_version.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/article_version_alternatives.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version_alternatives.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/author_notes.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/author_notes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/award_desc.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/award_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/award_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/back.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/back.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/body.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/body.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/break_mod.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/break_mod.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/city.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/city.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/col.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/col.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/colgroup.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/colgroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/conf_num.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_num.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/conf_theme.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_theme.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/conference.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/contrib_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/contributed_resource_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contributed_resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/copyright_year.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/copyright_year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/corresp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/corresp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/counts.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/counts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/custom_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/custom_meta_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/day.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/day.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/elocation_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/elocation_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/equation_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/equation_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/era.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/era.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/event.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/event_desc.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event_desc.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/extended_by.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/extended_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/fig_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/floats_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/floats_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/fpage.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/front.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/front_stub.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front_stub.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/funding_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/funding_statement.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/glyph_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/glyph_ref.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/history.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/history.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/hr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/hr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/index_term_range_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/index_term_range_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/institution_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/institution_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_sponsor.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_sponsor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/issue_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/journal_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/lpage.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/lpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/meta_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/meta_value.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_value.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/milestone_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/milestone_start.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/month.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/month.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/object_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/object_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/free_to_read.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/free_to_read.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/license_ref.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/license_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/abs.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/abs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/approx.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/approx.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arg.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arg.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cbytes.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cbytes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ceiling.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ceiling.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/condition.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/condition.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/conjugate.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/conjugate.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cs.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divide.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divide.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorial.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorial.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorof.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorof.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/floor.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/floor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginary.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginary.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/minus.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/minus.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/neq.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/neq.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/power.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/power.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/quotient.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/quotient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/real.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/real.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rem.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rem.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/root.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/root.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/share.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/share.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tendsto.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tendsto.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/arc_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/arc_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/extended.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/extended.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/locator_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/locator_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/resource_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/resource_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/simple.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/simple.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/title_elt_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/title_elt_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/overline_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/overline_start.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/page_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/page_range.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_range.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/postal_code.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/postal_code.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/principal_award_recipient.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_award_recipient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/principal_investigator.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/processing_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_date_not_available.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date_not_available.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_history.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_history.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/pub_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/publisher.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/publisher.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/ref_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/ref_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/resource_wrap.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_wrap.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/response.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/response.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/restricted_by.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/restricted_by.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/rp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/rt.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rt.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/season.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/season.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/self_uri.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/self_uri.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/series_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/series_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/sig.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/sig_block.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig_block.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/state.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/state.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/string_conf.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/string_conf.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/sub_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sub_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/support_description.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_description.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/support_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/support_source.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_source.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/table_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/tex_math.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tex_math.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_abstract.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/trans_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/underline_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/underline_start.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/volume_issue_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/volume_issue_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/word_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/word_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/jats/year.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/abstract.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/abstract_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/affiliation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/affiliation_info.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/article_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/author_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/beginning_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/beginning_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_document.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_document_set.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/book_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/chemical.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/chemical.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/citation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/citation_string.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/citation_string.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/coi_statement.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/coi_statement.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/collection_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/collection_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/collective_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/collective_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/comments_corrections.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/comments_corrections_ref_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections_ref_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/contribution_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/contribution_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/data_bank.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/data_bank_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/date_completed.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_completed.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/date_revised.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_revised.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/descriptor_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/descriptor_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/elocation_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/elocation_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/ending_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/ending_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/grant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/grant_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/investigator.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/investigator.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/issn.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/issn.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/journal.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/journal_issue.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal_issue.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/keyword_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_citation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_citation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/medline_journal_info.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_journal_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/mesh_heading.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/mesh_heading.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_abstract.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/other_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pagination.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pagination.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/param.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/param.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/personal_name_subject.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/personal_name_subject.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pub_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pub_med_pub_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_med_pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publisher.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publisher.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/publisher_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publisher_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_article_set.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_book_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_book_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/pubmed_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/qualifier_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/qualifier_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/reference.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/reference_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/section.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/section_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suffix.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suffix.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/suppl_mesh_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suppl_mesh_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/u.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/u.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/url.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/url_lang.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url_lang.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/vernacular_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/vernacular_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/src/pubmed_types/models/pubmed/volume_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/volume_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.2.0/PKG-INFO` & `pubmed_types-0.2.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed-types
-Version: 0.2.0
+Version: 0.2.0.dev0
 Summary: Pubmed XML parsing and typehints.
 Home-page: https://github.com/nicholas-schaub/pubmed-types
 License: MIT
 Author: Nick Schaub
 Author-email: nick.schaub@nih.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Dist: xsdata-pydantic[cli,lxml,soap] (>=22.10,<23.0)
 Project-URL: Issues, https://github.com/nicholas-schaub/pubmed-types/issues
 Project-URL: Repository, https://github.com/nicholas-schaub/pubmed-types
 Description-Content-Type: text/markdown
 
-# pubmed-types (v0.2.0)
+# pubmed-types (v0.2.0-dev0)
 
 <p align="center">
     <img src="https://img.shields.io/pypi/dm/pubmed-types?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/pubmed-types?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/pubmed-types?style=flat-square"/>
     <a href="https://github.com/tefra/xsdata-pydantic">
         <img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/Built%20with-xsdata--pydantic-blue">
@@ -80,15 +80,15 @@
 
 ```python
 import tarfile
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
-from pubmed_types import pmc_article
+from pubmed_types import parse_pubmed_xml
 
 # Input file source and output file destination
 source = (
     "ftp://ftp.ncbi.nlm.nih.gov"
     + "/pub/pmc/oa_bulk/oa_comm/xml"
     + "/oa_comm_xml.incr.2023-03-21.tar.gz"
 )
@@ -98,15 +98,15 @@
 # 1. Get an open access article dataset from the FTP server
 with closing(request.urlopen(source)) as url:
     with tarfile.open(fileobj=url, mode="r:gz") as fr:
         fr.extractall(destination)
 
 # 2. Parse the file
 file_path = destination.joinpath("PMC009xxxxxx").joinpath("PMC9970662.xml")
-full_text = pmc_article(file_path)
+full_text = parse_pubmed_xml(file_path)
 
 # 3. Print out the article title
 print(f"Title: {full_text.front.article_meta.title_group.article_title.content[0]}")
 ```
 
 Output:
 
@@ -118,35 +118,34 @@
 
 ```python
 import gzip
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
-from pubmed_types import pubmed_article_set
+from pubmed_types import parse_pubmed_xml, PubmedArticleSet
 
 # Input file source and output file destination
 source = "ftp://ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
 destination = Path("downloads").joinpath("pubmed23n1168.xml")
 destination.parent.mkdir(exist_ok=True)
 
 # 1. Get a pubmed citation daily update file from the FTP server
 with closing(request.urlopen(source)) as url:
     with gzip.GzipFile(fileobj=url, mode="rb") as fr:
         with open(destination, mode="wb") as fw:
             fw.write(fr.read())
 
 # 2. Parse the file
-article_set = pubmed_article_set(destination)
+article_set = parse_pubmed_xml(destination)
+assert isinstance(article_set, PubmedArticleSet)
 
 # 3. Get the number of citations in the file
 print(f"Number of citations: {len(article_set.pubmed_article)}")
-print(
-    f"{article_set.pubmed_article[0].medline_citation.article.article_title.content[0]}"
-)
+print(f"{article_set.pubmed_article[0].medline_citation.article.article_title.content[0]}")
 ```
 
 Output:
 
 ```bash
 Number of citations: 2543
 A Patent and Pattern Mother.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pubmed-types Version: 0.2.0 Summary: Pubmed XML
-parsing and typehints. Home-page: https://github.com/nicholas-schaub/pubmed-
-types License: MIT Author: Nick Schaub Author-email: nick.schaub@nih.gov
+Metadata-Version: 2.1 Name: pubmed-types Version: 0.2.0.dev0 Summary: Pubmed
+XML parsing and typehints. Home-page: https://github.com/nicholas-schaub/
+pubmed-types License: MIT Author: Nick Schaub Author-email: nick.schaub@nih.gov
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Medical
 Science Apps. Classifier: Topic :: Text Processing :: Markup :: XML Requires-
 Dist: xsdata-pydantic[cli,lxml,soap] (>=22.10,<23.0) Project-URL: Issues,
 https://github.com/nicholas-schaub/pubmed-types/issues Project-URL: Repository,
 https://github.com/nicholas-schaub/pubmed-types Description-Content-Type: text/
-markdown # pubmed-types (v0.2.0)
+markdown # pubmed-types (v0.2.0-dev0)
    [https://img.shields.io/pypi/dm/pubmed-types?style=flat-square] [https://
 img.shields.io/pypi/l/pubmed-types?style=flat-square] [https://img.shields.io/
 pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic] [./images/
                                  coverage.svg]
 ## Introduction A complete implementation of the XML schema for PMC Open Access
 articles and Pubmed article sets (citations). This package helps to parse
 PubMed XML data into Pydantic models. This validates the input xml data and
@@ -38,38 +38,39 @@
 classes have the benefit of providing type hints with tab completion for IDEs,
 making it easier to navigate the complex structure of the citation data. ## How
 do I use it? It is possible to use `xsdata-pydantic` and the autogenerated
 classes directly to parse an XML file, but we provide a convenience function to
 easily open PubMed XMl citations and PMC open access articles. ### Example 1: A
 PMC Open Access Article ```python import tarfile import urllib.request as
 request from contextlib import closing from pathlib import Path from
-pubmed_types import pmc_article # Input file source and output file destination
-source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/oa_comm/xml" + "/
-oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path("downloads")
-destination.mkdir(exist_ok=True) # 1. Get an open access article dataset from
-the FTP server with closing(request.urlopen(source)) as url: with tarfile.open
-(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2. Parse the
-file file_path = destination.joinpath("PMC009xxxxxx").joinpath
-("PMC9970662.xml") full_text = pmc_article(file_path) # 3. Print out the
+pubmed_types import parse_pubmed_xml # Input file source and output file
+destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/
+oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path
+("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access article
+dataset from the FTP server with closing(request.urlopen(source)) as url: with
+tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2.
+Parse the file file_path = destination.joinpath("PMC009xxxxxx").joinpath
+("PMC9970662.xml") full_text = parse_pubmed_xml(file_path) # 3. Print out the
 article title print(f"Title:
 {full_text.front.article_meta.title_group.article_title.content[0]}") ```
 Output: ```bash Title: Lactate as a myokine and exerkine: drivers and signals
 of physiology and metabolism ``` ### Example 2: A Pubmed baseline citation file
 ```python import gzip import urllib.request as request from contextlib import
-closing from pathlib import Path from pubmed_types import pubmed_article_set #
-Input file source and output file destination source = "ftp://
-ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
+closing from pathlib import Path from pubmed_types import parse_pubmed_xml,
+PubmedArticleSet # Input file source and output file destination source = "ftp:
+//ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
 destination = Path("downloads").joinpath("pubmed23n1168.xml")
 destination.parent.mkdir(exist_ok=True) # 1. Get a pubmed citation daily update
 file from the FTP server with closing(request.urlopen(source)) as url: with
 gzip.GzipFile(fileobj=url, mode="rb") as fr: with open(destination, mode="wb")
-as fw: fw.write(fr.read()) # 2. Parse the file article_set = pubmed_article_set
-(destination) # 3. Get the number of citations in the file print(f"Number of
-citations: {len(article_set.pubmed_article)}") print( f"
-{article_set.pubmed_article[0].medline_citation.article.article_title.content
-[0]}" ) ``` Output: ```bash Number of citations: 2543 A Patent and Pattern
-Mother. ``` ## FAQ ### Why does it take so long to parse a pubmed citation set
-There is a lot of data, and the schema is deep and complex. ### Why are the
-return structures so complicated? The return structures are a direct reflection
-of the XML format defined by the NLM. In the future some utility classes might
-be made for common components (title, authors, etc), but for now this is
-intended to be an unbiased way of parsing the XML.
+as fw: fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
+(destination) assert isinstance(article_set, PubmedArticleSet) # 3. Get the
+number of citations in the file print(f"Number of citations: {len
+(article_set.pubmed_article)}") print(f"{article_set.pubmed_article
+[0].medline_citation.article.article_title.content[0]}") ``` Output: ```bash
+Number of citations: 2543 A Patent and Pattern Mother. ``` ## FAQ ### Why does
+it take so long to parse a pubmed citation set There is a lot of data, and the
+schema is deep and complex. ### Why are the return structures so complicated?
+The return structures are a direct reflection of the XML format defined by the
+NLM. In the future some utility classes might be made for common components
+(title, authors, etc), but for now this is intended to be an unbiased way of
+parsing the XML.
```

