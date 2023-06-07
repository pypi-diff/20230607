# Comparing `tmp/plotguy-1.2.1.tar.gz` & `tmp/plotguy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.2.1.tar", last modified: Wed Jun  7 04:05:24 2023, max compression
+gzip compressed data, was "plotguy-1.2.2.tar", last modified: Wed Jun  7 04:53:31 2023, max compression
```

## Comparing `plotguy-1.2.1.tar` & `plotguy-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.364354 plotguy-1.2.1/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:05:24.364094 plotguy-1.2.1/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.1/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.363175 plotguy-1.2.1/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25752 2023-06-06 21:12:29.000000 plotguy-1.2.1/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.2.1/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    65233 2023-06-06 21:48:03.000000 plotguy-1.2.1/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    38123 2023-06-06 21:38:06.000000 plotguy-1.2.1/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.1/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.363914 plotguy-1.2.1/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-07 04:05:24.364400 plotguy-1.2.1/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-07 04:04:20.000000 plotguy-1.2.1/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.418426 plotguy-1.2.2/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:53:31.418259 plotguy-1.2.2/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.417334 plotguy-1.2.2/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25831 2023-06-07 04:50:28.000000 plotguy-1.2.2/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.2.2/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    65949 2023-06-07 04:51:18.000000 plotguy-1.2.2/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    38123 2023-06-06 21:38:06.000000 plotguy-1.2.2/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.2/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:53:31.418063 plotguy-1.2.2/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-07 04:53:31.000000 plotguy-1.2.2/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-07 04:53:31.418477 plotguy-1.2.2/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-07 04:53:23.000000 plotguy-1.2.2/setup.py
```

### Comparing `plotguy-1.2.1/plotguy/__init__.py` & `plotguy-1.2.2/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -628,15 +628,18 @@
                 year_return_list.append(0)
 
             first_equity_value = last_equity_value
 
         # cov_return
         return_year_std = np.std(year_return_list)
         return_year_mean = np.mean(year_return_list)
-        cov_return = round(return_year_std / return_year_mean, 3)
+        if return_year_mean == 0:
+            cov_return = 0
+        else:
+            cov_return = round(return_year_std / return_year_mean, 3)
         result_dict['cov_return'] = cov_return
 
     result_dict['risk_free_rate'] = risk_free_rate
 
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
     bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharp_ratio(df, 'close',
```

### Comparing `plotguy-1.2.1/plotguy/aggregate.py` & `plotguy-1.2.2/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.1/plotguy/components.py` & `plotguy-1.2.2/plotguy/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,24 +292,24 @@
         per_col_2_1.append(html.Div('Return on Capital'))
         per_col_2_1.append(html.Div('Ann. Return'))
         per_col_2_1.append(html.Div('Ann. Std'))
         per_col_2_1.append(html.Div('Ann. Sharp Ratio'))
         per_col_2_1.append(html.Div('MDD Dollar'))
         per_col_2_1.append(html.Div('MDD Percentage'))
 
-        for i in range(7):
+        for i in range(8):
             per_col_1_2.append(html.Div(df[keys[i]], style={'text-align': 'center'}))
         try:
             per_col_1_2.append(html.Div( "{:.2%}".format(risk_free_rate / 100) , style={'text-align': 'center'}))
         except:
             per_col_1_2.append(html.Div('-----', style={'text-align': 'center'}))
 
-        for i in range(7, 13):
+        for i in range(8, 14):
             per_col_2_2.append(html.Div(str(df[keys[i]]), style={'text-align': 'center'}))
-        for i in range(13, 19):
+        for i in range(14, 20):
             per_col_2_3.append(html.Div(str(df[keys[i]]), style={'text-align': 'center'}))
 
         per_col1.append(dbc.Row([dbc.Col(html.Div(per_col_1_1), width=6),
                                  dbc.Col(per_col_1_2, style={'padding': '0'}, width=6)]))
         per_col2.append(dbc.Row([dbc.Col(html.Div(per_col_2_1), width=6),
                                  dbc.Col(per_col_2_2, style={'padding': '0'}, width=3),
                                  dbc.Col(per_col_2_3, style={'padding': '0'}, width=3)
@@ -512,14 +512,15 @@
         df_signal_list = df_signal_list.loc[
             (df_signal_list['date'] >= chart3_start) & (df_signal_list['date'] <= chart3_end)]
 
         df_open = df_signal_list.loc[df_signal_list['action'] == 'open']
         df_profit = df_signal_list.loc[df_signal_list['action'] == 'profit_target']
         df_stop_loss = df_signal_list.loc[df_signal_list['action'] == 'stop_loss']
         df_close = df_signal_list.loc[df_signal_list['action'] == 'close_logic']
+        df_close = df_signal_list.loc[df_signal_list['action'] == 'close_logic']
 
         fig = go.Figure(data=[go.Candlestick(x=df['datetime'],
                                              open=df['open'],
                                              high=df['high'],
                                              low=df['low'],
                                              close=df['close'],
                                              increasing_line_color='white')
@@ -586,29 +587,36 @@
             para_combination = {}
             hovertemplate = "%{x}<br>"
             for key in para_key_list:
                 para_combination[key] = graph_df.iloc[i][key]
                 hovertemplate = hovertemplate + \
                                 key + " : " + str(graph_df.iloc[i][key]) + "<br>"
             hovertemplate = hovertemplate + "<br>"
-            hovertemplate = hovertemplate + "Return-BaH % Diff. : " + str(
-                round(graph_df.iloc[i]['return_to_bah'], 2)) + "<br>"
-            hovertemplate = hovertemplate + "Net Profit to MDD: " + str(
-                round(graph_df.iloc[i]['net_profit_to_mdd'], 2)) + "<br>"
-            hovertemplate = hovertemplate + "Sharp Ratio : " + str(graph_df.iloc[i]['annualized_sr']) + "<br>"
-            hovertemplate = hovertemplate + "MDD Percentage : " + "{:.0%}".format(
-                graph_df.iloc[i]['mdd_pct'] / 100) + "<br>"
+
             hovertemplate = hovertemplate + "Trade Count : " + str(graph_df.iloc[i]['num_of_trade']) + "<br>"
-            hovertemplate = hovertemplate + "COV (Count) : " + str(round(graph_df.iloc[i]['cov_count'], 2)) + "<br>"
-            hovertemplate = hovertemplate + "COV (Return) : " + str(round(graph_df.iloc[i]['cov_return'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "Net Profit : " + "{:,}".format(int(round(graph_df.iloc[i]['net_profit'], 0))) + "<br>"
+            hovertemplate = hovertemplate + "Net Profit to MDD: " + str(round(graph_df.iloc[i]['net_profit_to_mdd'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "Return-BaH % Diff. : " + "{:.0%}".format(float(graph_df.iloc[i]['return_to_bah']/100)) + "<br>"
             try:
-                hovertemplate = hovertemplate + "Win Rate : " + "{:.0%}".format(
-                    float(graph_df.iloc[i]['win_rate']) / 100) + "<br>"
+                hovertemplate = hovertemplate + "Win Rate : " + "{:.0%}".format(float(graph_df.iloc[i]['win_rate']) / 100) + "<br>"
             except:
                 hovertemplate = hovertemplate + "Win Rate : --" + "<br>"
+            hovertemplate = hovertemplate + "COV (Count) : " + str(round(graph_df.iloc[i]['cov_count'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "COV (Return) : " + str(round(graph_df.iloc[i]['cov_return'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "Total Commissionn : " + "{:,}".format(int(round(graph_df.iloc[i]['total_commission'], 2))) + "<br>"
+
+
+            hovertemplate = hovertemplate + "<br>"
+
+
+            hovertemplate = hovertemplate + "Return on Capital : " + "{:.0%}".format(graph_df.iloc[i]['return_on_capital']/100) + "<br>"
+            hovertemplate = hovertemplate + "Annual Return : " + "{:.0%}".format(graph_df.iloc[i]['annualized_return'] / 100) + "<br>"
+            hovertemplate = hovertemplate + "Sharp Ratio : " + str(graph_df.iloc[i]['annualized_sr']) + "<br>"
+            hovertemplate = hovertemplate + "MDD Percentage : " + "{:.0%}".format(graph_df.iloc[i]['mdd_pct'] / 100) + "<br>"
+
             hovertemplate = hovertemplate + "<br>"
 
             # para_combination for save_path generation
             reference_index = graph_df.iloc[i].reference_index
             para_combination = df_all_para_combination.loc[df_all_para_combination['reference_index'] == reference_index].to_dict('records')[0]
 
             line_colour = graph_df.loc[i].line_colour
@@ -1323,15 +1331,18 @@
 
             try:
                 year_return_list.append(float(year_return))
             except:
                 year_return_list.append(0)
 
         cov_count = round(np.std(year_count) / np.mean(year_count), 2)
-        cov_return = round(np.std(year_return_list) / np.mean(year_return_list), 2)
+        if np.mean(year_return_list) == 0:
+            cov_return = 0
+        else:
+            cov_return = round(np.std(year_return_list) / np.mean(year_return_list), 2)
 
         div = html.Div([
 
             html.Div('Performance', style={'color': 'Cyan', 'font-size': '15px'}),
 
             html.Div(style={'height': '5px'}),
```

### Comparing `plotguy-1.2.1/plotguy/equity_curves.py` & `plotguy-1.2.2/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.1/plotguy/signals.py` & `plotguy-1.2.2/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.1/setup.py` & `plotguy-1.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.2.1",
+    version="1.2.2",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

