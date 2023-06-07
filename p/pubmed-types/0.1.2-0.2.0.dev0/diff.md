# Comparing `tmp/pubmed_types-0.1.2.tar.gz` & `tmp/pubmed_types-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_types-0.1.2.tar", max compression
+gzip compressed data, was "pubmed_types-0.2.0.dev0.tar", max compression
```

## Comparing `pubmed_types-0.1.2.tar` & `pubmed_types-0.2.0.dev0.tar`

### file list

```diff
@@ -1,673 +1,665 @@
--rw-r--r--   0        0        0     1072 2023-05-25 16:03:32.757838 pubmed_types-0.1.2/LICENSE
--rw-r--r--   0        0        0     4359 2023-06-04 14:01:16.579993 pubmed_types-0.1.2/README.md
--rw-r--r--   0        0        0     1444 2023-06-04 14:01:16.575993 pubmed_types-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-04 14:01:16.579993 pubmed_types-0.1.2/src/pubmed_types/__init__.py
--rw-r--r--   0        0        0    24766 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/__init__.py
--rw-r--r--   0        0        0     7420 2023-06-03 02:44:01.924575 pubmed_types-0.1.2/src/pubmed_types/models/abbrev_journal_title.py
--rw-r--r--   0        0        0      610 2023-06-03 02:44:02.860562 pubmed_types-0.1.2/src/pubmed_types/models/abstract_1.py
--rw-r--r--   0        0        0     1645 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/abstract_text.py
--rw-r--r--   0        0        0      229 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/abstract_text_nlm_category.py
--rw-r--r--   0        0        0  1064015 2023-06-03 02:44:01.912575 pubmed_types-0.1.2/src/pubmed_types/models/access_date.py
--rw-r--r--   0        0        0      342 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/accession_number_list.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/affiliation.py
--rw-r--r--   0        0        0      588 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/affiliation_info.py
--rw-r--r--   0        0        0     1373 2023-06-03 02:44:01.924575 pubmed_types-0.1.2/src/pubmed_types/models/alt_text.py
--rw-r--r--   0        0        0     8831 2023-06-03 02:44:01.944575 pubmed_types-0.1.2/src/pubmed_types/models/app.py
--rw-r--r--   0        0        0     8786 2023-06-03 02:44:01.960574 pubmed_types-0.1.2/src/pubmed_types/models/app_group.py
--rw-r--r--   0        0        0      419 2023-06-03 02:18:03.813928 pubmed_types-0.1.2/src/pubmed_types/models/archive_copy_source.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/array_orientation.py
--rw-r--r--   0        0        0     3079 2023-06-03 02:44:02.864562 pubmed_types-0.1.2/src/pubmed_types/models/article_1.py
--rw-r--r--   0        0        0     2649 2023-06-03 02:44:02.876562 pubmed_types-0.1.2/src/pubmed_types/models/article_2.py
--rw-r--r--   0        0        0     1202 2023-06-03 02:44:01.960574 pubmed_types-0.1.2/src/pubmed_types/models/article_categories.py
--rw-r--r--   0        0        0      878 2023-06-03 02:44:02.576566 pubmed_types-0.1.2/src/pubmed_types/models/article_date.py
--rw-r--r--   0        0        0      369 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/article_dtd_version.py
--rw-r--r--   0        0        0     1423 2023-06-03 02:44:01.964574 pubmed_types-0.1.2/src/pubmed_types/models/article_id.py
--rw-r--r--   0        0        0      511 2023-06-03 02:44:02.876562 pubmed_types-0.1.2/src/pubmed_types/models/article_id_1.py
--rw-r--r--   0        0        0      303 2023-06-03 02:44:02.848563 pubmed_types-0.1.2/src/pubmed_types/models/article_id_id_type.py
--rw-r--r--   0        0        0      368 2023-06-03 02:44:02.580566 pubmed_types-0.1.2/src/pubmed_types/models/article_id_list.py
--rw-r--r--   0        0        0     9515 2023-06-03 02:44:01.980574 pubmed_types-0.1.2/src/pubmed_types/models/article_meta.py
--rw-r--r--   0        0        0      242 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/article_pub_model.py
--rw-r--r--   0        0        0      353 2023-06-03 02:18:03.769929 pubmed_types-0.1.2/src/pubmed_types/models/article_set.py
--rw-r--r--   0        0        0     1495 2023-06-03 02:44:02.880562 pubmed_types-0.1.2/src/pubmed_types/models/article_title_1.py
--rw-r--r--   0        0        0     3823 2023-06-03 02:44:01.988574 pubmed_types-0.1.2/src/pubmed_types/models/article_version.py
--rw-r--r--   0        0        0      827 2023-06-03 02:44:01.992574 pubmed_types-0.1.2/src/pubmed_types/models/article_version_alternatives.py
--rw-r--r--   0        0        0     1938 2023-06-03 02:44:02.580566 pubmed_types-0.1.2/src/pubmed_types/models/author.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/author_equal_contrib.py
--rw-r--r--   0        0        0      838 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/author_list.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/author_list_complete_yn.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/author_list_type.py
--rw-r--r--   0        0        0     1720 2023-06-03 02:44:02.000574 pubmed_types-0.1.2/src/pubmed_types/models/author_notes.py
--rw-r--r--   0        0        0       75 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/author_valid_yn.py
--rw-r--r--   0        0        0     2449 2023-06-03 02:44:02.004574 pubmed_types-0.1.2/src/pubmed_types/models/award_desc.py
--rw-r--r--   0        0        0     4315 2023-06-03 02:44:02.012574 pubmed_types-0.1.2/src/pubmed_types/models/award_group.py
--rw-r--r--   0        0        0     2442 2023-06-03 02:44:02.016574 pubmed_types-0.1.2/src/pubmed_types/models/award_name.py
--rw-r--r--   0        0        0     2079 2023-06-03 02:44:02.020574 pubmed_types-0.1.2/src/pubmed_types/models/back.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/beginning_date.py
--rw-r--r--   0        0        0     7356 2023-06-03 02:44:02.032574 pubmed_types-0.1.2/src/pubmed_types/models/body.py
--rw-r--r--   0        0        0       78 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/bold_toggle.py
--rw-r--r--   0        0        0     3125 2023-06-03 02:44:02.588566 pubmed_types-0.1.2/src/pubmed_types/models/book.py
--rw-r--r--   0        0        0     4185 2023-06-03 02:44:02.560566 pubmed_types-0.1.2/src/pubmed_types/models/book_document.py
--rw-r--r--   0        0        0      587 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/book_document_set.py
--rw-r--r--   0        0        0     1444 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/book_title.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/boxed_text_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/boxed_text_position.py
--rw-r--r--   0        0        0      529 2023-06-03 02:44:02.032574 pubmed_types-0.1.2/src/pubmed_types/models/break_mod.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/chem_struct_wrap_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/chem_struct_wrap_position.py
--rw-r--r--   0        0        0      592 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/chemical.py
--rw-r--r--   0        0        0      356 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/chemical_list.py
--rw-r--r--   0        0        0     1065 2023-06-03 02:44:02.592566 pubmed_types-0.1.2/src/pubmed_types/models/citation.py
--rw-r--r--   0        0        0     1344 2023-06-03 02:44:02.036574 pubmed_types-0.1.2/src/pubmed_types/models/city.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_executable.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_orientation.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.788563 pubmed_types-0.1.2/src/pubmed_types/models/code_position.py
--rw-r--r--   0        0        0      963 2023-06-03 02:44:02.596566 pubmed_types-0.1.2/src/pubmed_types/models/coi_statement.py
--rw-r--r--   0        0        0     1574 2023-06-03 02:44:02.036574 pubmed_types-0.1.2/src/pubmed_types/models/col.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/col_align.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/col_valign.py
--rw-r--r--   0        0        0     1765 2023-06-03 02:44:02.040573 pubmed_types-0.1.2/src/pubmed_types/models/colgroup.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/colgroup_align.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/colgroup_valign.py
--rw-r--r--   0        0        0     1450 2023-06-03 02:44:02.596566 pubmed_types-0.1.2/src/pubmed_types/models/collection_title.py
--rw-r--r--   0        0        0      965 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/collective_name.py
--rw-r--r--   0        0        0      934 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections.py
--rw-r--r--   0        0        0      424 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_list.py
--rw-r--r--   0        0        0     1025 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_ref_type.py
--rw-r--r--   0        0        0     7391 2023-06-03 02:44:02.052573 pubmed_types-0.1.2/src/pubmed_types/models/conf_num.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.064573 pubmed_types-0.1.2/src/pubmed_types/models/conf_theme.py
--rw-r--r--   0        0        0     4292 2023-06-03 02:44:02.068573 pubmed_types-0.1.2/src/pubmed_types/models/conference.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_corresp.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_deceased.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_equal_contrib.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:44:02.072573 pubmed_types-0.1.2/src/pubmed_types/models/contrib_id.py
--rw-r--r--   0        0        0       98 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/contrib_id_authenticated.py
--rw-r--r--   0        0        0     1889 2023-06-03 02:44:02.076573 pubmed_types-0.1.2/src/pubmed_types/models/contributed_resource_group.py
--rw-r--r--   0        0        0      768 2023-06-03 02:44:02.600566 pubmed_types-0.1.2/src/pubmed_types/models/contribution_date.py
--rw-r--r--   0        0        0     1083 2023-06-03 02:44:02.080573 pubmed_types-0.1.2/src/pubmed_types/models/copyright_year.py
--rw-r--r--   0        0        0     8856 2023-06-03 02:44:02.092573 pubmed_types-0.1.2/src/pubmed_types/models/corresp.py
--rw-r--r--   0        0        0      871 2023-06-03 02:44:02.096573 pubmed_types-0.1.2/src/pubmed_types/models/count.py
--rw-r--r--   0        0        0     1907 2023-06-03 02:44:02.100573 pubmed_types-0.1.2/src/pubmed_types/models/counts.py
--rw-r--r--   0        0        0     3702 2023-06-03 02:44:02.104573 pubmed_types-0.1.2/src/pubmed_types/models/custom_meta.py
--rw-r--r--   0        0        0     1389 2023-06-03 02:44:02.108573 pubmed_types-0.1.2/src/pubmed_types/models/custom_meta_group.py
--rw-r--r--   0        0        0      579 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/data_bank.py
--rw-r--r--   0        0        0      644 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list.py
--rw-r--r--   0        0        0       84 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list_complete_yn.py
--rw-r--r--   0        0        0      672 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/date_completed.py
--rw-r--r--   0        0        0      670 2023-06-03 02:44:02.604566 pubmed_types-0.1.2/src/pubmed_types/models/date_revised.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.108573 pubmed_types-0.1.2/src/pubmed_types/models/day.py
--rw-r--r--   0        0        0      338 2023-06-03 02:44:02.564566 pubmed_types-0.1.2/src/pubmed_types/models/delete_citation.py
--rw-r--r--   0        0        0      309 2023-06-03 02:44:02.564566 pubmed_types-0.1.2/src/pubmed_types/models/delete_document.py
--rw-r--r--   0        0        0      948 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name_major_topic_yn.py
--rw-r--r--   0        0        0       86 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name_type.py
--rw-r--r--   0        0        0      331 2023-06-03 02:44:02.884562 pubmed_types-0.1.2/src/pubmed_types/models/disp_formula_1.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.112573 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id.py
--rw-r--r--   0        0        0      809 2023-06-03 02:44:02.884562 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_1.py
--rw-r--r--   0        0        0       88 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_eid_type.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_valid_yn.py
--rw-r--r--   0        0        0      762 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/ending_date.py
--rw-r--r--   0        0        0      704 2023-06-03 02:44:02.116572 pubmed_types-0.1.2/src/pubmed_types/models/equation_count.py
--rw-r--r--   0        0        0     1328 2023-06-03 02:44:02.116572 pubmed_types-0.1.2/src/pubmed_types/models/era.py
--rw-r--r--   0        0        0     3816 2023-06-03 02:44:02.124572 pubmed_types-0.1.2/src/pubmed_types/models/event.py
--rw-r--r--   0        0        0     3116 2023-06-03 02:44:02.132572 pubmed_types-0.1.2/src/pubmed_types/models/event_desc.py
--rw-r--r--   0        0        0     3131 2023-06-03 02:44:02.136572 pubmed_types-0.1.2/src/pubmed_types/models/extended_by.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.140572 pubmed_types-0.1.2/src/pubmed_types/models/fig_count.py
--rw-r--r--   0        0        0      111 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/fig_group_orientation.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/fig_group_position.py
--rw-r--r--   0        0        0      106 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/fig_orientation.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/fig_position.py
--rw-r--r--   0        0        0      467 2023-06-03 02:18:03.781929 pubmed_types-0.1.2/src/pubmed_types/models/first_name.py
--rw-r--r--   0        0        0       78 2023-06-03 02:18:04.049925 pubmed_types-0.1.2/src/pubmed_types/models/first_name_empty_yn.py
--rw-r--r--   0        0        0      458 2023-06-03 02:18:03.777929 pubmed_types-0.1.2/src/pubmed_types/models/first_page.py
--rw-r--r--   0        0        0      112 2023-06-03 02:18:04.045925 pubmed_types-0.1.2/src/pubmed_types/models/first_page_lzero.py
--rw-r--r--   0        0        0     2865 2023-06-03 02:44:02.144572 pubmed_types-0.1.2/src/pubmed_types/models/floats_group.py
--rw-r--r--   0        0        0     1461 2023-06-03 02:44:02.148572 pubmed_types-0.1.2/src/pubmed_types/models/fpage.py
--rw-r--r--   0        0        0     2105 2023-06-03 02:44:02.156572 pubmed_types-0.1.2/src/pubmed_types/models/front.py
--rw-r--r--   0        0        0     9514 2023-06-03 02:44:02.168572 pubmed_types-0.1.2/src/pubmed_types/models/front_stub.py
--rw-r--r--   0        0        0     1657 2023-06-03 02:44:02.168572 pubmed_types-0.1.2/src/pubmed_types/models/funding_group.py
--rw-r--r--   0        0        0     9232 2023-06-03 02:44:02.184572 pubmed_types-0.1.2/src/pubmed_types/models/funding_statement.py
--rw-r--r--   0        0        0      327 2023-06-03 02:44:02.608566 pubmed_types-0.1.2/src/pubmed_types/models/gene_symbol_list.py
--rw-r--r--   0        0        0      465 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/general_note.py
--rw-r--r--   0        0        0      152 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/general_note_owner.py
--rw-r--r--   0        0        0     1866 2023-06-03 02:44:02.184572 pubmed_types-0.1.2/src/pubmed_types/models/glyph_data.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.188572 pubmed_types-0.1.2/src/pubmed_types/models/glyph_ref.py
--rw-r--r--   0        0        0      806 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/grant.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.612566 pubmed_types-0.1.2/src/pubmed_types/models/grant_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/grant_list_complete_yn.py
--rw-r--r--   0        0        0      110 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/graphic_orientation.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/graphic_position.py
--rw-r--r--   0        0        0      551 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/group.py
--rw-r--r--   0        0        0      338 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/group_list.py
--rw-r--r--   0        0        0      425 2023-06-03 02:44:02.888562 pubmed_types-0.1.2/src/pubmed_types/models/history_1.py
--rw-r--r--   0        0        0     7177 2023-06-03 02:44:02.908562 pubmed_types-0.1.2/src/pubmed_types/models/history_2.py
--rw-r--r--   0        0        0      528 2023-06-03 02:44:02.192571 pubmed_types-0.1.2/src/pubmed_types/models/hr.py
--rw-r--r--   0        0        0     3870 2023-06-03 02:18:03.805928 pubmed_types-0.1.2/src/pubmed_types/models/i.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/identifier.py
--rw-r--r--   0        0        0      718 2023-06-03 02:44:02.192571 pubmed_types-0.1.2/src/pubmed_types/models/index_term_range_end.py
--rw-r--r--   0        0        0     1475 2023-06-03 02:18:03.809928 pubmed_types-0.1.2/src/pubmed_types/models/individual_name.py
--rw-r--r--   0        0        0     2029 2023-06-03 02:44:02.200571 pubmed_types-0.1.2/src/pubmed_types/models/institution_id.py
--rw-r--r--   0        0        0     1537 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/investigator.py
--rw-r--r--   0        0        0      380 2023-06-03 02:44:02.616566 pubmed_types-0.1.2/src/pubmed_types/models/investigator_list.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/investigator_valid_yn.py
--rw-r--r--   0        0        0      515 2023-06-03 02:44:02.908562 pubmed_types-0.1.2/src/pubmed_types/models/issn_1.py
--rw-r--r--   0        0        0      100 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/issn_issn_type.py
--rw-r--r--   0        0        0     3124 2023-06-03 02:44:02.204571 pubmed_types-0.1.2/src/pubmed_types/models/issue_id.py
--rw-r--r--   0        0        0     7395 2023-06-03 02:44:02.216571 pubmed_types-0.1.2/src/pubmed_types/models/issue_sponsor.py
--rw-r--r--   0        0        0     7400 2023-06-03 02:44:02.228571 pubmed_types-0.1.2/src/pubmed_types/models/issue_subtitle.py
--rw-r--r--   0        0        0     1874 2023-06-03 02:44:02.228571 pubmed_types-0.1.2/src/pubmed_types/models/issue_title_group.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/italic_toggle.py
--rw-r--r--   0        0        0      508 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/item_list.py
--rw-r--r--   0        0        0      873 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/journal.py
--rw-r--r--   0        0        0     1543 2023-06-03 02:44:02.232571 pubmed_types-0.1.2/src/pubmed_types/models/journal_id.py
--rw-r--r--   0        0        0      942 2023-06-03 02:44:02.620566 pubmed_types-0.1.2/src/pubmed_types/models/journal_issue.py
--rw-r--r--   0        0        0      107 2023-06-03 02:44:02.832563 pubmed_types-0.1.2/src/pubmed_types/models/journal_issue_cited_medium.py
--rw-r--r--   0        0        0     2752 2023-06-03 02:44:02.236571 pubmed_types-0.1.2/src/pubmed_types/models/journal_meta.py
--rw-r--r--   0        0        0     7406 2023-06-03 02:44:02.252570 pubmed_types-0.1.2/src/pubmed_types/models/journal_subtitle.py
--rw-r--r--   0        0        0     7404 2023-06-03 02:44:02.264570 pubmed_types-0.1.2/src/pubmed_types/models/journal_title.py
--rw-r--r--   0        0        0     1683 2023-06-03 02:44:02.268570 pubmed_types-0.1.2/src/pubmed_types/models/journal_title_group.py
--rw-r--r--   0        0        0     1342 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/keyword.py
--rw-r--r--   0        0        0      601 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/keyword_list.py
--rw-r--r--   0        0        0      184 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/keyword_list_owner.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/keyword_major_topic_yn.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/location_label.py
--rw-r--r--   0        0        0      205 2023-06-03 02:44:02.852563 pubmed_types-0.1.2/src/pubmed_types/models/location_label_type.py
--rw-r--r--   0        0        0     1338 2023-06-03 02:44:02.272570 pubmed_types-0.1.2/src/pubmed_types/models/lpage.py
--rw-r--r--   0        0        0      108 2023-06-03 02:44:02.792563 pubmed_types-0.1.2/src/pubmed_types/models/media_orientation.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/media_position.py
--rw-r--r--   0        0        0     5578 2023-06-03 02:44:02.568566 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation.py
--rw-r--r--   0        0        0      178 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation_owner.py
--rw-r--r--   0        0        0      284 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/medline_citation_status.py
--rw-r--r--   0        0        0      813 2023-06-03 02:44:02.624565 pubmed_types-0.1.2/src/pubmed_types/models/medline_journal_info.py
--rw-r--r--   0        0        0      618 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading.py
--rw-r--r--   0        0        0      376 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading_list.py
--rw-r--r--   0        0        0     6803 2023-06-03 02:44:02.284570 pubmed_types-0.1.2/src/pubmed_types/models/meta_name.py
--rw-r--r--   0        0        0     6806 2023-06-03 02:44:02.296570 pubmed_types-0.1.2/src/pubmed_types/models/meta_value.py
--rw-r--r--   0        0        0     1408 2023-06-03 02:44:02.300570 pubmed_types-0.1.2/src/pubmed_types/models/milestone_end.py
--rw-r--r--   0        0        0     1414 2023-06-03 02:44:02.304570 pubmed_types-0.1.2/src/pubmed_types/models/milestone_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/monospace_toggle.py
--rw-r--r--   0        0        0     1334 2023-06-03 02:44:02.304570 pubmed_types-0.1.2/src/pubmed_types/models/month.py
--rw-r--r--   0        0        0      153 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/name_name_style.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.628565 pubmed_types-0.1.2/src/pubmed_types/models/name_of_substance.py
--rw-r--r--   0        0        0     1422 2023-06-03 02:44:02.308570 pubmed_types-0.1.2/src/pubmed_types/models/object_id.py
--rw-r--r--   0        0        0      354 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/object_list.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/object_mod.py
--rw-r--r--   0        0        0       81 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/option_correct.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/__init__.py
--rw-r--r--   0        0        0      124 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/__init__.py
--rw-r--r--   0        0        0      631 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py
--rw-r--r--   0        0        0      578 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/license_ref.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.989981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/__init__.py
--rw-r--r--   0        0        0    18558 2023-06-03 02:43:58.344624 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.116600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/and_mod.py
--rw-r--r--   0        0        0     2149 2023-06-03 02:44:00.364596 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.148599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccos.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccosh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccot.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccoth.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsc.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arccsch.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsec.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.188599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsech.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsin.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arcsinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.184599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctan.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arctanh.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.120600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/card.py
--rw-r--r--   0        0        0      466 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cartesianproduct.py
--rw-r--r--   0        0        0     1737 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py
--rw-r--r--   0        0        0     1584 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/codomain.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/columnalignstyle.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/complexes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.104600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/compose.py
--rw-r--r--   0        0        0  1555308 2023-06-03 02:44:00.088600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.120600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cos.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cosh.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cot.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/coth.py
--rw-r--r--   0        0        0     1767 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csc.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/csch.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/curl.py
--rw-r--r--   0        0        0      189 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/declare_occurrence.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/determinant.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/diff.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divergence.py
--rw-r--r--   0        0        0     1582 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/domain.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/emptyset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eq.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/equivalent.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/eulergamma.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exists.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exponentiale.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.116600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.148599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/false.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/forall.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gcd.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/geq.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/grad.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/gt.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ident.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/image.py
--rw-r--r--   0        0        0     1588 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginaryi.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/implies.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/in_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/infinity.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/int_mod.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/integers.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/intersect.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/interval.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.096600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/inverse.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lambda_mod.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/laplacian.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lcm.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/leq.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/limit.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/linestyle.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/list_order.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ln.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/log.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.140599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/lt.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maction_value.py
--rw-r--r--   0        0        0     2637 2023-06-03 02:44:00.268597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_groupalign.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup_value.py
--rw-r--r--   0        0        0     2605 2023-06-03 02:44:00.264598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_edge.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark_value.py
--rw-r--r--   0        0        0    74524 2023-06-03 02:44:00.364596 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accent.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_accentunder.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_align.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_bevelled.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_charalign.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_denomalign.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_dir.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_display.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_displaystyle.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_edge.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalcolumns.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_equalrows.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_fence.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.748564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_form.py
--rw-r--r--   0        0        0      199 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalign.py
--rw-r--r--   0        0        0      236 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignfirst.py
--rw-r--r--   0        0        0      235 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_indentalignlast.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.744564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_infixlinebreakstyle.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_largeop.py
--rw-r--r--   0        0        0      225 2023-06-03 02:44:02.752564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreak.py
--rw-r--r--   0        0        0      228 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_linebreakstyle.py
--rw-r--r--   0        0        0      208 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_location.py
--rw-r--r--   0        0        0      495 2023-06-03 02:44:02.756564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_longdivstyle.py
--rw-r--r--   0        0        0      641 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_movablelimits.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_numalign.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.768564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_overflow.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_separator.py
--rw-r--r--   0        0        0      204 2023-06-03 02:44:02.760564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_side.py
--rw-r--r--   0        0        0      200 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stackalign.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_stretchy.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.764564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_symmetric.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_value.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrix.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/matrixrow.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.128600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/max.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mean.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/median.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/menclose_value.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/merror_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfenced_value.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_denomalign.py
--rw-r--r--   0        0        0      165 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_numalign.py
--rw-r--r--   0        0        0      120 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mfrac_value.py
--rw-r--r--   0        0        0     5862 2023-06-03 02:44:00.256598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_fontweight.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.228598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/min.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py
--rw-r--r--   0        0        0     3231 2023-06-03 02:44:00.276597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py
--rw-r--r--   0        0        0      214 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_rowalign.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr_value.py
--rw-r--r--   0        0        0      499 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_longdivstyle.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlongdiv_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mmultiscripts_value.py
--rw-r--r--   0        0        0     5329 2023-06-03 02:44:00.232598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.732564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_value.py
--rw-r--r--   0        0        0    10043 2023-06-03 02:44:00.240598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_accent.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_dir.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fence.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_fontweight.py
--rw-r--r--   0        0        0      164 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_form.py
--rw-r--r--   0        0        0      197 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalign.py
--rw-r--r--   0        0        0      234 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignfirst.py
--rw-r--r--   0        0        0      233 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_indentalignlast.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_largeop.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreak.py
--rw-r--r--   0        0        0      226 2023-06-03 02:44:02.728564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_linebreakstyle.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_movablelimits.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_separator.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_stretchy.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.724564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_symmetric.py
--rw-r--r--   0        0        0      125 2023-06-03 02:44:02.720564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_value.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mode.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.100600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/moment.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_accent.py
--rw-r--r--   0        0        0      162 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_align.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mover_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mpadded_value.py
--rw-r--r--   0        0        0      137 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mphantom_value.py
--rw-r--r--   0        0        0     2432 2023-06-03 02:44:00.264598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mroot_value.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_dir.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.704564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mrow_value.py
--rw-r--r--   0        0        0     5585 2023-06-03 02:44:00.252598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_dir.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontstyle.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_fontweight.py
--rw-r--r--   0        0        0      639 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py
--rw-r--r--   0        0        0      131 2023-06-03 02:44:02.708564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_value.py
--rw-r--r--   0        0        0      213 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_location.py
--rw-r--r--   0        0        0      292 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarries_value.py
--rw-r--r--   0        0        0      211 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_location.py
--rw-r--r--   0        0        0      290 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mscarry_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msgroup_value.py
--rw-r--r--   0        0        0     3475 2023-06-03 02:44:00.260598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py
--rw-r--r--   0        0        0      121 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline_value.py
--rw-r--r--   0        0        0     5838 2023-06-03 02:44:00.248598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_dir.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_fontweight.py
--rw-r--r--   0        0        0      269 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_linebreak.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.712564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msqrt_value.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.740564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msrow_value.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_charalign.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_stackalign.py
--rw-r--r--   0        0        0      123 2023-06-03 02:44:02.664565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstack_value.py
--rw-r--r--   0        0        0      142 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accent.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_align.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_bevelled.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_charalign.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_denomalign.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_dir.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_displaystyle.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_edge.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_equalrows.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fence.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontstyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_fontweight.py
--rw-r--r--   0        0        0      168 2023-06-03 02:44:02.688565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_form.py
--rw-r--r--   0        0        0      201 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalign.py
--rw-r--r--   0        0        0      238 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignfirst.py
--rw-r--r--   0        0        0      237 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_indentalignlast.py
--rw-r--r--   0        0        0      187 2023-06-03 02:44:02.684565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_infixlinebreakstyle.py
--rw-r--r--   0        0        0      143 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_largeop.py
--rw-r--r--   0        0        0      227 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreak.py
--rw-r--r--   0        0        0      230 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_linebreakstyle.py
--rw-r--r--   0        0        0      210 2023-06-03 02:44:02.692565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_location.py
--rw-r--r--   0        0        0      497 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_longdivstyle.py
--rw-r--r--   0        0        0      643 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_movablelimits.py
--rw-r--r--   0        0        0      166 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_numalign.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.696565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_separator.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_side.py
--rw-r--r--   0        0        0      202 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stackalign.py
--rw-r--r--   0        0        0      144 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_stretchy.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.700564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_symmetric.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.680565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msub_value.py
--rw-r--r--   0        0        0      136 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msubsup_value.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msup_value.py
--rw-r--r--   0        0        0     6510 2023-06-03 02:44:00.272597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_displaystyle.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalcolumns.py
--rw-r--r--   0        0        0      145 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_equalrows.py
--rw-r--r--   0        0        0      206 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_side.py
--rw-r--r--   0        0        0      141 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.280597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtd.py
--rw-r--r--   0        0        0     5386 2023-06-03 02:44:00.244598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_dir.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontstyle.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_fontweight.py
--rw-r--r--   0        0        0      642 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py
--rw-r--r--   0        0        0      134 2023-06-03 02:44:02.716564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_value.py
--rw-r--r--   0        0        0     3175 2023-06-03 02:44:00.280597 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py
--rw-r--r--   0        0        0      207 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_rowalign.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.668565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr_value.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_accentunder.py
--rw-r--r--   0        0        0      163 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.676565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munder_value.py
--rw-r--r--   0        0        0      146 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accent.py
--rw-r--r--   0        0        0      151 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_accentunder.py
--rw-r--r--   0        0        0      167 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_align.py
--rw-r--r--   0        0        0      139 2023-06-03 02:44:02.672565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/munderover_value.py
--rw-r--r--   0        0        0      462 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/naturalnumbers.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.144599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py
--rw-r--r--   0        0        0     2401 2023-06-03 02:44:00.260598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py
--rw-r--r--   0        0        0      133 2023-06-03 02:44:02.736564 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none_value.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/not_mod.py
--rw-r--r--   0        0        0      454 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notanumber.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notin.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notprsubset.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/notsubset.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/or_mod.py
--rw-r--r--   0        0        0      458 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/outerproduct.py
--rw-r--r--   0        0        0      456 2023-06-03 02:44:00.156599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/partialdiff.py
--rw-r--r--   0        0        0      438 2023-06-03 02:44:00.216598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/pi.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/plus.py
--rw-r--r--   0        0        0     1580 2023-06-03 02:44:00.108600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.208598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/primes.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/product.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/prsubset.py
--rw-r--r--   0        0        0     1586 2023-06-03 02:44:00.104600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rationals.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.124600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.204599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/reals.py
--rw-r--r--   0        0        0     1576 2023-06-03 02:44:00.112600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py
--rw-r--r--   0        0        0     1578 2023-06-03 02:44:00.112600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/scalarproduct.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sdev.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sec.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.180599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sech.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/selector.py
--rw-r--r--   0        0        0      215 2023-06-03 02:44:00.092600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sep.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/setdiff.py
--rw-r--r--   0        0        0     1405 2023-06-03 02:44:00.088600 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sin.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sinh.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.164599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/subset.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.168599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/sum.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.172599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tan.py
--rw-r--r--   0        0        0      442 2023-06-03 02:44:00.176599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tanh.py
--rw-r--r--   0        0        0     1710 2023-06-03 02:44:00.152599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py
--rw-r--r--   0        0        0      444 2023-06-03 02:44:00.132599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/times.py
--rw-r--r--   0        0        0      452 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/transpose.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.212598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/true.py
--rw-r--r--   0        0        0      448 2023-06-03 02:44:00.160599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/union.py
--rw-r--r--   0        0        0      450 2023-06-03 02:44:00.192599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/variance.py
--rw-r--r--   0        0        0      446 2023-06-03 02:44:00.196599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vector.py
--rw-r--r--   0        0        0      460 2023-06-03 02:44:00.200599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/vectorproduct.py
--rw-r--r--   0        0        0      209 2023-06-03 02:44:00.224598 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/verticalalign.py
--rw-r--r--   0        0        0      440 2023-06-03 02:44:00.136599 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/xor.py
--rw-r--r--   0        0        0       15 2023-06-03 02:17:59.961981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/__init__.py
--rw-r--r--   0        0        0      488 2023-06-03 02:43:58.316624 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/__init__.py
--rw-r--r--   0        0        0      188 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/actuate_value.py
--rw-r--r--   0        0        0     1893 2023-06-03 02:43:58.428623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py
--rw-r--r--   0        0        0     1169 2023-06-03 02:43:58.420623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py
--rw-r--r--   0        0        0     1453 2023-06-03 02:43:58.428623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py
--rw-r--r--   0        0        0     1244 2023-06-03 02:43:58.424623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py
--rw-r--r--   0        0        0      193 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/show_value.py
--rw-r--r--   0        0        0     1940 2023-06-03 02:43:58.416623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py
--rw-r--r--   0        0        0     1203 2023-06-03 02:43:58.424623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py
--rw-r--r--   0        0        0      247 2023-06-03 02:44:02.660565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/type_value.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/__init__.py
--rw-r--r--   0        0        0       15 2023-06-03 02:18:00.009981 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/__init__.py
--rw-r--r--   0        0        0      120 2023-06-03 02:43:58.380623 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/__init__.py
--rw-r--r--   0        0        0      118 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/lang_value.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/org/w3/xml/pkg_1998/namespace/space_value.py
--rw-r--r--   0        0        0      997 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/other_abstract.py
--rw-r--r--   0        0        0      223 2023-06-03 02:44:02.844563 pubmed_types-0.1.2/src/pubmed_types/models/other_abstract_type.py
--rw-r--r--   0        0        0      518 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/other_id.py
--rw-r--r--   0        0        0      257 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/other_id_source.py
--rw-r--r--   0        0        0      863 2023-06-03 02:44:02.312570 pubmed_types-0.1.2/src/pubmed_types/models/overline_end.py
--rw-r--r--   0        0        0      747 2023-06-03 02:44:02.312570 pubmed_types-0.1.2/src/pubmed_types/models/overline_start.py
--rw-r--r--   0        0        0       82 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/overline_toggle.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.316570 pubmed_types-0.1.2/src/pubmed_types/models/page_count.py
--rw-r--r--   0        0        0     1349 2023-06-03 02:44:02.320570 pubmed_types-0.1.2/src/pubmed_types/models/page_range.py
--rw-r--r--   0        0        0      649 2023-06-03 02:44:02.636565 pubmed_types-0.1.2/src/pubmed_types/models/pagination.py
--rw-r--r--   0        0        0     1147 2023-06-03 02:44:02.636565 pubmed_types-0.1.2/src/pubmed_types/models/param.py
--rw-r--r--   0        0        0      831 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject.py
--rw-r--r--   0        0        0      426 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject_list.py
--rw-r--r--   0        0        0      461 2023-06-03 02:44:02.632565 pubmed_types-0.1.2/src/pubmed_types/models/pmid.py
--rw-r--r--   0        0        0     1366 2023-06-03 02:44:02.320570 pubmed_types-0.1.2/src/pubmed_types/models/postal_code.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/preformat_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.796563 pubmed_types-0.1.2/src/pubmed_types/models/preformat_position.py
--rw-r--r--   0        0        0     2142 2023-06-03 02:44:02.324570 pubmed_types-0.1.2/src/pubmed_types/models/principal_award_recipient.py
--rw-r--r--   0        0        0     1855 2023-06-03 02:44:02.328570 pubmed_types-0.1.2/src/pubmed_types/models/principal_investigator.py
--rw-r--r--   0        0        0     2483 2023-06-03 02:44:02.332569 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta.py
--rw-r--r--   0        0        0      148 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_base_tagset.py
--rw-r--r--   0        0        0      109 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_mathml_version.py
--rw-r--r--   0        0        0      138 2023-06-03 02:44:02.824563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_table_model.py
--rw-r--r--   0        0        0      116 2023-06-03 02:44:02.828563 pubmed_types-0.1.2/src/pubmed_types/models/processing_meta_tagset_family.py
--rw-r--r--   0        0        0      936 2023-06-03 02:44:02.912562 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_1.py
--rw-r--r--   0        0        0     2895 2023-06-03 02:44:02.916561 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_2.py
--rw-r--r--   0        0        0      740 2023-06-03 02:44:02.332569 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_not_available.py
--rw-r--r--   0        0        0      408 2023-06-03 02:18:04.041925 pubmed_types-0.1.2/src/pubmed_types/models/pub_date_pub_status.py
--rw-r--r--   0        0        0      708 2023-06-03 02:44:02.336569 pubmed_types-0.1.2/src/pubmed_types/models/pub_history.py
--rw-r--r--   0        0        0     2871 2023-06-03 02:44:02.340569 pubmed_types-0.1.2/src/pubmed_types/models/pub_id.py
--rw-r--r--   0        0        0     1462 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date.py
--rw-r--r--   0        0        0      496 2023-06-03 02:44:02.848563 pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date_pub_status.py
--rw-r--r--   0        0        0      423 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/publication_type.py
--rw-r--r--   0        0        0      400 2023-06-03 02:44:02.640565 pubmed_types-0.1.2/src/pubmed_types/models/publication_type_list.py
--rw-r--r--   0        0        0     1192 2023-06-03 02:18:03.561932 pubmed_types-0.1.2/src/pubmed_types/models/publisher.py
--rw-r--r--   0        0        0      606 2023-06-03 02:44:02.920561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_1.py
--rw-r--r--   0        0        0     1193 2023-06-03 02:44:02.920561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_2.py
--rw-r--r--   0        0        0     1013 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/publisher_name_1.py
--rw-r--r--   0        0        0      600 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article.py
--rw-r--r--   0        0        0      839 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article_set.py
--rw-r--r--   0        0        0      611 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article.py
--rw-r--r--   0        0        0      384 2023-06-03 02:44:02.556566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article_set.py
--rw-r--r--   0        0        0      991 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_data.py
--rw-r--r--   0        0        0     1217 2023-06-03 02:44:02.572566 pubmed_types-0.1.2/src/pubmed_types/models/pubmed_data.py
--rw-r--r--   0        0        0      724 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.840563 pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name_major_topic_yn.py
--rw-r--r--   0        0        0      268 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/question_question_response_type.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.344569 pubmed_types-0.1.2/src/pubmed_types/models/ref_count.py
--rw-r--r--   0        0        0      576 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/reference.py
--rw-r--r--   0        0        0      678 2023-06-03 02:44:02.644565 pubmed_types-0.1.2/src/pubmed_types/models/reference_list.py
--rw-r--r--   0        0        0      460 2023-06-03 02:18:03.773929 pubmed_types-0.1.2/src/pubmed_types/models/replaces.py
--rw-r--r--   0        0        0      192 2023-06-03 02:18:04.045925 pubmed_types-0.1.2/src/pubmed_types/models/replaces_id_type.py
--rw-r--r--   0        0        0     1440 2023-06-03 02:44:02.348569 pubmed_types-0.1.2/src/pubmed_types/models/resource_group.py
--rw-r--r--   0        0        0     2014 2023-06-03 02:44:02.348569 pubmed_types-0.1.2/src/pubmed_types/models/resource_id.py
--rw-r--r--   0        0        0     4999 2023-06-03 02:44:02.356569 pubmed_types-0.1.2/src/pubmed_types/models/resource_name.py
--rw-r--r--   0        0        0     1009 2023-06-03 02:44:02.360569 pubmed_types-0.1.2/src/pubmed_types/models/resource_wrap.py
--rw-r--r--   0        0        0     2223 2023-06-03 02:44:02.364569 pubmed_types-0.1.2/src/pubmed_types/models/response.py
--rw-r--r--   0        0        0     3137 2023-06-03 02:44:02.368569 pubmed_types-0.1.2/src/pubmed_types/models/restricted_by.py
--rw-r--r--   0        0        0       79 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/roman_toggle.py
--rw-r--r--   0        0        0      728 2023-06-03 02:44:02.368569 pubmed_types-0.1.2/src/pubmed_types/models/rp.py
--rw-r--r--   0        0        0     1346 2023-06-03 02:44:02.372569 pubmed_types-0.1.2/src/pubmed_types/models/rt.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.772564 pubmed_types-0.1.2/src/pubmed_types/models/sans_serif_toggle.py
--rw-r--r--   0        0        0       76 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/sc_toggle.py
--rw-r--r--   0        0        0     1337 2023-06-03 02:44:02.376569 pubmed_types-0.1.2/src/pubmed_types/models/season.py
--rw-r--r--   0        0        0      765 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/section.py
--rw-r--r--   0        0        0     1341 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/section_title.py
--rw-r--r--   0        0        0      347 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/sections.py
--rw-r--r--   0        0        0     9015 2023-06-03 02:44:02.388569 pubmed_types-0.1.2/src/pubmed_types/models/self_uri.py
--rw-r--r--   0        0        0     7416 2023-06-03 02:44:02.400569 pubmed_types-0.1.2/src/pubmed_types/models/series_text.py
--rw-r--r--   0        0        0     7394 2023-06-03 02:44:02.412568 pubmed_types-0.1.2/src/pubmed_types/models/series_title.py
--rw-r--r--   0        0        0     7912 2023-06-03 02:44:02.424568 pubmed_types-0.1.2/src/pubmed_types/models/sig.py
--rw-r--r--   0        0        0     8403 2023-06-03 02:44:02.440568 pubmed_types-0.1.2/src/pubmed_types/models/sig_block.py
--rw-r--r--   0        0        0     1361 2023-06-03 02:44:02.444568 pubmed_types-0.1.2/src/pubmed_types/models/state.py
--rw-r--r--   0        0        0       80 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/strike_toggle.py
--rw-r--r--   0        0        0     8497 2023-06-03 02:44:02.460568 pubmed_types-0.1.2/src/pubmed_types/models/string_conf.py
--rw-r--r--   0        0        0      159 2023-06-03 02:44:02.784563 pubmed_types-0.1.2/src/pubmed_types/models/string_name_name_style.py
--rw-r--r--   0        0        0       87 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/styled_content_toggle.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/sub_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/sub_arrange.py
--rw-r--r--   0        0        0     2576 2023-06-03 02:44:02.468568 pubmed_types-0.1.2/src/pubmed_types/models/sub_article.py
--rw-r--r--   0        0        0      999 2023-06-03 02:44:02.924561 pubmed_types-0.1.2/src/pubmed_types/models/suffix_1.py
--rw-r--r--   0        0        0      993 2023-06-03 02:44:02.928561 pubmed_types-0.1.2/src/pubmed_types/models/sup_1.py
--rw-r--r--   0        0        0       92 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/sup_arrange.py
--rw-r--r--   0        0        0      386 2023-06-03 02:44:02.648565 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_list.py
--rw-r--r--   0        0        0      668 2023-06-03 02:44:02.652565 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name.py
--rw-r--r--   0        0        0      185 2023-06-03 02:44:02.836563 pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name_type.py
--rw-r--r--   0        0        0      124 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/supplementary_material_orientation.py
--rw-r--r--   0        0        0      161 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/supplementary_material_position.py
--rw-r--r--   0        0        0     1316 2023-06-03 02:44:02.472568 pubmed_types-0.1.2/src/pubmed_types/models/support_description.py
--rw-r--r--   0        0        0     1500 2023-06-03 02:44:02.476568 pubmed_types-0.1.2/src/pubmed_types/models/support_group.py
--rw-r--r--   0        0        0     9397 2023-06-03 02:44:02.500567 pubmed_types-0.1.2/src/pubmed_types/models/support_source.py
--rw-r--r--   0        0        0      695 2023-06-03 02:44:02.500567 pubmed_types-0.1.2/src/pubmed_types/models/table_count.py
--rw-r--r--   0        0        0      220 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/table_frame.py
--rw-r--r--   0        0        0      140 2023-06-03 02:44:02.804563 pubmed_types-0.1.2/src/pubmed_types/models/table_rules.py
--rw-r--r--   0        0        0      117 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_group_orientation.py
--rw-r--r--   0        0        0      154 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_group_position.py
--rw-r--r--   0        0        0      112 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_orientation.py
--rw-r--r--   0        0        0      149 2023-06-03 02:44:02.800563 pubmed_types-0.1.2/src/pubmed_types/models/table_wrap_position.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tbody_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.820563 pubmed_types-0.1.2/src/pubmed_types/models/tbody_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/td_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/td_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/td_valign.py
--rw-r--r--   0        0        0     1386 2023-06-03 02:44:02.504567 pubmed_types-0.1.2/src/pubmed_types/models/tex_math.py
--rw-r--r--   0        0        0      128 2023-06-03 02:44:02.780563 pubmed_types-0.1.2/src/pubmed_types/models/tex_math_notation.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tfoot_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.816563 pubmed_types-0.1.2/src/pubmed_types/models/tfoot_valign.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_align.py
--rw-r--r--   0        0        0      129 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_scope.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.812563 pubmed_types-0.1.2/src/pubmed_types/models/th_valign.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/thead_align.py
--rw-r--r--   0        0        0      135 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/thead_valign.py
--rw-r--r--   0        0        0     1542 2023-06-03 02:44:02.508567 pubmed_types-0.1.2/src/pubmed_types/models/title_group.py
--rw-r--r--   0        0        0      147 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/tr_align.py
--rw-r--r--   0        0        0      132 2023-06-03 02:44:02.808563 pubmed_types-0.1.2/src/pubmed_types/models/tr_valign.py
--rw-r--r--   0        0        0     8912 2023-06-03 02:44:02.520567 pubmed_types-0.1.2/src/pubmed_types/models/trans_abstract.py
--rw-r--r--   0        0        0     7376 2023-06-03 02:44:02.532567 pubmed_types-0.1.2/src/pubmed_types/models/trans_subtitle.py
--rw-r--r--   0        0        0     1641 2023-06-03 02:44:02.536567 pubmed_types-0.1.2/src/pubmed_types/models/trans_title_group.py
--rw-r--r--   0        0        0     2610 2023-06-03 02:44:02.584566 pubmed_types-0.1.2/src/pubmed_types/models/u.py
--rw-r--r--   0        0        0      866 2023-06-03 02:44:02.536567 pubmed_types-0.1.2/src/pubmed_types/models/underline_end.py
--rw-r--r--   0        0        0      750 2023-06-03 02:44:02.540567 pubmed_types-0.1.2/src/pubmed_types/models/underline_start.py
--rw-r--r--   0        0        0       83 2023-06-03 02:44:02.776564 pubmed_types-0.1.2/src/pubmed_types/models/underline_toggle.py
--rw-r--r--   0        0        0      614 2023-06-03 02:44:02.652565 pubmed_types-0.1.2/src/pubmed_types/models/url.py
--rw-r--r--   0        0        0      661 2023-06-03 02:44:02.856562 pubmed_types-0.1.2/src/pubmed_types/models/url_lang.py
--rw-r--r--   0        0        0      150 2023-06-03 02:44:02.856562 pubmed_types-0.1.2/src/pubmed_types/models/url_type.py
--rw-r--r--   0        0        0     1072 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/vernacular_title.py
--rw-r--r--   0        0        0     2893 2023-06-03 02:44:02.544567 pubmed_types-0.1.2/src/pubmed_types/models/volume_issue_group.py
--rw-r--r--   0        0        0      962 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/volume_title.py
--rw-r--r--   0        0        0      692 2023-06-03 02:44:02.548566 pubmed_types-0.1.2/src/pubmed_types/models/word_count.py
--rw-r--r--   0        0        0      330 2023-06-03 02:44:02.656565 pubmed_types-0.1.2/src/pubmed_types/models/xs_pattern.py
--rw-r--r--   0        0        0     1627 2023-06-03 02:44:02.552566 pubmed_types-0.1.2/src/pubmed_types/models/year.py
--rw-r--r--   0        0        0     5511 1970-01-01 00:00:00.000000 pubmed_types-0.1.2/PKG-INFO
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

### Comparing `pubmed_types-0.1.2/LICENSE` & `pubmed_types-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/README.md` & `pubmed_types-0.2.0.dev0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-# pubmed-types (v0.1.2)
+# pubmed-types (v0.2.0-dev0)
 
 <p align="center">
     <img src="https://img.shields.io/pypi/dm/pubmed-types?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/pubmed-types?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/pubmed-types?style=flat-square"/>
-    <a href="https://github.com/tefra/xsdata-pydantic"><img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+    <a href="https://github.com/tefra/xsdata-pydantic">
+        <img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/Built%20with-xsdata--pydantic-blue">
+    </a>
+    <a href="https://github.com/dbrgn/coverage-badge">
+        <img src="./images/coverage.svg">
+    </a>
 </p>
 
 ## Introduction
 
 A complete implementation of the XML schema for PMC Open Access articles and Pubmed
 article sets (citations).
 
 This package helps to parse PubMed XML data into Pydantic models. This validates the
 input xml data and provides typehints for working with the complex XML structures
 present in PubMed data.
 
+## Most Recent Changes
+
+* **Breaking Change:** The `parse_pubmed_xml` is replaced by `pmc_article` and `pubmed_article_set`.
+* More test coverage
+* Pubmed Articles can now parse MathML
+* Restructured code to separate out `jats` (pmc open access articles) and `pubmed` (pubmed article set)
+* One unit test with 99% coverage
+* Added [CHANGELOG.md](CHANGELOG.md)
+
 ## Why do I need this?
 
 PubMed keeps track of 10s of millions of research data, and a complex XML structure is
 used to store it. Parsing XML on its own is challenging enough. Add to it the feature
 rich data inside of each citation, and you will find yourself with hours or days of
 navigating the XML structure.
 
@@ -72,16 +86,14 @@
 
 ```bash
 Title: Lactate as a myokine and exerkine: drivers and signals of physiology and metabolism
 ```
 
 ### Example 2: A Pubmed baseline citation file
 
-### Example 1: A PMC Open Access Article
-
 ```python
 import gzip
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
 from pubmed_types import parse_pubmed_xml, PubmedArticleSet
```

#### html2text {}

```diff
@@ -1,52 +1,57 @@
-# pubmed-types (v0.1.2)
+# pubmed-types (v0.2.0-dev0)
    [https://img.shields.io/pypi/dm/pubmed-types?style=flat-square] [https://
 img.shields.io/pypi/l/pubmed-types?style=flat-square] [https://img.shields.io/
-     pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic]
+pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic] [./images/
+                                 coverage.svg]
 ## Introduction A complete implementation of the XML schema for PMC Open Access
 articles and Pubmed article sets (citations). This package helps to parse
 PubMed XML data into Pydantic models. This validates the input xml data and
 provides typehints for working with the complex XML structures present in
-PubMed data. ## Why do I need this? PubMed keeps track of 10s of millions of
-research data, and a complex XML structure is used to store it. Parsing XML on
-its own is challenging enough. Add to it the feature rich data inside of each
-citation, and you will find yourself with hours or days of navigating the XML
-structure. The approach here was to autogenerate Pydantic classes to parse the
-XML using the `xsdata-pydantic` tool. This approach has the benefit of making
-sure every piece of data is parsed properly, and an error is thrown is
-something is missing or incorrect. Instead of using dictionaries to hold the
-data, Pydantic classes have the benefit of providing type hints with tab
-completion for IDEs, making it easier to navigate the complex structure of the
-citation data. ## How do I use it? It is possible to use `xsdata-pydantic` and
-the autogenerated classes directly to parse an XML file, but we provide a
-convenience function to easily open PubMed XMl citations and PMC open access
-articles. ### Example 1: A PMC Open Access Article ```python import tarfile
-import urllib.request as request from contextlib import closing from pathlib
-import Path from pubmed_types import parse_pubmed_xml # Input file source and
-output file destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/
-oa_bulk/oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination =
-Path("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access
-article dataset from the FTP server with closing(request.urlopen(source)) as
-url: with tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall
-(destination) # 2. Parse the file file_path = destination.joinpath
-("PMC009xxxxxx").joinpath("PMC9970662.xml") full_text = parse_pubmed_xml
-(file_path) # 3. Print out the article title print(f"Title:
+PubMed data. ## Most Recent Changes * **Breaking Change:** The
+`parse_pubmed_xml` is replaced by `pmc_article` and `pubmed_article_set`. *
+More test coverage * Pubmed Articles can now parse MathML * Restructured code
+to separate out `jats` (pmc open access articles) and `pubmed` (pubmed article
+set) * One unit test with 99% coverage * Added [CHANGELOG.md](CHANGELOG.md) ##
+Why do I need this? PubMed keeps track of 10s of millions of research data, and
+a complex XML structure is used to store it. Parsing XML on its own is
+challenging enough. Add to it the feature rich data inside of each citation,
+and you will find yourself with hours or days of navigating the XML structure.
+The approach here was to autogenerate Pydantic classes to parse the XML using
+the `xsdata-pydantic` tool. This approach has the benefit of making sure every
+piece of data is parsed properly, and an error is thrown is something is
+missing or incorrect. Instead of using dictionaries to hold the data, Pydantic
+classes have the benefit of providing type hints with tab completion for IDEs,
+making it easier to navigate the complex structure of the citation data. ## How
+do I use it? It is possible to use `xsdata-pydantic` and the autogenerated
+classes directly to parse an XML file, but we provide a convenience function to
+easily open PubMed XMl citations and PMC open access articles. ### Example 1: A
+PMC Open Access Article ```python import tarfile import urllib.request as
+request from contextlib import closing from pathlib import Path from
+pubmed_types import parse_pubmed_xml # Input file source and output file
+destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/
+oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path
+("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access article
+dataset from the FTP server with closing(request.urlopen(source)) as url: with
+tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2.
+Parse the file file_path = destination.joinpath("PMC009xxxxxx").joinpath
+("PMC9970662.xml") full_text = parse_pubmed_xml(file_path) # 3. Print out the
+article title print(f"Title:
 {full_text.front.article_meta.title_group.article_title.content[0]}") ```
 Output: ```bash Title: Lactate as a myokine and exerkine: drivers and signals
 of physiology and metabolism ``` ### Example 2: A Pubmed baseline citation file
-### Example 1: A PMC Open Access Article ```python import gzip import
-urllib.request as request from contextlib import closing from pathlib import
-Path from pubmed_types import parse_pubmed_xml, PubmedArticleSet # Input file
-source and output file destination source = "ftp://ftp.ncbi.nlm.nih.gov" + "/
-pubmed/updatefiles" + "/pubmed23n1168.xml.gz" destination = Path
-("downloads").joinpath("pubmed23n1168.xml") destination.parent.mkdir
-(exist_ok=True) # 1. Get a pubmed citation daily update file from the FTP
-server with closing(request.urlopen(source)) as url: with gzip.GzipFile
-(fileobj=url, mode="rb") as fr: with open(destination, mode="wb") as fw:
-fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
+```python import gzip import urllib.request as request from contextlib import
+closing from pathlib import Path from pubmed_types import parse_pubmed_xml,
+PubmedArticleSet # Input file source and output file destination source = "ftp:
+//ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
+destination = Path("downloads").joinpath("pubmed23n1168.xml")
+destination.parent.mkdir(exist_ok=True) # 1. Get a pubmed citation daily update
+file from the FTP server with closing(request.urlopen(source)) as url: with
+gzip.GzipFile(fileobj=url, mode="rb") as fr: with open(destination, mode="wb")
+as fw: fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
 (destination) assert isinstance(article_set, PubmedArticleSet) # 3. Get the
 number of citations in the file print(f"Number of citations: {len
 (article_set.pubmed_article)}") print(f"{article_set.pubmed_article
 [0].medline_citation.article.article_title.content[0]}") ``` Output: ```bash
 Number of citations: 2543 A Patent and Pattern Mother. ``` ## FAQ ### Why does
 it take so long to parse a pubmed citation set There is a lot of data, and the
 schema is deep and complex. ### Why are the return structures so complicated?
```

### Comparing `pubmed_types-0.1.2/pyproject.toml` & `pubmed_types-0.2.0.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pubmed-types"
-version = "0.1.2"
+version = "0.2.0-dev0"
 authors = ["Nick Schaub <nick.schaub@nih.gov>"]
 description = "Pubmed XML parsing and typehints."
 readme = "README.md"
 license = "MIT"
 packages = [{include = "pubmed_types", from = "src"}]
 homepage = "https://github.com/nicholas-schaub/pubmed-types"
 repository = "https://github.com/nicholas-schaub/pubmed-types"
@@ -32,13 +32,16 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.270"
 pre-commit = "^3.3.2"
 nox = "^2023.4.22"
 requests = "^2.31.0"
-pytest = "^5.2"
+pytest = "^7.3.1"
 bump2version = "^1.0.1"
+pytest-cov = "^4.1.0"
+pytest-xdist = "^3.3.1"
+coverage-badge = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from .abbrev_journal_title import AbbrevJournalTitle
-from .abstract_1 import Abstract1
-from .abstract_text import AbstractText
-from .abstract_text_nlm_category import AbstractTextNlmCategory
 from .access_date import (
     Abbrev,
-    Abstract2,
+    Abstract,
     AccessDate,
     Ack,
     AddrLine,
     Address,
     Aff,
     AffAlternatives,
     AltTitle,
@@ -53,16 +50,16 @@
     Date,
     DateInCitation,
     Def,
     DefHead,
     DefItem,
     DefList,
     Degrees,
+    DispFormula,
     DispFormulaGroup,
-    DispFormula2,
     DispQuote,
     Edition,
     ElementCitation,
     Email,
     Etal,
     Explanation,
     ExtLink,
@@ -191,110 +188,64 @@
     Version,
     Volume,
     VolumeId,
     VolumeSeries,
     X,
     Xref,
 )
-from .accession_number_list import AccessionNumberList
-from .affiliation import Affiliation
-from .affiliation_info import AffiliationInfo
 from .alt_text import AltText
 from .app import App
 from .app_group import AppGroup
 from .array_orientation import ArrayOrientation
-from .article_1 import Article1
-from .article_2 import Article2
+from .article import Article
 from .article_categories import ArticleCategories
-from .article_date import ArticleDate
 from .article_dtd_version import ArticleDtdVersion
 from .article_id import ArticleId
-from .article_id_1 import ArticleId1
-from .article_id_id_type import ArticleIdIdType
-from .article_id_list import ArticleIdList
 from .article_meta import ArticleMeta
-from .article_pub_model import ArticlePubModel
-from .article_title_1 import ArticleTitle1
 from .article_version import ArticleVersion
 from .article_version_alternatives import ArticleVersionAlternatives
-from .author import Author
-from .author_equal_contrib import AuthorEqualContrib
-from .author_list import AuthorList
-from .author_list_complete_yn import AuthorListCompleteYn
-from .author_list_type import AuthorListType
 from .author_notes import AuthorNotes
-from .author_valid_yn import AuthorValidYn
 from .award_desc import AwardDesc
 from .award_group import AwardGroup
 from .award_name import AwardName
 from .back import Back
-from .beginning_date import BeginningDate
 from .body import Body
 from .bold_toggle import BoldToggle
-from .book import Book
-from .book_document import BookDocument
-from .book_document_set import BookDocumentSet
-from .book_title import BookTitle
 from .boxed_text_orientation import BoxedTextOrientation
 from .boxed_text_position import BoxedTextPosition
 from .break_mod import Break
 from .chem_struct_wrap_orientation import ChemStructWrapOrientation
 from .chem_struct_wrap_position import ChemStructWrapPosition
-from .chemical import Chemical
-from .chemical_list import ChemicalList
-from .citation import Citation
 from .city import City
 from .code_executable import CodeExecutable
 from .code_orientation import CodeOrientation
 from .code_position import CodePosition
-from .coi_statement import CoiStatement
 from .col import Col
 from .col_align import ColAlign
 from .col_valign import ColValign
 from .colgroup import Colgroup
 from .colgroup_align import ColgroupAlign
 from .colgroup_valign import ColgroupValign
-from .collection_title import CollectionTitle
-from .collective_name import CollectiveName
-from .comments_corrections import CommentsCorrections
-from .comments_corrections_list import CommentsCorrectionsList
-from .comments_corrections_ref_type import CommentsCorrectionsRefType
 from .conf_num import ConfNum
 from .conf_theme import ConfTheme
 from .conference import Conference
 from .contrib_corresp import ContribCorresp
 from .contrib_deceased import ContribDeceased
 from .contrib_equal_contrib import ContribEqualContrib
 from .contrib_id import ContribId
 from .contrib_id_authenticated import ContribIdAuthenticated
 from .contributed_resource_group import ContributedResourceGroup
-from .contribution_date import ContributionDate
 from .copyright_year import CopyrightYear
 from .corresp import Corresp
 from .count import Count
 from .counts import Counts
 from .custom_meta import CustomMeta
 from .custom_meta_group import CustomMetaGroup
-from .data_bank import DataBank
-from .data_bank_list import DataBankList
-from .data_bank_list_complete_yn import DataBankListCompleteYn
-from .date_completed import DateCompleted
-from .date_revised import DateRevised
 from .day import Day
-from .delete_citation import DeleteCitation
-from .delete_document import DeleteDocument
-from .descriptor_name import DescriptorName
-from .descriptor_name_major_topic_yn import DescriptorNameMajorTopicYn
-from .descriptor_name_type import DescriptorNameType
-from .disp_formula_1 import DispFormula1
 from .elocation_id import ElocationId
-from .elocation_id_1 import ElocationId1
-from .elocation_id_eid_type import ElocationIdEidType
-from .elocation_id_valid_yn import ElocationIdValidYn
-from .ending_date import EndingDate
 from .equation_count import EquationCount
 from .era import Era
 from .event import Event
 from .event_desc import EventDesc
 from .extended_by import ExtendedBy
 from .fig_count import FigCount
 from .fig_group_orientation import FigGroupOrientation
@@ -303,158 +254,91 @@
 from .fig_position import FigPosition
 from .floats_group import FloatsGroup
 from .fpage import Fpage
 from .front import Front
 from .front_stub import FrontStub
 from .funding_group import FundingGroup
 from .funding_statement import FundingStatement
-from .gene_symbol_list import GeneSymbolList
-from .general_note import GeneralNote
-from .general_note_owner import GeneralNoteOwner
 from .glyph_data import GlyphData
 from .glyph_ref import GlyphRef
-from .grant import Grant
-from .grant_list import GrantList
-from .grant_list_complete_yn import GrantListCompleteYn
 from .graphic_orientation import GraphicOrientation
 from .graphic_position import GraphicPosition
-from .history_1 import History1
-from .history_2 import History2
+from .history import History
 from .hr import Hr
-from .identifier import Identifier
 from .index_term_range_end import IndexTermRangeEnd
 from .institution_id import InstitutionId
-from .investigator import Investigator
-from .investigator_list import InvestigatorList
-from .investigator_valid_yn import InvestigatorValidYn
-from .issn_1 import Issn1
-from .issn_issn_type import IssnIssnType
 from .issue_id import IssueId
 from .issue_sponsor import IssueSponsor
 from .issue_subtitle import IssueSubtitle
 from .issue_title_group import IssueTitleGroup
 from .italic_toggle import ItalicToggle
-from .item_list import ItemList
-from .journal import Journal
 from .journal_id import JournalId
-from .journal_issue import JournalIssue
-from .journal_issue_cited_medium import JournalIssueCitedMedium
 from .journal_meta import JournalMeta
 from .journal_subtitle import JournalSubtitle
 from .journal_title import JournalTitle
 from .journal_title_group import JournalTitleGroup
-from .keyword import Keyword
-from .keyword_list import KeywordList
-from .keyword_list_owner import KeywordListOwner
-from .keyword_major_topic_yn import KeywordMajorTopicYn
-from .location_label import LocationLabel
-from .location_label_type import LocationLabelType
 from .lpage import Lpage
 from .media_orientation import MediaOrientation
 from .media_position import MediaPosition
-from .medline_citation import MedlineCitation
-from .medline_citation_owner import MedlineCitationOwner
-from .medline_citation_status import MedlineCitationStatus
-from .medline_journal_info import MedlineJournalInfo
-from .mesh_heading import MeshHeading
-from .mesh_heading_list import MeshHeadingList
 from .meta_name import MetaName
 from .meta_value import MetaValue
 from .milestone_end import MilestoneEnd
 from .milestone_start import MilestoneStart
 from .monospace_toggle import MonospaceToggle
 from .month import Month
 from .name_name_style import NameNameStyle
-from .name_of_substance import NameOfSubstance
 from .object_id import ObjectId
-from .object_list import ObjectList
-from .object_mod import Object
 from .option_correct import OptionCorrect
-from .other_abstract import OtherAbstract
-from .other_abstract_type import OtherAbstractType
-from .other_id import OtherId
-from .other_id_source import OtherIdSource
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .overline_toggle import OverlineToggle
 from .page_count import PageCount
 from .page_range import PageRange
-from .pagination import Pagination
-from .param import Param
-from .personal_name_subject import PersonalNameSubject
-from .personal_name_subject_list import PersonalNameSubjectList
-from .pmid import Pmid
 from .postal_code import PostalCode
 from .preformat_orientation import PreformatOrientation
 from .preformat_position import PreformatPosition
 from .principal_award_recipient import PrincipalAwardRecipient
 from .principal_investigator import PrincipalInvestigator
 from .processing_meta import ProcessingMeta
 from .processing_meta_base_tagset import ProcessingMetaBaseTagset
 from .processing_meta_mathml_version import ProcessingMetaMathmlVersion
 from .processing_meta_table_model import ProcessingMetaTableModel
 from .processing_meta_tagset_family import ProcessingMetaTagsetFamily
-from .pub_date_1 import PubDate1
-from .pub_date_2 import PubDate2
+from .pub_date import PubDate
 from .pub_date_not_available import PubDateNotAvailable
 from .pub_history import PubHistory
 from .pub_id import PubId
-from .pub_med_pub_date import PubMedPubDate
-from .pub_med_pub_date_pub_status import PubMedPubDatePubStatus
-from .publication_type import PublicationType
-from .publication_type_list import PublicationTypeList
-from .publisher_1 import Publisher1
-from .publisher_2 import Publisher2
-from .publisher_name_1 import PublisherName1
-from .pubmed_article import PubmedArticle
-from .pubmed_article_set import PubmedArticleSet
-from .pubmed_book_article import PubmedBookArticle
-from .pubmed_book_article_set import PubmedBookArticleSet
-from .pubmed_book_data import PubmedBookData
-from .pubmed_data import PubmedData
-from .qualifier_name import QualifierName
-from .qualifier_name_major_topic_yn import QualifierNameMajorTopicYn
+from .publisher import Publisher
 from .question_question_response_type import QuestionQuestionResponseType
 from .ref_count import RefCount
-from .reference import Reference
-from .reference_list import ReferenceList
 from .resource_group import ResourceGroup
 from .resource_id import ResourceId
 from .resource_name import ResourceName
 from .resource_wrap import ResourceWrap
 from .response import Response
 from .restricted_by import RestrictedBy
 from .roman_toggle import RomanToggle
 from .rp import Rp
 from .rt import Rt
 from .sans_serif_toggle import SansSerifToggle
 from .sc_toggle import ScToggle
 from .season import Season
-from .section import Section
-from .section_title import SectionTitle
-from .sections import Sections
 from .self_uri import SelfUri
 from .series_text import SeriesText
 from .series_title import SeriesTitle
 from .sig import Sig
 from .sig_block import SigBlock
 from .state import State
 from .strike_toggle import StrikeToggle
 from .string_conf import StringConf
 from .string_name_name_style import StringNameNameStyle
 from .styled_content_toggle import StyledContentToggle
-from .sub_1 import Sub1
 from .sub_arrange import SubArrange
 from .sub_article import SubArticle
-from .suffix_1 import Suffix1
-from .sup_1 import Sup1
 from .sup_arrange import SupArrange
-from .suppl_mesh_list import SupplMeshList
-from .suppl_mesh_name import SupplMeshName
-from .suppl_mesh_name_type import SupplMeshNameType
 from .supplementary_material_orientation import SupplementaryMaterialOrientation
 from .supplementary_material_position import SupplementaryMaterialPosition
 from .support_description import SupportDescription
 from .support_group import SupportGroup
 from .support_source import SupportSource
 from .table_count import TableCount
 from .table_frame import TableFrame
@@ -479,39 +363,25 @@
 from .thead_valign import TheadValign
 from .title_group import TitleGroup
 from .tr_align import TrAlign
 from .tr_valign import TrValign
 from .trans_abstract import TransAbstract
 from .trans_subtitle import TransSubtitle
 from .trans_title_group import TransTitleGroup
-from .u import (
-    B,
-    I,
-    U,
-)
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 from .underline_toggle import UnderlineToggle
-from .url import Url
-from .url_lang import UrlLang
-from .url_type import UrlType
-from .vernacular_title import VernacularTitle
 from .volume_issue_group import VolumeIssueGroup
-from .volume_title import VolumeTitle
 from .word_count import WordCount
-from .xs_pattern import XsPattern
 from .year import Year
 
 __all__ = [
     "AbbrevJournalTitle",
-    "Abstract1",
-    "AbstractText",
-    "AbstractTextNlmCategory",
     "Abbrev",
-    "Abstract2",
+    "Abstract",
     "AccessDate",
     "Ack",
     "AddrLine",
     "Address",
     "Aff",
     "AffAlternatives",
     "AltTitle",
@@ -556,16 +426,16 @@
     "Date",
     "DateInCitation",
     "Def",
     "DefHead",
     "DefItem",
     "DefList",
     "Degrees",
+    "DispFormula",
     "DispFormulaGroup",
-    "DispFormula2",
     "DispQuote",
     "Edition",
     "ElementCitation",
     "Email",
     "Etal",
     "Explanation",
     "ExtLink",
@@ -693,110 +563,64 @@
     "VerseLine",
     "Version",
     "Volume",
     "VolumeId",
     "VolumeSeries",
     "X",
     "Xref",
-    "AccessionNumberList",
-    "Affiliation",
-    "AffiliationInfo",
     "AltText",
     "App",
     "AppGroup",
     "ArrayOrientation",
-    "Article1",
-    "Article2",
+    "Article",
     "ArticleCategories",
-    "ArticleDate",
     "ArticleDtdVersion",
     "ArticleId",
-    "ArticleId1",
-    "ArticleIdIdType",
-    "ArticleIdList",
     "ArticleMeta",
-    "ArticlePubModel",
-    "ArticleTitle1",
     "ArticleVersion",
     "ArticleVersionAlternatives",
-    "Author",
-    "AuthorEqualContrib",
-    "AuthorList",
-    "AuthorListCompleteYn",
-    "AuthorListType",
     "AuthorNotes",
-    "AuthorValidYn",
     "AwardDesc",
     "AwardGroup",
     "AwardName",
     "Back",
-    "BeginningDate",
     "Body",
     "BoldToggle",
-    "Book",
-    "BookDocument",
-    "BookDocumentSet",
-    "BookTitle",
     "BoxedTextOrientation",
     "BoxedTextPosition",
     "Break",
     "ChemStructWrapOrientation",
     "ChemStructWrapPosition",
-    "Chemical",
-    "ChemicalList",
-    "Citation",
     "City",
     "CodeExecutable",
     "CodeOrientation",
     "CodePosition",
-    "CoiStatement",
     "Col",
     "ColAlign",
     "ColValign",
     "Colgroup",
     "ColgroupAlign",
     "ColgroupValign",
-    "CollectionTitle",
-    "CollectiveName",
-    "CommentsCorrections",
-    "CommentsCorrectionsList",
-    "CommentsCorrectionsRefType",
     "ConfNum",
     "ConfTheme",
     "Conference",
     "ContribCorresp",
     "ContribDeceased",
     "ContribEqualContrib",
     "ContribId",
     "ContribIdAuthenticated",
     "ContributedResourceGroup",
-    "ContributionDate",
     "CopyrightYear",
     "Corresp",
     "Count",
     "Counts",
     "CustomMeta",
     "CustomMetaGroup",
-    "DataBank",
-    "DataBankList",
-    "DataBankListCompleteYn",
-    "DateCompleted",
-    "DateRevised",
     "Day",
-    "DeleteCitation",
-    "DeleteDocument",
-    "DescriptorName",
-    "DescriptorNameMajorTopicYn",
-    "DescriptorNameType",
-    "DispFormula1",
     "ElocationId",
-    "ElocationId1",
-    "ElocationIdEidType",
-    "ElocationIdValidYn",
-    "EndingDate",
     "EquationCount",
     "Era",
     "Event",
     "EventDesc",
     "ExtendedBy",
     "FigCount",
     "FigGroupOrientation",
@@ -805,158 +629,91 @@
     "FigPosition",
     "FloatsGroup",
     "Fpage",
     "Front",
     "FrontStub",
     "FundingGroup",
     "FundingStatement",
-    "GeneSymbolList",
-    "GeneralNote",
-    "GeneralNoteOwner",
     "GlyphData",
     "GlyphRef",
-    "Grant",
-    "GrantList",
-    "GrantListCompleteYn",
     "GraphicOrientation",
     "GraphicPosition",
-    "History1",
-    "History2",
+    "History",
     "Hr",
-    "Identifier",
     "IndexTermRangeEnd",
     "InstitutionId",
-    "Investigator",
-    "InvestigatorList",
-    "InvestigatorValidYn",
-    "Issn1",
-    "IssnIssnType",
     "IssueId",
     "IssueSponsor",
     "IssueSubtitle",
     "IssueTitleGroup",
     "ItalicToggle",
-    "ItemList",
-    "Journal",
     "JournalId",
-    "JournalIssue",
-    "JournalIssueCitedMedium",
     "JournalMeta",
     "JournalSubtitle",
     "JournalTitle",
     "JournalTitleGroup",
-    "Keyword",
-    "KeywordList",
-    "KeywordListOwner",
-    "KeywordMajorTopicYn",
-    "LocationLabel",
-    "LocationLabelType",
     "Lpage",
     "MediaOrientation",
     "MediaPosition",
-    "MedlineCitation",
-    "MedlineCitationOwner",
-    "MedlineCitationStatus",
-    "MedlineJournalInfo",
-    "MeshHeading",
-    "MeshHeadingList",
     "MetaName",
     "MetaValue",
     "MilestoneEnd",
     "MilestoneStart",
     "MonospaceToggle",
     "Month",
     "NameNameStyle",
-    "NameOfSubstance",
     "ObjectId",
-    "ObjectList",
-    "Object",
     "OptionCorrect",
-    "OtherAbstract",
-    "OtherAbstractType",
-    "OtherId",
-    "OtherIdSource",
     "OverlineEnd",
     "OverlineStart",
     "OverlineToggle",
     "PageCount",
     "PageRange",
-    "Pagination",
-    "Param",
-    "PersonalNameSubject",
-    "PersonalNameSubjectList",
-    "Pmid",
     "PostalCode",
     "PreformatOrientation",
     "PreformatPosition",
     "PrincipalAwardRecipient",
     "PrincipalInvestigator",
     "ProcessingMeta",
     "ProcessingMetaBaseTagset",
     "ProcessingMetaMathmlVersion",
     "ProcessingMetaTableModel",
     "ProcessingMetaTagsetFamily",
-    "PubDate1",
-    "PubDate2",
+    "PubDate",
     "PubDateNotAvailable",
     "PubHistory",
     "PubId",
-    "PubMedPubDate",
-    "PubMedPubDatePubStatus",
-    "PublicationType",
-    "PublicationTypeList",
-    "Publisher1",
-    "Publisher2",
-    "PublisherName1",
-    "PubmedArticle",
-    "PubmedArticleSet",
-    "PubmedBookArticle",
-    "PubmedBookArticleSet",
-    "PubmedBookData",
-    "PubmedData",
-    "QualifierName",
-    "QualifierNameMajorTopicYn",
+    "Publisher",
     "QuestionQuestionResponseType",
     "RefCount",
-    "Reference",
-    "ReferenceList",
     "ResourceGroup",
     "ResourceId",
     "ResourceName",
     "ResourceWrap",
     "Response",
     "RestrictedBy",
     "RomanToggle",
     "Rp",
     "Rt",
     "SansSerifToggle",
     "ScToggle",
     "Season",
-    "Section",
-    "SectionTitle",
-    "Sections",
     "SelfUri",
     "SeriesText",
     "SeriesTitle",
     "Sig",
     "SigBlock",
     "State",
     "StrikeToggle",
     "StringConf",
     "StringNameNameStyle",
     "StyledContentToggle",
-    "Sub1",
     "SubArrange",
     "SubArticle",
-    "Suffix1",
-    "Sup1",
     "SupArrange",
-    "SupplMeshList",
-    "SupplMeshName",
-    "SupplMeshNameType",
     "SupplementaryMaterialOrientation",
     "SupplementaryMaterialPosition",
     "SupportDescription",
     "SupportGroup",
     "SupportSource",
     "TableCount",
     "TableFrame",
@@ -981,23 +738,14 @@
     "TheadValign",
     "TitleGroup",
     "TrAlign",
     "TrValign",
     "TransAbstract",
     "TransSubtitle",
     "TransTitleGroup",
-    "B",
-    "I",
-    "U",
     "UnderlineEnd",
     "UnderlineStart",
     "UnderlineToggle",
-    "Url",
-    "UrlLang",
-    "UrlType",
-    "VernacularTitle",
     "VolumeIssueGroup",
-    "VolumeTitle",
     "WordCount",
-    "XsPattern",
     "Year",
 ]
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/abbrev_journal_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/abbrev_journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/abstract_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .abstract_text import AbstractText
 
 
 @dataclass
-class Abstract1:
-    class Meta:
-        name = "Abstract"
-
+class Abstract:
     abstract_text: List[AbstractText] = field(
         default_factory=list,
         metadata={
             "name": "AbstractText",
             "type": "Element",
             "min_occurs": 1,
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/abstract_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/abstract_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .abstract_text_nlm_category import AbstractTextNlmCategory
-from .access_date import (
-    Sub,
-    Sup,
-)
-from .disp_formula_1 import DispFormula1
+from .disp_formula import DispFormula
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
 class AbstractText:
     label: Optional[str] = field(
@@ -59,12 +57,12 @@
                 },
                 {
                     "name": "math",
                     "type": str,
                 },
                 {
                     "name": "DispFormula",
-                    "type": DispFormula1,
+                    "type": DispFormula,
                 },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/access_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/access_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 from .month import Month
 from .name_name_style import NameNameStyle
 from .object_id import ObjectId
 from .option_correct import OptionCorrect
 from .org.niso.schemas.ali.pkg_1.free_to_read import FreeToRead
 from .org.niso.schemas.ali.pkg_1.license_ref import LicenseRef
 from .org.w3.pkg_1998.math.math_ml.math import Math
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .org.w3.xml.pkg_1998.namespace.space_value import SpaceValue
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .overline_toggle import OverlineToggle
 from .page_count import PageCount
 from .page_range import PageRange
@@ -969,15 +969,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -991,31 +991,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -4133,15 +4133,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -4154,31 +4154,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -7541,15 +7541,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -7562,31 +7562,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -13454,15 +13454,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -13475,31 +13475,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -15953,15 +15953,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -15974,31 +15974,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -18507,15 +18507,15 @@
     long_desc: List["LongDesc"] = field(
         default_factory=list,
         metadata={
             "name": "long-desc",
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     email: List["Email"] = field(
         default_factory=list,
@@ -18634,15 +18634,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -18656,31 +18656,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -18714,15 +18714,15 @@
     )
     title: Optional["Title"] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -18795,15 +18795,15 @@
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
 
 
 @dataclass
-class DispFormula2:
+class DispFormula:
     """
     <div> <h3>Formula, Display</h3> </div>
     """
     class Meta:
         name = "disp-formula"
 
     content_type: Optional[str] = field(
@@ -19018,15 +19018,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "abstract",
-                    "type": Type["Abstract2"],
+                    "type": Type["Abstract"],
                 },
                 {
                     "name": "alt-text",
                     "type": AltText,
                 },
                 {
                     "name": "long-desc",
@@ -19112,15 +19112,15 @@
     )
     caption: List[Caption] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -19382,15 +19382,15 @@
     )
     caption: Optional[Caption] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -19435,15 +19435,15 @@
     )
     uri: List["Uri"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List["DispFormulaGroup"] = field(
@@ -19540,15 +19540,15 @@
     use_type: Optional[str] = field(
         default=None,
         metadata={
             "name": "use-type",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -19561,31 +19561,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -20249,15 +20249,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -20270,31 +20270,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -20342,15 +20342,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -20363,31 +20363,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -21160,15 +21160,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "break",
@@ -21541,15 +21541,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "break",
@@ -22144,15 +22144,15 @@
     )
     caption: List[Caption] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -22256,15 +22256,15 @@
     )
     code: List[Code] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     graphic: List["Graphic"] = field(
@@ -22387,15 +22387,15 @@
     )
     caption: List[Caption] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -22440,15 +22440,15 @@
     )
     uri: List["Uri"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -22619,15 +22619,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -22640,31 +22640,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -22705,15 +22705,15 @@
     )
     caption: List[Caption] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -22982,15 +22982,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -23287,15 +23287,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -23599,15 +23599,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -23930,15 +23930,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -24274,15 +24274,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -24688,15 +24688,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -25051,15 +25051,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -25382,15 +25382,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -25557,15 +25557,15 @@
     )
     caption: List[Caption] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -25610,15 +25610,15 @@
     )
     uri: List["Uri"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -26083,15 +26083,15 @@
                 },
                 {
                     "name": "table-wrap-group",
                     "type": TableWrapGroup,
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "citation-alternatives",
@@ -26202,15 +26202,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -26223,31 +26223,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -26340,15 +26340,15 @@
     long_desc: List["LongDesc"] = field(
         default_factory=list,
         metadata={
             "name": "long-desc",
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     email: List["Email"] = field(
         default_factory=list,
@@ -26467,15 +26467,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -26489,31 +26489,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -26554,15 +26554,15 @@
     )
     caption: Optional[Caption] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List["Abstract2"] = field(
+    abstract: List["Abstract"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -26881,15 +26881,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -27300,15 +27300,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -27651,15 +27651,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -27917,15 +27917,15 @@
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
 
 
 @dataclass
-class Abstract2:
+class Abstract:
     """
     <div> <h3>Abstract</h3> </div>
     """
     class Meta:
         name = "abstract"
 
     object_id: List[ObjectId] = field(
@@ -28086,15 +28086,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -28276,15 +28276,15 @@
     contrib_group: List["ContribGroup"] = field(
         default_factory=list,
         metadata={
             "name": "contrib-group",
             "type": "Element",
         }
     )
-    abstract: List[Abstract2] = field(
+    abstract: List[Abstract] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -28480,15 +28480,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -28645,15 +28645,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -28666,32 +28666,32 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title_attribute: Optional[str] = field(
         default=None,
         metadata={
             "name": "title",
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -28905,15 +28905,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -28927,31 +28927,31 @@
         default=None,
         metadata={
             "name": "role",
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -29129,15 +29129,15 @@
     )
     symbol: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -29150,31 +29150,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -30157,15 +30157,15 @@
     use_type: Optional[str] = field(
         default=None,
         metadata={
             "name": "use-type",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -30179,31 +30179,31 @@
         default=None,
         metadata={
             "name": "role",
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -30684,15 +30684,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
@@ -31165,15 +31165,15 @@
                 },
                 {
                     "name": "table-wrap-group",
                     "type": TableWrapGroup,
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "citation-alternatives",
@@ -31630,15 +31630,15 @@
                 },
                 {
                     "name": "table-wrap-group",
                     "type": TableWrapGroup,
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "def-list",
@@ -31900,15 +31900,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "array",
@@ -32189,15 +32189,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "array",
@@ -32485,15 +32485,15 @@
                 },
                 {
                     "name": "x",
                     "type": Type["X"],
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "chem-struct-wrap",
@@ -32895,15 +32895,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -32916,31 +32916,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -33260,15 +33260,15 @@
     vocab_term_identifier: Optional[str] = field(
         default=None,
         metadata={
             "name": "vocab-term-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -33281,31 +33281,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -33579,15 +33579,15 @@
                 },
                 {
                     "name": "table-wrap-group",
                     "type": TableWrapGroup,
                 },
                 {
                     "name": "disp-formula",
-                    "type": DispFormula2,
+                    "type": DispFormula,
                 },
                 {
                     "name": "disp-formula-group",
                     "type": DispFormulaGroup,
                 },
                 {
                     "name": "def-list",
@@ -33692,15 +33692,15 @@
     vocab_term_identifier: Optional[str] = field(
         default=None,
         metadata={
             "name": "vocab-term-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -33714,31 +33714,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -36748,15 +36748,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -36769,31 +36769,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -37307,15 +37307,15 @@
     )
     vol: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -37328,31 +37328,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -38200,15 +38200,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -38221,31 +38221,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -38320,15 +38320,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -38341,31 +38341,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -38611,15 +38611,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -38632,31 +38632,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -38894,15 +38894,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -38915,31 +38915,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -39170,15 +39170,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -39191,31 +39191,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
@@ -39452,15 +39452,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -39473,31 +39473,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/affiliation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/citation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class Affiliation:
+class Citation:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
@@ -37,10 +35,14 @@
                     "name": "sub",
                     "type": Sub,
                 },
                 {
                     "name": "u",
                     "type": U,
                 },
+                {
+                    "name": "math",
+                    "type": str,
+                },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/affiliation_info.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/alt_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/alt_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/app.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     AnswerSet,
     Array,
     BlockAlternatives,
     BoxedText,
     ChemStructWrap,
     Code,
     DefList,
+    DispFormula,
     DispFormulaGroup,
-    DispFormula2,
     DispQuote,
     Explanation,
     Fig,
     FigGroup,
     FnGroup,
     Glossary,
     Graphic,
@@ -210,15 +210,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/app_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/app_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
 from .access_date import (
-    Abstract2,
+    Abstract,
     Ack,
     Address,
     Alternatives,
     Answer,
     AnswerSet,
     Array,
     BlockAlternatives,
     BoxedText,
     ChemStructWrap,
     Code,
     DefList,
+    DispFormula,
     DispFormulaGroup,
-    DispFormula2,
     DispQuote,
     Explanation,
     Fig,
     FigGroup,
     Graphic,
     KwdGroup,
     Label,
@@ -73,15 +73,15 @@
     )
     title: Optional[Title] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    abstract: List[Abstract2] = field(
+    abstract: List[Abstract] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     kwd_group: List[KwdGroup] = field(
         default_factory=list,
@@ -229,15 +229,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .abstract_1 import Abstract1
+from .abstract import Abstract
 from .article_date import ArticleDate
 from .article_pub_model import ArticlePubModel
-from .article_title_1 import ArticleTitle1
+from .article_title import ArticleTitle
 from .author_list import AuthorList
 from .data_bank_list import DataBankList
-from .elocation_id_1 import ElocationId1
+from .elocation_id import ElocationId
 from .grant_list import GrantList
 from .journal import Journal
 from .pagination import Pagination
 from .publication_type_list import PublicationTypeList
 from .vernacular_title import VernacularTitle
 
 
 @dataclass
-class Article1:
-    class Meta:
-        name = "Article"
-
+class Article:
     pub_model: Optional[ArticlePubModel] = field(
         default=None,
         metadata={
             "name": "PubModel",
             "type": "Attribute",
             "required": True,
         }
@@ -32,38 +29,38 @@
         default=None,
         metadata={
             "name": "Journal",
             "type": "Element",
             "required": True,
         }
     )
-    article_title: Optional[ArticleTitle1] = field(
+    article_title: Optional[ArticleTitle] = field(
         default=None,
         metadata={
             "name": "ArticleTitle",
             "type": "Element",
             "required": True,
         }
     )
     pagination: Optional[Pagination] = field(
         default=None,
         metadata={
             "name": "Pagination",
             "type": "Element",
         }
     )
-    elocation_id: List[ElocationId1] = field(
+    elocation_id: List[ElocationId] = field(
         default_factory=list,
         metadata={
             "name": "ELocationID",
             "type": "Element",
             "max_occurs": 2,
         }
     )
-    abstract: Optional[Abstract1] = field(
+    abstract: Optional[Abstract] = field(
         default=None,
         metadata={
             "name": "Abstract",
             "type": "Element",
         }
     )
     author_list: Optional[AuthorList] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_2.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .processing_meta import ProcessingMeta
 from .response import Response
 from .sub_article import SubArticle
 
 
 @dataclass
-class Article2:
+class Article:
     """
     <div> <h3>Article</h3> </div>
     """
     class Meta:
         name = "article"
 
     processing_meta: Optional[ProcessingMeta] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_categories.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_categories.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .access_date import (
-    Abstract2,
+    Abstract,
     Aff,
     AffAlternatives,
     ContribGroup,
     Email,
     ExtLink,
     Isbn,
     Issue,
@@ -32,21 +32,21 @@
 from .author_notes import AuthorNotes
 from .conference import Conference
 from .counts import Counts
 from .custom_meta_group import CustomMetaGroup
 from .elocation_id import ElocationId
 from .fpage import Fpage
 from .funding_group import FundingGroup
-from .history_2 import History2
+from .history import History
 from .issue_id import IssueId
 from .issue_sponsor import IssueSponsor
 from .issue_title_group import IssueTitleGroup
 from .lpage import Lpage
 from .page_range import PageRange
-from .pub_date_2 import PubDate2
+from .pub_date import PubDate
 from .pub_date_not_available import PubDateNotAvailable
 from .pub_history import PubHistory
 from .self_uri import SelfUri
 from .support_group import SupportGroup
 from .title_group import TitleGroup
 from .trans_abstract import TransAbstract
 from .volume_issue_group import VolumeIssueGroup
@@ -124,15 +124,15 @@
     author_notes: Optional[AuthorNotes] = field(
         default=None,
         metadata={
             "name": "author-notes",
             "type": "Element",
         }
     )
-    pub_date: List[PubDate2] = field(
+    pub_date: List[PubDate] = field(
         default_factory=list,
         metadata={
             "name": "pub-date",
             "type": "Element",
         }
     )
     pub_date_not_available: Optional[PubDateNotAvailable] = field(
@@ -276,15 +276,15 @@
     supplementary_material: List[SupplementaryMaterial] = field(
         default_factory=list,
         metadata={
             "name": "supplementary-material",
             "type": "Element",
         }
     )
-    history: Optional[History2] = field(
+    history: Optional[History] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     pub_history: Optional[PubHistory] = field(
         default=None,
@@ -316,15 +316,15 @@
     related_object: List[RelatedObject] = field(
         default_factory=list,
         metadata={
             "name": "related-object",
             "type": "Element",
         }
     )
-    abstract: List[Abstract2] = field(
+    abstract: List[Abstract] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     trans_abstract: List[TransAbstract] = field(
         default_factory=list,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_title_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/article_title.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class ArticleTitle1:
-    class Meta:
-        name = "ArticleTitle"
-
+class ArticleTitle:
     book: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     sec: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_version.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 
 
 @dataclass
 class ArticleVersion:
     """
     <div> <h3>Article Version</h3> </div>
     """
@@ -90,15 +90,15 @@
     vocab_term_identifier: Optional[str] = field(
         default=None,
         metadata={
             "name": "vocab-term-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -111,31 +111,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/article_version_alternatives.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/article_version_alternatives.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/author.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .affiliation_info import AffiliationInfo
 from .author_equal_contrib import AuthorEqualContrib
 from .author_valid_yn import AuthorValidYn
 from .collective_name import CollectiveName
 from .identifier import Identifier
-from .suffix_1 import Suffix1
+from .suffix import Suffix
 
 
 @dataclass
 class Author:
     valid_yn: AuthorValidYn = field(
         default=AuthorValidYn.Y,
         metadata={
@@ -43,15 +43,15 @@
     initials: Optional[str] = field(
         default=None,
         metadata={
             "name": "Initials",
             "type": "Element",
         }
     )
-    suffix: Optional[Suffix1] = field(
+    suffix: Optional[Suffix] = field(
         default=None,
         metadata={
             "name": "Suffix",
             "type": "Element",
         }
     )
     collective_name: Optional[CollectiveName] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/author_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/author_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/author_notes.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/author_notes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/award_desc.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class AwardDesc:
+class AwardName:
     """
-    <div> <h3>Award Description</h3> </div>
+    <div> <h3>Award Name</h3> </div>
     """
     class Meta:
-        name = "award-desc"
+        name = "award-name"
 
     hreflang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -44,31 +44,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/award_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List, Optional, Union
 from .access_date import (
     AwardId,
     FundingSource,
 )
 from .award_desc import AwardDesc
 from .award_name import AwardName
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .principal_award_recipient import PrincipalAwardRecipient
 from .principal_investigator import PrincipalInvestigator
 from .support_source import SupportSource
 
 
 @dataclass
@@ -102,15 +102,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -123,31 +123,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/award_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,65 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class AwardName:
+class IssueId:
     """
-    <div> <h3>Award Name</h3> </div>
+    <div> <h3>Issue Identifier</h3> </div>
     """
     class Meta:
-        name = "award-name"
+        name = "issue-id"
 
+    assigning_authority: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "assigning-authority",
+            "type": "Attribute",
+        }
+    )
+    content_type: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "content-type",
+            "type": "Attribute",
+        }
+    )
     hreflang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    pub_id_type: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "pub-id-type",
+            "type": "Attribute",
+        }
+    )
+    specific_use: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "specific-use",
+            "type": "Attribute",
+        }
+    )
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -44,31 +72,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/back.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/back.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/beginning_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/beginning_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/body.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/body.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     AnswerSet,
     Array,
     BlockAlternatives,
     BoxedText,
     ChemStructWrap,
     Code,
     DefList,
+    DispFormula,
     DispFormulaGroup,
-    DispFormula2,
     DispQuote,
     Explanation,
     Fig,
     FigGroup,
     Graphic,
     ListType,
     Media,
@@ -183,15 +183,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/book.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .author_list import AuthorList
 from .beginning_date import BeginningDate
 from .book_title import BookTitle
 from .collection_title import CollectionTitle
-from .elocation_id_1 import ElocationId1
+from .elocation_id import ElocationId
 from .ending_date import EndingDate
 from .investigator_list import InvestigatorList
-from .pub_date_1 import PubDate1
-from .publisher_1 import Publisher1
+from .pub_date import PubDate
+from .publisher import Publisher
 from .volume_title import VolumeTitle
 
 
 @dataclass
 class Book:
-    publisher: Optional[Publisher1] = field(
+    publisher: Optional[Publisher] = field(
         default=None,
         metadata={
             "name": "Publisher",
             "type": "Element",
             "required": True,
         }
     )
@@ -27,15 +27,15 @@
         default=None,
         metadata={
             "name": "BookTitle",
             "type": "Element",
             "required": True,
         }
     )
-    pub_date: Optional[PubDate1] = field(
+    pub_date: Optional[PubDate] = field(
         default=None,
         metadata={
             "name": "PubDate",
             "type": "Element",
             "required": True,
         }
     )
@@ -98,15 +98,15 @@
     isbn: List[str] = field(
         default_factory=list,
         metadata={
             "name": "Isbn",
             "type": "Element",
         }
     )
-    elocation_id: List[ElocationId1] = field(
+    elocation_id: List[ElocationId] = field(
         default_factory=list,
         metadata={
             "name": "ELocationID",
             "type": "Element",
         }
     )
     medium: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/book_document.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .abstract_1 import Abstract1
+from .abstract import Abstract
 from .article_id_list import ArticleIdList
-from .article_title_1 import ArticleTitle1
+from .article_title import ArticleTitle
 from .author_list import AuthorList
 from .book import Book
 from .contribution_date import ContributionDate
 from .date_revised import DateRevised
 from .grant_list import GrantList
 from .investigator_list import InvestigatorList
 from .item_list import ItemList
@@ -50,15 +50,15 @@
     location_label: List[LocationLabel] = field(
         default_factory=list,
         metadata={
             "name": "LocationLabel",
             "type": "Element",
         }
     )
-    article_title: Optional[ArticleTitle1] = field(
+    article_title: Optional[ArticleTitle] = field(
         default=None,
         metadata={
             "name": "ArticleTitle",
             "type": "Element",
         }
     )
     vernacular_title: Optional[VernacularTitle] = field(
@@ -99,15 +99,15 @@
     publication_type: List[PublicationType] = field(
         default_factory=list,
         metadata={
             "name": "PublicationType",
             "type": "Element",
         }
     )
-    abstract: Optional[Abstract1] = field(
+    abstract: Optional[Abstract] = field(
         default=None,
         metadata={
             "name": "Abstract",
             "type": "Element",
         }
     )
     sections: Optional[Sections] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/book_document_set.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_document_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/book_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section_title.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class BookTitle:
+class SectionTitle:
     book: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     sec: Optional[str] = field(
@@ -55,14 +53,10 @@
                     "name": "sub",
                     "type": Sub,
                 },
                 {
                     "name": "u",
                     "type": U,
                 },
-                {
-                    "name": "math",
-                    "type": str,
-                },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/break_mod.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/break_mod.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/chemical.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/chemical.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/citation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/affiliation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class Citation:
+class Affiliation:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
@@ -37,14 +35,10 @@
                     "name": "sub",
                     "type": Sub,
                 },
                 {
                     "name": "u",
                     "type": U,
                 },
-                {
-                    "name": "math",
-                    "type": str,
-                },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/city.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/city.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/coi_statement.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/vernacular_title.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class CoiStatement:
+class VernacularTitle:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
@@ -37,10 +35,14 @@
                     "name": "sub",
                     "type": Sub,
                 },
                 {
                     "name": "u",
                     "type": U,
                 },
+                {
+                    "name": "math",
+                    "type": str,
+                },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/col.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/col.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/colgroup.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/colgroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/collection_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/book_title.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class CollectionTitle:
+class BookTitle:
     book: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     sec: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/collective_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/volume_title.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class CollectiveName:
+class VolumeTitle:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/comments_corrections_ref_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/comments_corrections_ref_type.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/conf_num.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_num.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/conf_theme.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conf_theme.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/conference.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/conference.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     ConfLoc,
     ConfName,
     ConfSponsor,
     X,
 )
 from .conf_num import ConfNum
 from .conf_theme import ConfTheme
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .string_conf import StringConf
 
 
 @dataclass
 class Conference:
     """
@@ -110,15 +110,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -131,31 +131,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/contrib_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contrib_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/contributed_resource_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/contributed_resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/contribution_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/contribution_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/copyright_year.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/copyright_year.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/corresp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/corresp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/counts.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/counts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/custom_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional, Union
 from .meta_name import MetaName
 from .meta_value import MetaValue
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
 class CustomMeta:
     """
     <div> <h3>Custom Metadata</h3> </div>
@@ -82,15 +82,15 @@
     vocab_term_identifier: Optional[str] = field(
         default=None,
         metadata={
             "name": "vocab-term-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -103,31 +103,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/custom_meta_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/custom_meta_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/data_bank.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/data_bank_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/data_bank_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/date_completed.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_completed.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/date_revised.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/date_revised.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/day.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/day.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/descriptor_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/descriptor_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/elocation_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/elocation_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/elocation_id_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/elocation_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pydantic.dataclasses import dataclass
 from typing import Optional
 from .elocation_id_eid_type import ElocationIdEidType
 from .elocation_id_valid_yn import ElocationIdValidYn
 
 
 @dataclass
-class ElocationId1:
+class ElocationId:
     class Meta:
         name = "ELocationID"
 
     eid_type: Optional[ElocationIdEidType] = field(
         default=None,
         metadata={
             "name": "EIdType",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/ending_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/ending_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/equation_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/equation_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/era.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/era.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/event.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     StringDate,
 )
 from .article_id import ArticleId
 from .article_version import ArticleVersion
 from .article_version_alternatives import ArticleVersionAlternatives
 from .event_desc import EventDesc
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
-from .pub_date_2 import PubDate2
+from .pub_date import PubDate
 from .pub_date_not_available import PubDateNotAvailable
 from .self_uri import SelfUri
 
 
 @dataclass
 class Event:
     """
@@ -52,15 +52,15 @@
     article_version_alternatives: Optional[ArticleVersionAlternatives] = field(
         default=None,
         metadata={
             "name": "article-version-alternatives",
             "type": "Element",
         }
     )
-    pub_date: List[PubDate2] = field(
+    pub_date: List[PubDate] = field(
         default_factory=list,
         metadata={
             "name": "pub-date",
             "type": "Element",
         }
     )
     pub_date_not_available: Optional[PubDateNotAvailable] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/event_desc.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/event_desc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     StringDate,
     Uri,
 )
 from .article_id import ArticleId
 from .article_version import ArticleVersion
 from .article_version_alternatives import ArticleVersionAlternatives
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
-from .pub_date_2 import PubDate2
+from .pub_date import PubDate
 from .pub_date_not_available import PubDateNotAvailable
 
 
 @dataclass
 class EventDesc:
     """
     <div> <h3>Event Description</h3> </div>
@@ -103,15 +103,15 @@
                 },
                 {
                     "name": "string-date",
                     "type": StringDate,
                 },
                 {
                     "name": "pub-date",
-                    "type": PubDate2,
+                    "type": PubDate,
                 },
                 {
                     "name": "pub-date-not-available",
                     "type": PubDateNotAvailable,
                 },
             ),
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/extended_by.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/extended_by.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 
 
 @dataclass
 class ExtendedBy:
     """
     <div> <h3>Extended-by Model</h3> </div>
     """
@@ -62,15 +62,15 @@
     vocab_term_identifier: Optional[str] = field(
         default=None,
         metadata={
             "name": "vocab-term-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -83,31 +83,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/fig_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fig_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/floats_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/floats_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/fpage.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/fpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/front.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/front_stub.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/front_stub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .access_date import (
-    Abstract2,
+    Abstract,
     Aff,
     AffAlternatives,
     ContribGroup,
     Email,
     ExtLink,
     Isbn,
     Issue,
@@ -32,21 +32,21 @@
 from .author_notes import AuthorNotes
 from .conference import Conference
 from .counts import Counts
 from .custom_meta_group import CustomMetaGroup
 from .elocation_id import ElocationId
 from .fpage import Fpage
 from .funding_group import FundingGroup
-from .history_2 import History2
+from .history import History
 from .issue_id import IssueId
 from .issue_sponsor import IssueSponsor
 from .issue_title_group import IssueTitleGroup
 from .lpage import Lpage
 from .page_range import PageRange
-from .pub_date_2 import PubDate2
+from .pub_date import PubDate
 from .pub_date_not_available import PubDateNotAvailable
 from .pub_history import PubHistory
 from .self_uri import SelfUri
 from .support_group import SupportGroup
 from .title_group import TitleGroup
 from .trans_abstract import TransAbstract
 from .volume_issue_group import VolumeIssueGroup
@@ -124,15 +124,15 @@
     author_notes: Optional[AuthorNotes] = field(
         default=None,
         metadata={
             "name": "author-notes",
             "type": "Element",
         }
     )
-    pub_date: List[PubDate2] = field(
+    pub_date: List[PubDate] = field(
         default_factory=list,
         metadata={
             "name": "pub-date",
             "type": "Element",
         }
     )
     pub_date_not_available: Optional[PubDateNotAvailable] = field(
@@ -276,15 +276,15 @@
     supplementary_material: List[SupplementaryMaterial] = field(
         default_factory=list,
         metadata={
             "name": "supplementary-material",
             "type": "Element",
         }
     )
-    history: Optional[History2] = field(
+    history: Optional[History] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     pub_history: Optional[PubHistory] = field(
         default=None,
@@ -316,15 +316,15 @@
     related_object: List[RelatedObject] = field(
         default_factory=list,
         metadata={
             "name": "related-object",
             "type": "Element",
         }
     )
-    abstract: List[Abstract2] = field(
+    abstract: List[Abstract] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     trans_abstract: List[TransAbstract] = field(
         default_factory=list,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/funding_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/funding_statement.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/funding_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     Xref,
 )
 from .hr import Hr
 from .index_term_range_end import IndexTermRangeEnd
 from .milestone_end import MilestoneEnd
 from .milestone_start import MilestoneStart
 from .org.w3.pkg_1998.math.math_ml.math import Math
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .tex_math import TexMath
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 
@@ -85,15 +85,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -106,31 +106,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/glyph_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_data.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/glyph_ref.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/glyph_ref.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/grant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/grant_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/grant_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/personal_name_subject.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional
-from .individual_name import IndividualName
+from typing import Optional
+from .suffix import Suffix
 
 
 @dataclass
-class Group:
-    group_name: Optional[str] = field(
+class PersonalNameSubject:
+    last_name: Optional[str] = field(
         default=None,
         metadata={
-            "name": "GroupName",
+            "name": "LastName",
             "type": "Element",
+            "required": True,
         }
     )
-    individual_name: List[IndividualName] = field(
-        default_factory=list,
+    fore_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "ForeName",
+            "type": "Element",
+        }
+    )
+    initials: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "Initials",
+            "type": "Element",
+        }
+    )
+    suffix: Optional[Suffix] = field(
+        default=None,
         metadata={
-            "name": "IndividualName",
+            "name": "Suffix",
             "type": "Element",
-            "min_occurs": 1,
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/history_2.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from .overline_start import OverlineStart
 from .tex_math import TexMath
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 
 
 @dataclass
-class History2:
+class History:
     """<div>
     <h3>History: Document History</h3>
     </div>"""
     class Meta:
         name = "history"
 
     id: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/hr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/hr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/i.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/u.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,171 +1,188 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Type
-from .access_date import (
-    Sub,
-    Sup,
-)
 
 
 @dataclass
-class I:
+class U:
     class Meta:
-        name = "i"
+        name = "u"
 
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
                 {
-                    "name": "sup",
-                    "type": Sup,
-                },
-                {
-                    "name": "inf",
-                    "type": Type["Inf"],
-                },
-                {
                     "name": "b",
                     "type": Type["B"],
                 },
                 {
-                    "name": "u",
-                    "type": Type["U"],
-                },
-                {
                     "name": "i",
                     "type": Type["I"],
                 },
                 {
+                    "name": "sup",
+                    "type": Type["Sup"],
+                },
+                {
                     "name": "sub",
-                    "type": Sub,
+                    "type": Type["Sub"],
+                },
+                {
+                    "name": "u",
+                    "type": Type["U"],
                 },
             ),
         }
     )
 
 
 @dataclass
-class U:
+class Sub:
     class Meta:
-        name = "u"
+        name = "sub"
 
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
                 {
-                    "name": "sup",
-                    "type": Sup,
-                },
-                {
-                    "name": "inf",
-                    "type": Type["Inf"],
-                },
-                {
                     "name": "b",
                     "type": Type["B"],
                 },
                 {
-                    "name": "u",
-                    "type": Type["U"],
+                    "name": "i",
+                    "type": Type["I"],
                 },
                 {
-                    "name": "i",
-                    "type": I,
+                    "name": "sup",
+                    "type": Type["Sup"],
                 },
                 {
                     "name": "sub",
-                    "type": Sub,
+                    "type": Type["Sub"],
+                },
+                {
+                    "name": "u",
+                    "type": U,
                 },
             ),
         }
     )
 
 
 @dataclass
-class B:
+class Sup:
     class Meta:
-        name = "b"
+        name = "sup"
 
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
                 {
-                    "name": "sup",
-                    "type": Sup,
-                },
-                {
-                    "name": "inf",
-                    "type": Type["Inf"],
-                },
-                {
                     "name": "b",
                     "type": Type["B"],
                 },
                 {
-                    "name": "u",
-                    "type": U,
+                    "name": "i",
+                    "type": Type["I"],
                 },
                 {
-                    "name": "i",
-                    "type": I,
+                    "name": "sup",
+                    "type": Type["Sup"],
                 },
                 {
                     "name": "sub",
                     "type": Sub,
                 },
+                {
+                    "name": "u",
+                    "type": U,
+                },
             ),
         }
     )
 
 
 @dataclass
-class Inf:
+class I:
     class Meta:
-        name = "inf"
+        name = "i"
 
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
                 {
-                    "name": "sup",
-                    "type": Sup,
+                    "name": "b",
+                    "type": Type["B"],
                 },
                 {
-                    "name": "inf",
-                    "type": Type["Inf"],
+                    "name": "i",
+                    "type": Type["I"],
                 },
                 {
-                    "name": "b",
-                    "type": B,
+                    "name": "sup",
+                    "type": Sup,
+                },
+                {
+                    "name": "sub",
+                    "type": Sub,
                 },
                 {
                     "name": "u",
                     "type": U,
                 },
+            ),
+        }
+    )
+
+
+@dataclass
+class B:
+    class Meta:
+        name = "b"
+
+    content: List[object] = field(
+        default_factory=list,
+        metadata={
+            "type": "Wildcard",
+            "namespace": "##any",
+            "mixed": True,
+            "choices": (
+                {
+                    "name": "b",
+                    "type": Type["B"],
+                },
                 {
                     "name": "i",
                     "type": I,
                 },
                 {
+                    "name": "sup",
+                    "type": Sup,
+                },
+                {
                     "name": "sub",
                     "type": Sub,
                 },
+                {
+                    "name": "u",
+                    "type": U,
+                },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/index_term_range_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/index_term_range_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/individual_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/investigator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .affiliation_info import AffiliationInfo
-from .first_name import FirstName
 from .identifier import Identifier
+from .investigator_valid_yn import InvestigatorValidYn
+from .suffix import Suffix
 
 
 @dataclass
-class IndividualName:
-    first_name: Optional[FirstName] = field(
-        default=None,
+class Investigator:
+    valid_yn: InvestigatorValidYn = field(
+        default=InvestigatorValidYn.Y,
         metadata={
-            "name": "FirstName",
-            "type": "Element",
+            "name": "ValidYN",
+            "type": "Attribute",
             "required": True,
         }
     )
-    middle_name: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "MiddleName",
-            "type": "Element",
-        }
-    )
     last_name: Optional[str] = field(
         default=None,
         metadata={
             "name": "LastName",
             "type": "Element",
             "required": True,
         }
     )
-    suffix: Optional[str] = field(
+    fore_name: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Suffix",
+            "name": "ForeName",
             "type": "Element",
         }
     )
-    affiliation: Optional[str] = field(
+    initials: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Affiliation",
+            "name": "Initials",
             "type": "Element",
         }
     )
-    affiliation_info: Optional[AffiliationInfo] = field(
+    suffix: Optional[Suffix] = field(
         default=None,
         metadata={
-            "name": "AffiliationInfo",
+            "name": "Suffix",
             "type": "Element",
         }
     )
     identifier: List[Identifier] = field(
         default_factory=list,
         metadata={
             "name": "Identifier",
             "type": "Element",
         }
     )
+    affiliation_info: List[AffiliationInfo] = field(
+        default_factory=list,
+        metadata={
+            "name": "AffiliationInfo",
+            "type": "Element",
+        }
+    )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/institution_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/institution_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/investigator.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/license_ref.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .affiliation_info import AffiliationInfo
-from .identifier import Identifier
-from .investigator_valid_yn import InvestigatorValidYn
-from .suffix_1 import Suffix1
+
+__NAMESPACE__ = "http://www.niso.org/schemas/ali/1.0/"
 
 
 @dataclass
-class Investigator:
-    valid_yn: InvestigatorValidYn = field(
-        default=InvestigatorValidYn.Y,
+class LicenseRef:
+    """
+    <div> <h3>License Reference (Niso Ali)</h3> </div>
+    """
+    class Meta:
+        name = "license_ref"
+        namespace = "http://www.niso.org/schemas/ali/1.0/"
+
+    content_type: Optional[str] = field(
+        default=None,
         metadata={
-            "name": "ValidYN",
+            "name": "content-type",
             "type": "Attribute",
-            "required": True,
         }
     )
-    last_name: Optional[str] = field(
+    id: Optional[str] = field(
         default=None,
         metadata={
-            "name": "LastName",
-            "type": "Element",
-            "required": True,
+            "type": "Attribute",
         }
     )
-    fore_name: Optional[str] = field(
+    specific_use: Optional[str] = field(
         default=None,
         metadata={
-            "name": "ForeName",
-            "type": "Element",
+            "name": "specific-use",
+            "type": "Attribute",
         }
     )
-    initials: Optional[str] = field(
+    start_date: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Initials",
-            "type": "Element",
+            "type": "Attribute",
         }
     )
-    suffix: Optional[Suffix1] = field(
+    base: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Suffix",
-            "type": "Element",
-        }
-    )
-    identifier: List[Identifier] = field(
-        default_factory=list,
-        metadata={
-            "name": "Identifier",
-            "type": "Element",
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
-    affiliation_info: List[AffiliationInfo] = field(
+    content: List[object] = field(
         default_factory=list,
         metadata={
-            "name": "AffiliationInfo",
-            "type": "Element",
+            "type": "Wildcard",
+            "namespace": "##any",
+            "mixed": True,
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/issn_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/issn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 from .issn_issn_type import IssnIssnType
 
 
 @dataclass
-class Issn1:
+class Issn:
     class Meta:
         name = "ISSN"
 
     issn_type: Optional[IssnIssnType] = field(
         default=None,
         metadata={
             "name": "IssnType",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/issue_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional, Union
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
-from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
+from typing import List, Optional
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 
 
 @dataclass
-class IssueId:
+class PubId:
     """
-    <div> <h3>Issue Identifier</h3> </div>
+    <div> <h3>Publication Identifier For a Cited Publication</h3> </div>
     """
     class Meta:
-        name = "issue-id"
+        name = "pub-id"
 
     assigning_authority: Optional[str] = field(
         default=None,
         metadata={
             "name": "assigning-authority",
             "type": "Attribute",
         }
     )
-    content_type: Optional[str] = field(
+    custom_type: Optional[str] = field(
         default=None,
         metadata={
-            "name": "content-type",
+            "name": "custom-type",
             "type": "Attribute",
         }
     )
     hreflang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -51,15 +50,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -72,50 +71,43 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
-    lang: Optional[Union[str, LangValue]] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "namespace": "http://www.w3.org/XML/1998/namespace",
-        }
-    )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/issue_sponsor.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_sponsor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/issue_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/issue_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/issue_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .issn_1 import Issn1
+from .issn import Issn
 from .journal_issue import JournalIssue
 
 
 @dataclass
 class Journal:
-    issn: Optional[Issn1] = field(
+    issn: Optional[Issn] = field(
         default=None,
         metadata={
             "name": "ISSN",
             "type": "Element",
         }
     )
     journal_issue: Optional[JournalIssue] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_issue.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/journal_issue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 from .journal_issue_cited_medium import JournalIssueCitedMedium
-from .pub_date_1 import PubDate1
+from .pub_date import PubDate
 
 
 @dataclass
 class JournalIssue:
     cited_medium: Optional[JournalIssueCitedMedium] = field(
         default=None,
         metadata={
@@ -25,15 +25,15 @@
     issue: Optional[str] = field(
         default=None,
         metadata={
             "name": "Issue",
             "type": "Element",
         }
     )
-    pub_date: Optional[PubDate1] = field(
+    pub_date: Optional[PubDate] = field(
         default=None,
         metadata={
             "name": "PubDate",
             "type": "Element",
             "required": True,
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Issn,
     IssnL,
     Notes,
 )
 from .custom_meta_group import CustomMetaGroup
 from .journal_id import JournalId
 from .journal_title_group import JournalTitleGroup
-from .publisher_2 import Publisher2
+from .publisher import Publisher
 from .self_uri import SelfUri
 
 
 @dataclass
 class JournalMeta:
     """
     <div> <h3>Journal Metadata</h3> </div>
@@ -74,15 +74,15 @@
     )
     isbn: List[Isbn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    publisher: Optional[Publisher2] = field(
+    publisher: Optional[Publisher] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     notes: List[Notes] = field(
         default_factory=list,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/journal_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/journal_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/keyword.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .keyword_major_topic_yn import KeywordMajorTopicYn
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
 class Keyword:
     major_topic_yn: KeywordMajorTopicYn = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/keyword_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/keyword_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/lpage.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/lpage.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/medline_citation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_citation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .article_1 import Article1
+from .article import Article
 from .chemical_list import ChemicalList
 from .coi_statement import CoiStatement
 from .comments_corrections_list import CommentsCorrectionsList
 from .date_completed import DateCompleted
 from .date_revised import DateRevised
 from .gene_symbol_list import GeneSymbolList
 from .general_note import GeneralNote
@@ -79,15 +79,15 @@
     date_revised: Optional[DateRevised] = field(
         default=None,
         metadata={
             "name": "DateRevised",
             "type": "Element",
         }
     )
-    article: Optional[Article1] = field(
+    article: Optional[Article] = field(
         default=None,
         metadata={
             "name": "Article",
             "type": "Element",
             "required": True,
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/medline_journal_info.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/medline_journal_info.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/mesh_heading.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/mesh_heading.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/meta_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/meta_value.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/meta_value.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/milestone_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/milestone_start.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/milestone_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/month.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/month.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/object_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/object_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/niso/schemas/ali/pkg_1/free_to_read.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from xsdata.models.datatype import XmlDate
-
-__NAMESPACE__ = "http://www.niso.org/schemas/ali/1.0/"
+from .medline_citation import MedlineCitation
+from .pubmed_data import PubmedData
 
 
 @dataclass
-class FreeToRead:
-    class Meta:
-        name = "free_to_read"
-        namespace = "http://www.niso.org/schemas/ali/1.0/"
-
-    end_date: Optional[XmlDate] = field(
+class PubmedArticle:
+    medline_citation: Optional[MedlineCitation] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "name": "MedlineCitation",
+            "type": "Element",
+            "required": True,
         }
     )
-    start_date: Optional[XmlDate] = field(
+    pubmed_data: Optional[PubmedData] = field(
         default=None,
         metadata={
-            "type": "Attribute",
-            "required": True,
+            "name": "PubmedData",
+            "type": "Element",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/__init__.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .abs import Abs
 from .and_mod import And
 from .annotation import Annotation
+from .annotation_xml import AnnotationXml
+from .annotation_xml_model import AnnotationXmlModel
 from .approx import Approx
 from .arccos import Arccos
 from .arccosh import Arccosh
 from .arccot import Arccot
 from .arccoth import Arccoth
 from .arccsc import Arccsc
 from .arccsch import Arccsch
@@ -21,16 +23,14 @@
 from .ceiling import Ceiling
 from .codomain import Codomain
 from .columnalignstyle import Columnalignstyle
 from .complexes import Complexes
 from .compose import Compose
 from .condition import (
     ImpliedMrow,
-    AnnotationXml,
-    AnnotationXmlModel,
     Apply,
     ApplyContent,
     Bind,
     BindContent,
     Bvar,
     Cerror,
     Ci,
@@ -254,14 +254,17 @@
 from .msgroup_value import MsgroupValue
 from .msline import Msline
 from .msline_value import MslineValue
 from .mspace import Mspace
 from .mspace_dir import MspaceDir
 from .mspace_fontstyle import MspaceFontstyle
 from .mspace_fontweight import MspaceFontweight
+from .mspace_indentalign import MspaceIndentalign
+from .mspace_indentalignfirst import MspaceIndentalignfirst
+from .mspace_indentalignlast import MspaceIndentalignlast
 from .mspace_linebreak import MspaceLinebreak
 from .mspace_mathvariant import MspaceMathvariant
 from .mspace_value import MspaceValue
 from .msqrt_value import MsqrtValue
 from .msrow_value import MsrowValue
 from .mstack_charalign import MstackCharalign
 from .mstack_stackalign import MstackStackalign
@@ -374,14 +377,16 @@
 from .verticalalign import Verticalalign
 from .xor import Xor
 
 __all__ = [
     "Abs",
     "And",
     "Annotation",
+    "AnnotationXml",
+    "AnnotationXmlModel",
     "Approx",
     "Arccos",
     "Arccosh",
     "Arccot",
     "Arccoth",
     "Arccsc",
     "Arccsch",
@@ -397,16 +402,14 @@
     "Cbytes",
     "Ceiling",
     "Codomain",
     "Columnalignstyle",
     "Complexes",
     "Compose",
     "ImpliedMrow",
-    "AnnotationXml",
-    "AnnotationXmlModel",
     "Apply",
     "ApplyContent",
     "Bind",
     "BindContent",
     "Bvar",
     "Cerror",
     "Ci",
@@ -629,14 +632,17 @@
     "MsgroupValue",
     "Msline",
     "MslineValue",
     "Mspace",
     "MspaceDir",
     "MspaceFontstyle",
     "MspaceFontweight",
+    "MspaceIndentalign",
+    "MspaceIndentalignfirst",
+    "MspaceIndentalignlast",
     "MspaceLinebreak",
     "MspaceMathvariant",
     "MspaceValue",
     "MsqrtValue",
     "MsrowValue",
     "MstackCharalign",
     "MstackStackalign",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/abs.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/abs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/annotation.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/approx.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/approx.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/arg.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/arg.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cbytes.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cbytes.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ceiling.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ceiling.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/condition.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import field
 from decimal import Decimal
 from pydantic.dataclasses import dataclass
 from typing import Dict, List, Optional, Type, Union
 from .abs import Abs
 from .and_mod import And
 from .annotation import Annotation
+from .annotation_xml import AnnotationXml
 from .approx import Approx
 from .arccos import Arccos
 from .arccosh import Arccosh
 from .arccot import Arccot
 from .arccoth import Arccoth
 from .arccsc import Arccsc
 from .arccsch import Arccsch
@@ -6310,17 +6311,17 @@
         metadata={
             "type": "Element",
         }
     )
 
 
 @dataclass
-class Mrow:
+class Reln:
     class Meta:
-        name = "mrow"
+        name = "reln"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
@@ -7150,1366 +7151,1032 @@
     )
     exponentiale: List[Exponentiale] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    maction: List["Maction"] = field(
+
+
+@dataclass
+class Bvar:
+    class Meta:
+        name = "bvar"
+        namespace = "http://www.w3.org/1998/Math/MathML"
+
+    ci: List["Ci"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    mlongdiv: List["Mlongdiv"] = field(
+    semantics: List["Bvar.Semantics"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    mstack: List["Mstack"] = field(
+    degree: List[Degree] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    mtable: List["Mtable"] = field(
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    xref: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    class_value: List[str] = field(
         default_factory=list,
         metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+
+    @dataclass
+    class Semantics:
+        ci: Optional["Ci"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        semantics: Optional["Bvar.Semantics"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        annotation: List[Annotation] = field(
+            default_factory=list,
+            metadata={
+                "type": "Element",
+            }
+        )
+        annotation_xml: List[AnnotationXml] = field(
+            default_factory=list,
+            metadata={
+                "name": "annotation-xml",
+                "type": "Element",
+            }
+        )
+        id: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        xref: Optional[object] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        class_value: List[str] = field(
+            default_factory=list,
+            metadata={
+                "name": "class",
+                "type": "Attribute",
+                "tokens": True,
+            }
+        )
+        style: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        href: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        other: Optional[object] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        other_attributes: Dict[str, str] = field(
+            default_factory=dict,
+            metadata={
+                "type": "Attributes",
+                "namespace": "##other",
+            }
+        )
+        encoding: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        definition_url: Optional[str] = field(
+            default=None,
+            metadata={
+                "name": "definitionURL",
+                "type": "Attribute",
+            }
+        )
+        cd: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        name: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+
+
+@dataclass
+class Fn:
+    class Meta:
+        name = "fn"
+        namespace = "http://www.w3.org/1998/Math/MathML"
+
+    apply: Optional["Apply"] = field(
+        default=None,
+        metadata={
             "type": "Element",
         }
     )
-    mmultiscripts: List["Mmultiscripts"] = field(
-        default_factory=list,
+    bind: Optional["Bind"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    munderover: List["Munderover"] = field(
-        default_factory=list,
+    ci: Optional["Ci"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mover: List["Mover"] = field(
-        default_factory=list,
+    cn: Optional["Cn"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    munder: List["Munder"] = field(
-        default_factory=list,
+    csymbol: Optional["Csymbol"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    msubsup: List["Msubsup"] = field(
-        default_factory=list,
+    cbytes: Optional[Cbytes] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    msup: List["Msup"] = field(
-        default_factory=list,
+    cerror: Optional["Cerror"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    msub: List["Msub"] = field(
-        default_factory=list,
+    cs: Optional[Cs] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    menclose: List["Menclose"] = field(
-        default_factory=list,
+    share: Optional[Share] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mfenced: List["Mfenced"] = field(
-        default_factory=list,
+    piecewise: Optional["Piecewise"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mphantom: List["Mphantom"] = field(
-        default_factory=list,
+    declare: Optional["Declare"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mpadded: List["Mpadded"] = field(
-        default_factory=list,
+    fn: Optional["Fn"] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    merror: List["Merror"] = field(
-        default_factory=list,
+    reln: Optional[Reln] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mstyle: List["Mstyle"] = field(
-        default_factory=list,
+    interval: Optional[Interval] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mroot: List["Mroot"] = field(
-        default_factory=list,
+    moment: Optional[Moment] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    msqrt: List["Msqrt"] = field(
-        default_factory=list,
+    log: Optional[Log] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mfrac: List["Mfrac"] = field(
-        default_factory=list,
+    ln: Optional[Ln] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mrow: List["Mrow"] = field(
-        default_factory=list,
+    image: Optional[Image] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    maligngroup: List[Maligngroup] = field(
-        default_factory=list,
+    codomain: Optional[Codomain] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    malignmark: List[Malignmark] = field(
-        default_factory=list,
+    domain: Optional[Domain] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    ms: List[Ms] = field(
-        default_factory=list,
+    ident: Optional[Ident] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mspace: List[Mspace] = field(
-        default_factory=list,
+    inverse: Optional[Inverse] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mtext: List[Mtext] = field(
-        default_factory=list,
+    lambda_value: Optional[Lambda] = field(
+        default=None,
         metadata={
+            "name": "lambda",
             "type": "Element",
         }
     )
-    mo: List[Mo] = field(
-        default_factory=list,
+    compose: Optional[Compose] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mn: List[Mn] = field(
-        default_factory=list,
+    quotient: Optional[Quotient] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    mi: List[Mi] = field(
-        default_factory=list,
+    divide: Optional[Divide] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    semantics: List["Mrow.Semantics"] = field(
-        default_factory=list,
+    minus: Optional[Minus] = field(
+        default=None,
         metadata={
             "type": "Element",
         }
     )
-    id: Optional[str] = field(
+    power: Optional[Power] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
         }
     )
-    xref: Optional[object] = field(
+    rem: Optional[Rem] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
         }
     )
-    class_value: List[str] = field(
-        default_factory=list,
+    root: Optional[Root] = field(
+        default=None,
         metadata={
-            "name": "class",
-            "type": "Attribute",
-            "tokens": True,
+            "type": "Element",
         }
     )
-    style: Optional[str] = field(
+    factorial: Optional[Factorial] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
         }
     )
-    href: Optional[str] = field(
+    abs: Optional[Abs] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
         }
     )
-    other: Optional[object] = field(
+    conjugate: Optional[Conjugate] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
         }
     )
-    other_attributes: Dict[str, str] = field(
-        default_factory=dict,
+    arg: Optional[Arg] = field(
+        default=None,
         metadata={
-            "type": "Attributes",
-            "namespace": "##other",
+            "type": "Element",
         }
     )
-    mathcolor: Optional[str] = field(
+    real: Optional[Real] = field(
         default=None,
         metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
+            "type": "Element",
         }
     )
-    mathbackground: Optional[Union[str, MrowValue]] = field(
+    imaginary: Optional[Imaginary] = field(
         default=None,
         metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
+            "type": "Element",
         }
     )
-    dir: Optional[MrowDir] = field(
+    floor: Optional[Floor] = field(
         default=None,
         metadata={
-            "type": "Attribute",
+            "type": "Element",
+        }
+    )
+    ceiling: Optional[Ceiling] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exp: Optional[Exp] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    min: Optional[Min] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    max: Optional[Max] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lcm: Optional[Lcm] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gcd: Optional[Gcd] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    times: Optional[Times] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    plus: Optional[Plus] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    xor: Optional[Xor] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    or_value: Optional[Or] = field(
+        default=None,
+        metadata={
+            "name": "or",
+            "type": "Element",
+        }
+    )
+    and_value: Optional[And] = field(
+        default=None,
+        metadata={
+            "name": "and",
+            "type": "Element",
+        }
+    )
+    not_value: Optional[Not] = field(
+        default=None,
+        metadata={
+            "name": "not",
+            "type": "Element",
+        }
+    )
+    equivalent: Optional[Equivalent] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    implies: Optional[Implies] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exists: Optional[Exists] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    forall: Optional[Forall] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    leq: Optional[Leq] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    geq: Optional[Geq] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lt: Optional[Lt] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gt: Optional[Gt] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eq: Optional[Eq] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tendsto: Optional[Tendsto] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    factorof: Optional[Factorof] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    approx: Optional[Approx] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    neq: Optional[Neq] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    int_value: Optional[Int] = field(
+        default=None,
+        metadata={
+            "name": "int",
+            "type": "Element",
+        }
+    )
+    diff: Optional[Diff] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    partialdiff: Optional[Partialdiff] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    laplacian: Optional[Laplacian] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    curl: Optional[Curl] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    grad: Optional[Grad] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    divergence: Optional[Divergence] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    list_value: Optional[ListType] = field(
+        default=None,
+        metadata={
+            "name": "list",
+            "type": "Element",
+        }
+    )
+    set: Optional[Set] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cartesianproduct: Optional[Cartesianproduct] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    intersect: Optional[Intersect] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    union: Optional[UnionType] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    setdiff: Optional[Setdiff] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notprsubset: Optional[Notprsubset] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notsubset: Optional[Notsubset] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notin: Optional[Notin] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    in_value: Optional[In] = field(
+        default=None,
+        metadata={
+            "name": "in",
+            "type": "Element",
+        }
+    )
+    prsubset: Optional[Prsubset] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    subset: Optional[Subset] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    card: Optional[Card] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sum: Optional[Sum] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    product: Optional[Product] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    limit: Optional[Limit] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctanh: Optional[Arctanh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsinh: Optional[Arcsinh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsech: Optional[Arcsech] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsec: Optional[Arcsec] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsch: Optional[Arccsch] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsc: Optional[Arccsc] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccoth: Optional[Arccoth] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccot: Optional[Arccot] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccosh: Optional[Arccosh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctan: Optional[Arctan] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccos: Optional[Arccos] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsin: Optional[Arcsin] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    coth: Optional[Coth] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csch: Optional[Csch] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sech: Optional[Sech] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tanh: Optional[Tanh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cosh: Optional[Cosh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sinh: Optional[Sinh] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cot: Optional[Cot] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csc: Optional[Csc] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sec: Optional[Sec] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tan: Optional[Tan] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cos: Optional[Cos] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sin: Optional[Sin] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mode: Optional[Mode] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    median: Optional[Median] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    variance: Optional[Variance] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sdev: Optional[Sdev] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mean: Optional[Mean] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrixrow: Optional[Matrixrow] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrix: Optional[Matrix] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vector: Optional[Vector] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    transpose: Optional[Transpose] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    determinant: Optional[Determinant] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    selector: Optional[Selector] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    outerproduct: Optional[Outerproduct] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    scalarproduct: Optional[Scalarproduct] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vectorproduct: Optional[Vectorproduct] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    emptyset: Optional[Emptyset] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    primes: Optional[Primes] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    complexes: Optional[Complexes] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    naturalnumbers: Optional[Naturalnumbers] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    rationals: Optional[Rationals] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    reals: Optional[Reals] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    integers: Optional[Integers] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    infinity: Optional[Infinity] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eulergamma: Optional[Eulergamma] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    pi: Optional[Pi] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    false: Optional[FalseType] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    true: Optional[TrueType] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notanumber: Optional[Notanumber] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    imaginaryi: Optional[Imaginaryi] = field(
+        default=None,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exponentiale: Optional[Exponentiale] = field(
+        default=None,
+        metadata={
+            "type": "Element",
         }
     )
-
-    @dataclass
-    class Semantics:
-        apply: Optional["Apply"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        bind: Optional["Bind"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        ci: Optional["Ci"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cn: Optional["Cn"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        csymbol: Optional["Csymbol"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cbytes: Optional[Cbytes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cerror: Optional["Cerror"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cs: Optional[Cs] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        share: Optional[Share] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        piecewise: Optional["Piecewise"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        declare: Optional["Declare"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        fn: Optional["Fn"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        reln: Optional["Reln"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        interval: Optional[Interval] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        moment: Optional[Moment] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        log: Optional[Log] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        ln: Optional[Ln] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        image: Optional[Image] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        codomain: Optional[Codomain] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        domain: Optional[Domain] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        ident: Optional[Ident] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        inverse: Optional[Inverse] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        lambda_value: Optional[Lambda] = field(
-            default=None,
-            metadata={
-                "name": "lambda",
-                "type": "Element",
-            }
-        )
-        compose: Optional[Compose] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        quotient: Optional[Quotient] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        divide: Optional[Divide] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        minus: Optional[Minus] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        power: Optional[Power] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        rem: Optional[Rem] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        root: Optional[Root] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        factorial: Optional[Factorial] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        abs: Optional[Abs] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        conjugate: Optional[Conjugate] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arg: Optional[Arg] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        real: Optional[Real] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        imaginary: Optional[Imaginary] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        floor: Optional[Floor] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        ceiling: Optional[Ceiling] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        exp: Optional[Exp] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        min: Optional[Min] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        max: Optional[Max] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        lcm: Optional[Lcm] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        gcd: Optional[Gcd] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        times: Optional[Times] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        plus: Optional[Plus] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        xor: Optional[Xor] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        or_value: Optional[Or] = field(
-            default=None,
-            metadata={
-                "name": "or",
-                "type": "Element",
-            }
-        )
-        and_value: Optional[And] = field(
-            default=None,
-            metadata={
-                "name": "and",
-                "type": "Element",
-            }
-        )
-        not_value: Optional[Not] = field(
-            default=None,
-            metadata={
-                "name": "not",
-                "type": "Element",
-            }
-        )
-        equivalent: Optional[Equivalent] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        implies: Optional[Implies] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        exists: Optional[Exists] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        forall: Optional[Forall] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        leq: Optional[Leq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        geq: Optional[Geq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        lt: Optional[Lt] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        gt: Optional[Gt] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        eq: Optional[Eq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        tendsto: Optional[Tendsto] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        factorof: Optional[Factorof] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        approx: Optional[Approx] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        neq: Optional[Neq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        int_value: Optional[Int] = field(
-            default=None,
-            metadata={
-                "name": "int",
-                "type": "Element",
-            }
-        )
-        diff: Optional[Diff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        partialdiff: Optional[Partialdiff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        laplacian: Optional[Laplacian] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        curl: Optional[Curl] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        grad: Optional[Grad] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        divergence: Optional[Divergence] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        list_value: Optional[ListType] = field(
-            default=None,
-            metadata={
-                "name": "list",
-                "type": "Element",
-            }
-        )
-        set: Optional[Set] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cartesianproduct: Optional[Cartesianproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        intersect: Optional[Intersect] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        union: Optional[UnionType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        setdiff: Optional[Setdiff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        notprsubset: Optional[Notprsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        notsubset: Optional[Notsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        notin: Optional[Notin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        in_value: Optional[In] = field(
-            default=None,
-            metadata={
-                "name": "in",
-                "type": "Element",
-            }
-        )
-        prsubset: Optional[Prsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        subset: Optional[Subset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        card: Optional[Card] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sum: Optional[Sum] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        product: Optional[Product] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        limit: Optional[Limit] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arctanh: Optional[Arctanh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arcsinh: Optional[Arcsinh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arcsech: Optional[Arcsech] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arcsec: Optional[Arcsec] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccsch: Optional[Arccsch] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccsc: Optional[Arccsc] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccoth: Optional[Arccoth] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccot: Optional[Arccot] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccosh: Optional[Arccosh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arctan: Optional[Arctan] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arccos: Optional[Arccos] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        arcsin: Optional[Arcsin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        coth: Optional[Coth] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        csch: Optional[Csch] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sech: Optional[Sech] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        tanh: Optional[Tanh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cosh: Optional[Cosh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sinh: Optional[Sinh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cot: Optional[Cot] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        csc: Optional[Csc] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sec: Optional[Sec] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        tan: Optional[Tan] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        cos: Optional[Cos] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sin: Optional[Sin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mode: Optional[Mode] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        median: Optional[Median] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        variance: Optional[Variance] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        sdev: Optional[Sdev] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mean: Optional[Mean] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        matrixrow: Optional[Matrixrow] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        matrix: Optional[Matrix] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        vector: Optional[Vector] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        transpose: Optional[Transpose] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        determinant: Optional[Determinant] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        selector: Optional[Selector] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        outerproduct: Optional[Outerproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        scalarproduct: Optional[Scalarproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        vectorproduct: Optional[Vectorproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        emptyset: Optional[Emptyset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        primes: Optional[Primes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        complexes: Optional[Complexes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        naturalnumbers: Optional[Naturalnumbers] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        rationals: Optional[Rationals] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        reals: Optional[Reals] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        integers: Optional[Integers] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        infinity: Optional[Infinity] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        eulergamma: Optional[Eulergamma] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        pi: Optional[Pi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        false: Optional[FalseType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        true: Optional[TrueType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        notanumber: Optional[Notanumber] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        imaginaryi: Optional[Imaginaryi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        exponentiale: Optional[Exponentiale] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        maction: Optional["Maction"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mlongdiv: Optional["Mlongdiv"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mstack: Optional["Mstack"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mtable: Optional["Mtable"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mmultiscripts: Optional["Mmultiscripts"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        munderover: Optional["Munderover"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mover: Optional["Mover"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        munder: Optional["Munder"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        msubsup: Optional["Msubsup"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        msup: Optional["Msup"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        msub: Optional["Msub"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        menclose: Optional["Menclose"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mfenced: Optional["Mfenced"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mphantom: Optional["Mphantom"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mpadded: Optional["Mpadded"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        merror: Optional["Merror"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mstyle: Optional["Mstyle"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mroot: Optional["Mroot"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        msqrt: Optional["Msqrt"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mfrac: Optional["Mfrac"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mrow: Optional["Mrow"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        maligngroup: Optional[Maligngroup] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        malignmark: Optional[Malignmark] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        ms: Optional[Ms] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mspace: Optional[Mspace] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mtext: Optional[Mtext] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mo: Optional[Mo] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mn: Optional[Mn] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        mi: Optional[Mi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        semantics: Optional["Mrow.Semantics"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        annotation: List[Annotation] = field(
-            default_factory=list,
-            metadata={
-                "type": "Element",
-            }
-        )
-        annotation_xml: List["AnnotationXml"] = field(
-            default_factory=list,
-            metadata={
-                "name": "annotation-xml",
-                "type": "Element",
-            }
-        )
-        id: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        xref: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        class_value: List[str] = field(
-            default_factory=list,
-            metadata={
-                "name": "class",
-                "type": "Attribute",
-                "tokens": True,
-            }
-        )
-        style: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        href: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other_attributes: Dict[str, str] = field(
-            default_factory=dict,
-            metadata={
-                "type": "Attributes",
-                "namespace": "##other",
-            }
-        )
-        encoding: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        definition_url: Optional[str] = field(
-            default=None,
-            metadata={
-                "name": "definitionURL",
-                "type": "Attribute",
-            }
-        )
-        cd: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        name: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
 
 
 @dataclass
-class Reln:
+class Declare:
     class Meta:
-        name = "reln"
+        name = "declare"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
@@ -8570,21 +8237,21 @@
     )
     declare: List["Declare"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     interval: List[Interval] = field(
         default_factory=list,
@@ -9339,20 +9006,57 @@
     )
     exponentiale: List[Exponentiale] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
+    type: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    scope: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    nargs: Optional[int] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    occurrence: Optional[DeclareOccurrence] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    encoding: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    definition_url: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "definitionURL",
+            "type": "Attribute",
+        }
+    )
 
 
 @dataclass
-class Fn:
+class Otherwise:
     class Meta:
-        name = "fn"
+        name = "otherwise"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: Optional["Apply"] = field(
         default=None,
         metadata={
             "type": "Element",
         }
@@ -9407,21 +9111,21 @@
     )
     piecewise: Optional["Piecewise"] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    declare: Optional["Declare"] = field(
+    declare: Optional[Declare] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
-    fn: Optional["Fn"] = field(
+    fn: Optional[Fn] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     reln: Optional[Reln] = field(
         default=None,
@@ -10182,20 +9886,78 @@
     )
     exponentiale: Optional[Exponentiale] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    xref: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    class_value: List[str] = field(
+        default_factory=list,
+        metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+    encoding: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    definition_url: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "definitionURL",
+            "type": "Attribute",
+        }
+    )
 
 
 @dataclass
-class Mfrac:
+class Piece:
     class Meta:
-        name = "mfrac"
+        name = "piece"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
@@ -10270,31 +10032,31 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -11301,252 +11063,2060 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    xref: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    class_value: List[str] = field(
+        default_factory=list,
+        metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+    encoding: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    definition_url: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "definitionURL",
+            "type": "Attribute",
+        }
+    )
+
+
+@dataclass
+class Piecewise:
+    class Meta:
+        name = "piecewise"
+        namespace = "http://www.w3.org/1998/Math/MathML"
+
+    piece: List[Piece] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    otherwise: List[Otherwise] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    xref: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    class_value: List[str] = field(
+        default_factory=list,
+        metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+    encoding: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    definition_url: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "definitionURL",
+            "type": "Attribute",
+        }
+    )
+
+
+@dataclass
+class Cerror:
+    class Meta:
+        name = "cerror"
+        namespace = "http://www.w3.org/1998/Math/MathML"
+
+    csymbol: List["Csymbol"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+            "min_occurs": 1,
+        }
+    )
+    apply: List["Apply"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    bind: List["Bind"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ci: List["Ci"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cn: List["Cn"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cbytes: List[Cbytes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cerror: List["Cerror"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cs: List[Cs] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    share: List[Share] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    piecewise: List[Piecewise] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    declare: List[Declare] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    fn: List[Fn] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    reln: List[Reln] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    interval: List[Interval] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    moment: List[Moment] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    log: List[Log] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ln: List[Ln] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    image: List[Image] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    codomain: List[Codomain] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    domain: List[Domain] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ident: List[Ident] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    inverse: List[Inverse] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lambda_value: List[Lambda] = field(
+        default_factory=list,
+        metadata={
+            "name": "lambda",
+            "type": "Element",
+        }
+    )
+    compose: List[Compose] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    quotient: List[Quotient] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    divide: List[Divide] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    minus: List[Minus] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    power: List[Power] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    rem: List[Rem] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    root: List[Root] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    factorial: List[Factorial] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    abs: List[Abs] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    conjugate: List[Conjugate] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arg: List[Arg] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    real: List[Real] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    imaginary: List[Imaginary] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    floor: List[Floor] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ceiling: List[Ceiling] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exp: List[Exp] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    min: List[Min] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    max: List[Max] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lcm: List[Lcm] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gcd: List[Gcd] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    times: List[Times] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    plus: List[Plus] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    xor: List[Xor] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    or_value: List[Or] = field(
+        default_factory=list,
+        metadata={
+            "name": "or",
+            "type": "Element",
+        }
+    )
+    and_value: List[And] = field(
+        default_factory=list,
+        metadata={
+            "name": "and",
+            "type": "Element",
+        }
+    )
+    not_value: List[Not] = field(
+        default_factory=list,
+        metadata={
+            "name": "not",
+            "type": "Element",
+        }
+    )
+    equivalent: List[Equivalent] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    implies: List[Implies] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exists: List[Exists] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    forall: List[Forall] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    leq: List[Leq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    geq: List[Geq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lt: List[Lt] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gt: List[Gt] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eq: List[Eq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tendsto: List[Tendsto] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    factorof: List[Factorof] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    approx: List[Approx] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    neq: List[Neq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    int_value: List[Int] = field(
+        default_factory=list,
+        metadata={
+            "name": "int",
+            "type": "Element",
+        }
+    )
+    diff: List[Diff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    partialdiff: List[Partialdiff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    laplacian: List[Laplacian] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    curl: List[Curl] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    grad: List[Grad] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    divergence: List[Divergence] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    list_value: List[ListType] = field(
+        default_factory=list,
+        metadata={
+            "name": "list",
+            "type": "Element",
+        }
+    )
+    set: List[Set] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cartesianproduct: List[Cartesianproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    intersect: List[Intersect] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    union: List[UnionType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    setdiff: List[Setdiff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notprsubset: List[Notprsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notsubset: List[Notsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notin: List[Notin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    in_value: List[In] = field(
+        default_factory=list,
+        metadata={
+            "name": "in",
+            "type": "Element",
+        }
+    )
+    prsubset: List[Prsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    subset: List[Subset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    card: List[Card] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sum: List[Sum] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    product: List[Product] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    limit: List[Limit] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctanh: List[Arctanh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsinh: List[Arcsinh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsech: List[Arcsech] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsec: List[Arcsec] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsch: List[Arccsch] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsc: List[Arccsc] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccoth: List[Arccoth] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccot: List[Arccot] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccosh: List[Arccosh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctan: List[Arctan] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccos: List[Arccos] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsin: List[Arcsin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    coth: List[Coth] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csch: List[Csch] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sech: List[Sech] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tanh: List[Tanh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cosh: List[Cosh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sinh: List[Sinh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cot: List[Cot] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csc: List[Csc] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sec: List[Sec] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tan: List[Tan] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cos: List[Cos] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sin: List[Sin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mode: List[Mode] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    median: List[Median] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    variance: List[Variance] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sdev: List[Sdev] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mean: List[Mean] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrixrow: List[Matrixrow] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrix: List[Matrix] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vector: List[Vector] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    transpose: List[Transpose] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    determinant: List[Determinant] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    selector: List[Selector] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    outerproduct: List[Outerproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    scalarproduct: List[Scalarproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vectorproduct: List[Vectorproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    emptyset: List[Emptyset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    primes: List[Primes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    complexes: List[Complexes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    naturalnumbers: List[Naturalnumbers] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    rationals: List[Rationals] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    reals: List[Reals] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    integers: List[Integers] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    infinity: List[Infinity] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eulergamma: List[Eulergamma] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    pi: List[Pi] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    false: List[FalseType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    true: List[TrueType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notanumber: List[Notanumber] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    imaginaryi: List[Imaginaryi] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exponentiale: List[Exponentiale] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    xref: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    class_value: List[str] = field(
+        default_factory=list,
+        metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+
+
+@dataclass
+class Mrow:
+    class Meta:
+        name = "mrow"
+        namespace = "http://www.w3.org/1998/Math/MathML"
+
+    apply: List["Apply"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    bind: List["Bind"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ci: List["Ci"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cn: List["Cn"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csymbol: List["Csymbol"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cbytes: List[Cbytes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cerror: List[Cerror] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cs: List[Cs] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    share: List[Share] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    piecewise: List[Piecewise] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    declare: List[Declare] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    fn: List[Fn] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    reln: List[Reln] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    interval: List[Interval] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    moment: List[Moment] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    log: List[Log] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ln: List[Ln] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    image: List[Image] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    codomain: List[Codomain] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    domain: List[Domain] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ident: List[Ident] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    inverse: List[Inverse] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lambda_value: List[Lambda] = field(
+        default_factory=list,
+        metadata={
+            "name": "lambda",
+            "type": "Element",
+        }
+    )
+    compose: List[Compose] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    quotient: List[Quotient] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    divide: List[Divide] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    minus: List[Minus] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    power: List[Power] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    rem: List[Rem] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    root: List[Root] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    factorial: List[Factorial] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    abs: List[Abs] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    conjugate: List[Conjugate] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arg: List[Arg] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    real: List[Real] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    imaginary: List[Imaginary] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    floor: List[Floor] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ceiling: List[Ceiling] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exp: List[Exp] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    min: List[Min] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    max: List[Max] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lcm: List[Lcm] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gcd: List[Gcd] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    times: List[Times] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    plus: List[Plus] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    xor: List[Xor] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    or_value: List[Or] = field(
+        default_factory=list,
+        metadata={
+            "name": "or",
+            "type": "Element",
+        }
+    )
+    and_value: List[And] = field(
+        default_factory=list,
+        metadata={
+            "name": "and",
+            "type": "Element",
+        }
+    )
+    not_value: List[Not] = field(
+        default_factory=list,
+        metadata={
+            "name": "not",
+            "type": "Element",
+        }
+    )
+    equivalent: List[Equivalent] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    implies: List[Implies] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exists: List[Exists] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    forall: List[Forall] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    leq: List[Leq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    geq: List[Geq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    lt: List[Lt] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    gt: List[Gt] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eq: List[Eq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tendsto: List[Tendsto] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    factorof: List[Factorof] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    approx: List[Approx] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    neq: List[Neq] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    int_value: List[Int] = field(
+        default_factory=list,
+        metadata={
+            "name": "int",
+            "type": "Element",
+        }
+    )
+    diff: List[Diff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    partialdiff: List[Partialdiff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    laplacian: List[Laplacian] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    curl: List[Curl] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    grad: List[Grad] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    divergence: List[Divergence] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    list_value: List[ListType] = field(
+        default_factory=list,
+        metadata={
+            "name": "list",
+            "type": "Element",
+        }
+    )
+    set: List[Set] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cartesianproduct: List[Cartesianproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    intersect: List[Intersect] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    union: List[UnionType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    setdiff: List[Setdiff] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notprsubset: List[Notprsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notsubset: List[Notsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notin: List[Notin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    in_value: List[In] = field(
+        default_factory=list,
+        metadata={
+            "name": "in",
+            "type": "Element",
+        }
+    )
+    prsubset: List[Prsubset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    subset: List[Subset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    card: List[Card] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sum: List[Sum] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    product: List[Product] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    limit: List[Limit] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctanh: List[Arctanh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsinh: List[Arcsinh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsech: List[Arcsech] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsec: List[Arcsec] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsch: List[Arccsch] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccsc: List[Arccsc] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccoth: List[Arccoth] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccot: List[Arccot] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccosh: List[Arccosh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arctan: List[Arctan] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arccos: List[Arccos] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    arcsin: List[Arcsin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    coth: List[Coth] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csch: List[Csch] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sech: List[Sech] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tanh: List[Tanh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cosh: List[Cosh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sinh: List[Sinh] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cot: List[Cot] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    csc: List[Csc] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sec: List[Sec] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    tan: List[Tan] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    cos: List[Cos] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sin: List[Sin] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mode: List[Mode] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    median: List[Median] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    variance: List[Variance] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    sdev: List[Sdev] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mean: List[Mean] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrixrow: List[Matrixrow] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    matrix: List[Matrix] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vector: List[Vector] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    transpose: List[Transpose] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    determinant: List[Determinant] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    selector: List[Selector] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    outerproduct: List[Outerproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    scalarproduct: List[Scalarproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    vectorproduct: List[Vectorproduct] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    emptyset: List[Emptyset] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    primes: List[Primes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    complexes: List[Complexes] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    naturalnumbers: List[Naturalnumbers] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    rationals: List[Rationals] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    reals: List[Reals] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    integers: List[Integers] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    infinity: List[Infinity] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    eulergamma: List[Eulergamma] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    pi: List[Pi] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    false: List[FalseType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    true: List[TrueType] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    notanumber: List[Notanumber] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    imaginaryi: List[Imaginaryi] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    exponentiale: List[Exponentiale] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
     maction: List["Maction"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mlongdiv: List["Mlongdiv"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mstack: List["Mstack"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mtable: List["Mtable"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mmultiscripts: List["Mmultiscripts"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     munderover: List["Munderover"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mover: List["Mover"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     munder: List["Munder"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     msubsup: List["Msubsup"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     msup: List["Msup"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     msub: List["Msub"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     menclose: List["Menclose"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mfenced: List["Mfenced"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mphantom: List["Mphantom"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mpadded: List["Mpadded"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     merror: List["Merror"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mstyle: List["Mstyle"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mroot: List["Mroot"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     msqrt: List["Msqrt"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mfrac: List["Mfrac"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
-    mrow: List[Mrow] = field(
+    mrow: List["Mrow"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     maligngroup: List[Maligngroup] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     malignmark: List[Malignmark] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     ms: List[Ms] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mspace: List[Mspace] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mtext: List[Mtext] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mo: List[Mo] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mn: List[Mn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mi: List[Mi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
-    semantics: List["Mfrac.Semantics"] = field(
+    semantics: List["Mrow.Semantics"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -11593,41 +13163,22 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MfracValue]] = field(
+    mathbackground: Optional[Union[str, MrowValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    linethickness: Optional[Union[str, MfracValue]] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
-        }
-    )
-    numalign: Optional[MfracNumalign] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    denomalign: Optional[MfracDenomalign] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    bevelled: Optional[MfracBevelled] = field(
+    dir: Optional[MrowDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
 
     @dataclass
@@ -11664,15 +13215,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -11682,33 +13233,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -12583,15 +14134,15 @@
         )
         mfrac: Optional["Mfrac"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        mrow: Optional[Mrow] = field(
+        mrow: Optional["Mrow"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         maligngroup: Optional[Maligngroup] = field(
             default=None,
@@ -12637,27 +14188,27 @@
         )
         mi: Optional[Mi] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        semantics: Optional["Mfrac.Semantics"] = field(
+        semantics: Optional["Mrow.Semantics"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -12729,897 +14280,17 @@
             metadata={
                 "type": "Attribute",
             }
         )
 
 
 @dataclass
-class Declare:
-    class Meta:
-        name = "declare"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    apply: List["Apply"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    bind: List["Bind"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ci: List["Ci"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cn: List["Cn"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csymbol: List["Csymbol"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cbytes: List[Cbytes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cerror: List["Cerror"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cs: List[Cs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    share: List[Share] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    piecewise: List["Piecewise"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    declare: List["Declare"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    fn: List[Fn] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reln: List[Reln] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    interval: List[Interval] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    moment: List[Moment] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    log: List[Log] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ln: List[Ln] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    image: List[Image] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    codomain: List[Codomain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    domain: List[Domain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ident: List[Ident] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    inverse: List[Inverse] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lambda_value: List[Lambda] = field(
-        default_factory=list,
-        metadata={
-            "name": "lambda",
-            "type": "Element",
-        }
-    )
-    compose: List[Compose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    quotient: List[Quotient] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divide: List[Divide] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    minus: List[Minus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    power: List[Power] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rem: List[Rem] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    root: List[Root] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorial: List[Factorial] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    abs: List[Abs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    conjugate: List[Conjugate] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arg: List[Arg] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    real: List[Real] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginary: List[Imaginary] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    floor: List[Floor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ceiling: List[Ceiling] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exp: List[Exp] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    min: List[Min] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    max: List[Max] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lcm: List[Lcm] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gcd: List[Gcd] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    times: List[Times] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    plus: List[Plus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    xor: List[Xor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    or_value: List[Or] = field(
-        default_factory=list,
-        metadata={
-            "name": "or",
-            "type": "Element",
-        }
-    )
-    and_value: List[And] = field(
-        default_factory=list,
-        metadata={
-            "name": "and",
-            "type": "Element",
-        }
-    )
-    not_value: List[Not] = field(
-        default_factory=list,
-        metadata={
-            "name": "not",
-            "type": "Element",
-        }
-    )
-    equivalent: List[Equivalent] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    implies: List[Implies] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exists: List[Exists] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    forall: List[Forall] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    leq: List[Leq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    geq: List[Geq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lt: List[Lt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gt: List[Gt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eq: List[Eq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tendsto: List[Tendsto] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorof: List[Factorof] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    approx: List[Approx] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    neq: List[Neq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    int_value: List[Int] = field(
-        default_factory=list,
-        metadata={
-            "name": "int",
-            "type": "Element",
-        }
-    )
-    diff: List[Diff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    partialdiff: List[Partialdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    laplacian: List[Laplacian] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    curl: List[Curl] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    grad: List[Grad] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divergence: List[Divergence] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    list_value: List[ListType] = field(
-        default_factory=list,
-        metadata={
-            "name": "list",
-            "type": "Element",
-        }
-    )
-    set: List[Set] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cartesianproduct: List[Cartesianproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    intersect: List[Intersect] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    union: List[UnionType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    setdiff: List[Setdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notprsubset: List[Notprsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notsubset: List[Notsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notin: List[Notin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    in_value: List[In] = field(
-        default_factory=list,
-        metadata={
-            "name": "in",
-            "type": "Element",
-        }
-    )
-    prsubset: List[Prsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    subset: List[Subset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    card: List[Card] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sum: List[Sum] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    product: List[Product] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    limit: List[Limit] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctanh: List[Arctanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsinh: List[Arcsinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsech: List[Arcsech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsec: List[Arcsec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsch: List[Arccsch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsc: List[Arccsc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccoth: List[Arccoth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccot: List[Arccot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccosh: List[Arccosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctan: List[Arctan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccos: List[Arccos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsin: List[Arcsin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    coth: List[Coth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csch: List[Csch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sech: List[Sech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tanh: List[Tanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cosh: List[Cosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sinh: List[Sinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cot: List[Cot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csc: List[Csc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sec: List[Sec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tan: List[Tan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cos: List[Cos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sin: List[Sin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mode: List[Mode] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    median: List[Median] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    variance: List[Variance] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sdev: List[Sdev] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mean: List[Mean] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrixrow: List[Matrixrow] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrix: List[Matrix] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vector: List[Vector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    transpose: List[Transpose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    determinant: List[Determinant] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    selector: List[Selector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    outerproduct: List[Outerproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    scalarproduct: List[Scalarproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vectorproduct: List[Vectorproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    emptyset: List[Emptyset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    primes: List[Primes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    complexes: List[Complexes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    naturalnumbers: List[Naturalnumbers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rationals: List[Rationals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reals: List[Reals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    integers: List[Integers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    infinity: List[Infinity] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eulergamma: List[Eulergamma] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    pi: List[Pi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    false: List[FalseType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    true: List[TrueType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notanumber: List[Notanumber] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginaryi: List[Imaginaryi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exponentiale: List[Exponentiale] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    type: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    scope: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    nargs: Optional[int] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    occurrence: Optional[DeclareOccurrence] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    encoding: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    definition_url: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "definitionURL",
-            "type": "Attribute",
-        }
-    )
-
-
-@dataclass
-class Mroot:
+class Mfrac:
     class Meta:
-        name = "mroot"
+        name = "mfrac"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
@@ -13662,15 +14333,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -13686,39 +14357,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -14877,15 +15548,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    mfrac: List[Mfrac] = field(
+    mfrac: List["Mfrac"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -14957,15 +15628,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    semantics: List["Mroot.Semantics"] = field(
+    semantics: List["Mfrac.Semantics"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -15017,21 +15688,46 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MrootValue]] = field(
+    mathbackground: Optional[Union[str, MfracValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
+    linethickness: Optional[Union[str, MfracValue]] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+        }
+    )
+    numalign: Optional[MfracNumalign] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    denomalign: Optional[MfracDenomalign] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    bevelled: Optional[MfracBevelled] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
             metadata={
                 "type": "Element",
@@ -15063,15 +15759,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -15081,33 +15777,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -15976,15 +16672,15 @@
         )
         msqrt: Optional["Msqrt"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        mfrac: Optional[Mfrac] = field(
+        mfrac: Optional["Mfrac"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         mrow: Optional[Mrow] = field(
             default=None,
@@ -16036,27 +16732,27 @@
         )
         mi: Optional[Mi] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        semantics: Optional["Mroot.Semantics"] = field(
+        semantics: Optional["Mfrac.Semantics"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -16128,1032 +16824,1368 @@
             metadata={
                 "type": "Attribute",
             }
         )
 
 
 @dataclass
-class Mfenced:
+class Mroot:
     class Meta:
-        name = "mfenced"
+        name = "mroot"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     bind: List["Bind"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     ci: List["Ci"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cn: List["Cn"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     csymbol: List["Csymbol"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cbytes: List[Cbytes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cs: List[Cs] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     share: List[Share] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     interval: List[Interval] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     moment: List[Moment] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     log: List[Log] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     ln: List[Ln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     image: List[Image] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     codomain: List[Codomain] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     domain: List[Domain] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     ident: List[Ident] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     inverse: List[Inverse] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     lambda_value: List[Lambda] = field(
         default_factory=list,
         metadata={
             "name": "lambda",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     compose: List[Compose] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     quotient: List[Quotient] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     divide: List[Divide] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     minus: List[Minus] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     power: List[Power] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     rem: List[Rem] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     root: List[Root] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     factorial: List[Factorial] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     abs: List[Abs] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     conjugate: List[Conjugate] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arg: List[Arg] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     real: List[Real] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     imaginary: List[Imaginary] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     floor: List[Floor] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     ceiling: List[Ceiling] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     exp: List[Exp] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     min: List[Min] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     max: List[Max] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     lcm: List[Lcm] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     gcd: List[Gcd] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     times: List[Times] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     plus: List[Plus] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     xor: List[Xor] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     or_value: List[Or] = field(
         default_factory=list,
         metadata={
             "name": "or",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     and_value: List[And] = field(
         default_factory=list,
         metadata={
             "name": "and",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     not_value: List[Not] = field(
         default_factory=list,
         metadata={
             "name": "not",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     equivalent: List[Equivalent] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     implies: List[Implies] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     exists: List[Exists] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     forall: List[Forall] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     leq: List[Leq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     geq: List[Geq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     lt: List[Lt] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     gt: List[Gt] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     eq: List[Eq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     tendsto: List[Tendsto] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     factorof: List[Factorof] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     approx: List[Approx] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     neq: List[Neq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     int_value: List[Int] = field(
         default_factory=list,
         metadata={
             "name": "int",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     diff: List[Diff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     partialdiff: List[Partialdiff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     laplacian: List[Laplacian] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     curl: List[Curl] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     grad: List[Grad] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     divergence: List[Divergence] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     list_value: List[ListType] = field(
         default_factory=list,
         metadata={
             "name": "list",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     set: List[Set] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cartesianproduct: List[Cartesianproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     intersect: List[Intersect] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     union: List[UnionType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     setdiff: List[Setdiff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     notprsubset: List[Notprsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     notsubset: List[Notsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     notin: List[Notin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     in_value: List[In] = field(
         default_factory=list,
         metadata={
             "name": "in",
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     prsubset: List[Prsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     subset: List[Subset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     card: List[Card] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sum: List[Sum] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     product: List[Product] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     limit: List[Limit] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arctanh: List[Arctanh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arcsinh: List[Arcsinh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arcsech: List[Arcsech] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arcsec: List[Arcsec] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccsch: List[Arccsch] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccsc: List[Arccsc] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccoth: List[Arccoth] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccot: List[Arccot] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccosh: List[Arccosh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arctan: List[Arctan] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arccos: List[Arccos] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     arcsin: List[Arcsin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     coth: List[Coth] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     csch: List[Csch] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sech: List[Sech] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     tanh: List[Tanh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cosh: List[Cosh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sinh: List[Sinh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cot: List[Cot] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     csc: List[Csc] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sec: List[Sec] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     tan: List[Tan] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     cos: List[Cos] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sin: List[Sin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mode: List[Mode] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     median: List[Median] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     variance: List[Variance] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     sdev: List[Sdev] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mean: List[Mean] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     matrixrow: List[Matrixrow] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     matrix: List[Matrix] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     vector: List[Vector] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     transpose: List[Transpose] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     determinant: List[Determinant] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     selector: List[Selector] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     outerproduct: List[Outerproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     scalarproduct: List[Scalarproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     vectorproduct: List[Vectorproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     emptyset: List[Emptyset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     primes: List[Primes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     complexes: List[Complexes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     naturalnumbers: List[Naturalnumbers] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     rationals: List[Rationals] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     reals: List[Reals] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     integers: List[Integers] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     infinity: List[Infinity] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     eulergamma: List[Eulergamma] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     pi: List[Pi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     false: List[FalseType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     true: List[TrueType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     notanumber: List[Notanumber] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     imaginaryi: List[Imaginaryi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     exponentiale: List[Exponentiale] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     maction: List["Maction"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mlongdiv: List["Mlongdiv"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mstack: List["Mstack"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mtable: List["Mtable"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mmultiscripts: List["Mmultiscripts"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     munderover: List["Munderover"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mover: List["Mover"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     munder: List["Munder"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     msubsup: List["Msubsup"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     msup: List["Msup"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     msub: List["Msub"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     menclose: List["Menclose"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mfenced: List["Mfenced"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mphantom: List["Mphantom"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mpadded: List["Mpadded"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     merror: List["Merror"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mstyle: List["Mstyle"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    mroot: List[Mroot] = field(
+    mroot: List["Mroot"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     msqrt: List["Msqrt"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mfrac: List[Mfrac] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mrow: List[Mrow] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     maligngroup: List[Maligngroup] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     malignmark: List[Malignmark] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     ms: List[Ms] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mspace: List[Mspace] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mtext: List[Mtext] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mo: List[Mo] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mn: List[Mn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     mi: List[Mi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
-    semantics: List["Mfenced.Semantics"] = field(
+    semantics: List["Mroot.Semantics"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "max_occurs": 2,
+            "sequence": 1,
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -17200,39 +18232,21 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MfencedValue]] = field(
+    mathbackground: Optional[Union[str, MrootValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    open: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    close: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    separators: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
             metadata={
                 "type": "Element",
@@ -17264,15 +18278,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -17282,33 +18296,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -18165,15 +19179,15 @@
         )
         mstyle: Optional["Mstyle"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        mroot: Optional[Mroot] = field(
+        mroot: Optional["Mroot"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         msqrt: Optional["Msqrt"] = field(
             default=None,
@@ -18237,27 +19251,27 @@
         )
         mi: Optional[Mi] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        semantics: Optional["Mfenced.Semantics"] = field(
+        semantics: Optional["Mroot.Semantics"] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -18329,2029 +19343,1032 @@
             metadata={
                 "type": "Attribute",
             }
         )
 
 
 @dataclass
-class Otherwise:
-    class Meta:
-        name = "otherwise"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    apply: Optional["Apply"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    bind: Optional["Bind"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ci: Optional["Ci"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cn: Optional["Cn"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csymbol: Optional["Csymbol"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cbytes: Optional[Cbytes] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cerror: Optional["Cerror"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cs: Optional[Cs] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    share: Optional[Share] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    piecewise: Optional["Piecewise"] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    declare: Optional[Declare] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    fn: Optional[Fn] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reln: Optional[Reln] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    interval: Optional[Interval] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    moment: Optional[Moment] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    log: Optional[Log] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ln: Optional[Ln] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    image: Optional[Image] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    codomain: Optional[Codomain] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    domain: Optional[Domain] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ident: Optional[Ident] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    inverse: Optional[Inverse] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lambda_value: Optional[Lambda] = field(
-        default=None,
-        metadata={
-            "name": "lambda",
-            "type": "Element",
-        }
-    )
-    compose: Optional[Compose] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    quotient: Optional[Quotient] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divide: Optional[Divide] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    minus: Optional[Minus] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    power: Optional[Power] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rem: Optional[Rem] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    root: Optional[Root] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorial: Optional[Factorial] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    abs: Optional[Abs] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    conjugate: Optional[Conjugate] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arg: Optional[Arg] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    real: Optional[Real] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginary: Optional[Imaginary] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    floor: Optional[Floor] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ceiling: Optional[Ceiling] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exp: Optional[Exp] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    min: Optional[Min] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    max: Optional[Max] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lcm: Optional[Lcm] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gcd: Optional[Gcd] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    times: Optional[Times] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    plus: Optional[Plus] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    xor: Optional[Xor] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    or_value: Optional[Or] = field(
-        default=None,
-        metadata={
-            "name": "or",
-            "type": "Element",
-        }
-    )
-    and_value: Optional[And] = field(
-        default=None,
-        metadata={
-            "name": "and",
-            "type": "Element",
-        }
-    )
-    not_value: Optional[Not] = field(
-        default=None,
-        metadata={
-            "name": "not",
-            "type": "Element",
-        }
-    )
-    equivalent: Optional[Equivalent] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    implies: Optional[Implies] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exists: Optional[Exists] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    forall: Optional[Forall] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    leq: Optional[Leq] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    geq: Optional[Geq] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lt: Optional[Lt] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gt: Optional[Gt] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eq: Optional[Eq] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tendsto: Optional[Tendsto] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorof: Optional[Factorof] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    approx: Optional[Approx] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    neq: Optional[Neq] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    int_value: Optional[Int] = field(
-        default=None,
-        metadata={
-            "name": "int",
-            "type": "Element",
-        }
-    )
-    diff: Optional[Diff] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    partialdiff: Optional[Partialdiff] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    laplacian: Optional[Laplacian] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    curl: Optional[Curl] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    grad: Optional[Grad] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divergence: Optional[Divergence] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    list_value: Optional[ListType] = field(
-        default=None,
-        metadata={
-            "name": "list",
-            "type": "Element",
-        }
-    )
-    set: Optional[Set] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cartesianproduct: Optional[Cartesianproduct] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    intersect: Optional[Intersect] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    union: Optional[UnionType] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    setdiff: Optional[Setdiff] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notprsubset: Optional[Notprsubset] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notsubset: Optional[Notsubset] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notin: Optional[Notin] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    in_value: Optional[In] = field(
-        default=None,
-        metadata={
-            "name": "in",
-            "type": "Element",
-        }
-    )
-    prsubset: Optional[Prsubset] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    subset: Optional[Subset] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    card: Optional[Card] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sum: Optional[Sum] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    product: Optional[Product] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    limit: Optional[Limit] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctanh: Optional[Arctanh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsinh: Optional[Arcsinh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsech: Optional[Arcsech] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsec: Optional[Arcsec] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsch: Optional[Arccsch] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsc: Optional[Arccsc] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccoth: Optional[Arccoth] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccot: Optional[Arccot] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccosh: Optional[Arccosh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctan: Optional[Arctan] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccos: Optional[Arccos] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsin: Optional[Arcsin] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    coth: Optional[Coth] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csch: Optional[Csch] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sech: Optional[Sech] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tanh: Optional[Tanh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cosh: Optional[Cosh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sinh: Optional[Sinh] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cot: Optional[Cot] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csc: Optional[Csc] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sec: Optional[Sec] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tan: Optional[Tan] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cos: Optional[Cos] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sin: Optional[Sin] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mode: Optional[Mode] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    median: Optional[Median] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    variance: Optional[Variance] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sdev: Optional[Sdev] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mean: Optional[Mean] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrixrow: Optional[Matrixrow] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrix: Optional[Matrix] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vector: Optional[Vector] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    transpose: Optional[Transpose] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    determinant: Optional[Determinant] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    selector: Optional[Selector] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    outerproduct: Optional[Outerproduct] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    scalarproduct: Optional[Scalarproduct] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vectorproduct: Optional[Vectorproduct] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    emptyset: Optional[Emptyset] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    primes: Optional[Primes] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    complexes: Optional[Complexes] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    naturalnumbers: Optional[Naturalnumbers] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rationals: Optional[Rationals] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reals: Optional[Reals] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    integers: Optional[Integers] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    infinity: Optional[Infinity] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eulergamma: Optional[Eulergamma] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    pi: Optional[Pi] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    false: Optional[FalseType] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    true: Optional[TrueType] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notanumber: Optional[Notanumber] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginaryi: Optional[Imaginaryi] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exponentiale: Optional[Exponentiale] = field(
-        default=None,
-        metadata={
-            "type": "Element",
-        }
-    )
-    id: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    xref: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    class_value: List[str] = field(
-        default_factory=list,
-        metadata={
-            "name": "class",
-            "type": "Attribute",
-            "tokens": True,
-        }
-    )
-    style: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    href: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other_attributes: Dict[str, str] = field(
-        default_factory=dict,
-        metadata={
-            "type": "Attributes",
-            "namespace": "##other",
-        }
-    )
-    encoding: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    definition_url: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "definitionURL",
-            "type": "Attribute",
-        }
-    )
-
-
-@dataclass
-class Piece:
+class Mfenced:
     class Meta:
-        name = "piece"
+        name = "mfenced"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     bind: List["Bind"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     ci: List["Ci"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cn: List["Cn"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     csymbol: List["Csymbol"] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cbytes: List[Cbytes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cs: List[Cs] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     share: List[Share] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     interval: List[Interval] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     moment: List[Moment] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     log: List[Log] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     ln: List[Ln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     image: List[Image] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     codomain: List[Codomain] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     domain: List[Domain] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     ident: List[Ident] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     inverse: List[Inverse] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     lambda_value: List[Lambda] = field(
         default_factory=list,
         metadata={
             "name": "lambda",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     compose: List[Compose] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     quotient: List[Quotient] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     divide: List[Divide] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     minus: List[Minus] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     power: List[Power] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     rem: List[Rem] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     root: List[Root] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     factorial: List[Factorial] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     abs: List[Abs] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     conjugate: List[Conjugate] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arg: List[Arg] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     real: List[Real] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     imaginary: List[Imaginary] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     floor: List[Floor] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     ceiling: List[Ceiling] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     exp: List[Exp] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     min: List[Min] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     max: List[Max] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     lcm: List[Lcm] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     gcd: List[Gcd] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     times: List[Times] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     plus: List[Plus] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     xor: List[Xor] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     or_value: List[Or] = field(
         default_factory=list,
         metadata={
             "name": "or",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     and_value: List[And] = field(
         default_factory=list,
         metadata={
             "name": "and",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     not_value: List[Not] = field(
         default_factory=list,
         metadata={
             "name": "not",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     equivalent: List[Equivalent] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     implies: List[Implies] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     exists: List[Exists] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     forall: List[Forall] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     leq: List[Leq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     geq: List[Geq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     lt: List[Lt] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     gt: List[Gt] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     eq: List[Eq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     tendsto: List[Tendsto] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     factorof: List[Factorof] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     approx: List[Approx] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     neq: List[Neq] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     int_value: List[Int] = field(
         default_factory=list,
         metadata={
             "name": "int",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     diff: List[Diff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     partialdiff: List[Partialdiff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     laplacian: List[Laplacian] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     curl: List[Curl] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     grad: List[Grad] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     divergence: List[Divergence] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     list_value: List[ListType] = field(
         default_factory=list,
         metadata={
             "name": "list",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     set: List[Set] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cartesianproduct: List[Cartesianproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     intersect: List[Intersect] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     union: List[UnionType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     setdiff: List[Setdiff] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     notprsubset: List[Notprsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     notsubset: List[Notsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     notin: List[Notin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     in_value: List[In] = field(
         default_factory=list,
         metadata={
             "name": "in",
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     prsubset: List[Prsubset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     subset: List[Subset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     card: List[Card] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sum: List[Sum] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     product: List[Product] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     limit: List[Limit] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arctanh: List[Arctanh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arcsinh: List[Arcsinh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arcsech: List[Arcsech] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arcsec: List[Arcsec] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccsch: List[Arccsch] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccsc: List[Arccsc] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccoth: List[Arccoth] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccot: List[Arccot] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccosh: List[Arccosh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arctan: List[Arctan] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arccos: List[Arccos] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     arcsin: List[Arcsin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     coth: List[Coth] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     csch: List[Csch] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sech: List[Sech] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     tanh: List[Tanh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cosh: List[Cosh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sinh: List[Sinh] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cot: List[Cot] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     csc: List[Csc] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sec: List[Sec] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     tan: List[Tan] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     cos: List[Cos] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sin: List[Sin] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mode: List[Mode] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     median: List[Median] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     variance: List[Variance] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     sdev: List[Sdev] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     mean: List[Mean] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     matrixrow: List[Matrixrow] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     matrix: List[Matrix] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     vector: List[Vector] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     transpose: List[Transpose] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     determinant: List[Determinant] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     selector: List[Selector] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     outerproduct: List[Outerproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     scalarproduct: List[Scalarproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     vectorproduct: List[Vectorproduct] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     emptyset: List[Emptyset] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     primes: List[Primes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     complexes: List[Complexes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     naturalnumbers: List[Naturalnumbers] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     rationals: List[Rationals] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     reals: List[Reals] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     integers: List[Integers] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     infinity: List[Infinity] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     eulergamma: List[Eulergamma] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     pi: List[Pi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     false: List[FalseType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     true: List[TrueType] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     notanumber: List[Notanumber] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     imaginaryi: List[Imaginaryi] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
         }
     )
     exponentiale: List[Exponentiale] = field(
         default_factory=list,
         metadata={
             "type": "Element",
-            "max_occurs": 2,
-            "sequence": 1,
+        }
+    )
+    maction: List["Maction"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mlongdiv: List["Mlongdiv"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mstack: List["Mstack"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mtable: List["Mtable"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mmultiscripts: List["Mmultiscripts"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    munderover: List["Munderover"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mover: List["Mover"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    munder: List["Munder"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    msubsup: List["Msubsup"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    msup: List["Msup"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    msub: List["Msub"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    menclose: List["Menclose"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mfenced: List["Mfenced"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mphantom: List["Mphantom"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mpadded: List["Mpadded"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    merror: List["Merror"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mstyle: List["Mstyle"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mroot: List[Mroot] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    msqrt: List["Msqrt"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mfrac: List[Mfrac] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mrow: List[Mrow] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    maligngroup: List[Maligngroup] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    malignmark: List[Malignmark] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    ms: List[Ms] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mspace: List[Mspace] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mtext: List[Mtext] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mo: List[Mo] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mn: List[Mn] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    mi: List[Mi] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
+        }
+    )
+    semantics: List["Mfenced.Semantics"] = field(
+        default_factory=list,
+        metadata={
+            "type": "Element",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -20391,28 +20408,1148 @@
     other_attributes: Dict[str, str] = field(
         default_factory=dict,
         metadata={
             "type": "Attributes",
             "namespace": "##other",
         }
     )
-    encoding: Optional[str] = field(
+    mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
+            "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    definition_url: Optional[str] = field(
+    mathbackground: Optional[Union[str, MfencedValue]] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
+        }
+    )
+    open: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    close: Optional[object] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    separators: Optional[object] = field(
         default=None,
         metadata={
-            "name": "definitionURL",
             "type": "Attribute",
         }
     )
 
+    @dataclass
+    class Semantics:
+        apply: Optional["Apply"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        bind: Optional["Bind"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        ci: Optional["Ci"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cn: Optional["Cn"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        csymbol: Optional["Csymbol"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cbytes: Optional[Cbytes] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cerror: Optional[Cerror] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cs: Optional[Cs] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        share: Optional[Share] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        piecewise: Optional[Piecewise] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        declare: Optional[Declare] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        fn: Optional[Fn] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        reln: Optional[Reln] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        interval: Optional[Interval] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        moment: Optional[Moment] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        log: Optional[Log] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        ln: Optional[Ln] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        image: Optional[Image] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        codomain: Optional[Codomain] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        domain: Optional[Domain] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        ident: Optional[Ident] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        inverse: Optional[Inverse] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        lambda_value: Optional[Lambda] = field(
+            default=None,
+            metadata={
+                "name": "lambda",
+                "type": "Element",
+            }
+        )
+        compose: Optional[Compose] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        quotient: Optional[Quotient] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        divide: Optional[Divide] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        minus: Optional[Minus] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        power: Optional[Power] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        rem: Optional[Rem] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        root: Optional[Root] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        factorial: Optional[Factorial] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        abs: Optional[Abs] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        conjugate: Optional[Conjugate] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arg: Optional[Arg] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        real: Optional[Real] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        imaginary: Optional[Imaginary] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        floor: Optional[Floor] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        ceiling: Optional[Ceiling] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        exp: Optional[Exp] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        min: Optional[Min] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        max: Optional[Max] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        lcm: Optional[Lcm] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        gcd: Optional[Gcd] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        times: Optional[Times] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        plus: Optional[Plus] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        xor: Optional[Xor] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        or_value: Optional[Or] = field(
+            default=None,
+            metadata={
+                "name": "or",
+                "type": "Element",
+            }
+        )
+        and_value: Optional[And] = field(
+            default=None,
+            metadata={
+                "name": "and",
+                "type": "Element",
+            }
+        )
+        not_value: Optional[Not] = field(
+            default=None,
+            metadata={
+                "name": "not",
+                "type": "Element",
+            }
+        )
+        equivalent: Optional[Equivalent] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        implies: Optional[Implies] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        exists: Optional[Exists] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        forall: Optional[Forall] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        leq: Optional[Leq] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        geq: Optional[Geq] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        lt: Optional[Lt] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        gt: Optional[Gt] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        eq: Optional[Eq] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        tendsto: Optional[Tendsto] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        factorof: Optional[Factorof] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        approx: Optional[Approx] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        neq: Optional[Neq] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        int_value: Optional[Int] = field(
+            default=None,
+            metadata={
+                "name": "int",
+                "type": "Element",
+            }
+        )
+        diff: Optional[Diff] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        partialdiff: Optional[Partialdiff] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        laplacian: Optional[Laplacian] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        curl: Optional[Curl] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        grad: Optional[Grad] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        divergence: Optional[Divergence] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        list_value: Optional[ListType] = field(
+            default=None,
+            metadata={
+                "name": "list",
+                "type": "Element",
+            }
+        )
+        set: Optional[Set] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cartesianproduct: Optional[Cartesianproduct] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        intersect: Optional[Intersect] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        union: Optional[UnionType] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        setdiff: Optional[Setdiff] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        notprsubset: Optional[Notprsubset] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        notsubset: Optional[Notsubset] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        notin: Optional[Notin] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        in_value: Optional[In] = field(
+            default=None,
+            metadata={
+                "name": "in",
+                "type": "Element",
+            }
+        )
+        prsubset: Optional[Prsubset] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        subset: Optional[Subset] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        card: Optional[Card] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sum: Optional[Sum] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        product: Optional[Product] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        limit: Optional[Limit] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arctanh: Optional[Arctanh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arcsinh: Optional[Arcsinh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arcsech: Optional[Arcsech] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arcsec: Optional[Arcsec] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccsch: Optional[Arccsch] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccsc: Optional[Arccsc] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccoth: Optional[Arccoth] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccot: Optional[Arccot] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccosh: Optional[Arccosh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arctan: Optional[Arctan] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arccos: Optional[Arccos] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        arcsin: Optional[Arcsin] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        coth: Optional[Coth] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        csch: Optional[Csch] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sech: Optional[Sech] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        tanh: Optional[Tanh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cosh: Optional[Cosh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sinh: Optional[Sinh] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cot: Optional[Cot] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        csc: Optional[Csc] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sec: Optional[Sec] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        tan: Optional[Tan] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        cos: Optional[Cos] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sin: Optional[Sin] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mode: Optional[Mode] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        median: Optional[Median] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        variance: Optional[Variance] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        sdev: Optional[Sdev] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mean: Optional[Mean] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        matrixrow: Optional[Matrixrow] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        matrix: Optional[Matrix] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        vector: Optional[Vector] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        transpose: Optional[Transpose] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        determinant: Optional[Determinant] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        selector: Optional[Selector] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        outerproduct: Optional[Outerproduct] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        scalarproduct: Optional[Scalarproduct] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        vectorproduct: Optional[Vectorproduct] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        emptyset: Optional[Emptyset] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        primes: Optional[Primes] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        complexes: Optional[Complexes] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        naturalnumbers: Optional[Naturalnumbers] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        rationals: Optional[Rationals] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        reals: Optional[Reals] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        integers: Optional[Integers] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        infinity: Optional[Infinity] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        eulergamma: Optional[Eulergamma] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        pi: Optional[Pi] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        false: Optional[FalseType] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        true: Optional[TrueType] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        notanumber: Optional[Notanumber] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        imaginaryi: Optional[Imaginaryi] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        exponentiale: Optional[Exponentiale] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        maction: Optional["Maction"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mlongdiv: Optional["Mlongdiv"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mstack: Optional["Mstack"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mtable: Optional["Mtable"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mmultiscripts: Optional["Mmultiscripts"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        munderover: Optional["Munderover"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mover: Optional["Mover"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        munder: Optional["Munder"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        msubsup: Optional["Msubsup"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        msup: Optional["Msup"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        msub: Optional["Msub"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        menclose: Optional["Menclose"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mfenced: Optional["Mfenced"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mphantom: Optional["Mphantom"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mpadded: Optional["Mpadded"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        merror: Optional["Merror"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mstyle: Optional["Mstyle"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mroot: Optional[Mroot] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        msqrt: Optional["Msqrt"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mfrac: Optional[Mfrac] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mrow: Optional[Mrow] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        maligngroup: Optional[Maligngroup] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        malignmark: Optional[Malignmark] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        ms: Optional[Ms] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mspace: Optional[Mspace] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mtext: Optional[Mtext] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mo: Optional[Mo] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mn: Optional[Mn] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        mi: Optional[Mi] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        semantics: Optional["Mfenced.Semantics"] = field(
+            default=None,
+            metadata={
+                "type": "Element",
+            }
+        )
+        annotation: List[Annotation] = field(
+            default_factory=list,
+            metadata={
+                "type": "Element",
+            }
+        )
+        annotation_xml: List[AnnotationXml] = field(
+            default_factory=list,
+            metadata={
+                "name": "annotation-xml",
+                "type": "Element",
+            }
+        )
+        id: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        xref: Optional[object] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        class_value: List[str] = field(
+            default_factory=list,
+            metadata={
+                "name": "class",
+                "type": "Attribute",
+                "tokens": True,
+            }
+        )
+        style: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        href: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        other: Optional[object] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        other_attributes: Dict[str, str] = field(
+            default_factory=dict,
+            metadata={
+                "type": "Attributes",
+                "namespace": "##other",
+            }
+        )
+        encoding: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        definition_url: Optional[str] = field(
+            default=None,
+            metadata={
+                "name": "definitionURL",
+                "type": "Attribute",
+            }
+        )
+        cd: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+        name: Optional[str] = field(
+            default=None,
+            metadata={
+                "type": "Attribute",
+            }
+        )
+
 
 @dataclass
 class Msub:
     class Meta:
         name = "msub"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
@@ -20460,15 +21597,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -20484,39 +21621,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -21826,15 +22963,15 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     subscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
@@ -21868,15 +23005,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -21886,33 +23023,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -22853,15 +23990,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -22933,981 +24070,14 @@
             metadata={
                 "type": "Attribute",
             }
         )
 
 
 @dataclass
-class Piecewise:
-    class Meta:
-        name = "piecewise"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    piece: List[Piece] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    otherwise: List[Otherwise] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    id: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    xref: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    class_value: List[str] = field(
-        default_factory=list,
-        metadata={
-            "name": "class",
-            "type": "Attribute",
-            "tokens": True,
-        }
-    )
-    style: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    href: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other_attributes: Dict[str, str] = field(
-        default_factory=dict,
-        metadata={
-            "type": "Attributes",
-            "namespace": "##other",
-        }
-    )
-    encoding: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    definition_url: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "definitionURL",
-            "type": "Attribute",
-        }
-    )
-
-
-@dataclass
-class Cerror:
-    class Meta:
-        name = "cerror"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    csymbol: List["Csymbol"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "min_occurs": 1,
-        }
-    )
-    apply: List["Apply"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    bind: List["Bind"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ci: List["Ci"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cn: List["Cn"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cbytes: List[Cbytes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cerror: List["Cerror"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cs: List[Cs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    share: List[Share] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    piecewise: List[Piecewise] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    declare: List[Declare] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    fn: List[Fn] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reln: List[Reln] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    interval: List[Interval] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    moment: List[Moment] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    log: List[Log] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ln: List[Ln] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    image: List[Image] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    codomain: List[Codomain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    domain: List[Domain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ident: List[Ident] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    inverse: List[Inverse] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lambda_value: List[Lambda] = field(
-        default_factory=list,
-        metadata={
-            "name": "lambda",
-            "type": "Element",
-        }
-    )
-    compose: List[Compose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    quotient: List[Quotient] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divide: List[Divide] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    minus: List[Minus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    power: List[Power] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rem: List[Rem] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    root: List[Root] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorial: List[Factorial] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    abs: List[Abs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    conjugate: List[Conjugate] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arg: List[Arg] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    real: List[Real] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginary: List[Imaginary] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    floor: List[Floor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    ceiling: List[Ceiling] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exp: List[Exp] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    min: List[Min] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    max: List[Max] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lcm: List[Lcm] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gcd: List[Gcd] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    times: List[Times] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    plus: List[Plus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    xor: List[Xor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    or_value: List[Or] = field(
-        default_factory=list,
-        metadata={
-            "name": "or",
-            "type": "Element",
-        }
-    )
-    and_value: List[And] = field(
-        default_factory=list,
-        metadata={
-            "name": "and",
-            "type": "Element",
-        }
-    )
-    not_value: List[Not] = field(
-        default_factory=list,
-        metadata={
-            "name": "not",
-            "type": "Element",
-        }
-    )
-    equivalent: List[Equivalent] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    implies: List[Implies] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exists: List[Exists] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    forall: List[Forall] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    leq: List[Leq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    geq: List[Geq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    lt: List[Lt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    gt: List[Gt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eq: List[Eq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tendsto: List[Tendsto] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    factorof: List[Factorof] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    approx: List[Approx] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    neq: List[Neq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    int_value: List[Int] = field(
-        default_factory=list,
-        metadata={
-            "name": "int",
-            "type": "Element",
-        }
-    )
-    diff: List[Diff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    partialdiff: List[Partialdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    laplacian: List[Laplacian] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    curl: List[Curl] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    grad: List[Grad] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    divergence: List[Divergence] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    list_value: List[ListType] = field(
-        default_factory=list,
-        metadata={
-            "name": "list",
-            "type": "Element",
-        }
-    )
-    set: List[Set] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cartesianproduct: List[Cartesianproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    intersect: List[Intersect] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    union: List[UnionType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    setdiff: List[Setdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notprsubset: List[Notprsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notsubset: List[Notsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notin: List[Notin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    in_value: List[In] = field(
-        default_factory=list,
-        metadata={
-            "name": "in",
-            "type": "Element",
-        }
-    )
-    prsubset: List[Prsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    subset: List[Subset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    card: List[Card] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sum: List[Sum] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    product: List[Product] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    limit: List[Limit] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctanh: List[Arctanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsinh: List[Arcsinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsech: List[Arcsech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsec: List[Arcsec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsch: List[Arccsch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccsc: List[Arccsc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccoth: List[Arccoth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccot: List[Arccot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccosh: List[Arccosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arctan: List[Arctan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arccos: List[Arccos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    arcsin: List[Arcsin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    coth: List[Coth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csch: List[Csch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sech: List[Sech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tanh: List[Tanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cosh: List[Cosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sinh: List[Sinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cot: List[Cot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    csc: List[Csc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sec: List[Sec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    tan: List[Tan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    cos: List[Cos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sin: List[Sin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mode: List[Mode] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    median: List[Median] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    variance: List[Variance] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    sdev: List[Sdev] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    mean: List[Mean] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrixrow: List[Matrixrow] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    matrix: List[Matrix] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vector: List[Vector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    transpose: List[Transpose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    determinant: List[Determinant] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    selector: List[Selector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    outerproduct: List[Outerproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    scalarproduct: List[Scalarproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    vectorproduct: List[Vectorproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    emptyset: List[Emptyset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    primes: List[Primes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    complexes: List[Complexes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    naturalnumbers: List[Naturalnumbers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    rationals: List[Rationals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    reals: List[Reals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    integers: List[Integers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    infinity: List[Infinity] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    eulergamma: List[Eulergamma] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    pi: List[Pi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    false: List[FalseType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    true: List[TrueType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    notanumber: List[Notanumber] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    imaginaryi: List[Imaginaryi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    exponentiale: List[Exponentiale] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    id: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    xref: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    class_value: List[str] = field(
-        default_factory=list,
-        metadata={
-            "name": "class",
-            "type": "Attribute",
-            "tokens": True,
-        }
-    )
-    style: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    href: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other_attributes: Dict[str, str] = field(
-        default_factory=dict,
-        metadata={
-            "type": "Attributes",
-            "namespace": "##other",
-        }
-    )
-
-
-@dataclass
 class Msup:
     class Meta:
         name = "msup"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     apply: List["Apply"] = field(
         default_factory=list,
@@ -23953,15 +24123,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -23977,39 +24147,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -25319,15 +25489,15 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     superscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
@@ -25361,15 +25531,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -25379,33 +25549,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -26346,15 +26516,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -26479,15 +26649,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
@@ -26503,39 +26673,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
@@ -27845,22 +28015,22 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     subscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     superscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
@@ -27894,15 +28064,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -27912,33 +28082,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -28879,15 +29049,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -29012,15 +29182,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -29036,39 +29206,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -30425,15 +30595,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -30443,33 +30613,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -31410,15 +31580,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -31543,15 +31713,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -31567,39 +31737,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 2,
             "sequence": 1,
         }
     )
@@ -32956,15 +33126,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -32974,33 +33144,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -33941,15 +34111,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -34074,15 +34244,15 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
@@ -34098,39 +34268,39 @@
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "max_occurs": 3,
             "sequence": 1,
         }
     )
@@ -35493,15 +35663,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -35511,33 +35681,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -36478,15 +36648,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -36599,15 +36769,15 @@
     )
     cbytes: List[Cbytes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     cs: List[Cs] = field(
         default_factory=list,
@@ -36617,33 +36787,33 @@
     )
     share: List[Share] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
         }
     )
     interval: List[Interval] = field(
         default_factory=list,
@@ -37653,22 +37823,22 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     subscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     superscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
@@ -37702,15 +37872,15 @@
         )
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         cs: Optional[Cs] = field(
             default=None,
@@ -37720,33 +37890,33 @@
         )
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
             }
         )
         interval: Optional[Interval] = field(
             default=None,
@@ -38687,15 +38857,15 @@
         )
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
             }
         )
         id: Optional[str] = field(
@@ -38810,15 +38980,15 @@
     cbytes: List[Cbytes] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
-    cerror: List["Cerror"] = field(
+    cerror: List[Cerror] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
     cs: List[Cs] = field(
@@ -38831,36 +39001,36 @@
     share: List[Share] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
-    piecewise: List["Piecewise"] = field(
+    piecewise: List[Piecewise] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
-    declare: List["Declare"] = field(
+    declare: List[Declare] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
-    fn: List["Fn"] = field(
+    fn: List[Fn] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
-    reln: List["Reln"] = field(
+    reln: List[Reln] = field(
         default_factory=list,
         metadata={
             "type": "Element",
             "namespace": "http://www.w3.org/1998/Math/MathML",
         }
     )
     interval: List[Interval] = field(
@@ -39996,15 +40166,15 @@
         cbytes: Optional[Cbytes] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        cerror: Optional["Cerror"] = field(
+        cerror: Optional[Cerror] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
         cs: Optional[Cs] = field(
@@ -40017,36 +40187,36 @@
         share: Optional[Share] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        piecewise: Optional["Piecewise"] = field(
+        piecewise: Optional[Piecewise] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        declare: Optional["Declare"] = field(
+        declare: Optional[Declare] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        fn: Optional["Fn"] = field(
+        fn: Optional[Fn] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        reln: Optional["Reln"] = field(
+        reln: Optional[Reln] = field(
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
         interval: Optional[Interval] = field(
@@ -41144,15 +41314,15 @@
         annotation: List[Annotation] = field(
             default_factory=list,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
-        annotation_xml: List["AnnotationXml"] = field(
+        annotation_xml: List[AnnotationXml] = field(
             default_factory=list,
             metadata={
                 "name": "annotation-xml",
                 "type": "Element",
                 "namespace": "http://www.w3.org/1998/Math/MathML",
             }
         )
@@ -41433,43 +41603,43 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     height: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*([\+\-]?[0-9]*(\.[0-9]*)?\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace)))\s*",
+            "pattern": r"\s*([\+\-]?[0-9]*([0-9]\.?|\.[0-9])[0-9]*\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace))?)\s*",
         }
     )
     depth: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*([\+\-]?[0-9]*(\.[0-9]*)?\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace)))\s*",
+            "pattern": r"\s*([\+\-]?[0-9]*([0-9]\.?|\.[0-9])[0-9]*\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace))?)\s*",
         }
     )
     width: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*([\+\-]?[0-9]*(\.[0-9]*)?\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace)))\s*",
+            "pattern": r"\s*([\+\-]?[0-9]*([0-9]\.?|\.[0-9])[0-9]*\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace))?)\s*",
         }
     )
     lspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*([\+\-]?[0-9]*(\.[0-9]*)?\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace)))\s*",
+            "pattern": r"\s*([\+\-]?[0-9]*([0-9]\.?|\.[0-9])[0-9]*\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace))?)\s*",
         }
     )
     voffset: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*([\+\-]?[0-9]*(\.[0-9]*)?\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace)))\s*",
+            "pattern": r"\s*([\+\-]?[0-9]*([0-9]\.?|\.[0-9])[0-9]*\s*((%?\s*(height|depth|width)?)|e[mx]|in|cm|mm|p[xtc]|((negative)?((very){0,2}thi(n|ck)|medium)mathspace))?)\s*",
         }
     )
 
 
 @dataclass
 class Mphantom(ImpliedMrow):
     class Meta:
@@ -41687,15 +41857,15 @@
             "type": "Attribute",
         }
     )
     scriptminsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     infixlinebreakstyle: Optional[MstyleInfixlinebreakstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41744,15 +41914,15 @@
             "type": "Attribute",
         }
     )
     charspacing: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     close: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41771,15 +41941,15 @@
             "tokens": True,
         }
     )
     columnspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     columnspan: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -41805,15 +41975,15 @@
             "type": "Attribute",
         }
     )
     depth: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     dir: Optional[MstyleDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41869,15 +42039,15 @@
             "pattern": r"(\s*\{\s*(left|center|right|decimalpoint)(\s+(left|center|right|decimalpoint))*\})*\s*",
         }
     )
     height: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentalign: Optional[MstyleIndentalign] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41894,29 +42064,29 @@
             "type": "Attribute",
         }
     )
     indentshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentshiftfirst: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentshiftlast: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indenttarget: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41927,15 +42097,15 @@
             "type": "Attribute",
         }
     )
     leftoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     length: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41958,22 +42128,22 @@
             "type": "Attribute",
         }
     )
     lineleading: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     linethickness: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     location: Optional[MstyleLocation] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -41990,62 +42160,62 @@
             "type": "Attribute",
         }
     )
     lspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mathsize: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mathvariant: Optional[MstyleMathvariant] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     maxsize: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     minlabelspacing: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     minsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     movablelimits: Optional[MstyleMovablelimits] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     mslinethickness: Optional[Union[str, MstyleValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     notation: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -42068,15 +42238,15 @@
             "type": "Attribute",
         }
     )
     rightoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     rowalign: List[Verticalalign] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
             "tokens": True,
@@ -42089,15 +42259,15 @@
             "tokens": True,
         }
     )
     rowspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     rowspan: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -42109,15 +42279,15 @@
             "type": "Attribute",
         }
     )
     rspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     selection: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -42158,42 +42328,42 @@
             "type": "Attribute",
         }
     )
     subscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     superscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     symmetric: Optional[MstyleSymmetric] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     valign: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     width: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     fontfamily: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -42210,15 +42380,15 @@
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
@@ -42231,2742 +42401,59 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     veryverythinmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     verythinmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     thinmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mediummathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     thickmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     verythickmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     veryverythickmathspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
-        }
-    )
-
-
-@dataclass
-class AnnotationXmlModel:
-    class Meta:
-        name = "annotation-xml.model"
-
-    apply: List["Apply"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    bind: List["Bind"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    ci: List["Ci"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cn: List["Cn"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    csymbol: List["Csymbol"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cbytes: List[Cbytes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cerror: List["Cerror"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cs: List[Cs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    share: List[Share] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    piecewise: List["Piecewise"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    declare: List["Declare"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    fn: List["Fn"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    reln: List["Reln"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    interval: List[Interval] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    moment: List[Moment] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    log: List[Log] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    ln: List[Ln] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    image: List[Image] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    codomain: List[Codomain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    domain: List[Domain] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    ident: List[Ident] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    inverse: List[Inverse] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    lambda_value: List[Lambda] = field(
-        default_factory=list,
-        metadata={
-            "name": "lambda",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    compose: List[Compose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    quotient: List[Quotient] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    divide: List[Divide] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    minus: List[Minus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    power: List[Power] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    rem: List[Rem] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    root: List[Root] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    factorial: List[Factorial] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    abs: List[Abs] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    conjugate: List[Conjugate] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arg: List[Arg] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    real: List[Real] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    imaginary: List[Imaginary] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    floor: List[Floor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    ceiling: List[Ceiling] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    exp: List[Exp] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    min: List[Min] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    max: List[Max] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    lcm: List[Lcm] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    gcd: List[Gcd] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    times: List[Times] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    plus: List[Plus] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    xor: List[Xor] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    or_value: List[Or] = field(
-        default_factory=list,
-        metadata={
-            "name": "or",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    and_value: List[And] = field(
-        default_factory=list,
-        metadata={
-            "name": "and",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    not_value: List[Not] = field(
-        default_factory=list,
-        metadata={
-            "name": "not",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    equivalent: List[Equivalent] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    implies: List[Implies] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    exists: List[Exists] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    forall: List[Forall] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    leq: List[Leq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    geq: List[Geq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    lt: List[Lt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    gt: List[Gt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    eq: List[Eq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    tendsto: List[Tendsto] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    factorof: List[Factorof] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    approx: List[Approx] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    neq: List[Neq] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    int_value: List[Int] = field(
-        default_factory=list,
-        metadata={
-            "name": "int",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    diff: List[Diff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    partialdiff: List[Partialdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    laplacian: List[Laplacian] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    curl: List[Curl] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    grad: List[Grad] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    divergence: List[Divergence] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    list_value: List[ListType] = field(
-        default_factory=list,
-        metadata={
-            "name": "list",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    set: List[Set] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cartesianproduct: List[Cartesianproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    intersect: List[Intersect] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    union: List[UnionType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    setdiff: List[Setdiff] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    notprsubset: List[Notprsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    notsubset: List[Notsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    notin: List[Notin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    in_value: List[In] = field(
-        default_factory=list,
-        metadata={
-            "name": "in",
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    prsubset: List[Prsubset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    subset: List[Subset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    card: List[Card] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sum: List[Sum] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    product: List[Product] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    limit: List[Limit] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arctanh: List[Arctanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arcsinh: List[Arcsinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arcsech: List[Arcsech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arcsec: List[Arcsec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccsch: List[Arccsch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccsc: List[Arccsc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccoth: List[Arccoth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccot: List[Arccot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccosh: List[Arccosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arctan: List[Arctan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arccos: List[Arccos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    arcsin: List[Arcsin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    coth: List[Coth] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    csch: List[Csch] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sech: List[Sech] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    tanh: List[Tanh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cosh: List[Cosh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sinh: List[Sinh] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cot: List[Cot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    csc: List[Csc] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sec: List[Sec] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    tan: List[Tan] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    cos: List[Cos] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sin: List[Sin] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mode: List[Mode] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    median: List[Median] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    variance: List[Variance] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    sdev: List[Sdev] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mean: List[Mean] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    matrixrow: List[Matrixrow] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    matrix: List[Matrix] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    vector: List[Vector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    transpose: List[Transpose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    determinant: List[Determinant] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    selector: List[Selector] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    outerproduct: List[Outerproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    scalarproduct: List[Scalarproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    vectorproduct: List[Vectorproduct] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    emptyset: List[Emptyset] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    primes: List[Primes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    complexes: List[Complexes] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    naturalnumbers: List[Naturalnumbers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    rationals: List[Rationals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    reals: List[Reals] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    integers: List[Integers] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    infinity: List[Infinity] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    eulergamma: List[Eulergamma] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    pi: List[Pi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    false: List[FalseType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    true: List[TrueType] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    notanumber: List[Notanumber] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    imaginaryi: List[Imaginaryi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    exponentiale: List[Exponentiale] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    maction: List["Maction"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mlongdiv: List["Mlongdiv"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mstack: List["Mstack"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mtable: List[Mtable] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mmultiscripts: List[Mmultiscripts] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    munderover: List[Munderover] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mover: List[Mover] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    munder: List[Munder] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    msubsup: List[Msubsup] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    msup: List[Msup] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    msub: List[Msub] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    menclose: List[Menclose] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mfenced: List[Mfenced] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mphantom: List[Mphantom] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mpadded: List[Mpadded] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    merror: List[Merror] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mstyle: List[Mstyle] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mroot: List[Mroot] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    msqrt: List[Msqrt] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mfrac: List[Mfrac] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mrow: List[Mrow] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    maligngroup: List[Maligngroup] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    malignmark: List[Malignmark] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    ms: List[Ms] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mspace: List[Mspace] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mtext: List[Mtext] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mo: List[Mo] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mn: List[Mn] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    mi: List[Mi] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    semantics: List["AnnotationXmlModel.Semantics"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-            "namespace": "http://www.w3.org/1998/Math/MathML",
-        }
-    )
-    other_element: List[object] = field(
-        default_factory=list,
-        metadata={
-            "type": "Wildcard",
-            "namespace": "##other",
-        }
-    )
-    local_element: List[object] = field(
-        default_factory=list,
-        metadata={
-            "type": "Wildcard",
-            "namespace": "##local",
-        }
-    )
-
-    @dataclass
-    class Semantics:
-        apply: Optional["Apply"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        bind: Optional["Bind"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        ci: Optional["Ci"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cn: Optional["Cn"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        csymbol: Optional["Csymbol"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cbytes: Optional[Cbytes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cerror: Optional["Cerror"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cs: Optional[Cs] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        share: Optional[Share] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        piecewise: Optional["Piecewise"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        declare: Optional["Declare"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        fn: Optional["Fn"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        reln: Optional["Reln"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        interval: Optional[Interval] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        moment: Optional[Moment] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        log: Optional[Log] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        ln: Optional[Ln] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        image: Optional[Image] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        codomain: Optional[Codomain] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        domain: Optional[Domain] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        ident: Optional[Ident] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        inverse: Optional[Inverse] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        lambda_value: Optional[Lambda] = field(
-            default=None,
-            metadata={
-                "name": "lambda",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        compose: Optional[Compose] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        quotient: Optional[Quotient] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        divide: Optional[Divide] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        minus: Optional[Minus] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        power: Optional[Power] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        rem: Optional[Rem] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        root: Optional[Root] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        factorial: Optional[Factorial] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        abs: Optional[Abs] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        conjugate: Optional[Conjugate] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arg: Optional[Arg] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        real: Optional[Real] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        imaginary: Optional[Imaginary] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        floor: Optional[Floor] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        ceiling: Optional[Ceiling] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        exp: Optional[Exp] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        min: Optional[Min] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        max: Optional[Max] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        lcm: Optional[Lcm] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        gcd: Optional[Gcd] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        times: Optional[Times] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        plus: Optional[Plus] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        xor: Optional[Xor] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        or_value: Optional[Or] = field(
-            default=None,
-            metadata={
-                "name": "or",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        and_value: Optional[And] = field(
-            default=None,
-            metadata={
-                "name": "and",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        not_value: Optional[Not] = field(
-            default=None,
-            metadata={
-                "name": "not",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        equivalent: Optional[Equivalent] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        implies: Optional[Implies] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        exists: Optional[Exists] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        forall: Optional[Forall] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        leq: Optional[Leq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        geq: Optional[Geq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        lt: Optional[Lt] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        gt: Optional[Gt] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        eq: Optional[Eq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        tendsto: Optional[Tendsto] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        factorof: Optional[Factorof] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        approx: Optional[Approx] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        neq: Optional[Neq] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        int_value: Optional[Int] = field(
-            default=None,
-            metadata={
-                "name": "int",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        diff: Optional[Diff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        partialdiff: Optional[Partialdiff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        laplacian: Optional[Laplacian] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        curl: Optional[Curl] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        grad: Optional[Grad] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        divergence: Optional[Divergence] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        list_value: Optional[ListType] = field(
-            default=None,
-            metadata={
-                "name": "list",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        set: Optional[Set] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cartesianproduct: Optional[Cartesianproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        intersect: Optional[Intersect] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        union: Optional[UnionType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        setdiff: Optional[Setdiff] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        notprsubset: Optional[Notprsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        notsubset: Optional[Notsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        notin: Optional[Notin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        in_value: Optional[In] = field(
-            default=None,
-            metadata={
-                "name": "in",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        prsubset: Optional[Prsubset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        subset: Optional[Subset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        card: Optional[Card] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sum: Optional[Sum] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        product: Optional[Product] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        limit: Optional[Limit] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arctanh: Optional[Arctanh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arcsinh: Optional[Arcsinh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arcsech: Optional[Arcsech] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arcsec: Optional[Arcsec] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccsch: Optional[Arccsch] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccsc: Optional[Arccsc] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccoth: Optional[Arccoth] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccot: Optional[Arccot] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccosh: Optional[Arccosh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arctan: Optional[Arctan] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arccos: Optional[Arccos] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        arcsin: Optional[Arcsin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        coth: Optional[Coth] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        csch: Optional[Csch] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sech: Optional[Sech] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        tanh: Optional[Tanh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cosh: Optional[Cosh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sinh: Optional[Sinh] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cot: Optional[Cot] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        csc: Optional[Csc] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sec: Optional[Sec] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        tan: Optional[Tan] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        cos: Optional[Cos] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sin: Optional[Sin] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mode: Optional[Mode] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        median: Optional[Median] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        variance: Optional[Variance] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        sdev: Optional[Sdev] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mean: Optional[Mean] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        matrixrow: Optional[Matrixrow] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        matrix: Optional[Matrix] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        vector: Optional[Vector] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        transpose: Optional[Transpose] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        determinant: Optional[Determinant] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        selector: Optional[Selector] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        outerproduct: Optional[Outerproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        scalarproduct: Optional[Scalarproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        vectorproduct: Optional[Vectorproduct] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        emptyset: Optional[Emptyset] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        primes: Optional[Primes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        complexes: Optional[Complexes] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        naturalnumbers: Optional[Naturalnumbers] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        rationals: Optional[Rationals] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        reals: Optional[Reals] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        integers: Optional[Integers] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        infinity: Optional[Infinity] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        eulergamma: Optional[Eulergamma] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        pi: Optional[Pi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        false: Optional[FalseType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        true: Optional[TrueType] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        notanumber: Optional[Notanumber] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        imaginaryi: Optional[Imaginaryi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        exponentiale: Optional[Exponentiale] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        maction: Optional["Maction"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mlongdiv: Optional["Mlongdiv"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mstack: Optional["Mstack"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mtable: Optional[Mtable] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mmultiscripts: Optional[Mmultiscripts] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        munderover: Optional[Munderover] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mover: Optional[Mover] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        munder: Optional[Munder] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        msubsup: Optional[Msubsup] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        msup: Optional[Msup] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        msub: Optional[Msub] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        menclose: Optional[Menclose] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mfenced: Optional[Mfenced] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mphantom: Optional[Mphantom] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mpadded: Optional[Mpadded] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        merror: Optional[Merror] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mstyle: Optional[Mstyle] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mroot: Optional[Mroot] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        msqrt: Optional[Msqrt] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mfrac: Optional[Mfrac] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mrow: Optional[Mrow] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        maligngroup: Optional[Maligngroup] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        malignmark: Optional[Malignmark] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        ms: Optional[Ms] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mspace: Optional[Mspace] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mtext: Optional[Mtext] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mo: Optional[Mo] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mn: Optional[Mn] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        mi: Optional[Mi] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        semantics: Optional["AnnotationXmlModel.Semantics"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        annotation: List[Annotation] = field(
-            default_factory=list,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        annotation_xml: List["AnnotationXml"] = field(
-            default_factory=list,
-            metadata={
-                "name": "annotation-xml",
-                "type": "Element",
-                "namespace": "http://www.w3.org/1998/Math/MathML",
-            }
-        )
-        id: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        xref: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        class_value: List[str] = field(
-            default_factory=list,
-            metadata={
-                "name": "class",
-                "type": "Attribute",
-                "tokens": True,
-            }
-        )
-        style: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        href: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other_attributes: Dict[str, str] = field(
-            default_factory=dict,
-            metadata={
-                "type": "Attributes",
-                "namespace": "##other",
-            }
-        )
-        encoding: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        definition_url: Optional[str] = field(
-            default=None,
-            metadata={
-                "name": "definitionURL",
-                "type": "Attribute",
-            }
-        )
-        cd: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        name: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-
-
-@dataclass
-class AnnotationXml(AnnotationXmlModel):
-    class Meta:
-        name = "annotation-xml"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    id: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    xref: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    class_value: List[str] = field(
-        default_factory=list,
-        metadata={
-            "name": "class",
-            "type": "Attribute",
-            "tokens": True,
-        }
-    )
-    style: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    href: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other: Optional[object] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    other_attributes: Dict[str, str] = field(
-        default_factory=dict,
-        metadata={
-            "type": "Attributes",
-            "namespace": "##other",
-        }
-    )
-    cd: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    name: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    encoding: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    definition_url: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "definitionURL",
-            "type": "Attribute",
-        }
-    )
-    src: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-
-
-@dataclass
-class Bvar:
-    class Meta:
-        name = "bvar"
-        namespace = "http://www.w3.org/1998/Math/MathML"
-
-    ci: List["Ci"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-    semantics: List["Bvar.Semantics"] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
-    degree: List[Degree] = field(
-        default_factory=list,
-        metadata={
-            "type": "Element",
-        }
-    )
-
-    @dataclass
-    class Semantics:
-        ci: Optional["Ci"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        semantics: Optional["Bvar.Semantics"] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-            }
-        )
-        annotation: List[Annotation] = field(
-            default_factory=list,
-            metadata={
-                "type": "Element",
-            }
-        )
-        annotation_xml: List[AnnotationXml] = field(
-            default_factory=list,
-            metadata={
-                "name": "annotation-xml",
-                "type": "Element",
-            }
-        )
-        id: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        xref: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        class_value: List[str] = field(
-            default_factory=list,
-            metadata={
-                "name": "class",
-                "type": "Attribute",
-                "tokens": True,
-            }
-        )
-        style: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        href: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other: Optional[object] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        other_attributes: Dict[str, str] = field(
-            default_factory=dict,
-            metadata={
-                "type": "Attributes",
-                "namespace": "##other",
-            }
-        )
-        encoding: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        definition_url: Optional[str] = field(
-            default=None,
-            metadata={
-                "name": "definitionURL",
-                "type": "Attribute",
-            }
-        )
-        cd: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
-        name: Optional[str] = field(
-            default=None,
-            metadata={
-                "type": "Attribute",
-            }
-        )
 
 
 @dataclass
 class Mscarry:
     class Meta:
         name = "mscarry"
         namespace = "http://www.w3.org/1998/Math/MathML"
@@ -54905,15 +52392,15 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     align: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*(top|bottom|center|baseline|axis)\s*[0-9]*",
+            "pattern": r"\s*(top|bottom|center|baseline|axis)(\s+-?[0-9]+)?\s*",
         }
     )
     stackalign: Optional[MstackStackalign] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -54924,15 +52411,15 @@
             "type": "Attribute",
         }
     )
     charspacing: Optional[Union[str, MstackValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
 
     @dataclass
     class Semantics:
         apply: Optional["Apply"] = field(
             default=None,
@@ -62829,14 +60316,15 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     actiontype: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
+            "required": True,
         }
     )
     selection: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/conjugate.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/conjugate.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/cs.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/cs.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/divide.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/divide.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/exp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/exp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorial.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorial.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/factorof.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/factorof.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/floor.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/floor.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/imaginary.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/imaginary.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/maligngroup.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/maligngroup.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/malignmark.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/malignmark.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import field
 from decimal import Decimal
 from pydantic.dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 from .abs import Abs
 from .and_mod import And
 from .annotation import Annotation
+from .annotation_xml import AnnotationXml
 from .approx import Approx
 from .arccos import Arccos
 from .arccosh import Arccosh
 from .arccot import Arccot
 from .arccoth import Arccoth
 from .arccsc import Arccsc
 from .arccsch import Arccsch
@@ -24,15 +25,14 @@
 from .cbytes import Cbytes
 from .ceiling import Ceiling
 from .codomain import Codomain
 from .columnalignstyle import Columnalignstyle
 from .complexes import Complexes
 from .compose import Compose
 from .condition import (
-    AnnotationXml,
     Apply,
     Bind,
     Cerror,
     Ci,
     Cn,
     Csymbol,
     Declare,
@@ -1266,15 +1266,15 @@
             "type": "Attribute",
         }
     )
     scriptminsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     infixlinebreakstyle: Optional[MathInfixlinebreakstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1323,15 +1323,15 @@
             "type": "Attribute",
         }
     )
     charspacing: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     close: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1350,15 +1350,15 @@
             "tokens": True,
         }
     )
     columnspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     columnspan: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -1384,15 +1384,15 @@
             "type": "Attribute",
         }
     )
     depth: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     dir: Optional[MathDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1448,15 +1448,15 @@
             "pattern": r"(\s*\{\s*(left|center|right|decimalpoint)(\s+(left|center|right|decimalpoint))*\})*\s*",
         }
     )
     height: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentalign: Optional[MathIndentalign] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1473,29 +1473,29 @@
             "type": "Attribute",
         }
     )
     indentshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentshiftfirst: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentshiftlast: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indenttarget: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1506,15 +1506,15 @@
             "type": "Attribute",
         }
     )
     leftoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     length: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1537,22 +1537,22 @@
             "type": "Attribute",
         }
     )
     lineleading: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     linethickness: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     location: Optional[MathLocation] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1569,62 +1569,62 @@
             "type": "Attribute",
         }
     )
     lspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mathsize: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mathvariant: Optional[MathMathvariant] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     maxsize: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     minlabelspacing: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     minsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     movablelimits: Optional[MathMovablelimits] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     mslinethickness: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     notation: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1647,15 +1647,15 @@
             "type": "Attribute",
         }
     )
     rightoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     rowalign: List[Verticalalign] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
             "tokens": True,
@@ -1668,15 +1668,15 @@
             "tokens": True,
         }
     )
     rowspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     rowspan: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -1688,15 +1688,15 @@
             "type": "Attribute",
         }
     )
     rspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     selection: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1737,42 +1737,42 @@
             "type": "Attribute",
         }
     )
     subscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     superscriptshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     symmetric: Optional[MathSymmetric] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     valign: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     width: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1822,15 +1822,15 @@
             "type": "Attribute",
         }
     )
     maxwidth: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     overflow: Optional[MathOverflow] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -1842,31 +1842,31 @@
         }
     )
     altimg_width: Optional[str] = field(
         default=None,
         metadata={
             "name": "altimg-width",
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     altimg_height: Optional[str] = field(
         default=None,
         metadata={
             "name": "altimg-height",
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     altimg_valign: Optional[Union[str, MathValue]] = field(
         default=None,
         metadata={
             "name": "altimg-valign",
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     alttext: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/math_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/math_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,29 +80,29 @@
             "type": "Attribute",
         }
     )
     width: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     height: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     valign: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     alt: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -119,15 +119,15 @@
             "type": "Attribute",
         }
     )
     mathsize: Optional[Union[str, MglyphValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     fontfamily: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -144,15 +144,15 @@
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mglyph_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 from .malignmark import Malignmark
 from .mglyph import Mglyph
-from .mi_dir import MiDir
-from .mi_fontstyle import MiFontstyle
-from .mi_fontweight import MiFontweight
-from .mi_mathvariant import MiMathvariant
-from .mi_value import MiValue
+from .mn_dir import MnDir
+from .mn_fontstyle import MnFontstyle
+from .mn_fontweight import MnFontweight
+from .mn_mathvariant import MnMathvariant
+from .mn_value import MnValue
 
 __NAMESPACE__ = "http://www.w3.org/1998/Math/MathML"
 
 
 @dataclass
-class Mi:
+class Mn:
     class Meta:
-        name = "mi"
+        name = "mn"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -66,73 +66,73 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MiValue]] = field(
+    mathbackground: Optional[Union[str, MnValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathvariant: Optional[MiMathvariant] = field(
+    mathvariant: Optional[MnMathvariant] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    mathsize: Optional[Union[str, MiValue]] = field(
+    mathsize: Optional[Union[str, MnValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
-    dir: Optional[MiDir] = field(
+    dir: Optional[MnDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontfamily: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontweight: Optional[MiFontweight] = field(
+    fontweight: Optional[MnFontweight] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontstyle: Optional[MiFontstyle] = field(
+    fontstyle: Optional[MnFontstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    background: Optional[Union[str, MiValue]] = field(
+    background: Optional[Union[str, MnValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     content: List[object] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/minus.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/minus.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mlabeledtr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mlabeledtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 from .malignmark import Malignmark
 from .mglyph import Mglyph
-from .mn_dir import MnDir
-from .mn_fontstyle import MnFontstyle
-from .mn_fontweight import MnFontweight
-from .mn_mathvariant import MnMathvariant
-from .mn_value import MnValue
+from .mi_dir import MiDir
+from .mi_fontstyle import MiFontstyle
+from .mi_fontweight import MiFontweight
+from .mi_mathvariant import MiMathvariant
+from .mi_value import MiValue
 
 __NAMESPACE__ = "http://www.w3.org/1998/Math/MathML"
 
 
 @dataclass
-class Mn:
+class Mi:
     class Meta:
-        name = "mn"
+        name = "mi"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -66,73 +66,73 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MnValue]] = field(
+    mathbackground: Optional[Union[str, MiValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathvariant: Optional[MnMathvariant] = field(
+    mathvariant: Optional[MiMathvariant] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    mathsize: Optional[Union[str, MnValue]] = field(
+    mathsize: Optional[Union[str, MiValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
-    dir: Optional[MnDir] = field(
+    dir: Optional[MiDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontfamily: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontweight: Optional[MnFontweight] = field(
+    fontweight: Optional[MiFontweight] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontstyle: Optional[MnFontstyle] = field(
+    fontstyle: Optional[MiFontstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    background: Optional[Union[str, MnValue]] = field(
+    background: Optional[Union[str, MiValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     content: List[object] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mn_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             "type": "Attribute",
         }
     )
     mathsize: Optional[Union[str, MoValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     dir: Optional[MoDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -127,15 +127,15 @@
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
@@ -166,22 +166,22 @@
             "type": "Attribute",
         }
     )
     lspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     rspace: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     stretchy: Optional[MoStretchy] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -192,22 +192,22 @@
             "type": "Attribute",
         }
     )
     maxsize: Optional[Union[str, MoValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     minsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     largeop: Optional[MoLargeop] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -230,15 +230,15 @@
             "type": "Attribute",
         }
     )
     lineleading: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     linebreakstyle: Optional[MoLinebreakstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -255,15 +255,15 @@
             "type": "Attribute",
         }
     )
     indentshift: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indenttarget: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -274,28 +274,28 @@
             "type": "Attribute",
         }
     )
     indentshiftfirst: Optional[Union[str, MoValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     indentalignlast: Optional[MoIndentalignlast] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     indentshiftlast: Optional[Union[str, MoValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mo_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mprescripts.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mprescripts.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             "type": "Attribute",
         }
     )
     mathsize: Optional[Union[str, MsValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     dir: Optional[MsDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -114,15 +114,15 @@
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/ms_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/msline.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/msline.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,24 +83,24 @@
             "type": "Attribute",
         }
     )
     leftoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     rightoverhang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     mslinethickness: Optional[Union[str, MslineValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Dict, List, Optional, Union
-from .mspace_dir import MspaceDir
-from .mspace_fontstyle import MspaceFontstyle
-from .mspace_fontweight import MspaceFontweight
-from .mspace_linebreak import MspaceLinebreak
-from .mspace_mathvariant import MspaceMathvariant
-from .mspace_value import MspaceValue
+from .malignmark import Malignmark
+from .mglyph import Mglyph
+from .mtext_dir import MtextDir
+from .mtext_fontstyle import MtextFontstyle
+from .mtext_fontweight import MtextFontweight
+from .mtext_mathvariant import MtextMathvariant
+from .mtext_value import MtextValue
 
 __NAMESPACE__ = "http://www.w3.org/1998/Math/MathML"
 
 
 @dataclass
-class Mspace:
+class Mtext:
     class Meta:
-        name = "mspace"
+        name = "mtext"
         namespace = "http://www.w3.org/1998/Math/MathML"
 
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -65,99 +66,90 @@
     mathcolor: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathbackground: Optional[Union[str, MspaceValue]] = field(
+    mathbackground: Optional[Union[str, MtextValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    mathvariant: Optional[MspaceMathvariant] = field(
+    mathvariant: Optional[MtextMathvariant] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    mathsize: Optional[Union[str, MspaceValue]] = field(
+    mathsize: Optional[Union[str, MtextValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
-    dir: Optional[MspaceDir] = field(
+    dir: Optional[MtextDir] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontfamily: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontweight: Optional[MspaceFontweight] = field(
+    fontweight: Optional[MtextFontweight] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    fontstyle: Optional[MspaceFontstyle] = field(
+    fontstyle: Optional[MtextFontstyle] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     fontsize: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     color: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    background: Optional[Union[str, MspaceValue]] = field(
+    background: Optional[Union[str, MtextValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
-    width: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
-        }
-    )
-    height: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
-        }
-    )
-    depth: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
-        }
-    )
-    linebreak: Optional[MspaceLinebreak] = field(
-        default=None,
+    content: List[object] = field(
+        default_factory=list,
         metadata={
-            "type": "Attribute",
+            "type": "Wildcard",
+            "namespace": "##any",
+            "mixed": True,
+            "choices": (
+                {
+                    "name": "mglyph",
+                    "type": Mglyph,
+                },
+                {
+                    "name": "malignmark",
+                    "type": Malignmark,
+                },
+            ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mspace_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mstyle_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtable.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtable.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             "pattern": r"\s*((#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?)|[aA][qQ][uU][aA]|[bB][lL][aA][cC][kK]|[bB][lL][uU][eE]|[fF][uU][cC][hH][sS][iI][aA]|[gG][rR][aA][yY]|[gG][rR][eE][eE][nN]|[lL][iI][mM][eE]|[mM][aA][rR][oO][oO][nN]|[nN][aA][vV][yY]|[oO][lL][iI][vV][eE]|[pP][uU][rR][pP][lL][eE]|[rR][eE][dD]|[sS][iI][lL][vV][eE][rR]|[tT][eE][aA][lL]|[wW][hH][iI][tT][eE]|[yY][eE][lL][lL][oO][wW])\s*",
         }
     )
     align: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*(top|bottom|center|baseline|axis)\s*[0-9]*",
+            "pattern": r"\s*(top|bottom|center|baseline|axis)(\s+-?[0-9]+)?\s*",
         }
     )
     rowalign: List[Verticalalign] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
             "tokens": True,
@@ -134,30 +134,30 @@
             "tokens": True,
         }
     )
     width: Optional[Union[str, MtableValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
     rowspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     columnspacing: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
             "tokens": True,
         }
     )
     rowlines: List[Linestyle] = field(
         default_factory=list,
         metadata={
             "type": "Attribute",
@@ -209,10 +209,10 @@
             "type": "Attribute",
         }
     )
     minlabelspacing: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "pattern": r"\s*((-?[0-9]*(\.[0-9]*)?(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
+            "pattern": r"\s*((-?[0-9]*([0-9]\.?|\.[0-9])[0-9]*(e[mx]|in|cm|mm|p[xtc]|%)?)|(negative)?((very){0,2}thi(n|ck)|medium)mathspace)\s*",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtext_mathvariant.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/mtr.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/mtr.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/neq.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/neq.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/none.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/none.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/power.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/power.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/quotient.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/quotient.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/real.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/real.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/rem.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/rem.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/root.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/root.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/share.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/share.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1998/math/math_ml/tendsto.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/tendsto.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/arc_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/arc_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .actuate_value import ActuateValue
-from .show_value import ShowValue
-from .type_value import TypeValue
+from .actuate_type import ActuateType
+from .show_type import ShowType
+from .type_type import TypeType
 
 __NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
 class ArcType:
     """
@@ -18,17 +18,17 @@
     :ivar actuate:
     :ivar from_value:
     :ivar to: from and to have default behavior when values are missing
     """
     class Meta:
         name = "arcType"
 
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.ARC,
+        default=TypeType.ARC,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
             "required": True,
         }
     )
     arcrole: Optional[str] = field(
@@ -41,22 +41,22 @@
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     from_value: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/extended.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/extended.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .type_value import TypeValue
+from .type_type import TypeType
 
 __NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
 class Extended:
     """Intended for use as the type of user-declared elements to make them extended
@@ -14,17 +14,17 @@
     Note that the elements referenced in the content model are all
     abstract. The intention is that by simply declaring elements with
     these as their substitutionGroup, all the right things will happen.
     """
     class Meta:
         name = "extended"
 
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.EXTENDED,
+        default=TypeType.EXTENDED,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
             "required": True,
         }
     )
     role: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/locator_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/locator_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .type_value import TypeValue
+from .type_type import TypeType
 
 __NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
 class LocatorType:
     """
@@ -15,17 +15,17 @@
     :ivar title:
     :ivar label: label is not required, but locators have no particular
         XLink function if they are not labeled.
     """
     class Meta:
         name = "locatorType"
 
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.LOCATOR,
+        default=TypeType.LOCATOR,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
             "required": True,
         }
     )
     href: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/resource_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,70 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .type_value import TypeValue
+from .actuate_type import ActuateType
+from .show_type import ShowType
+from .type_type import TypeType
 
 __NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
-class ResourceType:
+class Simple:
+    """
+    Intended for use as the type of user-declared elements to make them simple
+    links.
+    """
     class Meta:
-        name = "resourceType"
+        name = "simple"
 
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.RESOURCE,
+        default=TypeType.SIMPLE,
+        metadata={
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/1999/xlink",
+        }
+    )
+    href: Optional[str] = field(
+        default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
-            "required": True,
         }
     )
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
+    arcrole: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/1999/xlink",
+        }
+    )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    label: Optional[str] = field(
+    show: Optional[ShowType] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/1999/xlink",
+        }
+    )
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     content: List[object] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/simple.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_award_recipient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional
-from .actuate_value import ActuateValue
-from .show_value import ShowValue
-from .type_value import TypeValue
-
-__NAMESPACE__ = "http://www.w3.org/1999/xlink"
+from typing import List, Optional, Union
+from .access_date import (
+    Institution,
+    InstitutionWrap,
+    Name,
+    NameAlternatives,
+    StringName,
+)
+from .contrib_id import ContribId
+from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class Simple:
+class PrincipalAwardRecipient:
     """
-    Intended for use as the type of user-declared elements to make them simple
-    links.
+    <div> <h3>Principal Award Recipient</h3> </div>
     """
     class Meta:
-        name = "simple"
+        name = "principal-award-recipient"
 
-    type: TypeValue = field(
-        init=False,
-        default=TypeValue.SIMPLE,
-        metadata={
-            "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
-        }
-    )
-    href: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
-        }
-    )
-    role: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
-        }
-    )
-    arcrole: Optional[str] = field(
+    id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    title: Optional[str] = field(
+    specific_use: Optional[str] = field(
         default=None,
         metadata={
+            "name": "specific-use",
             "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    base: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    lang: Optional[Union[str, LangValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/1999/xlink",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
+            "choices": (
+                {
+                    "name": "contrib-id",
+                    "type": ContribId,
+                },
+                {
+                    "name": "name",
+                    "type": Name,
+                },
+                {
+                    "name": "name-alternatives",
+                    "type": NameAlternatives,
+                },
+                {
+                    "name": "institution",
+                    "type": Institution,
+                },
+                {
+                    "name": "institution-wrap",
+                    "type": InstitutionWrap,
+                },
+                {
+                    "name": "string-name",
+                    "type": StringName,
+                },
+            ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/org/w3/pkg_1999/xlink/title_elt_type.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/title_elt_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
-from .type_value import TypeValue
+from .type_type import TypeType
 from ...xml.pkg_1998.namespace.lang_value import LangValue
 
 __NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
 class TitleEltType:
@@ -15,17 +15,17 @@
         motivation for title elements in addition to attributes, and so
         is provided here for convenience.
     :ivar content:
     """
     class Meta:
         name = "titleEltType"
 
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.TITLE,
+        default=TypeType.TITLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
             "required": True,
         }
     )
     lang: Optional[Union[str, LangValue]] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/other_abstract.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_abstract.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/other_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/other_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/overline_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_end.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/overline_start.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/overline_start.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/page_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_count.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/page_range.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/page_range.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pagination.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pagination.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/param.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/param.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
 class Param:
     name: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/personal_name_subject.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_date.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .suffix_1 import Suffix1
 
 
 @dataclass
-class PersonalNameSubject:
-    last_name: Optional[str] = field(
+class PubDate:
+    year: Optional[str] = field(
         default=None,
         metadata={
-            "name": "LastName",
+            "name": "Year",
             "type": "Element",
-            "required": True,
         }
     )
-    fore_name: Optional[str] = field(
+    month: Optional[str] = field(
         default=None,
         metadata={
-            "name": "ForeName",
+            "name": "Month",
             "type": "Element",
         }
     )
-    initials: Optional[str] = field(
+    day: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Initials",
+            "name": "Day",
             "type": "Element",
         }
     )
-    suffix: Optional[Suffix1] = field(
+    season: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Suffix",
+            "name": "Season",
+            "type": "Element",
+        }
+    )
+    medline_date: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "MedlineDate",
             "type": "Element",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/postal_code.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/postal_code.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/principal_award_recipient.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/principal_investigator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
 from .access_date import (
-    Institution,
-    InstitutionWrap,
     Name,
     NameAlternatives,
     StringName,
 )
 from .contrib_id import ContribId
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class PrincipalAwardRecipient:
+class PrincipalInvestigator:
     """
-    <div> <h3>Principal Award Recipient</h3> </div>
+    <div> <h3>Principal Investigator Recipient</h3> </div>
     """
     class Meta:
-        name = "principal-award-recipient"
+        name = "principal-investigator"
 
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
@@ -63,21 +61,13 @@
                     "type": Name,
                 },
                 {
                     "name": "name-alternatives",
                     "type": NameAlternatives,
                 },
                 {
-                    "name": "institution",
-                    "type": Institution,
-                },
-                {
-                    "name": "institution-wrap",
-                    "type": InstitutionWrap,
-                },
-                {
                     "name": "string-name",
                     "type": StringName,
                 },
             ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/principal_investigator.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/season.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
-from .access_date import (
-    Name,
-    NameAlternatives,
-    StringName,
-)
-from .contrib_id import ContribId
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class PrincipalInvestigator:
+class Season:
     """
-    <div> <h3>Principal Investigator Recipient</h3> </div>
+    <div> <h3>Season</h3> </div>
     """
     class Meta:
-        name = "principal-investigator"
+        name = "season"
 
+    content_type: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "content-type",
+            "type": "Attribute",
+        }
+    )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     specific_use: Optional[str] = field(
@@ -47,27 +48,9 @@
     )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
-            "choices": (
-                {
-                    "name": "contrib-id",
-                    "type": ContribId,
-                },
-                {
-                    "name": "name",
-                    "type": Name,
-                },
-                {
-                    "name": "name-alternatives",
-                    "type": NameAlternatives,
-                },
-                {
-                    "name": "string-name",
-                    "type": StringName,
-                },
-            ),
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/processing_meta.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/processing_meta.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_start.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass
-class PubDate1:
+class UnderlineStart:
+    """
+    <div> <h3>Underline Start</h3> </div>
+    """
     class Meta:
-        name = "PubDate"
+        name = "underline-start"
 
-    year: Optional[str] = field(
+    id: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Year",
-            "type": "Element",
+            "type": "Attribute",
+            "required": True,
         }
     )
-    month: Optional[str] = field(
+    specific_use: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Month",
-            "type": "Element",
+            "name": "specific-use",
+            "type": "Attribute",
         }
     )
-    day: Optional[str] = field(
+    base: Optional[str] = field(
         default=None,
         metadata={
-            "name": "Day",
-            "type": "Element",
-        }
-    )
-    season: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "Season",
-            "type": "Element",
-        }
-    )
-    medline_date: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "MedlineDate",
-            "type": "Element",
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_2.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .month import Month
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .season import Season
 from .year import Year
 
 
 @dataclass
-class PubDate2:
+class PubDate:
     """
     <div> <h3>Publication Date</h3> </div>
     """
     class Meta:
         name = "pub-date"
 
     day: List[Day] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_date_not_available.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_date_not_available.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_history.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/pub_history.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/restricted_by.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 
 
 @dataclass
-class PubId:
+class RestrictedBy:
     """
-    <div> <h3>Publication Identifier For a Cited Publication</h3> </div>
+    <div> <h3>Restricted-by Model</h3> </div>
     """
     class Meta:
-        name = "pub-id"
+        name = "restricted-by"
 
     assigning_authority: Optional[str] = field(
         default=None,
         metadata={
             "name": "assigning-authority",
             "type": "Attribute",
         }
     )
-    custom_type: Optional[str] = field(
+    designator: Optional[str] = field(
         default=None,
         metadata={
-            "name": "custom-type",
             "type": "Attribute",
         }
     )
     hreflang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -36,29 +35,42 @@
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    pub_id_type: Optional[str] = field(
+    vocab: Optional[str] = field(
         default=None,
         metadata={
-            "name": "pub-id-type",
             "type": "Attribute",
         }
     )
-    specific_use: Optional[str] = field(
+    vocab_identifier: Optional[str] = field(
         default=None,
         metadata={
-            "name": "specific-use",
+            "name": "vocab-identifier",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    vocab_term: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "vocab-term",
+            "type": "Attribute",
+        }
+    )
+    vocab_term_identifier: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "vocab-term-identifier",
+            "type": "Attribute",
+        }
+    )
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -71,31 +83,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pub_med_pub_date.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pub_med_pub_date.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/publisher.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/publisher.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/publisher_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/word_count.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .publisher_name_1 import PublisherName1
 
 
 @dataclass
-class Publisher1:
+class WordCount:
+    """
+    <div> <h3>Word Count</h3> </div>
+    """
     class Meta:
-        name = "Publisher"
+        name = "word-count"
 
-    publisher_name: Optional[PublisherName1] = field(
+    count: Optional[str] = field(
         default=None,
         metadata={
-            "name": "PublisherName",
-            "type": "Element",
+            "type": "Attribute",
             "required": True,
         }
     )
-    publisher_location: Optional[str] = field(
+    id: Optional[str] = field(
         default=None,
         metadata={
-            "name": "PublisherLocation",
-            "type": "Element",
+            "type": "Attribute",
+        }
+    )
+    base: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/publisher_2.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/tex_math.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
-from .access_date import (
-    PublisherLoc,
-    PublisherName,
-)
+from .tex_math_notation import TexMathNotation
 
 
 @dataclass
-class Publisher2:
+class TexMath:
     """
-    <div> <h3>Publisher</h3> </div>
+    <div> <h3>Tex Math Equation</h3> </div>
     """
     class Meta:
-        name = "publisher"
+        name = "tex-math"
 
-    publisher_name: List[PublisherName] = field(
-        default_factory=list,
+    content_type: Optional[str] = field(
+        default=None,
         metadata={
-            "name": "publisher-name",
-            "type": "Element",
-            "sequence": 1,
+            "name": "content-type",
+            "type": "Attribute",
         }
     )
-    publisher_loc: List[PublisherLoc] = field(
-        default_factory=list,
+    id: Optional[str] = field(
+        default=None,
         metadata={
-            "name": "publisher-loc",
-            "type": "Element",
-            "sequence": 1,
+            "type": "Attribute",
         }
     )
-    content_type: Optional[str] = field(
+    notation: Optional[TexMathNotation] = field(
         default=None,
         metadata={
-            "name": "content-type",
             "type": "Attribute",
         }
     )
-    id: Optional[str] = field(
+    specific_use: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "specific-use",
+            "type": "Attribute",
+        }
+    )
+    version: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     base: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
+    content: List[object] = field(
+        default_factory=list,
+        metadata={
+            "type": "Wildcard",
+            "namespace": "##any",
+            "mixed": True,
+        }
+    )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/publisher_name_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/coi_statement.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class PublisherName1:
-    class Meta:
-        name = "PublisherName"
-
+class CoiStatement:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/ref_count.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
-from .medline_citation import MedlineCitation
-from .pubmed_data import PubmedData
 
 
 @dataclass
-class PubmedArticle:
-    medline_citation: Optional[MedlineCitation] = field(
+class RefCount:
+    """
+    <div> <h3>Reference Count</h3> </div>
+    """
+    class Meta:
+        name = "ref-count"
+
+    count: Optional[str] = field(
         default=None,
         metadata={
-            "name": "MedlineCitation",
-            "type": "Element",
+            "type": "Attribute",
             "required": True,
         }
     )
-    pubmed_data: Optional[PubmedData] = field(
+    id: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    base: Optional[str] = field(
         default=None,
         metadata={
-            "name": "PubmedData",
-            "type": "Element",
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_article_set.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_article_set.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_book_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_book_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 from .article_id_list import ArticleIdList
-from .history_1 import History1
+from .history import History
 from .object_list import ObjectList
 
 
 @dataclass
 class PubmedBookData:
-    history: Optional[History1] = field(
+    history: Optional[History] = field(
         default=None,
         metadata={
             "name": "History",
             "type": "Element",
         }
     )
     publication_status: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/pubmed_data.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/pubmed_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional
 from .article_id_list import ArticleIdList
-from .history_1 import History1
+from .history import History
 from .object_list import ObjectList
 from .reference_list import ReferenceList
 
 
 @dataclass
 class PubmedData:
-    history: Optional[History1] = field(
+    history: Optional[History] = field(
         default=None,
         metadata={
             "name": "History",
             "type": "Element",
         }
     )
     publication_status: Optional[str] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/qualifier_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/qualifier_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/ref_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/table_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass
-class RefCount:
+class TableCount:
     """
-    <div> <h3>Reference Count</h3> </div>
+    <div> <h3>Table Count</h3> </div>
     """
     class Meta:
-        name = "ref-count"
+        name = "table-count"
 
     count: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/reference.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/reference_list.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/reference_list.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/resource_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/resource_id.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_id.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/resource_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     SansSerif,
     Sc,
     Strike,
     Sub,
     Sup,
     Underline,
 )
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 
 
@@ -55,15 +55,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -76,31 +76,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/resource_wrap.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/resource_wrap.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/response.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/response.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/restricted_by.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/award_desc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,37 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from typing import List, Optional, Union
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
+from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class RestrictedBy:
+class AwardDesc:
     """
-    <div> <h3>Restricted-by Model</h3> </div>
+    <div> <h3>Award Description</h3> </div>
     """
     class Meta:
-        name = "restricted-by"
+        name = "award-desc"
 
-    assigning_authority: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "assigning-authority",
-            "type": "Attribute",
-        }
-    )
-    designator: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
     hreflang: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    vocab: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    vocab_identifier: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "vocab-identifier",
-            "type": "Attribute",
-        }
-    )
-    vocab_term: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "vocab-term",
-            "type": "Attribute",
-        }
-    )
-    vocab_term_identifier: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "vocab-term-identifier",
-            "type": "Attribute",
-        }
-    )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -83,43 +44,50 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
+    lang: Optional[Union[str, LangValue]] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
+        }
+    )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
         }
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/rp.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rp.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/rt.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/rt.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/season.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
+from .contributed_resource_group import ContributedResourceGroup
+from .funding_group import FundingGroup
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class Season:
+class SupportGroup:
     """
-    <div> <h3>Season</h3> </div>
+    <div> <h3>Support Group</h3> </div>
     """
     class Meta:
-        name = "season"
+        name = "support-group"
 
-    content_type: Optional[str] = field(
-        default=None,
+    funding_group: List[FundingGroup] = field(
+        default_factory=list,
         metadata={
-            "name": "content-type",
-            "type": "Attribute",
+            "name": "funding-group",
+            "type": "Element",
+        }
+    )
+    contributed_resource_group: List[ContributedResourceGroup] = field(
+        default_factory=list,
+        metadata={
+            "name": "contributed-resource-group",
+            "type": "Element",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
@@ -42,15 +51,7 @@
     lang: Optional[Union[str, LangValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
-    content: List[object] = field(
-        default_factory=list,
-        metadata={
-            "type": "Wildcard",
-            "namespace": "##any",
-            "mixed": True,
-        }
-    )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/section.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/section.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/section_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/underline_end.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,40 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional
-from .access_date import (
-    Sub,
-    Sup,
-)
-from .u import (
-    B,
-    I,
-    U,
-)
+from typing import Optional
 
 
 @dataclass
-class SectionTitle:
-    book: Optional[str] = field(
+class UnderlineEnd:
+    """
+    <div> <h3>Underline End</h3> </div>
+    """
+    class Meta:
+        name = "underline-end"
+
+    id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    sec: Optional[str] = field(
+    rid: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
+            "required": True,
         }
     )
-    part: Optional[str] = field(
+    specific_use: Optional[str] = field(
         default=None,
         metadata={
+            "name": "specific-use",
             "type": "Attribute",
         }
     )
-    content: List[object] = field(
-        default_factory=list,
+    base: Optional[str] = field(
+        default=None,
         metadata={
-            "type": "Wildcard",
-            "namespace": "##any",
-            "mixed": True,
-            "choices": (
-                {
-                    "name": "b",
-                    "type": B,
-                },
-                {
-                    "name": "i",
-                    "type": I,
-                },
-                {
-                    "name": "sup",
-                    "type": Sup,
-                },
-                {
-                    "name": "sub",
-                    "type": Sub,
-                },
-                {
-                    "name": "u",
-                    "type": U,
-                },
-            ),
+            "type": "Attribute",
+            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/self_uri.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/self_uri.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     Xref,
 )
 from .hr import Hr
 from .index_term_range_end import IndexTermRangeEnd
 from .milestone_end import MilestoneEnd
 from .milestone_start import MilestoneStart
 from .org.w3.pkg_1998.math.math_ml.math import Math
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .tex_math import TexMath
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 
@@ -89,15 +89,15 @@
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -110,31 +110,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/series_text.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_text.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/series_title.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/series_title.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/sig.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/sig_block.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sig_block.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/state.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/state.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/string_conf.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/string_conf.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/sub_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/collective_name.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class Sub1:
-    class Meta:
-        name = "sub"
-
+class CollectiveName:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/sub_article.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/sub_article.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/suffix_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suffix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class Suffix1:
-    class Meta:
-        name = "Suffix"
-
+class Suffix:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/sup_1.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/publisher_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List
-from .access_date import (
-    Sub,
-    Sup,
-)
 from .u import (
     B,
     I,
+    Sub,
+    Sup,
     U,
 )
 
 
 @dataclass
-class Sup1:
-    class Meta:
-        name = "sup"
-
+class PublisherName:
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
             "mixed": True,
             "choices": (
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/suppl_mesh_name.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/suppl_mesh_name.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/support_description.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_description.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/support_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/year.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
-from .contributed_resource_group import ContributedResourceGroup
-from .funding_group import FundingGroup
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 
 
 @dataclass
-class SupportGroup:
+class Year:
     """
-    <div> <h3>Support Group</h3> </div>
+    <div> <h3>Year</h3> </div>
     """
     class Meta:
-        name = "support-group"
+        name = "year"
 
-    funding_group: List[FundingGroup] = field(
-        default_factory=list,
+    calendar: Optional[str] = field(
+        default=None,
         metadata={
-            "name": "funding-group",
-            "type": "Element",
+            "type": "Attribute",
         }
     )
-    contributed_resource_group: List[ContributedResourceGroup] = field(
-        default_factory=list,
+    content_type: Optional[str] = field(
+        default=None,
         metadata={
-            "name": "contributed-resource-group",
-            "type": "Element",
+            "name": "content-type",
+            "type": "Attribute",
         }
     )
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
+    iso_8601_date: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "iso-8601-date",
+            "type": "Attribute",
+        }
+    )
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
@@ -51,7 +55,15 @@
     lang: Optional[Union[str, LangValue]] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
+    content: List[object] = field(
+        default_factory=list,
+        metadata={
+            "type": "Wildcard",
+            "namespace": "##any",
+            "mixed": True,
+        }
+    )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/support_source.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/support_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     Xref,
 )
 from .hr import Hr
 from .index_term_range_end import IndexTermRangeEnd
 from .milestone_end import MilestoneEnd
 from .milestone_start import MilestoneStart
 from .org.w3.pkg_1998.math.math_ml.math import Math
-from .org.w3.pkg_1999.xlink.actuate_value import ActuateValue
-from .org.w3.pkg_1999.xlink.show_value import ShowValue
-from .org.w3.pkg_1999.xlink.type_value import TypeValue
+from .org.w3.pkg_1999.xlink.actuate_type import ActuateType
+from .org.w3.pkg_1999.xlink.show_type import ShowType
+from .org.w3.pkg_1999.xlink.type_type import TypeType
 from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
 from .overline_end import OverlineEnd
 from .overline_start import OverlineStart
 from .tex_math import TexMath
 from .underline_end import UnderlineEnd
 from .underline_start import UnderlineStart
 
@@ -97,15 +97,15 @@
     support_type: Optional[str] = field(
         default=None,
         metadata={
             "name": "support-type",
             "type": "Attribute",
         }
     )
-    actuate: Optional[ActuateValue] = field(
+    actuate: Optional[ActuateType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     href: Optional[str] = field(
@@ -118,31 +118,31 @@
     role: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    show: Optional[ShowValue] = field(
+    show: Optional[ShowType] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    type: TypeValue = field(
+    type: TypeType = field(
         init=False,
-        default=TypeValue.SIMPLE,
+        default=TypeType.SIMPLE,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     base: Optional[str] = field(
         default=None,
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/table_count.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
+from .url_lang import UrlLang
+from .url_type import UrlType
 
 
 @dataclass
-class TableCount:
-    """
-    <div> <h3>Table Count</h3> </div>
-    """
+class Url:
     class Meta:
-        name = "table-count"
+        name = "URL"
 
-    count: Optional[str] = field(
+    lang: Optional[UrlLang] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "required": True,
         }
     )
-    id: Optional[str] = field(
+    type: Optional[UrlType] = field(
         default=None,
         metadata={
+            "name": "Type",
             "type": "Attribute",
         }
     )
-    base: Optional[str] = field(
-        default=None,
+    value: str = field(
+        default="",
         metadata={
-            "type": "Attribute",
-            "namespace": "http://www.w3.org/XML/1998/namespace",
+            "required": True,
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/tex_math.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1998/math/math_ml/annotation_xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,90 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional
-from .tex_math_notation import TexMathNotation
+from typing import Dict, List, Optional
+from .annotation_xml_model import AnnotationXmlModel
+
+__NAMESPACE__ = "http://www.w3.org/1998/Math/MathML"
 
 
 @dataclass
-class TexMath:
-    """
-    <div> <h3>Tex Math Equation</h3> </div>
-    """
+class AnnotationXml(AnnotationXmlModel):
     class Meta:
-        name = "tex-math"
+        name = "annotation-xml"
+        namespace = "http://www.w3.org/1998/Math/MathML"
 
-    content_type: Optional[str] = field(
+    id: Optional[str] = field(
         default=None,
         metadata={
-            "name": "content-type",
             "type": "Attribute",
         }
     )
-    id: Optional[str] = field(
+    xref: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    notation: Optional[TexMathNotation] = field(
+    class_value: List[str] = field(
+        default_factory=list,
+        metadata={
+            "name": "class",
+            "type": "Attribute",
+            "tokens": True,
+        }
+    )
+    style: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    specific_use: Optional[str] = field(
+    href: Optional[str] = field(
         default=None,
         metadata={
-            "name": "specific-use",
             "type": "Attribute",
         }
     )
-    version: Optional[str] = field(
+    other: Optional[object] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    base: Optional[str] = field(
+    other_attributes: Dict[str, str] = field(
+        default_factory=dict,
+        metadata={
+            "type": "Attributes",
+            "namespace": "##other",
+        }
+    )
+    cd: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
-    content: List[object] = field(
-        default_factory=list,
+    name: Optional[str] = field(
+        default=None,
         metadata={
-            "type": "Wildcard",
-            "namespace": "##any",
-            "mixed": True,
+            "type": "Attribute",
+        }
+    )
+    encoding: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    definition_url: Optional[str] = field(
+        default=None,
+        metadata={
+            "name": "definitionURL",
+            "type": "Attribute",
+        }
+    )
+    src: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/trans_abstract.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     AnswerSet,
     Array,
     BlockAlternatives,
     BoxedText,
     ChemStructWrap,
     Code,
     DefList,
+    DispFormula,
     DispFormulaGroup,
-    DispFormula2,
     DispQuote,
     Explanation,
     Fig,
     FigGroup,
     FnGroup,
     Glossary,
     Graphic,
@@ -217,15 +217,15 @@
     table_wrap_group: List[TableWrapGroup] = field(
         default_factory=list,
         metadata={
             "name": "table-wrap-group",
             "type": "Element",
         }
     )
-    disp_formula: List[DispFormula2] = field(
+    disp_formula: List[DispFormula] = field(
         default_factory=list,
         metadata={
             "name": "disp-formula",
             "type": "Element",
         }
     )
     disp_formula_group: List[DispFormulaGroup] = field(
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/trans_subtitle.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_subtitle.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/trans_title_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/trans_title_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/underline_end.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/niso/schemas/ali/pkg_1/free_to_read.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
 from typing import Optional
 
+__NAMESPACE__ = "http://www.niso.org/schemas/ali/1.0/"
+
 
 @dataclass
-class UnderlineEnd:
+class FreeToRead:
     """
-    <div> <h3>Underline End</h3> </div>
+    <div> <h3>Free to Read (Niso Ali)</h3> </div>
     """
     class Meta:
-        name = "underline-end"
+        name = "free_to_read"
+        namespace = "http://www.niso.org/schemas/ali/1.0/"
 
-    id: Optional[str] = field(
+    content_type: Optional[str] = field(
         default=None,
         metadata={
+            "name": "content-type",
             "type": "Attribute",
         }
     )
-    rid: Optional[str] = field(
+    end_date: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
+    id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "required": True,
         }
     )
     specific_use: Optional[str] = field(
         default=None,
         metadata={
             "name": "specific-use",
             "type": "Attribute",
         }
     )
+    start_date: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Attribute",
+        }
+    )
     base: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "namespace": "http://www.w3.org/XML/1998/namespace",
         }
     )
```

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/url_lang.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/pubmed/url_lang.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/volume_issue_group.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/volume_issue_group.py`

 * *Files identical despite different names*

### Comparing `pubmed_types-0.1.2/src/pubmed_types/models/year.py` & `pubmed_types-0.2.0.dev0/src/pubmed_types/models/jats/org/w3/pkg_1999/xlink/resource_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,48 @@
 from dataclasses import field
 from pydantic.dataclasses import dataclass
-from typing import List, Optional, Union
-from .org.w3.xml.pkg_1998.namespace.lang_value import LangValue
+from typing import List, Optional
+from .type_type import TypeType
+
+__NAMESPACE__ = "http://www.w3.org/1999/xlink"
 
 
 @dataclass
-class Year:
-    """
-    <div> <h3>Year</h3> </div>
-    """
+class ResourceType:
     class Meta:
-        name = "year"
+        name = "resourceType"
 
-    calendar: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    content_type: Optional[str] = field(
-        default=None,
-        metadata={
-            "name": "content-type",
-            "type": "Attribute",
-        }
-    )
-    id: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Attribute",
-        }
-    )
-    iso_8601_date: Optional[str] = field(
-        default=None,
+    type: TypeType = field(
+        init=False,
+        default=TypeType.RESOURCE,
         metadata={
-            "name": "iso-8601-date",
             "type": "Attribute",
+            "namespace": "http://www.w3.org/1999/xlink",
+            "required": True,
         }
     )
-    specific_use: Optional[str] = field(
+    role: Optional[str] = field(
         default=None,
         metadata={
-            "name": "specific-use",
             "type": "Attribute",
+            "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    base: Optional[str] = field(
+    title: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/XML/1998/namespace",
+            "namespace": "http://www.w3.org/1999/xlink",
         }
     )
-    lang: Optional[Union[str, LangValue]] = field(
+    label: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
-            "namespace": "http://www.w3.org/XML/1998/namespace",
+            "namespace": "http://www.w3.org/1999/xlink",
         }
     )
     content: List[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "##any",
```

### Comparing `pubmed_types-0.1.2/PKG-INFO` & `pubmed_types-0.2.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed-types
-Version: 0.1.2
+Version: 0.2.0.dev0
 Summary: Pubmed XML parsing and typehints.
 Home-page: https://github.com/nicholas-schaub/pubmed-types
 License: MIT
 Author: Nick Schaub
 Author-email: nick.schaub@nih.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,32 +20,46 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Dist: xsdata-pydantic[cli,lxml,soap] (>=22.10,<23.0)
 Project-URL: Issues, https://github.com/nicholas-schaub/pubmed-types/issues
 Project-URL: Repository, https://github.com/nicholas-schaub/pubmed-types
 Description-Content-Type: text/markdown
 
-# pubmed-types (v0.1.2)
+# pubmed-types (v0.2.0-dev0)
 
 <p align="center">
     <img src="https://img.shields.io/pypi/dm/pubmed-types?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/pubmed-types?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/pubmed-types?style=flat-square"/>
-    <a href="https://github.com/tefra/xsdata-pydantic"><img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+    <a href="https://github.com/tefra/xsdata-pydantic">
+        <img alt="Built with: xsdata-pydantic" src="https://img.shields.io/badge/Built%20with-xsdata--pydantic-blue">
+    </a>
+    <a href="https://github.com/dbrgn/coverage-badge">
+        <img src="./images/coverage.svg">
+    </a>
 </p>
 
 ## Introduction
 
 A complete implementation of the XML schema for PMC Open Access articles and Pubmed
 article sets (citations).
 
 This package helps to parse PubMed XML data into Pydantic models. This validates the
 input xml data and provides typehints for working with the complex XML structures
 present in PubMed data.
 
+## Most Recent Changes
+
+* **Breaking Change:** The `parse_pubmed_xml` is replaced by `pmc_article` and `pubmed_article_set`.
+* More test coverage
+* Pubmed Articles can now parse MathML
+* Restructured code to separate out `jats` (pmc open access articles) and `pubmed` (pubmed article set)
+* One unit test with 99% coverage
+* Added [CHANGELOG.md](CHANGELOG.md)
+
 ## Why do I need this?
 
 PubMed keeps track of 10s of millions of research data, and a complex XML structure is
 used to store it. Parsing XML on its own is challenging enough. Add to it the feature
 rich data inside of each citation, and you will find yourself with hours or days of
 navigating the XML structure.
 
@@ -98,16 +112,14 @@
 
 ```bash
 Title: Lactate as a myokine and exerkine: drivers and signals of physiology and metabolism
 ```
 
 ### Example 2: A Pubmed baseline citation file
 
-### Example 1: A PMC Open Access Article
-
 ```python
 import gzip
 import urllib.request as request
 from contextlib import closing
 from pathlib import Path
 
 from pubmed_types import parse_pubmed_xml, PubmedArticleSet
```

#### html2text {}

```diff
@@ -1,67 +1,72 @@
-Metadata-Version: 2.1 Name: pubmed-types Version: 0.1.2 Summary: Pubmed XML
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
-markdown # pubmed-types (v0.1.2)
+markdown # pubmed-types (v0.2.0-dev0)
    [https://img.shields.io/pypi/dm/pubmed-types?style=flat-square] [https://
 img.shields.io/pypi/l/pubmed-types?style=flat-square] [https://img.shields.io/
-     pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic]
+pypi/v/pubmed-types?style=flat-square] [Built_with:_xsdata-pydantic] [./images/
+                                 coverage.svg]
 ## Introduction A complete implementation of the XML schema for PMC Open Access
 articles and Pubmed article sets (citations). This package helps to parse
 PubMed XML data into Pydantic models. This validates the input xml data and
 provides typehints for working with the complex XML structures present in
-PubMed data. ## Why do I need this? PubMed keeps track of 10s of millions of
-research data, and a complex XML structure is used to store it. Parsing XML on
-its own is challenging enough. Add to it the feature rich data inside of each
-citation, and you will find yourself with hours or days of navigating the XML
-structure. The approach here was to autogenerate Pydantic classes to parse the
-XML using the `xsdata-pydantic` tool. This approach has the benefit of making
-sure every piece of data is parsed properly, and an error is thrown is
-something is missing or incorrect. Instead of using dictionaries to hold the
-data, Pydantic classes have the benefit of providing type hints with tab
-completion for IDEs, making it easier to navigate the complex structure of the
-citation data. ## How do I use it? It is possible to use `xsdata-pydantic` and
-the autogenerated classes directly to parse an XML file, but we provide a
-convenience function to easily open PubMed XMl citations and PMC open access
-articles. ### Example 1: A PMC Open Access Article ```python import tarfile
-import urllib.request as request from contextlib import closing from pathlib
-import Path from pubmed_types import parse_pubmed_xml # Input file source and
-output file destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/
-oa_bulk/oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination =
-Path("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access
-article dataset from the FTP server with closing(request.urlopen(source)) as
-url: with tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall
-(destination) # 2. Parse the file file_path = destination.joinpath
-("PMC009xxxxxx").joinpath("PMC9970662.xml") full_text = parse_pubmed_xml
-(file_path) # 3. Print out the article title print(f"Title:
+PubMed data. ## Most Recent Changes * **Breaking Change:** The
+`parse_pubmed_xml` is replaced by `pmc_article` and `pubmed_article_set`. *
+More test coverage * Pubmed Articles can now parse MathML * Restructured code
+to separate out `jats` (pmc open access articles) and `pubmed` (pubmed article
+set) * One unit test with 99% coverage * Added [CHANGELOG.md](CHANGELOG.md) ##
+Why do I need this? PubMed keeps track of 10s of millions of research data, and
+a complex XML structure is used to store it. Parsing XML on its own is
+challenging enough. Add to it the feature rich data inside of each citation,
+and you will find yourself with hours or days of navigating the XML structure.
+The approach here was to autogenerate Pydantic classes to parse the XML using
+the `xsdata-pydantic` tool. This approach has the benefit of making sure every
+piece of data is parsed properly, and an error is thrown is something is
+missing or incorrect. Instead of using dictionaries to hold the data, Pydantic
+classes have the benefit of providing type hints with tab completion for IDEs,
+making it easier to navigate the complex structure of the citation data. ## How
+do I use it? It is possible to use `xsdata-pydantic` and the autogenerated
+classes directly to parse an XML file, but we provide a convenience function to
+easily open PubMed XMl citations and PMC open access articles. ### Example 1: A
+PMC Open Access Article ```python import tarfile import urllib.request as
+request from contextlib import closing from pathlib import Path from
+pubmed_types import parse_pubmed_xml # Input file source and output file
+destination source = ( "ftp://ftp.ncbi.nlm.nih.gov" + "/pub/pmc/oa_bulk/
+oa_comm/xml" + "/oa_comm_xml.incr.2023-03-21.tar.gz" ) destination = Path
+("downloads") destination.mkdir(exist_ok=True) # 1. Get an open access article
+dataset from the FTP server with closing(request.urlopen(source)) as url: with
+tarfile.open(fileobj=url, mode="r:gz") as fr: fr.extractall(destination) # 2.
+Parse the file file_path = destination.joinpath("PMC009xxxxxx").joinpath
+("PMC9970662.xml") full_text = parse_pubmed_xml(file_path) # 3. Print out the
+article title print(f"Title:
 {full_text.front.article_meta.title_group.article_title.content[0]}") ```
 Output: ```bash Title: Lactate as a myokine and exerkine: drivers and signals
 of physiology and metabolism ``` ### Example 2: A Pubmed baseline citation file
-### Example 1: A PMC Open Access Article ```python import gzip import
-urllib.request as request from contextlib import closing from pathlib import
-Path from pubmed_types import parse_pubmed_xml, PubmedArticleSet # Input file
-source and output file destination source = "ftp://ftp.ncbi.nlm.nih.gov" + "/
-pubmed/updatefiles" + "/pubmed23n1168.xml.gz" destination = Path
-("downloads").joinpath("pubmed23n1168.xml") destination.parent.mkdir
-(exist_ok=True) # 1. Get a pubmed citation daily update file from the FTP
-server with closing(request.urlopen(source)) as url: with gzip.GzipFile
-(fileobj=url, mode="rb") as fr: with open(destination, mode="wb") as fw:
-fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
+```python import gzip import urllib.request as request from contextlib import
+closing from pathlib import Path from pubmed_types import parse_pubmed_xml,
+PubmedArticleSet # Input file source and output file destination source = "ftp:
+//ftp.ncbi.nlm.nih.gov" + "/pubmed/updatefiles" + "/pubmed23n1168.xml.gz"
+destination = Path("downloads").joinpath("pubmed23n1168.xml")
+destination.parent.mkdir(exist_ok=True) # 1. Get a pubmed citation daily update
+file from the FTP server with closing(request.urlopen(source)) as url: with
+gzip.GzipFile(fileobj=url, mode="rb") as fr: with open(destination, mode="wb")
+as fw: fw.write(fr.read()) # 2. Parse the file article_set = parse_pubmed_xml
 (destination) assert isinstance(article_set, PubmedArticleSet) # 3. Get the
 number of citations in the file print(f"Number of citations: {len
 (article_set.pubmed_article)}") print(f"{article_set.pubmed_article
 [0].medline_citation.article.article_title.content[0]}") ``` Output: ```bash
 Number of citations: 2543 A Patent and Pattern Mother. ``` ## FAQ ### Why does
 it take so long to parse a pubmed citation set There is a lot of data, and the
 schema is deep and complex. ### Why are the return structures so complicated?
```

