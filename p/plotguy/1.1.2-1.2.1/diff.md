# Comparing `tmp/plotguy-1.1.2.tar.gz` & `tmp/plotguy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.1.2.tar", last modified: Mon Jun  5 01:05:10 2023, max compression
+gzip compressed data, was "plotguy-1.2.1.tar", last modified: Wed Jun  7 04:05:24 2023, max compression
```

## Comparing `plotguy-1.1.2.tar` & `plotguy-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.876574 plotguy-1.1.2/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-05 01:05:10.876405 plotguy-1.1.2/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.1.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.875410 plotguy-1.1.2/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25317 2023-06-05 00:25:28.000000 plotguy-1.1.2/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.1.2/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    64265 2023-06-05 01:01:48.000000 plotguy-1.1.2/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37809 2023-06-05 00:51:56.000000 plotguy-1.1.2/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.1.2/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.876182 plotguy-1.1.2/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 01:05:10.876628 plotguy-1.1.2/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-05 01:03:52.000000 plotguy-1.1.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.364354 plotguy-1.2.1/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:05:24.364094 plotguy-1.2.1/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.1/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.363175 plotguy-1.2.1/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25752 2023-06-06 21:12:29.000000 plotguy-1.2.1/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.2.1/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    65233 2023-06-06 21:48:03.000000 plotguy-1.2.1/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    38123 2023-06-06 21:38:06.000000 plotguy-1.2.1/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.1/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-07 04:05:24.363914 plotguy-1.2.1/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-07 04:05:24.000000 plotguy-1.2.1/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-07 04:05:24.364400 plotguy-1.2.1/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-07 04:04:20.000000 plotguy-1.2.1/setup.py
```

### Comparing `plotguy-1.1.2/plotguy/__init__.py` & `plotguy-1.2.1/plotguy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -589,15 +589,15 @@
         df3 = df3.set_index('date')
         signal_year_count = df3.groupby(lambda x: x.year).size()
 
         signal_year_std = np.std(signal_year_count)
         signal_year_mean = np.mean(signal_year_count)
         cov = round(signal_year_std / signal_year_mean, 3)
 
-        result_dict['cov'] = cov
+        result_dict['cov_count'] = cov
 
         # Win rate by year
         for year in year_list:
             try:
                 result_dict[str(year)] = win_rate_dict[year][0]
                 result_dict[f'{year}_win_rate'] = win_rate_dict[year][3]
 
@@ -605,30 +605,40 @@
                 # print(e)
                 result_dict[str(year)] = 0
                 result_dict[f'{year}_win_rate'] = '--'
 
         # Performance by year
         first_equity_value = 0
         last_equity_value = 0
+        year_return_list = []
         for year in year_list:
             if not df.loc[df['year'] == year].empty:  # if trade
                 if first_equity_value == 0:  # if 1st year, set beginning as the first equity_value
                     first_equity_value = df.loc[df['year'] == year].iloc[0].equity_value
                 last_equity_value = df.loc[df['year'] == year].iloc[-1].equity_value
                 yearly_return = (last_equity_value - first_equity_value) / first_equity_value
                 if np.isnan(yearly_return):
                     result_dict[f'{year}_return'] = 0
+                    year_return_list.append(0)
                 else:
                     result_dict[f'{year}_return'] = int(yearly_return * 100)
+                    year_return_list.append(int(yearly_return * 100))
 
             else:  # no trade
                 result_dict[f'{year}_return'] = '-----'
+                year_return_list.append(0)
 
             first_equity_value = last_equity_value
 
+        # cov_return
+        return_year_std = np.std(year_return_list)
+        return_year_mean = np.mean(year_return_list)
+        cov_return = round(return_year_std / return_year_mean, 3)
+        result_dict['cov_return'] = cov_return
+
     result_dict['risk_free_rate'] = risk_free_rate
 
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
     bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharp_ratio(df, 'close',
                                                                                          risk_free_rate)
     initial_capital = df.loc[df.index[0], 'equity_value']
```

### Comparing `plotguy-1.1.2/plotguy/aggregate.py` & `plotguy-1.2.1/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.1.2/plotguy/components.py` & `plotguy-1.2.1/plotguy/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,18 @@
                                                        {'label': 'Return-BaH % Diff. <', 'value': 'return_to_bah<'},
                                                        {'label': 'Sharp Ratio >', 'value': 'annualized_sr>'},
                                                        {'label': 'Sharp Ratio <', 'value': 'annualized_sr<'},
                                                        {'label': 'MDD Percentage >', 'value': 'mdd_pct>'},
                                                        {'label': 'MDD Percentage <', 'value': 'mdd_pct<'},
                                                        {'label': 'Trade Count >', 'value': 'num_of_trade>'},
                                                        {'label': 'Trade Count <', 'value': 'num_of_trade<'},
-                                                       {'label': 'COV >', 'value': 'cov>'},
-                                                       {'label': 'COV <', 'value': 'cov<'},
+                                                       {'label': 'COV (Count) >', 'value': 'cov_count>'},
+                                                       {'label': 'COV (Count) <', 'value': 'cov_count<'},
+                                                       {'label': 'COV (Return) >', 'value': 'cov_return>'},
+                                                       {'label': 'COV (Return) <', 'value': 'cov_return<'},
                                                        {'label': 'Win Rate >', 'value': 'win_rate>'},
                                                        {'label': 'Win Rate <', 'value': 'win_rate<'},
                                                    ],
                                                    style={'border-radius': '5px', 'font-size': '12px'}),
                                style={'padding-left': '15px', 'width': '175px'})
 
     filter_dropdown_disabled = html.Div(id='filter_dropdown',
@@ -222,15 +224,16 @@
         per_col_2_3 = [html.Div('BaH',style={'text-align': 'center', 'font-weight': 'bold', 'color':'yellow'})]
 
         keys = ['num_of_trade',
                 'net_profit',
                 'net_profit_to_mdd',
                 'return_to_bah',
                 'win_rate',
-                'cov',
+                'cov_count',
+                'cov_return',
                 'total_commission',
                 'return_on_capital',
                 'annualized_return',
                 'annualized_std',
                 'annualized_sr',
                 'mdd_dollar',
                 'mdd_pct',
@@ -250,15 +253,16 @@
 
             df['mdd_dollar'] = "{:,}".format(int(round(df['mdd_dollar'], 0)))
             df['mdd_pct'] = "{:.0%}".format(df['mdd_pct'] / 100)
             df['return_on_capital'] = "{:.0%}".format(df['return_on_capital'] / 100)
             df['annualized_return'] = "{:.0%}".format(df['annualized_return'] / 100)
             df['annualized_std'] = "{:.0%}".format(df['annualized_std'] / 100)
 
-            df['cov'] = round(df['cov'], 2)
+            df['cov_count'] = round(df['cov_count'], 2)
+            df['cov_return'] = round(df['cov_return'], 2)
 
             try:
                 df['win_rate'] = "{:.0%}".format( float(df['win_rate']) / 100)
             except Exception as e:
                 df['win_rate'] = '--'
 
             df['return_to_bah'] = "{:.0%}".format(df['return_to_bah'] / 100)
@@ -276,15 +280,16 @@
 
 
         per_col_1_1.append(html.Div('Number of Trade'))
         per_col_1_1.append(html.Div('Net Profit'))
         per_col_1_1.append(html.Div('Net Profit/MDD'))
         per_col_1_1.append(html.Div('Return-BaH % Diff.'))
         per_col_1_1.append(html.Div('Win Rate'))
-        per_col_1_1.append(html.Div('COV'))
+        per_col_1_1.append(html.Div('COV (Count)'))
+        per_col_1_1.append(html.Div('COV (Return)'))
         per_col_1_1.append(html.Div('Total Commission'))
         per_col_1_1.append(html.Div('Risk Free Rate'))
 
         per_col_2_1.append(html.Div('Return on Capital'))
         per_col_2_1.append(html.Div('Ann. Return'))
         per_col_2_1.append(html.Div('Ann. Std'))
         per_col_2_1.append(html.Div('Ann. Sharp Ratio'))
@@ -397,15 +402,16 @@
 
     filter_options = {
         'num_of_trade':'Trade Count',
         'return_on_capital': 'Return on Capital',
         'annualized_return': 'Annualized Return',
         'annualized_sr': 'Sharp Ratio',
         'mdd_pct':'MDD Percentage',
-        'cov':'COV',
+        'cov_count':'COV (Count)',
+        'cov_return': 'COV (Return)',
         'win_rate':'Win Rate',
         'return_to_bah': 'Return/BnH % Diff.',
         'exclude': 'Exclude',
         }
     def update_filter_div(self, filter_list):
         filter_button = []
         for i, element in enumerate(filter_list):
@@ -588,15 +594,16 @@
                 round(graph_df.iloc[i]['return_to_bah'], 2)) + "<br>"
             hovertemplate = hovertemplate + "Net Profit to MDD: " + str(
                 round(graph_df.iloc[i]['net_profit_to_mdd'], 2)) + "<br>"
             hovertemplate = hovertemplate + "Sharp Ratio : " + str(graph_df.iloc[i]['annualized_sr']) + "<br>"
             hovertemplate = hovertemplate + "MDD Percentage : " + "{:.0%}".format(
                 graph_df.iloc[i]['mdd_pct'] / 100) + "<br>"
             hovertemplate = hovertemplate + "Trade Count : " + str(graph_df.iloc[i]['num_of_trade']) + "<br>"
-            hovertemplate = hovertemplate + "COV : " + str(round(graph_df.iloc[i]['cov'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "COV (Count) : " + str(round(graph_df.iloc[i]['cov_count'], 2)) + "<br>"
+            hovertemplate = hovertemplate + "COV (Return) : " + str(round(graph_df.iloc[i]['cov_return'], 2)) + "<br>"
             try:
                 hovertemplate = hovertemplate + "Win Rate : " + "{:.0%}".format(
                     float(graph_df.iloc[i]['win_rate']) / 100) + "<br>"
             except:
                 hovertemplate = hovertemplate + "Win Rate : --" + "<br>"
             hovertemplate = hovertemplate + "<br>"
 
@@ -1044,14 +1051,15 @@
         for folder in folders:
             df_saved = pd.read_csv(f'{folder}/saved_strategies.csv')
             for i, row in df_saved.iterrows():
                 equity_path = f'{folder}/{row["path"]}'
 
                 dict = {}
                 # parameters = ast.literal_eval(row['para_combination'])
+
                 dict['para_combination'] = ast.literal_eval(row['para_combination'])
                 para_combination = ast.literal_eval(row['para_combination'])
                 dict['para_combination'] = para_combination
                 file_format = para_combination['file_format']
                 save_name = plotguy.filename_only(para_combination)
                 ref_code = plotguy.path_reference_code(save_name)
 
@@ -1136,15 +1144,15 @@
 
                 if key == 'mdd_pct':
                     item = 'MDD Percentage'
                     _value = "{:.0%}".format(value/100)
                     performance_text.append(html.Div(f'{item} : {_value}', style={'line-height': line_height}))
 
                 if key == 'return_on_capital':
-                    item = 'Return on Capital'
+                    item = 'ReturnOnCapital'
                     _value = "{:.0%}".format(value/100)
                     performance_text.append(html.Div(f'{item} : {_value}', style={'line-height': line_height}))
 
                 # performance_text.append(html.Div(f'{key} : {value}',style={'line-height': line_height}))
 
             choices.append({
                 "label": html.Div([
@@ -1299,37 +1307,45 @@
 
         year_col = []
         year_count = []
         year_count_col = []
         year_win_rate_col = []
         year_return_col = []
 
+        year_return_list = []
         for year in year_list:
             year_col.append(html.Div(year))
             year_count.append(int(total_dict[f'{year}']))
             year_count_col.append(html.Div(int(total_dict[f'{year}'])))
             rate = total_dict[f'{year}_win_count']/total_dict[f'{year}']
             year_win_rate_col.append(html.Div( "{:.0%}".format(rate) ))
             year_return = total_dict[f'{year}_return']
             year_return_col.append(html.Div( "{:.0%}".format(year_return) ))
 
-        cov = round(np.std(year_count) / np.mean(year_count), 2)
+            try:
+                year_return_list.append(float(year_return))
+            except:
+                year_return_list.append(0)
+
+        cov_count = round(np.std(year_count) / np.mean(year_count), 2)
+        cov_return = round(np.std(year_return_list) / np.mean(year_return_list), 2)
 
         div = html.Div([
 
             html.Div('Performance', style={'color': 'Cyan', 'font-size': '15px'}),
 
             html.Div(style={'height': '5px'}),
 
             dbc.Row([
                 dbc.Col([html.Div('Number of Trade'),
                          html.Div('Net Profit'),
                          html.Div('Net Profit/MDD'),
                          html.Div('Win Rate'),
-                         html.Div('COV'),
+                         html.Div('COV (Count)'),
+                         html.Div('COV (Return)'),
                          html.Div('Total Commission'),
                          html.Div('Risk Free Rate'),
                          html.Div(style={'height': '10px'}),
                          html.Div('Return on Capital'),
                          html.Div('Ann. Return'),
                          html.Div('Ann. Std'),
                          html.Div('Ann. Sharp Ratio'),
@@ -1338,15 +1354,16 @@
                          ],
                         style={'padding-left':'13px'},
                         width=7),
                 dbc.Col([html.Div(num_of_trade),
                          html.Div(net_profit),
                          html.Div(net_profit_to_mdd),
                          html.Div(win_rate),
-                         html.Div(cov),
+                         html.Div(cov_count),
+                         html.Div(cov_return),
                          html.Div(total_commission),
                          html.Div("{:.2%}".format(risk_free_rate_float / 100)),
                          html.Div(style={'height': '10px'}),
                          html.Div(return_on_capital),
                          html.Div(annualized_return),
                          html.Div(annualized_std),
                          html.Div(annualized_sr),
```

### Comparing `plotguy-1.1.2/plotguy/equity_curves.py` & `plotguy-1.2.1/plotguy/equity_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,15 +678,23 @@
 
                         if self.line_selected > -1:
                             saved_df = pd.read_csv('saved_strategies.csv')
 
                             if not save_path in list(saved_df['path']):
 
                                 para_pop = self.para_combination.copy()
-                                para_pop.pop('df')
+                                try:
+                                    para_pop.pop('df')
+                                except:
+                                    pass
+
+                                try:
+                                    para_pop.pop('holiday_list')
+                                except:
+                                    pass
 
                                 df_dict = {'path': save_path,
                                            'para_combination':str(para_pop),
                                            'initial': self.initial_capital,
                                            'net_profit_to_mdd': self.net_profit_to_mdd,
                                            'net_profit': self.net_profit,
                                            'mdd_dollar':self.mdd_dollar,
```

### Comparing `plotguy-1.1.2/plotguy/signals.py` & `plotguy-1.2.1/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.1.2/setup.py` & `plotguy-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.1.2",
+    version="1.2.1",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

