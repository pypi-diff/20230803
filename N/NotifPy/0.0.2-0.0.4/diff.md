# Comparing `tmp/NotifPy-0.0.2.tar.gz` & `tmp/NotifPy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotifPy-0.0.2.tar", last modified: Wed Aug  2 16:40:42 2023, max compression
+gzip compressed data, was "NotifPy-0.0.4.tar", last modified: Thu Aug  3 21:07:37 2023, max compression
```

## Comparing `NotifPy-0.0.2.tar` & `NotifPy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.192705 NotifPy-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-08-02 13:31:49.000000 NotifPy-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.168706 NotifPy-0.0.2/NotifPy/
--rw-rw-rw-   0        0        0     2523 2023-08-02 14:41:28.000000 NotifPy-0.0.2/NotifPy/EmailNotif.py
--rw-rw-rw-   0        0        0      927 2023-08-02 14:16:23.000000 NotifPy-0.0.2/NotifPy/SMSNotif.py
--rw-rw-rw-   0        0        0        0 2023-08-02 13:20:01.000000 NotifPy-0.0.2/NotifPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:40:42.191717 NotifPy-0.0.2/NotifPy.egg-info/
--rw-rw-rw-   0        0        0     2979 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 16:40:42.000000 NotifPy-0.0.2/NotifPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2979 2023-08-02 16:40:42.193705 NotifPy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2023-08-02 15:14:13.000000 NotifPy-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-08-02 13:28:49.000000 NotifPy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      580 2023-08-02 16:40:42.195705 NotifPy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:37.011819 NotifPy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 21:07:27.000000 NotifPy-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:37.011819 NotifPy-0.0.4/NotifPy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-03 21:07:27.000000 NotifPy-0.0.4/NotifPy/EmailNotif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 21:07:27.000000 NotifPy-0.0.4/NotifPy/SMSNotif.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:27.000000 NotifPy-0.0.4/NotifPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:37.011819 NotifPy-0.0.4/NotifPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-08-03 21:07:37.000000 NotifPy-0.0.4/NotifPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 21:07:37.000000 NotifPy-0.0.4/NotifPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:07:37.000000 NotifPy-0.0.4/NotifPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 21:07:37.000000 NotifPy-0.0.4/NotifPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-08-03 21:07:37.011819 NotifPy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-03 21:07:27.000000 NotifPy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 21:07:27.000000 NotifPy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-03 21:07:37.011819 NotifPy-0.0.4/setup.cfg
```

### Comparing `NotifPy-0.0.2/LICENSE` & `NotifPy-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Arian F
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Arian F
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `NotifPy-0.0.2/NotifPy/EmailNotif.py` & `NotifPy-0.0.4/NotifPy/EmailNotif.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import smtplib
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-
-
-class email_notif: 
-    def __init__(self, sender_address=None, sender_password=None, recipient_email=None ):
-        self.sender_address = sender_address
-        self.sender_password = sender_password
-        self.recipient_email = recipient_email
-
-    def EmailSender(self, subject='', body='', html='', email_provider='gmail', custom_server=None, custom_port=None):
-        sender_email = self.sender_address  #your email address eg 'foo@example.com'
-        sender_password = self.sender_password      #your email password eg '123'
-        recipient_email = self.recipient_email  #recipient's email address eg 'foo2@example.com'
-
-        # Create a message object
-        if html:
-            msg = MIMEMultipart('alternative')
-            
-
-            part1 = MIMEText(body, 'plain')
-            part2 = MIMEText(html, 'html')
-
-
-            msg.attach(part1)
-            msg.attach(part2)
-        else:
-            msg = MIMEText(body)
-
-        msg['Subject'] = subject
-        msg['From'] = sender_email
-        msg['To'] = recipient_email
-
-        try:
-
-            #gmail
-            if email_provider.lower() == 'gmail':
-                print('Note: Due to recent google policy, 16 character app password is needed for gmail. How to get it? https://support.google.com/accounts/answer/6010255?hl=en')
-                server = smtplib.SMTP('smtp.gmail.com', 587)  # Gmail SMTP server and port
-            elif email_provider.lower() == 'yahoo':
-            #yahoo
-                server = smtplib.SMTP('smtp.mail.yahoo.com', 587)  # Yahoo SMTP server and port
-            #outlook/hotmail
-            elif email_provider.lower() == 'outlook':
-                server = smtplib.SMTP('smtp-mail.outlook.com', 587)
-            else:
-                print(f'None of gmail, yahoo and outlook. Then on custom using server {custom_server} and port {custom_port}')
-                server = smtplib.SMTP(custom_server, custom_port)
-            server.starttls()
-
-            # Log in to the sender's email account
-            server.login(sender_email, sender_password)
-
-            # Send the email
-            server.sendmail(sender_email, recipient_email, msg.as_string())
-
-            # Close the connection
-            server.quit()
-            print("Email sent successfully!")
-        except Exception as e:
-            print("Error sending email:", e)
-
+import smtplib
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+
+
+class email_notif: 
+    def __init__(self, sender_address=None, sender_password=None, recipient_email=None ):
+        self.sender_address = sender_address
+        self.sender_password = sender_password
+        self.recipient_email = recipient_email
+
+    def EmailSender(self, subject='', body='', html='', email_provider='gmail', custom_server=None, custom_port=None):
+        sender_email = self.sender_address  #your email address eg 'foo@example.com'
+        sender_password = self.sender_password      #your email password eg '123'
+        recipient_email = self.recipient_email  #recipient's email address eg 'foo2@example.com'
+
+        # Create a message object
+        if html:
+            msg = MIMEMultipart('alternative')
+            
+
+            part1 = MIMEText(body, 'plain')
+            part2 = MIMEText(html, 'html')
+
+
+            msg.attach(part1)
+            msg.attach(part2)
+        else:
+            msg = MIMEText(body)
+
+        msg['Subject'] = subject
+        msg['From'] = sender_email
+        msg['To'] = recipient_email
+
+        try:
+
+            #gmail
+            if email_provider.lower() == 'gmail':
+                print('Note: Due to recent google policy, 16 character app password is needed for gmail. How to get it? https://support.google.com/accounts/answer/6010255?hl=en')
+                server = smtplib.SMTP('smtp.gmail.com', 587)  # Gmail SMTP server and port
+            elif email_provider.lower() == 'yahoo':
+            #yahoo
+                server = smtplib.SMTP('smtp.mail.yahoo.com', 587)  # Yahoo SMTP server and port
+            #outlook/hotmail
+            elif email_provider.lower() == 'outlook':
+                server = smtplib.SMTP('smtp-mail.outlook.com', 587)
+            else:
+                print(f'None of gmail, yahoo and outlook. Then on custom using server {custom_server} and port {custom_port}')
+                server = smtplib.SMTP(custom_server, custom_port)
+            server.starttls()
+
+            # Log in to the sender's email account
+            server.login(sender_email, sender_password)
+
+            # Send the email
+            server.sendmail(sender_email, recipient_email, msg.as_string())
+
+            # Close the connection
+            server.quit()
+            print("Email sent successfully!")
+        except Exception as e:
+            print("Error sending email:", e)
+
```

### Comparing `NotifPy-0.0.2/NotifPy/SMSNotif.py` & `NotifPy-0.0.4/NotifPy/SMSNotif.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from twilio.rest import Client
-
-
-class SMS_notif:
-    def __init__(self, body, recipient_phone_number):
-        self.body = body 
-        self.recipient_phone_number = recipient_phone_number 
-    def twillio(self, account_sid, auth_token, twilio_phone_number):
-        self.account_sid = account_sid
-        self.auth_token = auth_token
-        self.twilio_phone_number = twilio_phone_number
-
-        try:
-            # Create a Twilio client
-            client = Client(self.account_sid, self.auth_token)
-
-            # Send the SMS
-            message = client.messages.create(
-                body=self.body,
-                from_=self.twilio_phone_number,
-                to=self.recipient_phone_number
-            )
-
-            print("SMS sent successfully! SID:", message.sid) #message.sid is like unqiue id of an SMS
-        except Exception as e:
-            print("Error sending SMS:", e)
-
+from twilio.rest import Client
+
+
+class SMS_notif:
+    def __init__(self, body, recipient_phone_number):
+        self.body = body 
+        self.recipient_phone_number = recipient_phone_number 
+    def twillio(self, account_sid, auth_token, twilio_phone_number):
+        self.account_sid = account_sid
+        self.auth_token = auth_token
+        self.twilio_phone_number = twilio_phone_number
+
+        try:
+            # Create a Twilio client
+            client = Client(self.account_sid, self.auth_token)
+
+            # Send the SMS
+            message = client.messages.create(
+                body=self.body,
+                from_=self.twilio_phone_number,
+                to=self.recipient_phone_number
+            )
+
+            print("SMS sent successfully! SID:", message.sid) #message.sid is like unqiue id of an SMS
+        except Exception as e:
+            print("Error sending SMS:", e)
+
```

