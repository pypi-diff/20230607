# Comparing `tmp/art-daq-1.1.2.tar.gz` & `tmp/art-daq-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "art-daq-1.1.2.tar", last modified: Thu Apr 27 09:29:41 2023, max compression
+gzip compressed data, was "art-daq-2.0.1.tar", last modified: Wed Jun  7 11:40:44 2023, max compression
```

## Comparing `art-daq-1.1.2.tar` & `art-daq-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.280942 art-daq-1.1.2/
--rw-rw-rw-   0        0        0     1087 2023-03-18 07:37:39.000000 art-daq-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      714 2023-04-27 09:29:41.279943 art-daq-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4330 2023-04-23 12:57:02.000000 art-daq-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.270937 art-daq-1.1.2/art_daq/
--rw-rw-rw-   0        0        0     9272 2023-04-23 12:56:06.000000 art-daq-1.1.2/art_daq/MIN.py
--rw-rw-rw-   0        0        0     2167 2023-04-23 12:56:13.000000 art-daq-1.1.2/art_daq/__init__.py
--rw-rw-rw-   0        0        0    15663 2023-04-23 12:55:54.000000 art-daq-1.1.2/art_daq/daq.py
-drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.277937 art-daq-1.1.2/art_daq.egg-info/
--rw-rw-rw-   0        0        0      714 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 09:29:41.280942 art-daq-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-23 12:55:41.000000 art-daq-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:40:44.870246 art-daq-2.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 07:37:39.000000 art-daq-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-06-07 11:40:44.869245 art-daq-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4330 2023-04-23 12:57:02.000000 art-daq-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 11:40:44.859723 art-daq-2.0.1/art_daq/
+-rw-rw-rw-   0        0        0    18622 2023-06-07 11:34:41.000000 art-daq-2.0.1/art_daq/MIN.py
+-rw-rw-rw-   0        0        0     2246 2023-06-07 11:00:53.000000 art-daq-2.0.1/art_daq/__init__.py
+-rw-rw-rw-   0        0        0    16253 2023-06-07 10:59:19.000000 art-daq-2.0.1/art_daq/daq.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:40:44.868239 art-daq-2.0.1/art_daq.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-07 11:40:44.000000 art-daq-2.0.1/art_daq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-07 11:40:44.000000 art-daq-2.0.1/art_daq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:40:44.000000 art-daq-2.0.1/art_daq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 11:40:44.000000 art-daq-2.0.1/art_daq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 11:40:44.000000 art-daq-2.0.1/art_daq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:40:44.870246 art-daq-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-06-07 11:03:24.000000 art-daq-2.0.1/setup.py
```

### Comparing `art-daq-1.1.2/LICENSE` & `art-daq-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `art-daq-1.1.2/PKG-INFO` & `art-daq-2.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: art-daq
-Version: 1.1.2
+Version: 2.0.1
 Summary: Paquete para usar la tarjeta de NI, USB-6001
 Home-page: https://github.com/Julumisan/art-daq
 Author: Juan Luis
 Author-email: julumisan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `art-daq-1.1.2/README.md` & `art-daq-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `art-daq-1.1.2/art_daq/__init__.py` & `art-daq-2.0.1/art_daq/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Mar 18 16:05:36 2023
 
 @author: Julu
-@version: 1.1.2
+@version: 2.0.1
 
 El archivo init.py es necesario para que Python reconozca que este es un paquete. Debe estar vacío para evitar una dependencia cíclica.
 
 Para utilizar la librería, se debe importar de la siguiente manera: "from art_daq import daq"
 
 La siguiente es una lista de las funciones que se encuentran en este paquete:
 
@@ -15,14 +15,15 @@
     get_state_digital(chan_d): lee el estado actual del canal digital especificado en el parámetro chan_d.
     set_voltage_analogic(chan_a, voltage): establece el voltaje del canal analógico especificado en el parámetro chan_a en el valor especificado en el parámetro voltage (float).
     set_voltage_digital(chan_d, voltage): establece el voltaje del canal digital especificado en el parámetro chan_d en el valor especificado en el parámetro voltage (bool).
     daq_timer(chan_a, duration): configura una tarea de adquisición de datos que espera durante una cantidad de tiempo determinada.
     all_digital_safe(device_name): establece todas las líneas de salida a False.
     all_analogic_safe(device_name): configura todos los canales analógicos de salida a 0V.
     safe_state(device_name): establece un voltaje seguro en todas las salidas.
+    read_digital_input(chan_d): lee el estado de un canal digital de entrada.
 
 Además de estas funciones, también se incluyen las funciones para generar señales:
 
     generate_sine_wave(device_name, ao_channel, frequency, amplitude, duration): genera una señal sinusoidal con la frecuencia, amplitud y duración especificadas en los parámetros.
     generate_square_wave(device_name, ao_channel, frequency, amplitude, duration): genera una señal cuadrada con la frecuencia, amplitud y duración especificadas en los parámetros.
     generate_triangle_wave(device_name, ao_channel, frequency, amplitude, duration, steps=100): genera una señal triangular con la frecuencia, amplitud y duración especificadas en los parámetros. El parámetro opcional "steps" especifica la cantidad de pasos en cada rampa de la señal triangular.
 """
```

### Comparing `art-daq-1.1.2/art_daq/daq.py` & `art-daq-2.0.1/art_daq/daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     -Temporizador.
     -Posibilidad de elección automática de tarjeta con get_connected_device
     -Generación de ondas cuadradas/triangulares/sinusoidales
 
 
 @author: Julu
 
-@version: v1.1.2
+@version: v2.0.1
 
 Esta nueva versión cuenta con todas las funcionalidades previstas, comentarios
 aclaratorios acerca del uso de las funciones, tanto de su función como de 
 qué parámetros se usan y su formato.
 
 """
 
@@ -207,14 +207,30 @@
         None
         
     """   
     with nidaqmx.Task() as task:
         task.do_channels.add_do_chan(chan_d) # Especificar la salida digital X.Y del dispositivo DAQ
         task.write(voltage) # Establecer el voltaje en el canal digital
         
+        
+def read_digital_input(chan_d: str) -> bool:
+    """
+    Lee el estado de un canal digital de entrada.
+    chan_d tiene el formato "Dev/portX/lineY"
+    
+    Args:
+        chan_d: el identificador del canal digital de salida, en el formato "Dev/portX/lineY".
+        
+    Returns:
+        bool: el estado del canal digital de entrada (True si está encendido, False si está apagado).
+    """
+    with nidaqmx.Task() as task:
+        task.di_channels.add_di_chan(chan_d)  # Especificar la entrada digital X.Y del dispositivo DAQ
+        return task.read()
+        
     
         
 def safe_state(device_name: str) -> None:
     """
     Establece un voltaje seguro y conocido en todas las salidas de un dispositivo NI. Se recomienda su uso para iniciar y
     finalizar el programa.
```

### Comparing `art-daq-1.1.2/art_daq.egg-info/PKG-INFO` & `art-daq-2.0.1/art_daq.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: art-daq
-Version: 1.1.2
+Version: 2.0.1
 Summary: Paquete para usar la tarjeta de NI, USB-6001
 Home-page: https://github.com/Julumisan/art-daq
 Author: Juan Luis
 Author-email: julumisan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `art-daq-1.1.2/setup.py` & `art-daq-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 """
 
 from setuptools import setup
 
 setup(
     name='art-daq',
-    version='1.1.2',
+    version='2.0.1',
     description='Paquete para usar la tarjeta de NI, USB-6001',
     packages=['art_daq'],
     install_requires=[
         'nidaqmx',
         'matplotlib',
-        'numpy'
+        'numpy',
+        'pyvisa'
     ],
     
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

