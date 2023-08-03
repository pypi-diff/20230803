# Comparing `tmp/sentry_cli-2.20.3.tar.gz` & `tmp/sentry_cli-2.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.20.3.tar", last modified: Mon Jul 31 09:59:18 2023, max compression
+gzip compressed data, was "sentry_cli-2.20.4.tar", last modified: Thu Aug  3 11:59:15 2023, max compression
```

## Comparing `sentry_cli-2.20.3.tar` & `sentry_cli-2.20.4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.428130 sentry_cli-2.20.3/
--rw-r--r--   0 runner    (1001) docker     (123)    80991 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-31 09:59:18.428130 sentry_cli-2.20.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.412130 sentry_cli-2.20.3/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-31 09:59:18.000000 sentry_cli-2.20.3/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-31 09:59:18.000000 sentry_cli-2.20.3/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:59:18.000000 sentry_cli-2.20.3/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:59:18.000000 sentry_cli-2.20.3/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 09:59:18.432130 sentry_cli-2.20.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.412130 sentry_cli-2.20.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    90307 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.416130 sentry_cli-2.20.3/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.416130 sentry_cli-2.20.3/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.416130 sentry_cli-2.20.3/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.416130 sentry_cli-2.20.3/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.416130 sentry_cli-2.20.3/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.420130 sentry_cli-2.20.3/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/issues/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.420130 sentry_cli-2.20.3/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.420130 sentry_cli-2.20.3/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.420130 sentry_cli-2.20.3/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.420130 sentry_cli-2.20.3/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.424130 sentry_cli-2.20.3/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.424130 sentry_cli-2.20.3/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.424130 sentry_cli-2.20.3/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    24715 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.428130 sentry_cli-2.20.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.428130 sentry_cli-2.20.3/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:59:18.428130 sentry_cli-2.20.3/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    40019 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-31 09:59:02.000000 sentry_cli-2.20.3/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.060944 sentry_cli-2.20.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    81464 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-08-03 11:59:15.060944 sentry_cli-2.20.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.044943 sentry_cli-2.20.4/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-08-03 11:59:15.000000 sentry_cli-2.20.4/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-03 11:59:15.000000 sentry_cli-2.20.4/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:59:15.000000 sentry_cli-2.20.4/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:59:15.000000 sentry_cli-2.20.4/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 11:59:15.064944 sentry_cli-2.20.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.044943 sentry_cli-2.20.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    90307 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.048944 sentry_cli-2.20.4/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/issues/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.052944 sentry_cli-2.20.4/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.056944 sentry_cli-2.20.4/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    24715 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.060944 sentry_cli-2.20.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.060944 sentry_cli-2.20.4/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:59:15.060944 sentry_cli-2.20.4/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-08-03 11:58:54.000000 sentry_cli-2.20.4/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.20.3/Cargo.lock` & `sentry_cli-2.20.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1323,14 +1323,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb6648b65cc40174967a26b2cd7a5d859a33a7cfeef7fd1007a50de62c1f2788"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "magic_string"
+version = "0.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8033ce8c43f7ccb207e4699f30eed50d7526379ee08fab47159f80b7934e18"
+dependencies = [
+ "base64",
+ "regex",
+ "serde",
+ "serde_json",
+ "vlq",
+]
+
+[[package]]
 name = "match_cfg"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ffbee8634e0d45d258acb448e7eaab3fce7a0a467395d4d9f228e3c1f01fb2e4"
 
 [[package]]
 name = "maybe-owned"
@@ -2185,15 +2198,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.20.3"
+version = "2.20.4"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2217,14 +2230,15 @@
  "insta",
  "itertools",
  "java-properties",
  "lazy_static",
  "libc",
  "log",
  "mac-process-info",
+ "magic_string",
  "might-be-minified",
  "mockito",
  "open",
  "openssl-probe",
  "osascript",
  "parking_lot",
  "percent-encoding",
@@ -2464,17 +2478,17 @@
 dependencies = [
  "libc",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "sourcemap"
-version = "6.3.0"
+version = "6.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8df03d85f2767c45e61b4453eb6144153c80399e4fdd6407a6d16cb87cc0347"
+checksum = "e9221a6bba3e9cfa7decfe64edf5233311e1bf837ea3234df6e7f35836e1093d"
 dependencies = [
  "data-encoding",
  "debugid",
  "if_chain",
  "rustc_version 0.2.3",
  "scroll 0.10.2",
  "serde",
@@ -2944,14 +2958,20 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "vlq"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "65dd7eed29412da847b0f78bcec0ac98588165988a8cfe41d4ea1d429f8ccfff"
+
+[[package]]
 name = "wait-timeout"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f200f5b12eb75f8c1ed65abd4b2db8a6e1b138a20de009dacee265a2498f3f6"
 dependencies = [
  "libc",
 ]
```

### Comparing `sentry_cli-2.20.3/Cargo.toml` & `sentry_cli-2.20.4/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.20.3"
+version = "2.20.4"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -61,24 +61,25 @@
   "anyhow",
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
-sourcemap = { version = "6.3.0", features = ["ram_bundle"] }
+sourcemap = { version = "6.4.0", features = ["ram_bundle"] }
 symbolic = { version = "12.1.5", features = ["debuginfo-serde", "il2cpp"] }
 thiserror = "1.0.38"
 url = "2.3.1"
 username = "0.2.0"
 uuid = { version = "1.3.0", features = ["v4", "serde"] }
 walkdir = "2.3.2"
 which = "4.4.0"
 zip = "0.6.4"
 data-encoding = "2.3.3"
+magic_string = "0.3.4"
 
 [dev-dependencies]
 insta = { version = "1.26.0", features = ["redactions", "yaml"] }
 mockito = "0.31.1"
 predicates = "2.1.5"
 tempfile = "3.3.0"
 trycmd = "0.14.11"
```

### Comparing `sentry_cli-2.20.3/LICENSE` & `sentry_cli-2.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/PKG-INFO` & `sentry_cli-2.20.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.20.3
+Version: 2.20.4
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.20.3 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.20.4 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.20.3/README.md` & `sentry_cli-2.20.4/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/build.rs` & `sentry_cli-2.20.4/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.20.4/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.20.3
+Version: 2.20.4
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.20.3 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.20.4 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.20.3/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.20.4/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/setup.cfg` & `sentry_cli-2.20.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/setup.py` & `sentry_cli-2.20.4/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/api.rs` & `sentry_cli-2.20.4/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/bashsupport.sh` & `sentry_cli-2.20.4/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/bash_hook.rs` & `sentry_cli-2.20.4/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.20.4/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.20.4/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/check.rs` & `sentry_cli-2.20.4/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/find.rs` & `sentry_cli-2.20.4/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/mod.rs` & `sentry_cli-2.20.4/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.20.4/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/debug_files/upload.rs` & `sentry_cli-2.20.4/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/deploys/list.rs` & `sentry_cli-2.20.4/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/deploys/mod.rs` & `sentry_cli-2.20.4/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/deploys/new.rs` & `sentry_cli-2.20.4/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/events/list.rs` & `sentry_cli-2.20.4/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/events/mod.rs` & `sentry_cli-2.20.4/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/files/delete.rs` & `sentry_cli-2.20.4/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/files/list.rs` & `sentry_cli-2.20.4/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/files/mod.rs` & `sentry_cli-2.20.4/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/files/upload.rs` & `sentry_cli-2.20.4/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/info.rs` & `sentry_cli-2.20.4/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/issues/list.rs` & `sentry_cli-2.20.4/src/commands/issues/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/issues/mod.rs` & `sentry_cli-2.20.4/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/issues/mute.rs` & `sentry_cli-2.20.4/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/issues/resolve.rs` & `sentry_cli-2.20.4/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/issues/unresolve.rs` & `sentry_cli-2.20.4/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/login.rs` & `sentry_cli-2.20.4/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/mod.rs` & `sentry_cli-2.20.4/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/monitors/list.rs` & `sentry_cli-2.20.4/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/monitors/mod.rs` & `sentry_cli-2.20.4/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/monitors/run.rs` & `sentry_cli-2.20.4/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/organizations/list.rs` & `sentry_cli-2.20.4/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/organizations/mod.rs` & `sentry_cli-2.20.4/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/projects/list.rs` & `sentry_cli-2.20.4/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/projects/mod.rs` & `sentry_cli-2.20.4/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/react_native/appcenter.rs` & `sentry_cli-2.20.4/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/react_native/gradle.rs` & `sentry_cli-2.20.4/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/react_native/mod.rs` & `sentry_cli-2.20.4/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/react_native/xcode.rs` & `sentry_cli-2.20.4/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/archive.rs` & `sentry_cli-2.20.4/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/delete.rs` & `sentry_cli-2.20.4/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/finalize.rs` & `sentry_cli-2.20.4/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/info.rs` & `sentry_cli-2.20.4/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/list.rs` & `sentry_cli-2.20.4/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/mod.rs` & `sentry_cli-2.20.4/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/new.rs` & `sentry_cli-2.20.4/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/restore.rs` & `sentry_cli-2.20.4/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/releases/set_commits.rs` & `sentry_cli-2.20.4/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/repos/list.rs` & `sentry_cli-2.20.4/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/repos/mod.rs` & `sentry_cli-2.20.4/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/send_envelope.rs` & `sentry_cli-2.20.4/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/send_event.rs` & `sentry_cli-2.20.4/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.20.4/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.20.4/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.20.4/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.20.4/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.20.4/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/uninstall.rs` & `sentry_cli-2.20.4/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/update.rs` & `sentry_cli-2.20.4/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/commands/upload_proguard.rs` & `sentry_cli-2.20.4/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/config.rs` & `sentry_cli-2.20.4/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/constants.rs` & `sentry_cli-2.20.4/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/android.rs` & `sentry_cli-2.20.4/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/appcenter.rs` & `sentry_cli-2.20.4/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/args.rs` & `sentry_cli-2.20.4/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/chunks.rs` & `sentry_cli-2.20.4/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/codepush.rs` & `sentry_cli-2.20.4/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/cordova.rs` & `sentry_cli-2.20.4/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/dif.rs` & `sentry_cli-2.20.4/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/dif_upload.rs` & `sentry_cli-2.20.4/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/enc.rs` & `sentry_cli-2.20.4/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/event.rs` & `sentry_cli-2.20.4/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/file_search.rs` & `sentry_cli-2.20.4/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/file_upload.rs` & `sentry_cli-2.20.4/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/formatting.rs` & `sentry_cli-2.20.4/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/fs.rs` & `sentry_cli-2.20.4/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/http.rs` & `sentry_cli-2.20.4/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/logging.rs` & `sentry_cli-2.20.4/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/progress.rs` & `sentry_cli-2.20.4/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/releases.rs` & `sentry_cli-2.20.4/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/retry.rs` & `sentry_cli-2.20.4/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.20.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.20.4/src/utils/sourcemaps/inject.rs`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,34 @@
 use regex::Regex;
 use symbolic::common::{clean_path, join_path};
 
 use std::fmt;
 use std::io::{BufRead, Write};
 use std::path::PathBuf;
 
-use anyhow::{bail, Context, Result};
+use anyhow::Result;
 use lazy_static::lazy_static;
-use log::debug;
+
+use magic_string::{GenerateDecodedMapOptions, MagicString};
 use sentry::types::DebugId;
-use serde_json::Value;
+use sourcemap::SourceMap;
 
 const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}();"#;
 const DEBUGID_PLACEHOLDER: &str = "__SENTRY_DEBUG_ID__";
 const DEBUGID_COMMENT_PREFIX: &str = "//# debugId";
 
 lazy_static! {
-    static ref USE_PRAGMA_RE: Regex = Regex::new(r#"^"use \w+";|^'use \w+';"#).unwrap();
+    // A regex that captures
+    // 1. an optional initial hashbang,
+    // 2. a block of line comments, block comments, and empty lines,
+    // 3. and an optional `"use strict";` statement.`
+    static ref PRE_INJECT_RE: Regex = Regex::new(
+        r#"^(#!.*[\n\r])?(?:\s*|/\*(?:.|\r|\n)*?\*/|//.*[\n\r])*(?:"[^"]*";|'[^']*';[\n\r]?)?"#
+    )
+    .unwrap();
 }
 
 fn print_section_with_debugid(
     f: &mut fmt::Formatter<'_>,
     title: &str,
     data: &[(PathBuf, DebugId)],
 ) -> fmt::Result {
@@ -101,118 +109,56 @@
 /// Fixes up a minified JS source file with a debug id.
 ///
 /// This changes the source file in several ways:
 /// 1. The source code snippet
 /// `<CODE_SNIPPET>[<debug_id>]`
 /// is inserted at the earliest possible position, which is after an
 /// optional hashbang, followed by a
-/// block of comments, empty lines, and `"use […]";` or `'use […]';` pragmas.
+/// block of comments, empty lines, and an optional `"use […]";` or `'use […]';` pragma.
 /// 2. A comment of the form `//# debugId=<debug_id>` is appended to the file.
-/// 3. The last source mapping comment (a comment starting with
-/// `//# sourceMappingURL=` or `//@ sourceMappingURL=`) is moved to
-/// the very end of the file, after the debug id comment from 2.
-///
-/// This function will naturally mess with the correspondence between a source file
-/// and its sourcemap. Use [`insert_empty_mapping`] on the sourcemap to fix this.
-/// # Example
-/// ```
-/// let file = "
-/// // a
-/// // comment
-/// // block
-///
-/// // another
-/// // comment
-/// // block
-///
-/// 'use strict';
-/// function t(t) {
-///   return '[object Object]' === Object.prototype.toString.call(t);
-/// }
-/// //# sourceMappingURL=/path/to/sourcemap
-/// ";
-///
-/// let mut file = file.as_bytes().to_vec();
-/// fixup_js_file(&mut file, DebugId::default()).unwrap();
-///
-/// assert_eq!(
-///     std::str::from_utf8(&file).unwrap(),
-///     r#"
-/// // a
-/// // comment
-/// // block
-///
-/// // another
-/// // comment
-/// // block
 ///
-/// 'use strict';
-/// !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
-/// function t(t) {
-///   return '[object Object]' === Object.prototype.toString.call(t);
-/// }
-/// //# debugId=00000000-0000-0000-0000-000000000000
-/// //# sourceMappingURL=/path/to/sourcemap
-/// "#
-/// );
-/// ```
-pub fn fixup_js_file(js_contents: &mut Vec<u8>, debug_id: DebugId) -> Result<()> {
-    let mut js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
+/// This function returns a [`SourceMap`] that maps locations in the injected file
+/// to their corresponding places in the original file.
+pub fn fixup_js_file(js_contents: &mut Vec<u8>, debug_id: DebugId) -> Result<SourceMap> {
+    let contents = std::str::from_utf8(js_contents)?;
+
+    let m = PRE_INJECT_RE
+        .find(contents)
+        .expect("regex is infallible")
+        .range();
+
+    let code_snippet = format!(
+        "\n{}\n",
+        CODE_SNIPPET_TEMPLATE.replace(DEBUGID_PLACEHOLDER, &debug_id.to_string())
+    );
+
+    let debug_id_comment = format!("\n{DEBUGID_COMMENT_PREFIX}={debug_id}\n");
+
+    let mut magic = MagicString::new(contents);
+
+    magic
+        .append_left(m.end as u32, &code_snippet)
+        .unwrap()
+        .append(&debug_id_comment)
+        .unwrap();
 
     js_contents.clear();
+    write!(js_contents, "{}", magic.to_string())?;
 
-    // Find the last source mapping URL comment, it's the only one that matters
-    let sourcemap_comment_idx = js_lines
-        .iter()
-        .enumerate()
-        .rev()
-        .find(|(_idx, line)| {
-            line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
+    let map = magic
+        .generate_map(GenerateDecodedMapOptions {
+            source: Some("pre_injection.js".to_string()),
+            include_content: true,
+            ..Default::default()
         })
-        .map(|(idx, _)| idx);
-
-    let sourcemap_comment = sourcemap_comment_idx.map(|idx| js_lines.remove(idx));
-
-    let mut js_lines = js_lines.into_iter().peekable();
-
-    // Handle initial hashbang
-    if let Some(hashbang) = js_lines.next_if(|line| line.trim().starts_with("#!")) {
-        writeln!(js_contents, "{hashbang}")?;
-    }
+        .unwrap();
 
-    // Write comments and empty lines at the start back to the file
-    while let Some(comment_or_empty) =
-        js_lines.next_if(|line| line.trim().is_empty() || line.trim().starts_with("//"))
-    {
-        writeln!(js_contents, "{comment_or_empty}")?;
-    }
+    let map = map.to_string().unwrap();
 
-    // Write use statements back to the file
-    while let Some(use_pragma) = js_lines.next_if(|line| USE_PRAGMA_RE.is_match(line)) {
-        writeln!(js_contents, "{use_pragma}")?;
-    }
-
-    // Inject the code snippet
-    let to_inject = CODE_SNIPPET_TEMPLATE.replace(DEBUGID_PLACEHOLDER, &debug_id.to_string());
-    writeln!(js_contents, "{to_inject}")?;
-
-    // Write other lines
-    for line in js_lines {
-        writeln!(js_contents, "{line}")?;
-    }
-
-    // Write the debug id comment
-    writeln!(js_contents, "{DEBUGID_COMMENT_PREFIX}={debug_id}")?;
-
-    // Lastly, write the source mapping URL comment, if there was one
-    if let Some(sourcemap_comment) = sourcemap_comment {
-        writeln!(js_contents, "{sourcemap_comment}")?;
-    }
-
-    Ok(())
+    Ok(SourceMap::from_slice(map.as_bytes()).unwrap())
 }
 
 /// Fixes up a minified JS source file with a debug id without messing with mappings.
 ///
 /// This changes the source file in several ways:
 /// 1. The source code snippet
 /// `<CODE_SNIPPET>[<debug_id>]` is appended to the file.
@@ -227,52 +173,45 @@
 /// it is desirable to insert the code snippet as early as possible to make sure it runs
 /// even when an error is raised in the file.
 pub fn fixup_js_file_end(js_contents: &mut Vec<u8>, debug_id: DebugId) -> Result<()> {
     let mut js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
 
     js_contents.clear();
 
-    let sourcemap_comment_idx = js_lines
-        .iter()
-        .enumerate()
-        .rev()
-        .find(|(_idx, line)| {
-            line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
-        })
-        .map(|(idx, _)| idx);
+    let sourcemap_comment_idx = js_lines.iter().rposition(|line| {
+        line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
+    });
 
     let sourcemap_comment = sourcemap_comment_idx.map(|idx| js_lines.remove(idx));
 
     for line in js_lines.into_iter() {
         writeln!(js_contents, "{line}")?;
     }
 
     let to_inject = CODE_SNIPPET_TEMPLATE.replace(DEBUGID_PLACEHOLDER, &debug_id.to_string());
     writeln!(js_contents, "{to_inject}")?;
-    writeln!(js_contents, "{DEBUGID_COMMENT_PREFIX}={debug_id}")?;
-
     if let Some(sourcemap_comment) = sourcemap_comment {
         writeln!(js_contents, "{sourcemap_comment}")?;
     }
+    writeln!(js_contents, "{DEBUGID_COMMENT_PREFIX}={debug_id}")?;
 
     Ok(())
 }
 
 /// Replaces a JS file's source mapping url with a new one.
 ///
 /// Only the bottommost source mapping url comment will be updated. If there
 /// are no source mapping url comments in the file, this is a no-op.
 pub fn replace_sourcemap_url(js_contents: &mut Vec<u8>, new_url: &str) -> Result<()> {
     let js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
 
-    let sourcemap_comment_idx = match js_lines.iter().enumerate().rev().find(|(_idx, line)| {
+    let Some(sourcemap_comment_idx) = js_lines.iter().rposition(|line| {
         line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
-    }) {
-        Some((idx, _)) => idx,
-        None => return Ok(()),
+    }) else {
+        return Ok(());
     };
 
     js_contents.clear();
 
     for line in &js_lines[0..sourcemap_comment_idx] {
         writeln!(js_contents, "{line}")?;
     }
@@ -291,82 +230,14 @@
     let mut hash = sha1_smol::Sha1::new();
     hash.update(bytes);
     let mut sha1_bytes = [0u8; 16];
     sha1_bytes.copy_from_slice(&hash.digest().bytes()[..16]);
     DebugId::from_uuid(uuid::Builder::from_sha1_bytes(sha1_bytes).into_uuid())
 }
 
-/// Fixes up a sourcemap file with a debug id.
-///
-/// If the file already contains a debug id under the `debug_id` key, it is left unmodified.
-/// Otherwise, a fresh debug id is inserted under that key.
-///
-/// In either case, the value of the `debug_id` key is returned.
-pub fn fixup_sourcemap(sourcemap_contents: &mut Vec<u8>) -> Result<(DebugId, bool)> {
-    match sourcemap::decode_slice(sourcemap_contents).context("Invalid sourcemap")? {
-        sourcemap::DecodedMap::Regular(mut sm) => {
-            if let Some(debug_id) = sm.get_debug_id() {
-                debug!("Sourcemap already has a debug id");
-                Ok((debug_id, false))
-            } else {
-                let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
-                sm.set_debug_id(Some(debug_id));
-
-                sourcemap_contents.clear();
-                sm.to_writer(sourcemap_contents)?;
-                Ok((debug_id, true))
-            }
-        }
-        sourcemap::DecodedMap::Hermes(mut smh) => {
-            if let Some(debug_id) = smh.get_debug_id() {
-                debug!("Sourcemap already has a debug id");
-                Ok((debug_id, false))
-            } else {
-                let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
-                smh.set_debug_id(Some(debug_id));
-
-                sourcemap_contents.clear();
-                smh.to_writer(sourcemap_contents)?;
-                Ok((debug_id, true))
-            }
-        }
-        sourcemap::DecodedMap::Index(_) => {
-            bail!("DebugId injection is not supported for sourcemap indexes")
-        }
-    }
-}
-
-/// This adds an empty mapping at the start of a sourcemap.
-///
-/// This is used to adjust a sourcemap when the corresponding source file has a
-/// new line injected near the top (see [`fixup_js_file`]).
-pub fn insert_empty_mapping(sourcemap_contents: &mut Vec<u8>) -> Result<()> {
-    let mut sourcemap: Value = serde_json::from_slice(sourcemap_contents)?;
-
-    let Some(map) = sourcemap.as_object_mut() else {
-        bail!("Invalid sourcemap");
-    };
-
-    let Some(mappings) = map.get_mut("mappings") else {
-        bail!("Invalid sourcemap");
-    };
-
-    let Value::String(mappings) = mappings else {
-        bail!("Invalid sourcemap");
-    };
-
-    // Insert empty mapping at the start
-    *mappings = format!(";{mappings}");
-
-    sourcemap_contents.clear();
-    serde_json::to_writer(sourcemap_contents, &sourcemap)?;
-
-    Ok(())
-}
-
 /// Computes a normalized sourcemap URL from a source file's own URL und the relative URL of its sourcemap.
 ///
 /// Roughly, this will combine a source URL of `some/dir/source.js` and a sourcemap URL of `path/to/source.min.js`
 /// to `some/dir/path/to/source.min.js`, taking `..` and `.` path segments as well as absolute sourcemap URLs
 /// into account.
 ///
 /// Leading `./` segments will be preserved.
@@ -437,73 +308,42 @@
     }
 
     matches
 }
 
 #[cfg(test)]
 mod tests {
-    use std::io::Write;
-
     use sentry::types::DebugId;
 
     use crate::utils::fs::TempFile;
 
     use super::*;
 
     #[test]
-    fn test_fixup_sourcemap() {
-        for sourcemap_path in &[
-            "server/chunks/1.js.map",
-            "server/edge-runtime-webpack.js.map",
-            "server/pages/_document.js.map",
-            "server/pages/asdf.js.map",
-            "static/chunks/575-bb7d7e0e6de8d623.js.map",
-            "static/chunks/app/client/page-d5742c254d9533f8.js.map",
-            "static/chunks/pages/asdf-05b39167abbe433b.js.map",
-        ] {
-            let mut sourcemap_contents = std::fs::read(format!(
-                "tests/integration/_fixtures/inject/{sourcemap_path}"
-            ))
-            .unwrap();
-
-            assert!(
-                sourcemap::decode_slice(&sourcemap_contents).is_ok(),
-                "sourcemap is valid before injection"
-            );
-
-            fixup_sourcemap(&mut sourcemap_contents).unwrap();
-
-            assert!(
-                sourcemap::decode_slice(&sourcemap_contents).is_ok(),
-                "sourcemap is valid after injection"
-            );
-        }
-    }
-
-    #[test]
     fn test_fixup_js_file() {
         let source = r#"//# sourceMappingURL=fake1
 some line
 //# sourceMappingURL=fake2
 //# sourceMappingURL=real
 something else"#;
 
         let debug_id = DebugId::default();
 
         let mut source = Vec::from(source);
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"//# sourceMappingURL=fake1
+
 !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake2
+//# sourceMappingURL=real
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
-//# sourceMappingURL=real
 "#;
 
         assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
     }
 
     #[test]
     fn test_fixup_js_file_fs_roundtrip() {
@@ -543,14 +383,15 @@
             file.write_all(&source).unwrap();
         }
 
         let result = std::fs::read_to_string(temp_file.path()).unwrap();
         let expected = r#"//# sourceMappingURL=fake
 
 
+
 !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
@@ -558,17 +399,17 @@
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
+//# sourceMappingURL=real
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
-//# sourceMappingURL=real
 "#;
 
         println!("{}", result);
         assert_eq!(result, expected);
     }
 
     #[test]
@@ -590,22 +431,23 @@
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"#!/bin/node
 //# sourceMappingURL=fake1
 
   // some other comment
-"use strict"; rest of the line
-'use strict';
+"use strict";
 !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
+ rest of the line
+'use strict';
 some line
 //# sourceMappingURL=fake2
+//# sourceMappingURL=real
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
-//# sourceMappingURL=real
 "#;
 
         assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
     }
 
     #[test]
     fn test_fixup_js_file_fake_use_strict() {
@@ -626,22 +468,23 @@
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"#!/bin/node
 //# sourceMappingURL=fake1
 
   // some other comment
-"use strict"; rest of the line
+"use strict";
 !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
+ rest of the line
 (this.foo=this.bar||[]).push([[2],[function(e,t,n){"use strict"; […] }
 some line
 //# sourceMappingURL=fake2
+//# sourceMappingURL=real
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
-//# sourceMappingURL=real
 "#;
 
         assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
     }
 
     #[test]
     fn test_normalize_sourcemap_url() {
```

### Comparing `sentry_cli-2.20.3/src/utils/sourcemaps.rs` & `sentry_cli-2.20.4/src/utils/sourcemaps.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 use anyhow::{bail, Context, Error, Result};
 use console::style;
 use indicatif::ProgressStyle;
 use log::{debug, info, warn};
 use sentry::types::DebugId;
 use sha1_smol::Digest;
+use sourcemap::SourceMap;
 use symbolic::debuginfo::js::{
     discover_debug_id, discover_sourcemap_embedded_debug_id, discover_sourcemaps_location,
 };
 use symbolic::debuginfo::sourcebundle::SourceFileType;
 use url::Url;
-use uuid::Uuid;
 
 use crate::api::Api;
 use crate::utils::enc::decode_unknown_string;
 use crate::utils::file_search::ReleaseFileMatch;
 use crate::utils::file_upload::{
     initialize_legacy_release_upload, FileUpload, SourceFile, SourceFiles, UploadContext,
 };
@@ -786,142 +786,174 @@
             if let Some(debug_id) = self.debug_ids.get(source_url) {
                 report
                     .previously_injected
                     .push((source_url.into(), *debug_id));
                 continue;
             }
 
-            // Find or generate a debug id and determine whether we can inject the
-            // code snippet at the start of the source file. This is determined by whether
-            // we are able to adjust the sourcemap accordingly.
-            let (debug_id, inject_at_start) = {
-                match sourcemap_url {
-                    None => {
-                        // no source map at all, try a deterministic debug id from the contents
-                        let debug_id = self
-                            .sources
-                            .get(source_url)
-                            .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
-                            .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
-                        (debug_id, false)
-                    }
-                    Some(sourcemap_url) => {
-                        if let Some(encoded) = sourcemap_url.strip_prefix(DATA_PREAMBLE) {
-                            // Handle embedded sourcemaps
-
-                            // Update the embedded sourcemap and write it back to the source file
-                            let Ok(mut decoded) = data_encoding::BASE64.decode(encoded.as_bytes()) else {
-                                bail!("Invalid embedded sourcemap in source file {source_url}");
-                            };
-
-                            inject::insert_empty_mapping(&mut decoded)?;
-                            let encoded = data_encoding::BASE64.encode(&decoded);
-                            let new_sourcemap_url = format!("{DATA_PREAMBLE}{encoded}");
+            // Modify the source file and the sourcemap.
+            // There are several cases to consider according to whether we have a sourcemap for the source file and
+            // whether it's embedded or external.
+            let debug_id = match sourcemap_url {
+                None => {
+                    // Case 1: We have no sourcemap for the source file. Hash the file contents for the debug id.
+                    let source_file = self.sources.get_mut(source_url).unwrap();
+                    let debug_id = inject::debug_id_from_bytes_hashed(&source_file.contents);
+
+                    // If we don't have a sourcemap, it's not safe to inject the code snippet at the beginning,
+                    // because that would throw off all the mappings. Instead, inject the snippet at the very end.
+                    // This isn't ideal, but it's the best we can do in this case.
+                    inject::fixup_js_file_end(&mut source_file.contents, debug_id)
+                        .context(format!("Failed to process {}", source_file.path.display()))?;
+                    debug_id
+                }
+                Some(sourcemap_url) => {
+                    if let Some(encoded) = sourcemap_url.strip_prefix(DATA_PREAMBLE) {
+                        // Case 2: The source file has an embedded sourcemap.
+
+                        let Ok(mut decoded) = data_encoding::BASE64.decode(encoded.as_bytes())
+                        else {
+                            bail!("Invalid embedded sourcemap in source file {source_url}");
+                        };
+
+                        let sourcemap = SourceMap::from_slice(&decoded)
+                            .context("Invalid embedded sourcemap in source file {source_url}")?;
+
+                        let debug_id = sourcemap
+                            .get_debug_id()
+                            .unwrap_or_else(|| inject::debug_id_from_bytes_hashed(&decoded));
+
+                        let source_file = self.sources.get_mut(source_url).unwrap();
+                        let adjustment_map =
+                            inject::fixup_js_file(&mut source_file.contents, debug_id).context(
+                                format!("Failed to process {}", source_file.path.display()),
+                            )?;
+                        let mut adjusted_map =
+                            SourceMap::adjust_mappings(&sourcemap, &adjustment_map);
+                        adjusted_map.set_debug_id(Some(debug_id));
+
+                        decoded.clear();
+                        adjusted_map.to_writer(&mut decoded)?;
+
+                        let encoded = data_encoding::BASE64.encode(&decoded);
+                        let new_sourcemap_url = format!("{DATA_PREAMBLE}{encoded}");
+
+                        inject::replace_sourcemap_url(
+                            &mut source_file.contents,
+                            &new_sourcemap_url,
+                        )?;
+                        *sourcemap_url = new_sourcemap_url;
 
-                            let source_file = self.sources.get_mut(source_url).unwrap();
+                        debug_id
+                    } else {
+                        // Handle external sourcemaps
 
-                            // hash the new source map url for the debug id
-                            let debug_id =
-                                inject::debug_id_from_bytes_hashed(new_sourcemap_url.as_bytes());
+                        let normalized = inject::normalize_sourcemap_url(source_url, sourcemap_url);
+                        let matches = inject::find_matching_paths(&sourcemaps, &normalized);
 
-                            inject::replace_sourcemap_url(
-                                &mut source_file.contents,
-                                &new_sourcemap_url,
-                            )?;
-                            *sourcemap_url = new_sourcemap_url;
+                        let sourcemap_url = match &matches[..] {
+                            [] => normalized,
+                            [x] => x.to_string(),
+                            _ => {
+                                warn!("Ambiguous matches for sourcemap path {normalized}:");
+                                for path in matches {
+                                    warn!("{path}");
+                                }
+                                normalized
+                            }
+                        };
 
-                            (debug_id, true)
-                        } else {
-                            // Handle external sourcemaps
+                        if self.sources.contains_key(&sourcemap_url) {
+                            // Case 3: We have an external sourcemap for the source file.
 
-                            let normalized =
-                                inject::normalize_sourcemap_url(source_url, sourcemap_url);
-                            let matches = inject::find_matching_paths(&sourcemaps, &normalized);
-
-                            let sourcemap_url = match &matches[..] {
-                                [] => normalized,
-                                [x] => x.to_string(),
-                                _ => {
-                                    warn!("Ambiguous matches for sourcemap path {normalized}:");
-                                    for path in matches {
-                                        warn!("{path}");
+                            // We need to do a bit of a dance here because we can't mutably
+                            // borrow the source file and the sourcemap at the same time.
+                            let (sourcemap, debug_id, debug_id_fresh) = {
+                                let sourcemap_file = &self.sources[&sourcemap_url];
+
+                                let sm = SourceMap::from_slice(&sourcemap_file.contents).context(
+                                    format!("Invalid sourcemap at {}", sourcemap_file.url),
+                                )?;
+
+                                match sm.get_debug_id() {
+                                    Some(debug_id) => (sm, debug_id, false),
+                                    None => {
+                                        let debug_id = inject::debug_id_from_bytes_hashed(
+                                            &sourcemap_file.contents,
+                                        );
+                                        (sm, debug_id, true)
                                     }
-                                    normalized
                                 }
                             };
 
-                            match self.sources.get_mut(&sourcemap_url) {
-                                None => {
-                                    debug!("Sourcemap file {} not found", sourcemap_url);
-                                    // source map cannot be found, fall back to hashing the contents if
-                                    // available.  The v4 fallback should not happen.
-                                    let debug_id = self
-                                        .sources
-                                        .get(source_url)
-                                        .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
-                                        .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
-                                    (debug_id, false)
-                                }
-                                Some(sourcemap_file) => {
-                                    inject::insert_empty_mapping(&mut sourcemap_file.contents)
-                                        .context(format!(
-                                            "Failed to process {}",
-                                            sourcemap_file.path.display()
-                                        ))?;
-
-                                    let (debug_id, sourcemap_modified) =
-                                        inject::fixup_sourcemap(&mut sourcemap_file.contents)
-                                            .context(format!(
-                                                "Failed to process {}",
-                                                sourcemap_file.path.display()
-                                            ))?;
-
-                                    sourcemap_file
-                                        .headers
-                                        .push(("debug-id".to_string(), debug_id.to_string()));
-
-                                    if !dry_run {
-                                        let mut file = std::fs::File::create(&sourcemap_file.path)?;
-                                        file.write_all(&sourcemap_file.contents).context(
-                                            format!(
-                                                "Failed to write sourcemap file {}",
-                                                sourcemap_file.path.display()
-                                            ),
-                                        )?;
-                                    }
-
-                                    if sourcemap_modified {
-                                        report
-                                            .sourcemaps
-                                            .push((sourcemap_file.path.clone(), debug_id));
-                                    } else {
-                                        report
-                                            .skipped_sourcemaps
-                                            .push((sourcemap_file.path.clone(), debug_id));
-                                    }
+                            let source_file = self.sources.get_mut(source_url).unwrap();
+                            let adjustment_map =
+                                inject::fixup_js_file(&mut source_file.contents, debug_id)
+                                    .context(format!(
+                                        "Failed to process {}",
+                                        source_file.path.display()
+                                    ))?;
+                            let mut adjusted_map =
+                                SourceMap::adjust_mappings(&sourcemap, &adjustment_map);
+                            adjusted_map.set_debug_id(Some(debug_id));
+
+                            let sourcemap_file = self.sources.get_mut(&sourcemap_url).unwrap();
+                            sourcemap_file.contents.clear();
+                            adjusted_map.to_writer(&mut sourcemap_file.contents)?;
+
+                            sourcemap_file
+                                .headers
+                                .push(("debug-id".to_string(), debug_id.to_string()));
+
+                            if !dry_run {
+                                let mut file = std::fs::File::create(&sourcemap_file.path)?;
+                                file.write_all(&sourcemap_file.contents).context(format!(
+                                    "Failed to write sourcemap file {}",
+                                    sourcemap_file.path.display()
+                                ))?;
+                            }
 
-                                    (debug_id, true)
-                                }
+                            if debug_id_fresh {
+                                report
+                                    .sourcemaps
+                                    .push((sourcemap_file.path.clone(), debug_id));
+                            } else {
+                                report
+                                    .skipped_sourcemaps
+                                    .push((sourcemap_file.path.clone(), debug_id));
                             }
+
+                            debug_id
+                        } else {
+                            // Case 4: We have a URL for the external sourcemap, but we can't find it.
+                            // This is substantially the same as case 1.
+                            debug!("Sourcemap file {} not found", sourcemap_url);
+                            // source map cannot be found, fall back to hashing the contents.
+                            let source_file = self.sources.get_mut(source_url).unwrap();
+                            let debug_id =
+                                inject::debug_id_from_bytes_hashed(&source_file.contents);
+
+                            // If we don't have a sourcemap, it's not safe to inject the code snippet at the beginning,
+                            // because that would throw off all the mappings. Instead, inject the snippet at the very end.
+                            // This isn't ideal, but it's the best we can do in this case.
+                            inject::fixup_js_file_end(&mut source_file.contents, debug_id)
+                                .context(format!(
+                                    "Failed to process {}",
+                                    source_file.path.display()
+                                ))?;
+
+                            debug_id
                         }
                     }
                 }
             };
 
-            // Finally, inject the debug id and the code snippet into the source file
+            // Finally, some housekeeping.
             let source_file = self.sources.get_mut(source_url).unwrap();
 
-            if inject_at_start {
-                inject::fixup_js_file(&mut source_file.contents, debug_id)
-                    .context(format!("Failed to process {}", source_file.path.display()))?;
-            } else {
-                inject::fixup_js_file_end(&mut source_file.contents, debug_id)
-                    .context(format!("Failed to process {}", source_file.path.display()))?;
-            }
-
             source_file
                 .headers
                 .push(("debug-id".to_string(), debug_id.to_string()));
             self.debug_ids.insert(source_url.clone(), debug_id);
 
             if !dry_run {
                 let mut file = std::fs::File::create(&source_file.path)?;
```

### Comparing `sentry_cli-2.20.3/src/utils/system.rs` & `sentry_cli-2.20.4/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/ui.rs` & `sentry_cli-2.20.4/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/update.rs` & `sentry_cli-2.20.4/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/vcs.rs` & `sentry_cli-2.20.4/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.20.3/src/utils/xcode.rs` & `sentry_cli-2.20.4/src/utils/xcode.rs`

 * *Files identical despite different names*

