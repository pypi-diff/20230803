# Comparing `tmp/asmek_authcogs-1.1.2.tar.gz` & `tmp/asmek_authcogs-1.1.3.tar.gz`

## Comparing `asmek_authcogs-1.1.2.tar` & `asmek_authcogs-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/app_settings.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/apps.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/auth_hooks.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/eve-o-4.png
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/smt_bomb_icon-1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/about.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/auth.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/links.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/siege.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0001_initial.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0002_alter_link_name.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0003_alter_general_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/LICENSE
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/app_settings.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/apps.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/auth_hooks.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/eve-o-4.png
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/Images/smt_bomb_icon-1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/about.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/auth.py
+-rw-r--r--   0        0        0     8292 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/links.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/recruit.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/cogs/siege.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0002_alter_link_name.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/0003_alter_general_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/asmek_authcogs/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.3/PKG-INFO
```

### Comparing `asmek_authcogs-1.1.2/CHANGELOG.md` & `asmek_authcogs-1.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/.github/workflows/publish.yml` & `asmek_authcogs-1.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/models.py` & `asmek_authcogs-1.1.3/asmek_authcogs/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 Create your models in here
 """
 
 # Django
 from django.db import models
 
 
-class General(models.Model):
+class AuthCogs(models.Model):
     """Meta model for app permissions"""
 
     class Meta:
         """Meta definitions"""
 
         managed = False
         default_permissions = ()
-        permissions = (("basic_access", "Basic access to this app"),("siege_control", "Control siege colours"),)
+        permissions = (
+            ("basic_access", "Basic access to this app"),
+            ("siege_control", "Control siege colours"),
+        )
 
 
 class Link(models.Model):
     description = models.TextField(max_length=500)
     name = models.CharField(max_length=255, null=False, unique=True)
     url = models.CharField(max_length=255, null=False)
     thumbnail = models.CharField(max_length=255)
```

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/Images/eve-o-4.png` & `asmek_authcogs-1.1.3/asmek_authcogs/Images/eve-o-4.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/Images/smt_bomb_icon-1.png` & `asmek_authcogs-1.1.3/asmek_authcogs/Images/smt_bomb_icon-1.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/cogs/about.py` & `asmek_authcogs-1.1.3/asmek_authcogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/cogs/auth.py` & `asmek_authcogs-1.1.3/asmek_authcogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/cogs/links.py` & `asmek_authcogs-1.1.3/asmek_authcogs/cogs/links.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
                 await interaction.response.send_message(msg, ephemeral=True)
             except Exception as e:
                 await interaction.response.send_message(e, ephemeral=True)
             self.stop()
 
     @links_commands.command(name="list", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("link.manage_links")
+    @sender_has_perm("asmek_authcogs.manage_links")
     async def list(self, ctx):
         """
         list all current links
         """
         embed = Embed()
         embed.title = "All the links!!"
         embed.description = f"A list of all links currently stored by the auth bot!"
@@ -177,34 +177,34 @@
         await ctx.respond(embed=embed, ephemeral=False)
 
     # //=============================================================================
     # // Add, edit, delete commands
     # //=============================================================================
 
     @links_commands.command(name="add", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    # @sender_has_perm("link.manage_links")
+    @sender_has_perm("asmek_authcogs.manage_links")
     async def add(self, ctx):
         """
         add new link
         """
         add_modal = Links.AddModal()
         await ctx.send_modal(add_modal)
 
     @links_commands.command(name="edit", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("link.manage_links")
+    @sender_has_perm("asmek_authcogs.manage_links")
     @option("name", description="Search for a Link!", autocomplete=search_links)
     async def edit(self, ctx, name: str):
         """
         edit link
         """
         edit_modal = Links.EditModal(name)
         await ctx.send_modal(edit_modal)
 
     @links_commands.command(name="delete", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("link.manage_links")
+    @sender_has_perm("asmek_authcogs.manage_links")
     @option("name", description="Search for a Link!", autocomplete=search_links)
     async def delete(self, ctx, name: str):
         """
         delete link
         """
         delete_modal = Links.DeleteModal(name)
         await ctx.send_modal(delete_modal)
```

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/cogs/siege.py` & `asmek_authcogs-1.1.3/asmek_authcogs/cogs/siege.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,52 +17,65 @@
         self.bot = bot
 
     siege_commands = SlashCommandGroup(
         "siege",
         "SIEGE COLOURS!",
         guild_ids=[int(settings.DISCORD_GUILD_ID)],
     )
-    
+
     @siege_commands.command(name="green", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("general.siege_control")
-    async def green(self, ctx,*,msg=''):
+    @sender_has_perm("asmek_authcogs.siege_control")
+    async def green(self, ctx, *, msg=""):
         """
         All Clear
         """
         if len(msg) == 0:
-            msg = 'SIEGE GREEN - Crab on!'
+            msg = "SIEGE GREEN - Crab on!"
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
-        await siege_channel.send(' @here '+ msg + '\nhttps://media.discordapp.net/attachments/478100446238474282/671250121178218496/Green_w_Excav.gif')
-        await siege_channel.edit(name = 'delve-status-💸')
+        await siege_channel.send(
+            " @here "
+            + msg
+            + "\nhttps://media.discordapp.net/attachments/478100446238474282/671250121178218496/Green_w_Excav.gif"
+        )
+        await siege_channel.edit(name="delve-status-💸")
         return await ctx.respond("Siege status updated to GREEN", ephemeral=True)
-    
+
     @siege_commands.command(name="amber", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("general.siege_control")
-    async def amber(self, ctx,*,msg=''):
+    @sender_has_perm("asmek_authcogs.siege_control")
+    async def amber(self, ctx, *, msg=""):
         """
         Ratting caps should dock, rorqs max tank
         """
         if len(msg) == 0:
-            msg = 'SIEGE AMBER - Caps dock / Rorqs max tank!'
+            msg = "SIEGE AMBER - Caps dock / Rorqs max tank!"
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
-        await siege_channel.send('@here '+ msg + '\nhttps://media.discordapp.net/attachments/726469660916318218/829165923436331039/unknown.png')
-        await siege_channel.edit(name = 'delve-status-🟠')
+        await siege_channel.send(
+            "@here "
+            + msg
+            + "\nhttps://media.discordapp.net/attachments/726469660916318218/829165923436331039/unknown.png"
+        )
+        await siege_channel.edit(name="delve-status-🟠")
         return await ctx.respond("Siege status updated to AMBER", ephemeral=True)
-    
+
     @siege_commands.command(name="red", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("general.siege_control")
-    async def red(self, ctx,*,msg=''):
+    @sender_has_perm("asmek_authcogs.siege_control")
+    async def red(self, ctx, *, msg=""):
         """
         Everyone should dock up
         """
         if len(msg) == 0:
-            msg = 'SIEGE RED - Delve is dangerous!'
+            msg = "SIEGE RED - Delve is dangerous!"
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
-        await siege_channel.send('@here '+ msg + '\nhttps://media.discordapp.net/attachments/478100446238474282/671250121345728542/Red_Final.gif')
-        await siege_channel.edit(name = 'delve-status-🔴')
+        await siege_channel.send(
+            "@here "
+            + msg
+            + "\nhttps://media.discordapp.net/attachments/478100446238474282/671250121345728542/Red_Final.gif"
+        )
+        await siege_channel.edit(name="delve-status-🔴")
         return await ctx.respond("Siege status updated to RED", ephemeral=True)
-        
+
+
 def setup(bot):
     bot.add_cog(Siege(bot))
```

### Comparing `asmek_authcogs-1.1.2/asmek_authcogs/migrations/0001_initial.py` & `asmek_authcogs-1.1.3/asmek_authcogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/.gitignore` & `asmek_authcogs-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/LICENSE` & `asmek_authcogs-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/README.md` & `asmek_authcogs-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/pyproject.toml` & `asmek_authcogs-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.2/PKG-INFO` & `asmek_authcogs-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmek-authcogs
-Version: 1.1.2
+Version: 1.1.3
 Summary: ASMEK customized cogs for aa-discordbot
 Project-URL: Documentation, https://github.com/AstrumMechanica/asmek-authcogs#readme
 Project-URL: Issues, https://github.com/AstrumMechanica/asmek-authcogs/issues
 Project-URL: Source, https://github.com/AstrumMechanica/asmek-authcogs
 Author-email: AstrumMechanica <astrummechanica@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
```

