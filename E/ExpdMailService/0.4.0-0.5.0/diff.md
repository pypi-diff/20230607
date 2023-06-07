# Comparing `tmp/ExpdMailService-0.4.0.tar.gz` & `tmp/ExpdMailService-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdMailService-0.4.0.tar", last modified: Mon Mar 20 07:15:57 2023, max compression
+gzip compressed data, was "dist\ExpdMailService-0.5.0.tar", last modified: Wed Jun  7 02:38:24 2023, max compression
```

## Comparing `ExpdMailService-0.4.0.tar` & `ExpdMailService-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/
--rw-rw-rw-   0        0        0      294 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-03-08 08:22:39.000000 ExpdMailService-0.4.0/README.md
--rw-rw-rw-   0        0        0      115 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-03-20 07:14:12.000000 ExpdMailService-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService/
--rw-rw-rw-   0        0        0       63 2023-03-03 07:52:18.000000 ExpdMailService-0.4.0/src/ExpdMailService/__init__.py
--rw-rw-rw-   0        0        0     4941 2023-03-20 07:15:14.000000 ExpdMailService-0.4.0/src/ExpdMailService/send_mail.py
-drwxrwxrwx   0        0        0        0 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/
--rw-rw-rw-   0        0        0      294 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-20 07:15:57.000000 ExpdMailService-0.4.0/src/ExpdMailService.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/
+-rw-rw-rw-   0        0        0      268 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2023-06-07 02:36:34.000000 ExpdMailService-0.5.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-07 02:36:19.000000 ExpdMailService-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService/
+-rw-rw-rw-   0        0        0     4943 2023-06-07 02:35:59.000000 ExpdMailService-0.5.0/src/ExpdMailService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 02:38:24.000000 ExpdMailService-0.5.0/src/ExpdMailService.egg-info/top_level.txt
```

### Comparing `ExpdMailService-0.4.0/src/ExpdMailService/send_mail.py` & `ExpdMailService-0.5.0/src/ExpdMailService/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 encoders.encode_base64(part)
                 file_path, file_name = path.split(f)
                 part.add_header('Content-Disposition', f"attachment; filename={make_header([(file_name, 'UTF-8')]).encode('UTF-8')}")
                 msg.attach(part)
         # ------------------------------------------------------
         server = smtplib.SMTP(self.mail_server, 465)
         server.starttls()
-        server.set_debuglevel(1)
+        # server.set_debuglevel(1)
         server.sendmail(from_addr=self.sender, to_addrs=self.receiver, msg=msg.as_string())
         server.quit()
         logger.debug("Mail sent successfully.")
 
 
 
 if __name__ == '__main__':
```

