# Comparing `tmp/prioritization_discovery-0.4.1.tar.gz` & `tmp/prioritization_discovery-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prioritization_discovery-0.4.1.tar", max compression
+gzip compressed data, was "prioritization_discovery-0.4.2.tar", max compression
```

## Comparing `prioritization_discovery-0.4.1.tar` & `prioritization_discovery-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11349 2023-06-07 13:59:09.692561 prioritization_discovery-0.4.1/LICENSE
--rw-r--r--   0        0        0     2040 2023-06-07 14:06:50.331582 prioritization_discovery-0.4.1/README.md
--rw-r--r--   0        0        0      702 2023-06-07 14:09:20.291116 prioritization_discovery-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-07 13:59:09.693210 prioritization_discovery-0.4.1/src/prioritization_discovery/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-07 13:59:09.693325 prioritization_discovery-0.4.1/src/prioritization_discovery/config.py
--rw-r--r--   0        0        0     5144 2023-06-07 13:59:09.693472 prioritization_discovery-0.4.1/src/prioritization_discovery/discovery.py
--rw-r--r--   0        0        0    12334 2023-06-07 13:59:09.693649 prioritization_discovery-0.4.1/src/prioritization_discovery/rules.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2040 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/README.md
+-rw-r--r--   0        0        0      702 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/config.py
+-rw-r--r--   0        0        0     4984 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/discovery.py
+-rw-r--r--   0        0        0    12584 2023-06-07 14:19:08.736693 prioritization_discovery-0.4.2/src/prioritization_discovery/rules.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 prioritization_discovery-0.4.2/PKG-INFO
```

### Comparing `prioritization_discovery-0.4.1/LICENSE` & `prioritization_discovery-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.1/README.md` & `prioritization_discovery-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `prioritization_discovery-0.4.1/pyproject.toml` & `prioritization_discovery-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prioritization-discovery"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prioritization_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `prioritization_discovery-0.4.1/src/prioritization_discovery/config.py` & `prioritization_discovery-0.4.2/src/prioritization_discovery/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class EventLogIDs:
-    case: str = 'case_id'  # ID of the case instance of the process (trace)
-    activity: str = 'Activity'  # Name of the executed activity in this activity instance
-    start_time: str = 'start_time'  # Timestamp in which this activity instance started
-    end_time: str = 'end_time'  # Timestamp in which this activity instance ended
-    resource: str = 'Resource'  # ID of the resource that executed this activity instance
-    enabled_time: str = 'enabled_time'  # Enable time of this activity instance
+    case: str = "case_id"  # ID of the case instance of the process (trace)
+    activity: str = "Activity"  # Name of the executed activity in this activity instance
+    start_time: str = "start_time"  # Timestamp in which this activity instance started
+    end_time: str = "end_time"  # Timestamp in which this activity instance ended
+    resource: str = "Resource"  # ID of the resource that executed this activity instance
+    enabled_time: str = "enabled_time"  # Enable time of this activity instance
 
 
-DEFAULT_CSV_IDS = EventLogIDs(case='case_id',
-                              activity='Activity',
-                              start_time='start_time',
-                              end_time='end_time',
-                              resource='Resource',
-                              enabled_time='enabled_time')
+DEFAULT_CSV_IDS = EventLogIDs(
+    case="case_id",
+    activity="Activity",
+    start_time="start_time",
+    end_time="end_time",
+    resource="Resource",
+    enabled_time="enabled_time",
+)
 
 # Prefixes for internal use in prioritization discovery
 PRIORITIZED_PREFIX = "prioritized"
 DELAYED_PREFIX = "delayed"
```

### Comparing `prioritization_discovery-0.4.1/src/prioritization_discovery/discovery.py` & `prioritization_discovery-0.4.2/src/prioritization_discovery/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import pandas as pd
 import pandasql as ps
 
 from .config import DELAYED_PREFIX, PRIORITIZED_PREFIX
 from .rules import discover_prioritization_rules
 
 
-def discover_priority_rules(
-        event_log: pd.DataFrame,
-        attributes: list[str]
-) -> list:
+def discover_priority_rules(event_log: pd.DataFrame, attributes: list[str]) -> list:
     """
     Given an event log and the list of case attributes to consider, discover the different priority levels and the corresponding rules. The
     priority levels establish a hierarchy in the prioritization when executed the activities in a process. For example, the activity
     instances of a case with a high priority, when enabled, would be executed before the enabled activities of a case with lower priority.
 
     :param event_log:   event log to analyze.
     :param attributes:  list of column names for the attributes to use as features for the prioritization (the case attributes).
 
     :return: a list of dicts with the priority level and the corresponding rules.
     """
     # Discover the activity instances that have been prioritized w.r.t. others.
-    outcome = 'outcome'
+    outcome = "outcome"
     prioritized_instances = _discover_prioritized_instances(event_log, attributes, outcome)
     # Discover the priority levels and rules that classify a case in its level.
     priority_rules = discover_prioritization_rules(prioritized_instances, outcome)
     # Return rules
     return priority_rules
 
 
 def _discover_prioritized_instances(
-        event_log: pd.DataFrame,
-        attributes: list[str],
-        outcome: str = 'outcome'
+    event_log: pd.DataFrame, attributes: list[str], outcome: str = "outcome"
 ) -> pd.DataFrame:
     """
     Discover activity instances that are prioritized over others. This means they are not being executed following a FIFO order, i.e., in
     the order they are enabled.
 
     :param event_log:   event log to analyze.
     :param attributes:  list of column names for the attributes to use as features for the prioritization.
@@ -43,78 +38,70 @@
     :return: a pd.DataFrame with each of the observations (positive and negative) of prioritization found in the event log.
     """
     # Dictionaries with the attribute name and delayed/prioritized renamed values
     delayed_attributes = {attribute: _add_prefix(DELAYED_PREFIX, attribute) for attribute in attributes}
     prioritized_attributes = {attribute: _add_prefix(PRIORITIZED_PREFIX, attribute) for attribute in attributes}
     # Define columns for the SQL query
     columns = [
-                  "delayed.{} as {}".format(attribute, delayed_attributes[attribute]) for attribute in delayed_attributes
-              ] + [
-                  "prioritized.{} as {}".format(attribute, prioritized_attributes[attribute]) for attribute in prioritized_attributes
-              ]
+        "delayed.{} as {}".format(attribute, delayed_attributes[attribute]) for attribute in delayed_attributes
+    ] + [
+        "prioritized.{} as {}".format(attribute, prioritized_attributes[attribute])
+        for attribute in prioritized_attributes
+    ]
     # Query the prioritized and delayed events
-    prioritizations = ps.sqldf("""
+    prioritizations = ps.sqldf(
+        """
         SELECT {}
         FROM event_log as delayed, event_log as prioritized
         WHERE (delayed.enabled_time < prioritized.enabled_time and 
                 delayed.start_time > prioritized.start_time and 
                 delayed.Resource = prioritized.Resource)
-    """.format(", ".join(columns)), locals())
+    """.format(
+            ", ".join(columns)
+        ),
+        locals(),
+    )
     # Split the log so each activity instance is an observation
     prioritized_instances = _split_to_individual_observations(
-        prioritizations,
-        list(delayed_attributes.values()),
-        list(prioritized_attributes.values()),
-        outcome
+        prioritizations, list(delayed_attributes.values()), list(prioritized_attributes.values()), outcome
     )
     # Return extended observations
     return prioritized_instances
 
 
 def _split_to_individual_observations(
-        event_log: pd.DataFrame,
-        delayed_attributes: list[str],
-        prioritized_attributes: list[str],
-        outcome: str
+    event_log: pd.DataFrame, delayed_attributes: list[str], prioritized_attributes: list[str], outcome: str
 ) -> pd.DataFrame:
     """
     Split the received pd.DataFrame with the prioritized instances (delayed and prioritized) into positive (prioritized) and negative
     (delayed) ones.
 
     :param event_log:               event log to split into delayed and prioritized instances.
     :param delayed_attributes:      list of column names of attributes for delayed observations.
     :param prioritized_attributes:  list of column names of attributes for prioritized observations.
     :param outcome                  ID of the column with the variable to predict (1 positive, 0 negative).
 
     :return:
     """
     # Get the columns of the delayed instances
     delayed_instances = event_log[delayed_attributes].rename(
-        {
-            column_name: _remove_prefix(DELAYED_PREFIX, column_name)
-            for column_name in delayed_attributes
-        },
-        axis=1
+        {column_name: _remove_prefix(DELAYED_PREFIX, column_name) for column_name in delayed_attributes}, axis=1
     )
     delayed_instances[outcome] = 0
     # Get the columns of the prioritized instances
     prioritized_instances = event_log[prioritized_attributes].rename(
-        {
-            column_name: _remove_prefix(PRIORITIZED_PREFIX, column_name)
-            for column_name in prioritized_attributes
-        },
-        axis=1
+        {column_name: _remove_prefix(PRIORITIZED_PREFIX, column_name) for column_name in prioritized_attributes}, axis=1
     )
     prioritized_instances[outcome] = 1
     # Return both individual delayed and prioritized instances (don't reset index
     return pd.concat([delayed_instances, prioritized_instances])
 
 
 def _add_prefix(prefix: str, name: str) -> str:
     return "{}_{}".format(prefix, name)
 
 
 def _remove_prefix(prefix: str, name: str) -> str:
     if name.startswith(prefix):
-        return name[len(prefix) + 1:]
+        return name[len(prefix) + 1 :]
     else:
         return name
```

### Comparing `prioritization_discovery-0.4.1/src/prioritization_discovery/rules.py` & `prioritization_discovery-0.4.2/src/prioritization_discovery/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import copy
 import re
 
 import pandas as pd
 from sklearn.tree import DecisionTreeClassifier, _tree
 
 
-def discover_prioritization_rules(
-        data: pd.DataFrame,
-        outcome: str
-) -> list:
+def discover_prioritization_rules(data: pd.DataFrame, outcome: str) -> list:
     """
     Discover, incrementally, rules to set the priority level of an activity instance in such a way that; when two activity instances are
     waiting to be executed (enabled), the one with the highest priority goes first. To do this, first discover the cases in the event log
     that have been prioritized (an activity enabled after another got executed first). Then, discover the rules (based on their attributes)
     that best describe the observed prioritizations.
 
     :param data:    pd.DataFrame with the observations of delayed and prioritized activity instances. The two activity instances
@@ -22,15 +19,17 @@
 
     :return: a list of dicts with the priority level and the corresponding rules.
     """
     # Create empty list for the incremental models
     models = []
     # Get the data we'll be using in each iteration
     filtered_data = pd.get_dummies(data)
-    dummy_columns = {column: list(data[column].unique()) for column in data.columns if column not in filtered_data.columns}
+    dummy_columns = {
+        column: list(data[column].unique()) for column in data.columns if column not in filtered_data.columns
+    }
     # Extract rules level by level
     continue_search = True
     while continue_search:
         # Discover a new model for the current observations
         model = _get_rules(filtered_data, outcome)
         # If any rule has been discovered
         if len(model) > 0:
@@ -48,24 +47,21 @@
             # If no rules have been discovered, end search
             continue_search = False
     # Create empty list for priority levels
     priority_levels = []
     current_lvl = 1
     for model in models:
         parsed_model = model
-        priority_levels += [{'priority_level': current_lvl, 'rules': parsed_model}]
+        priority_levels += [{"priority_level": current_lvl, "rules": parsed_model}]
         current_lvl += 1
     # Return list of level rules
     return priority_levels
 
 
-def _get_rules(
-        data: pd.DataFrame,
-        outcome: str
-) -> list:
+def _get_rules(data: pd.DataFrame, outcome: str) -> list:
     """
     Discover one rule that lead to the positive outcome in the observations passed as argument in [data]. To do this, it uses a decision
     tree classifier to discover a rule 5 times, and gets the one with the highest confidence.
 
     :param data:    pd.DataFrame with one observation per row.
     :param outcome: ID of the column with the variable to predict (1 positive, 0 negative).
     :return: the discovered rules with the highest confidence.
@@ -78,94 +74,103 @@
         new_model = DecisionTreeClassifier()
         new_model.fit(data[[column for column in data.columns if column is not outcome]], data[outcome])
         best_rules = _tree_to_best_rules(new_model, [column for column in data.columns if column is not outcome])
         # If any rule has been discovered
         if len(best_rules) > 0:
             # Measure confidence
             predictions = _predict(best_rules, data.drop([outcome], axis=1))
-            true_positives = [
-                p and a
-                for (p, a) in zip(predictions, data[outcome])
-            ]
+            true_positives = [p and a for (p, a) in zip(predictions, data[outcome])]
             confidence = sum(true_positives) / sum(predictions)
             # Retain if it's better than the previous one
             if confidence > best_confidence:
                 best_confidence = confidence
                 best_rules = best_rules
     # Return the best one, or None if no rules found in any iteration
     return best_rules
 
 
 def _tree_to_best_rules(tree, feature_names) -> list:
     # Extract tree structure
     tree_ = tree.tree_
     # Get the feature used in each non-leaf node
-    feature_name = [
-        feature_names[i] if i != _tree.TREE_UNDEFINED else "undefined!"
-        for i in tree_.feature
-    ]
+    feature_name = [feature_names[i] if i != _tree.TREE_UNDEFINED else "undefined!" for i in tree_.feature]
     # Go depth-first over the rules storing the best one
-    best_rule = {'impurity': 1.0, 'sample_size': 0, 'rules': []}
+    best_rule = {"impurity": 1.0, "sample_size": 0, "rules": []}
     missing_nodes = [0]
     current_rules = [[]]
     while len(missing_nodes) > 0:
         current_node = missing_nodes.pop()
         current_rule = current_rules.pop()
         if tree_.feature[current_node] != _tree.TREE_UNDEFINED:
             # Decision node: add rule and keep search through each child
             name = feature_name[current_node]
             threshold = tree_.threshold[current_node]
             # Add ID and rule for left and right children
             missing_nodes += [tree_.children_left[current_node], tree_.children_right[current_node]]
             current_rules += [
-                current_rule + [{'attribute': name, 'condition': '<=', 'value': threshold}],
-                current_rule + [{'attribute': name, 'condition': '>', 'value': threshold}]
+                current_rule + [{"attribute": name, "condition": "<=", "value": threshold}],
+                current_rule + [{"attribute": name, "condition": ">", "value": threshold}],
             ]
         else:
             # Leaf node
             current_impurity = tree_.impurity[current_node]
             current_sample_sizes = tree_.value[current_node][0]  # Number of positive samples
             # If it is the best leaf node, save it
-            if (
-                    current_sample_sizes[0] < current_sample_sizes[1] and  # Less samples with negative outcome
-                    (current_impurity < best_rule['impurity'] or
-                     (current_impurity == best_rule['impurity'] and current_sample_sizes[1] > best_rule['sample_size']))
+            if current_sample_sizes[0] < current_sample_sizes[1] and (  # Less samples with negative outcome
+                current_impurity < best_rule["impurity"]
+                or (current_impurity == best_rule["impurity"] and current_sample_sizes[1] > best_rule["sample_size"])
             ):
-                best_rule['impurity'] = current_impurity
-                best_rule['sample_size'] = current_sample_sizes[1]
-                best_rule['rules'] = _summarize_rules(current_rule)
+                best_rule["impurity"] = current_impurity
+                best_rule["sample_size"] = current_sample_sizes[1]
+                best_rule["rules"] = _summarize_rules(current_rule)
     # Return best rules (wrapped in a list)
-    return [best_rule['rules']]
+    return [best_rule["rules"]]
 
 
 def _summarize_rules(rules: list) -> list:
     filtered_rules = []
     # Merge rules by same feature
-    attributes = {rule['attribute'] for rule in rules}
+    attributes = {rule["attribute"] for rule in rules}
     for attribute in attributes:
-        operators = {rule['condition'] for rule in rules if rule['attribute'] == attribute}
+        operators = {rule["condition"] for rule in rules if rule["attribute"] == attribute}
         if len(operators) > 1:
             # Add interval rule
-            filtered_rules += [{
-                'attribute': attribute,
-                'condition': 'in',
-                'value': "({},{}]".format(
-                    max([rule['value'] for rule in rules if rule['attribute'] == attribute and rule['condition'] == ">"]),
-                    min([rule['value'] for rule in rules if rule['attribute'] == attribute and rule['condition'] == "<="])
-                )
-            }]
+            filtered_rules += [
+                {
+                    "attribute": attribute,
+                    "condition": "in",
+                    "value": "({},{}]".format(
+                        max(
+                            [
+                                rule["value"]
+                                for rule in rules
+                                if rule["attribute"] == attribute and rule["condition"] == ">"
+                            ]
+                        ),
+                        min(
+                            [
+                                rule["value"]
+                                for rule in rules
+                                if rule["attribute"] == attribute and rule["condition"] == "<="
+                            ]
+                        ),
+                    ),
+                }
+            ]
         else:
             # Add single rule
             operator = operators.pop()
-            values = [rule['value'] for rule in rules if rule['attribute'] == attribute]
-            filtered_rules += [{
-                'attribute': attribute,
-                'condition': operator,
-                'value': str(min(values)) if operator == "<=" else str(max(values))
-            }]
+            values = [rule["value"] for rule in rules if rule["attribute"] == attribute]
+            filtered_rules += [
+                {
+                    "attribute": attribute,
+                    "condition": operator,
+                    "value": str(min(values)) if operator == "<=" else str(max(values)),
+                }
+            ]
     # Return rules
     return filtered_rules
 
 
 def _predict(rules: list, data: pd.DataFrame) -> list:
     predictions = []
     # Predict each observation
@@ -178,92 +183,85 @@
     # Return predictions
     return predictions
 
 
 def _fulfill_ruleset(rules: list, observation: pd.Series):
     fulfills = True
     for rule in rules:
-        values = [float(value) for value in re.findall(r'[\d.]+', rule['value'])]
+        values = [float(value) for value in re.findall(r"[\d.]+", rule["value"])]
         if (
-                (rule['condition'] == "<=" and observation[rule['attribute']] > values[0]) or
-                (rule['condition'] == ">" and observation[rule['attribute']] <= values[0]) or
-                (rule['condition'] == "in" and observation[rule['attribute']] <= values[0]) or
-                (rule['condition'] == "in" and observation[rule['attribute']] > values[1])
+            (rule["condition"] == "<=" and observation[rule["attribute"]] > values[0])
+            or (rule["condition"] == ">" and observation[rule["attribute"]] <= values[0])
+            or (rule["condition"] == "in" and observation[rule["attribute"]] <= values[0])
+            or (rule["condition"] == "in" and observation[rule["attribute"]] > values[1])
         ):
             fulfills = False
     return fulfills
 
 
 def _reverse_one_hot_encoding(model: list, dummy_columns: dict, data: pd.DataFrame) -> list:
     # Deep copy of the list
     new_model = copy.deepcopy(model)
     # Correct the dummy columns removing the values that are no longer present in the dataset
     new_dummy_columns = {}
     for column in dummy_columns:
-        new_values = [
-            value
-            for value in dummy_columns[column]
-            if (data["{}_{}".format(column, value)] == 1).any()
-        ]
+        new_values = [value for value in dummy_columns[column] if (data["{}_{}".format(column, value)] == 1).any()]
         new_dummy_columns[column] = new_values
     # For each ruleset (list of rules combined by ANDs such as all must be fulfilled)
     for ruleset in new_model:
         # Process each ruleset individually
         _reverse_one_hot_encoding_ruleset(ruleset, new_dummy_columns)
     # Return parsed rules
     return new_model
 
 
 def _reverse_one_hot_encoding_ruleset(ruleset: list, dummy_columns: dict):
     # Initialize
     dummy_map = {  # Dict with dummified name as key, and pair with column+value as value
-        "{}_{}".format(column, value): (column, value)
-        for column in dummy_columns
-        for value in dummy_columns[column]
+        "{}_{}".format(column, value): (column, value) for column in dummy_columns for value in dummy_columns[column]
     }
     diff_than_attributes = {  # Empty list for each attribute to store the assigned values
-        attribute: []
-        for attribute in dummy_columns
+        attribute: [] for attribute in dummy_columns
     }
     equal_to_attributes = []  # Attributes with a rule '='
     rules_to_remove = []  # Indices of the rules to remove because of redundancy
     # Parse each rule in the ruleset
     for rule in ruleset:
-        if rule['attribute'] in dummy_map:
-            (orig_name, orig_value) = dummy_map[rule['attribute']]
-            rule['attribute'] = orig_name
-            rule['value'] = orig_value
-            if rule['condition'] == ">":
-                rule['condition'] = "="
+        if rule["attribute"] in dummy_map:
+            (orig_name, orig_value) = dummy_map[rule["attribute"]]
+            rule["attribute"] = orig_name
+            rule["value"] = orig_value
+            if rule["condition"] == ">":
+                rule["condition"] = "="
                 equal_to_attributes += [orig_name]
             else:
-                rule['condition'] = "!="
+                rule["condition"] = "!="
                 diff_than_attributes[orig_name] += [orig_value]
     # Remove rules with '!=' if there's also a rule with '='
     for attribute in set(equal_to_attributes):
         rules_to_remove += [  # Get the index of the rules of this attribute with "!=" condition
-            index
-            for index, rule in enumerate(ruleset)
-            if rule['attribute'] == attribute and rule['condition'] == "!="
+            index for index, rule in enumerate(ruleset) if rule["attribute"] == attribute and rule["condition"] == "!="
         ]
     # Check if any categorical rule with N possible values got N-1 times '!=' (meaning it's '=' to the missing value).
     for attribute in diff_than_attributes:
-        if (attribute not in equal_to_attributes and
-                len(diff_than_attributes[attribute]) > 0 and
-                len(diff_than_attributes[attribute]) == len(dummy_columns[attribute]) - 1):
+        if (
+            attribute not in equal_to_attributes
+            and len(diff_than_attributes[attribute]) > 0
+            and len(diff_than_attributes[attribute]) == len(dummy_columns[attribute]) - 1
+        ):
             # Attribute has N possible values, and N-1 rules saying 'different from', simplify it
             new_rule = {
-                'attribute': attribute,
-                'condition': "=",
-                'value': [  # Get the missing value in all "!=" rules for this attribute
-                    value
-                    for value in dummy_columns[attribute]
-                    if value not in diff_than_attributes[attribute]
-                ][0]  # Get the first element (there should be only one)
+                "attribute": attribute,
+                "condition": "=",
+                "value": [  # Get the missing value in all "!=" rules for this attribute
+                    value for value in dummy_columns[attribute] if value not in diff_than_attributes[attribute]
+                ][
+                    0
+                ],  # Get the first element (there should be only one)
             }
             # Get the index of the rules of this attribute with "!=" condition
-            rules_to_remove += [index for index, rule in enumerate(ruleset) if rule['attribute'] == attribute]
+            rules_to_remove += [index for index, rule in enumerate(ruleset) if rule["attribute"] == attribute]
             # Add new rule to ruleset
             ruleset += [new_rule]
     # Remove redundant rules
     for i in sorted(rules_to_remove, reverse=True):
         del ruleset[i]
```

### Comparing `prioritization_discovery-0.4.1/PKG-INFO` & `prioritization_discovery-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prioritization-discovery
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python algorithm to discover, from an event log, prioritization rules that lead to one activity instance to be executed before another.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

