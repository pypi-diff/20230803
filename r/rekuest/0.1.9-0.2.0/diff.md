# Comparing `tmp/rekuest-0.1.9.tar.gz` & `tmp/rekuest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rekuest-0.1.9.tar", max compression
+gzip compressed data, was "rekuest-0.2.0.tar", max compression
```

## Comparing `rekuest-0.1.9.tar` & `rekuest-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,86 @@
--rw-r--r--   0        0        0     1517 2022-12-12 13:51:24.301171 rekuest-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       22 2022-08-25 12:20:46.369966 rekuest-0.1.9/rekuest/__init__.py
--rw-r--r--   0        0        0        1 2022-08-25 10:31:18.596463 rekuest-0.1.9/rekuest/actors/__init__.py
--rw-r--r--   0        0        0     3586 2022-12-12 13:46:33.108527 rekuest-0.1.9/rekuest/actors/actify.py
--rw-r--r--   0        0        0     7031 2022-12-06 17:30:19.488474 rekuest-0.1.9/rekuest/actors/base.py
--rw-r--r--   0        0        0      613 2022-12-05 15:15:47.261117 rekuest-0.1.9/rekuest/actors/builder.py
--rw-r--r--   0        0        0     1603 2022-12-05 14:32:45.913282 rekuest-0.1.9/rekuest/actors/contexts.py
--rw-r--r--   0        0        0      362 2022-12-05 13:19:02.249265 rekuest-0.1.9/rekuest/actors/errors.py
--rw-r--r--   0        0        0    12906 2022-12-06 17:34:36.992666 rekuest-0.1.9/rekuest/actors/functional.py
--rw-r--r--   0        0        0     1263 2022-12-05 14:39:02.873555 rekuest-0.1.9/rekuest/actors/helper.py
--rw-r--r--   0        0        0        0 2022-12-01 15:45:42.916521 rekuest-0.1.9/rekuest/actors/reactive/__init__.py
--rw-r--r--   0        0        0     1247 2022-12-05 15:05:17.796217 rekuest-0.1.9/rekuest/actors/reactive/api.py
--rw-r--r--   0        0        0      896 2022-12-05 13:19:57.921368 rekuest-0.1.9/rekuest/actors/vars.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.624462 rekuest-0.1.9/rekuest/agents/__init__.py
--rw-r--r--   0        0        0     6054 2022-12-05 15:15:16.293077 rekuest-0.1.9/rekuest/agents/base.py
--rw-r--r--   0        0        0      220 2022-08-25 10:31:18.632462 rekuest-0.1.9/rekuest/agents/errors.py
--rw-r--r--   0        0        0     3249 2022-08-25 10:35:28.798383 rekuest-0.1.9/rekuest/agents/stateful.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.632462 rekuest-0.1.9/rekuest/agents/transport/__init__.py
--rw-r--r--   0        0        0     3175 2022-09-27 09:09:22.881016 rekuest-0.1.9/rekuest/agents/transport/base.py
--rw-r--r--   0        0        0      461 2022-08-25 10:34:32.742780 rekuest-0.1.9/rekuest/agents/transport/errors.py
--rw-r--r--   0        0        0     2782 2022-12-02 15:00:09.037818 rekuest-0.1.9/rekuest/agents/transport/mock.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.636462 rekuest-0.1.9/rekuest/agents/transport/protocols/__init__.py
--rw-r--r--   0        0        0     3653 2022-12-01 15:23:53.003087 rekuest-0.1.9/rekuest/agents/transport/protocols/agent_json.py
--rw-r--r--   0        0        0    10082 2022-11-23 16:04:14.281104 rekuest-0.1.9/rekuest/agents/transport/websocket.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.656462 rekuest-0.1.9/rekuest/api/__init__.py
--rw-r--r--   0        0        0    67401 2022-12-12 10:58:02.194161 rekuest-0.1.9/rekuest/api/schema.py
--rw-r--r--   0        0        0     1271 2022-10-20 14:03:19.356166 rekuest-0.1.9/rekuest/contrib/fakts/websocket_agent_transport.py
--rw-r--r--   0        0        0     1211 2022-08-25 12:29:20.810549 rekuest-0.1.9/rekuest/contrib/fakts/websocket_postman_transport.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.728461 rekuest-0.1.9/rekuest/definition/__init__.py
--rw-r--r--   0        0        0    19717 2022-12-12 13:51:14.385152 rekuest-0.1.9/rekuest/definition/define.py
--rw-r--r--   0        0        0      249 2022-12-05 15:08:46.848542 rekuest-0.1.9/rekuest/definition/errors.py
--rw-r--r--   0        0        0     6774 2022-12-12 13:41:25.791605 rekuest-0.1.9/rekuest/definition/registry.py
--rw-r--r--   0        0        0      646 2022-12-05 15:05:49.416268 rekuest-0.1.9/rekuest/definition/validate.py
--rw-r--r--   0        0        0       90 2022-11-30 13:49:18.470756 rekuest-0.1.9/rekuest/errors.py
--rw-r--r--   0        0        0      920 2022-08-25 10:47:01.999333 rekuest-0.1.9/rekuest/funcs.py
--rw-r--r--   0        0        0     2095 2022-12-05 17:05:20.434796 rekuest-0.1.9/rekuest/messages.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.744461 rekuest-0.1.9/rekuest/postmans/__init__.py
--rw-r--r--   0        0        0      643 2022-12-05 16:17:31.519175 rekuest-0.1.9/rekuest/postmans/base.py
--rw-r--r--   0        0        0      151 2022-12-01 14:49:59.808507 rekuest-0.1.9/rekuest/postmans/errors.py
--rw-r--r--   0        0        0     8723 2022-09-23 09:25:56.259978 rekuest-0.1.9/rekuest/postmans/graphql.py
--rw-r--r--   0        0        0     4298 2022-12-05 16:54:26.530043 rekuest-0.1.9/rekuest/postmans/stateful.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.9/rekuest/postmans/transport/__init__.py
--rw-r--r--   0        0        0     1280 2022-12-05 16:39:10.928875 rekuest-0.1.9/rekuest/postmans/transport/base.py
--rw-r--r--   0        0        0     1021 2022-08-25 10:49:34.430923 rekuest-0.1.9/rekuest/postmans/transport/errors.py
--rw-r--r--   0        0        0     8087 2022-12-05 17:08:29.899229 rekuest-0.1.9/rekuest/postmans/transport/mock.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.9/rekuest/postmans/transport/protocols/__init__.py
--rw-r--r--   0        0        0     4991 2022-12-05 16:58:37.734336 rekuest-0.1.9/rekuest/postmans/transport/protocols/postman_json.py
--rw-r--r--   0        0        0    10175 2022-08-25 10:49:28.822937 rekuest-0.1.9/rekuest/postmans/transport/websocket.py
--rw-r--r--   0        0        0    21597 2022-12-06 14:29:03.394722 rekuest-0.1.9/rekuest/postmans/utils.py
--rw-r--r--   0        0        0      186 2022-08-25 10:31:18.752461 rekuest-0.1.9/rekuest/postmans/vars.py
--rw-r--r--   0        0        0        0 2022-08-25 11:16:08.136616 rekuest-0.1.9/rekuest/qt/__init__.py
--rw-r--r--   0        0        0     4121 2022-12-06 17:36:21.501006 rekuest-0.1.9/rekuest/qt/builders.py
--rw-r--r--   0        0        0     1268 2022-11-21 13:26:05.412588 rekuest-0.1.9/rekuest/rath.py
--rw-r--r--   0        0        0     2544 2022-12-05 14:15:28.460731 rekuest-0.1.9/rekuest/rekuest.py
--rw-r--r--   0        0        0     3498 2022-12-01 15:36:15.091875 rekuest-0.1.9/rekuest/scalars.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.792461 rekuest-0.1.9/rekuest/structures/__init__.py
--rw-r--r--   0        0        0     2181 2022-11-28 14:20:15.138457 rekuest-0.1.9/rekuest/structures/annotations.py
--rw-r--r--   0        0        0      587 2022-11-28 12:45:12.088963 rekuest-0.1.9/rekuest/structures/builder.py
--rw-r--r--   0        0        0      814 2022-11-28 12:16:43.444977 rekuest-0.1.9/rekuest/structures/default.py
--rw-r--r--   0        0        0     1180 2022-11-30 13:50:37.642886 rekuest-0.1.9/rekuest/structures/errors.py
--rw-r--r--   0        0        0     9294 2022-11-21 09:42:40.677788 rekuest-0.1.9/rekuest/structures/registry.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.796461 rekuest-0.1.9/rekuest/structures/serialization/__init__.py
--rw-r--r--   0        0        0     7918 2022-12-12 11:04:10.482091 rekuest-0.1.9/rekuest/structures/serialization/actor.py
--rw-r--r--   0        0        0     8427 2022-11-30 13:28:41.156812 rekuest-0.1.9/rekuest/structures/serialization/postman.py
--rw-r--r--   0        0        0     4010 2022-11-30 12:57:40.854191 rekuest-0.1.9/rekuest/structures/serialization/utils.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.808461 rekuest-0.1.9/rekuest/traits/__init__.py
--rw-r--r--   0        0        0     1647 2022-08-25 10:31:18.808461 rekuest-0.1.9/rekuest/traits/node.py
--rw-r--r--   0        0        0     5290 2022-12-06 10:25:13.668992 rekuest-0.1.9/rekuest/traits/ports.py
--rw-r--r--   0        0        0      741 2022-12-01 15:45:42.916521 rekuest-0.1.9/rekuest/utils.py
--rw-r--r--   0        0        0      705 2022-11-30 13:48:53.622714 rekuest-0.1.9/rekuest/widgets.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 rekuest-0.1.9/setup.py
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 rekuest-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1834 2023-08-02 20:32:32.034892 rekuest-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-05 16:17:36.433300 rekuest-0.2.0/rekuest/__init__.py
+-rw-r--r--   0        0        0       59 2023-03-04 11:58:07.077358 rekuest-0.2.0/rekuest/actors/__init__.py
+-rw-r--r--   0        0        0     4155 2023-08-02 20:32:09.434783 rekuest-0.2.0/rekuest/actors/actify.py
+-rw-r--r--   0        0        0    10236 2023-05-31 15:32:48.038312 rekuest-0.2.0/rekuest/actors/base.py
+-rw-r--r--   0        0        0     1979 2023-08-02 20:32:09.434783 rekuest-0.2.0/rekuest/actors/contexts.py
+-rw-r--r--   0        0        0     1045 2023-05-17 11:10:56.167527 rekuest-0.2.0/rekuest/actors/errors.py
+-rw-r--r--   0        0        0    14682 2023-08-02 20:32:09.434783 rekuest-0.2.0/rekuest/actors/functional.py
+-rw-r--r--   0        0        0     1705 2023-05-17 13:12:08.717804 rekuest-0.2.0/rekuest/actors/helper.py
+-rw-r--r--   0        0        0       54 2023-03-04 12:18:26.237481 rekuest-0.2.0/rekuest/actors/reactive/__init__.py
+-rw-r--r--   0        0        0     1275 2023-03-04 12:23:12.425482 rekuest-0.2.0/rekuest/actors/reactive/api.py
+-rw-r--r--   0        0        0        0 2023-04-19 13:53:51.063259 rekuest-0.2.0/rekuest/actors/transport/__init__.py
+-rw-r--r--   0        0        0     7456 2023-05-28 14:02:21.768854 rekuest-0.2.0/rekuest/actors/transport/local_transport.py
+-rw-r--r--   0        0        0     7456 2023-07-06 09:33:50.477257 rekuest-0.2.0/rekuest/actors/transport/queue_transport.py
+-rw-r--r--   0        0        0     1569 2023-05-28 13:09:47.522456 rekuest-0.2.0/rekuest/actors/transport/types.py
+-rw-r--r--   0        0        0     2291 2023-06-09 07:10:22.921014 rekuest-0.2.0/rekuest/actors/types.py
+-rw-r--r--   0        0        0      962 2023-08-02 20:32:09.434783 rekuest-0.2.0/rekuest/actors/vars.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.624462 rekuest-0.2.0/rekuest/agents/__init__.py
+-rw-r--r--   0        0        0    14336 2023-08-02 20:32:09.434783 rekuest-0.2.0/rekuest/agents/base.py
+-rw-r--r--   0        0        0      219 2023-03-04 12:00:57.861400 rekuest-0.2.0/rekuest/agents/errors.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.632462 rekuest-0.2.0/rekuest/agents/transport/__init__.py
+-rw-r--r--   0        0        0     3200 2023-05-30 08:02:11.951016 rekuest-0.2.0/rekuest/agents/transport/base.py
+-rw-r--r--   0        0        0      826 2023-05-28 10:44:13.129933 rekuest-0.2.0/rekuest/agents/transport/errors.py
+-rw-r--r--   0        0        0     2888 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/agents/transport/mock.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.636462 rekuest-0.2.0/rekuest/agents/transport/protocols/__init__.py
+-rw-r--r--   0        0        0     3836 2023-05-28 13:17:04.317994 rekuest-0.2.0/rekuest/agents/transport/protocols/agent_json.py
+-rw-r--r--   0        0        0      736 2023-05-28 13:01:04.665881 rekuest-0.2.0/rekuest/agents/transport/types.py
+-rw-r--r--   0        0        0    12000 2023-05-30 11:11:03.705198 rekuest-0.2.0/rekuest/agents/transport/websocket.py
+-rw-r--r--   0        0        0        0 2023-03-10 11:41:43.651825 rekuest-0.2.0/rekuest/agents/types.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.656462 rekuest-0.2.0/rekuest/api/__init__.py
+-rw-r--r--   0        0        0    94278 2023-07-06 12:02:30.786845 rekuest-0.2.0/rekuest/api/schema.py
+-rw-r--r--   0        0        0        0 2023-05-17 08:04:48.579861 rekuest-0.2.0/rekuest/collection/__init__.py
+-rw-r--r--   0        0        0     3356 2023-07-06 12:40:45.903313 rekuest-0.2.0/rekuest/collection/collector.py
+-rw-r--r--   0        0        0     1421 2023-06-29 15:29:01.961644 rekuest-0.2.0/rekuest/collection/shelve.py
+-rw-r--r--   0        0        0     1242 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/contrib/arkitekt/websocket_agent_transport.py
+-rw-r--r--   0        0        0     1169 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/contrib/arkitekt/websocket_postman_transport.py
+-rw-r--r--   0        0        0      885 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/contrib/rath/set_assignation_link.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.728461 rekuest-0.2.0/rekuest/definition/__init__.py
+-rw-r--r--   0        0        0    24899 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/definition/define.py
+-rw-r--r--   0        0        0      366 2023-05-19 09:15:36.328136 rekuest-0.2.0/rekuest/definition/errors.py
+-rw-r--r--   0        0        0      294 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/definition/guards.py
+-rw-r--r--   0        0        0     3033 2023-06-29 15:25:34.216651 rekuest-0.2.0/rekuest/definition/registry.py
+-rw-r--r--   0        0        0     1008 2023-03-04 13:28:09.737506 rekuest-0.2.0/rekuest/definition/utils.py
+-rw-r--r--   0        0        0      989 2023-05-17 15:15:21.415428 rekuest-0.2.0/rekuest/definition/validate.py
+-rw-r--r--   0        0        0     1261 2023-06-27 15:02:33.284258 rekuest-0.2.0/rekuest/effects.py
+-rw-r--r--   0        0        0       90 2022-11-30 13:49:18.470756 rekuest-0.2.0/rekuest/errors.py
+-rw-r--r--   0        0        0      920 2022-08-25 10:47:01.999333 rekuest-0.2.0/rekuest/funcs.py
+-rw-r--r--   0        0        0     2162 2023-05-28 13:00:49.881822 rekuest-0.2.0/rekuest/messages.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.744461 rekuest-0.2.0/rekuest/postmans/__init__.py
+-rw-r--r--   0        0        0     1428 2023-05-18 14:46:31.292204 rekuest-0.2.0/rekuest/postmans/base.py
+-rw-r--r--   0        0        0      582 2023-06-08 07:23:11.443250 rekuest-0.2.0/rekuest/postmans/errors.py
+-rw-r--r--   0        0        0     9569 2023-06-08 15:46:05.353997 rekuest-0.2.0/rekuest/postmans/graphql.py
+-rw-r--r--   0        0        0     4377 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/postmans/stateful.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.2.0/rekuest/postmans/transport/__init__.py
+-rw-r--r--   0        0        0     1199 2023-03-04 12:10:36.185467 rekuest-0.2.0/rekuest/postmans/transport/base.py
+-rw-r--r--   0        0        0     1021 2022-08-25 10:49:34.430923 rekuest-0.2.0/rekuest/postmans/transport/errors.py
+-rw-r--r--   0        0        0     8073 2023-03-04 12:10:36.185467 rekuest-0.2.0/rekuest/postmans/transport/mock.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.2.0/rekuest/postmans/transport/protocols/__init__.py
+-rw-r--r--   0        0        0     4983 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/postmans/transport/protocols/postman_json.py
+-rw-r--r--   0        0        0    10592 2023-03-04 12:17:41.849481 rekuest-0.2.0/rekuest/postmans/transport/websocket.py
+-rw-r--r--   0        0        0    24488 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/postmans/utils.py
+-rw-r--r--   0        0        0      186 2022-08-25 10:31:18.752461 rekuest-0.2.0/rekuest/postmans/vars.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:16:08.136616 rekuest-0.2.0/rekuest/qt/__init__.py
+-rw-r--r--   0        0        0     5256 2023-05-30 08:01:48.994917 rekuest-0.2.0/rekuest/qt/builders.py
+-rw-r--r--   0        0        0     1358 2023-03-04 12:10:36.185467 rekuest-0.2.0/rekuest/rath.py
+-rw-r--r--   0        0        0     9651 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/register.py
+-rw-r--r--   0        0        0     2175 2023-05-19 09:38:05.899368 rekuest-0.2.0/rekuest/rekuest.py
+-rw-r--r--   0        0        0     4974 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/scalars.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.792461 rekuest-0.2.0/rekuest/structures/__init__.py
+-rw-r--r--   0        0        0     2150 2023-03-04 12:10:36.181467 rekuest-0.2.0/rekuest/structures/annotations.py
+-rw-r--r--   0        0        0     2552 2023-07-06 09:43:49.923985 rekuest-0.2.0/rekuest/structures/default.py
+-rw-r--r--   0        0        0     1180 2022-11-30 13:50:37.642886 rekuest-0.2.0/rekuest/structures/errors.py
+-rw-r--r--   0        0        0      580 2023-07-06 12:34:18.717287 rekuest-0.2.0/rekuest/structures/parse_collectables.py
+-rw-r--r--   0        0        0    11103 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/structures/registry.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.796461 rekuest-0.2.0/rekuest/structures/serialization/__init__.py
+-rw-r--r--   0        0        0     8965 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/structures/serialization/actor.py
+-rw-r--r--   0        0        0    10980 2023-08-02 20:32:09.438783 rekuest-0.2.0/rekuest/structures/serialization/postman.py
+-rw-r--r--   0        0        0     1412 2023-07-06 11:04:57.711298 rekuest-0.2.0/rekuest/structures/serialization/predication.py
+-rw-r--r--   0        0        0     4003 2023-03-04 12:10:36.185467 rekuest-0.2.0/rekuest/structures/serialization/utils.py
+-rw-r--r--   0        0        0      323 2023-05-25 11:29:41.836949 rekuest-0.2.0/rekuest/structures/types.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.808461 rekuest-0.2.0/rekuest/traits/__init__.py
+-rw-r--r--   0        0        0     1658 2023-03-04 12:34:42.417498 rekuest-0.2.0/rekuest/traits/node.py
+-rw-r--r--   0        0        0     5366 2023-06-05 09:10:11.978729 rekuest-0.2.0/rekuest/traits/ports.py
+-rw-r--r--   0        0        0      272 2023-06-27 14:43:00.601308 rekuest-0.2.0/rekuest/utils.py
+-rw-r--r--   0        0        0     3057 2023-06-27 13:40:49.968584 rekuest-0.2.0/rekuest/widgets.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 rekuest-0.2.0/PKG-INFO
```

### Comparing `rekuest-0.1.9/pyproject.toml` & `rekuest-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 [tool.poetry]
 name = "rekuest"
-version = "0.1.9"
+version = "0.2.0"
 description = "rpc and node backbone"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "rekuest" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 docstring-parser = ">=0.11"
 inflection = "^0.5.1"
 websockets = "^10.0"
-rath = ">=0.3.4"
-koil = ">=0.2.10"
 pydantic = ">=1.9.0"
 annotated-types = "^0.4.0"
-pytest-asyncio = "^0.20.2"
-pytest-aiohttp = "^1.0.4"
+rath = ">=0.4.0"
+
+[tool.ruff]
+extend-select = ["ANN", "D1"]
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
 
+# Same as Black.
+line-length = 100
 
 [tool.poetry.group.dev.dependencies]
 testcontainers = "3.7.0"
 autoflake = "^1.7.7"
 pytest = "^7.2.0"
-PyQtWebEngine = "^5.15.5"
-PyQt5 = "^5.15.6"
-pytest-qt = "^4.2.0"
 pytest-asyncio = "^0.20.2"
-turms = { version = ">=0.2.3", python = "^3.9" }
+turms = { version = ">=0.3.1", python = "^3.9" }
 aiohttp = "^3.8.3"
 websockets = "^10.4"
-black = "^22.10.0"
+black = "^23.1.0"
 pytest-cov = "^4.0.0"
 pytest-aiohttp = "^1.0.4"
+ruff = "^0.0.254"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `rekuest-0.1.9/rekuest/actors/actify.py` & `rekuest-0.2.0/rekuest/actors/actify.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from rekuest.actors.base import Actor
 from rekuest.actors.functional import (
     FunctionalFuncActor,
     FunctionalGenActor,
     FunctionalThreadedFuncActor,
     FunctionalThreadedGenActor,
+    FunctionalProcessedFuncActor,
+    FunctionalProcessedGenActor,
 )
 
 import inspect
 from rekuest.structures.registry import StructureRegistry
 from rekuest.agents.transport.base import AgentTransport
 from rekuest.messages import Provision
-import inspect
-from .builder import ActorBuilder
 from rekuest.definition.define import prepare_definition
-from typing import Protocol, runtime_checkable, Callable
+from rekuest.actors.types import ActorBuilder
+from rekuest.api.schema import PortGroupInput, DefinitionInput, WidgetInput, EffectInput
+from typing import Optional, Any, Dict, Union, Callable, Coroutine, Type, List, Tuple
+from rekuest.actors.base import Passport
+from rekuest.actors.transport.types import ActorTransport
 
 
 async def async_none_provide(prov: Provision):
     """Do nothing on provide"""
     return None
 
 
@@ -30,64 +33,58 @@
     """Higher order builder for actors#
 
     This is a higher order builder for actors. It takes a Actor class and
     returns a builder function that inserts the parameters into the class
     constructor. Akin to a partial function.
     """
 
-    def inside_builder(
-        provision: Provision,
-        transport: AgentTransport,
-    ):
-
+    def inside_builder(**kwargs):
         return builder(
-            provision=provision,
-            transport=transport,
+            **kwargs,
             **params,
         )
 
-    inside_builder.__name__ = builder.__name__
-    inside_builder.__definition__ = params["definition"]
-
     return inside_builder
 
 
-@runtime_checkable
-class Actifier(Protocol):
-    """An actifier is a function that takes a callable and a structure registry
-    as well as optional arguments
-
-    """
-
-    def __call__(
-        self, function: Callable, structure_registry: StructureRegistry, **kwargs
-    ) -> ActorBuilder:
-        ...
-
-
 def reactify(
     function,
     structure_registry: StructureRegistry,
     bypass_shrink=False,
     bypass_expand=False,
     on_provide=None,
-    widgets=None,
-    interfaces=None,
     on_unprovide=None,
+    collections: List[str] = None,
+    effects: Dict[str, EffectInput] = None,
+    port_groups: Optional[List[PortGroupInput]] = None,
+    groups: Optional[Dict[str, List[str]]] = None,
+    is_test_for: Optional[List[str]] = None,
+    widgets: Dict[str, WidgetInput] = None,
+    interfaces: List[str] = [],
+    in_process: bool = False,
     **params,
-) -> ActorBuilder:
+) -> Tuple[DefinitionInput, ActorBuilder]:
     """Reactify a function
 
-    This function takes a callable (of type async or sync function or generator) and returns a builder function that
-    creates an actor that makes the function callable from the rekuest server. The callable will be both in the context
-    of  an assignation and a provision helper, enabling the usage of the function as a provision helper.
+    This function takes a callable (of type async or sync function or generator) and
+    returns a builder function that creates an actor that makes the function callable
+    from the rekuest server.
     """
 
     definition = prepare_definition(
-        function, structure_registry, widgets=widgets, interfaces=interfaces
+        function,
+        structure_registry,
+        widgets=widgets,
+        interfaces=interfaces,
+        port_groups=port_groups,
+        collections=collections,
+        groups=groups,
+        effects=effects,
+        is_test_for=is_test_for,
+        **params,
     )
 
     is_coroutine = inspect.iscoroutinefunction(function)
     is_asyncgen = inspect.isasyncgenfunction(function)
     is_method = inspect.ismethod(function)
 
     is_generatorfunction = inspect.isgeneratorfunction(function)
@@ -97,20 +94,33 @@
         "assign": function,
         "expand_inputs": not bypass_expand,
         "shrink_outputs": not bypass_shrink,
         "on_provide": on_provide if on_provide else async_none_provide,
         "on_unprovide": on_unprovide if on_unprovide else async_none_unprovide,
         "structure_registry": structure_registry,
         "definition": definition,
-        **params,
     }
 
+    print(in_process)
+
     if is_coroutine:
-        return higher_order_builder(FunctionalFuncActor, **actor_attributes)
+        return definition, higher_order_builder(FunctionalFuncActor, **actor_attributes)
     elif is_asyncgen:
-        return higher_order_builder(FunctionalGenActor, **actor_attributes)
-    elif is_generatorfunction:
-        return higher_order_builder(FunctionalThreadedGenActor, **actor_attributes)
-    elif is_function or is_method:
-        return higher_order_builder(FunctionalThreadedFuncActor, **actor_attributes)
+        return definition, higher_order_builder(FunctionalGenActor, **actor_attributes)
+    elif is_generatorfunction and not in_process:
+        return definition, higher_order_builder(
+            FunctionalThreadedGenActor, **actor_attributes
+        )
+    elif (is_function or is_method) and not in_process:
+        return definition, higher_order_builder(
+            FunctionalThreadedFuncActor, **actor_attributes
+        )
+    elif is_generatorfunction and in_process:
+        return definition, higher_order_builder(
+            FunctionalProcessedGenActor, **actor_attributes
+        )
+    elif (is_function or is_method) and in_process:
+        return definition, higher_order_builder(
+            FunctionalProcessedFuncActor, **actor_attributes
+        )
     else:
         raise NotImplementedError("No way of converting this to a function")
```

### Comparing `rekuest-0.1.9/rekuest/actors/base.py` & `rekuest-0.2.0/rekuest/actors/transport/local_transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,204 +1,253 @@
-from typing import Any, Dict, Optional, Union
+from abc import abstractmethod
+from typing import Any, Awaitable, Callable, List, Optional, Union
 
-from pydantic import BaseModel, Field, PrivateAttr
-from rekuest.agents.transport.base import AgentTransport
-from rekuest.structures.registry import (
-    StructureRegistry,
-)
-import asyncio
-import logging
+from rekuest.messages import Assignation, Unassignation, Provision, Unprovision
 from rekuest.api.schema import (
-    AssignationLogLevel,
-    AssignationStatus,
-    ProvisionFragment,
-    ProvisionFragmentTemplate,
-    ProvisionLogLevel,
+    LogLevelInput,
     ProvisionMode,
     ProvisionStatus,
-    aget_template,
-    TemplateFragment,
+    AssignationStatus,
+)
+from koil.composition import KoiledModel
+from typing import Protocol, runtime_checkable
+from rekuest.agents.transport.protocols.agent_json import (
+    AssignationChangedMessage,
+    ProvisionChangedMessage,
+    ProvisionMode,
 )
-from rekuest.messages import Assignation, Provision, Unassignation
-from rekuest.actors.errors import UnknownMessageError
-from koil.types import Contextual
-from rekuest.definition.define import DefinitionInput
+import logging
+import asyncio
+from rekuest.agents.transport.base import AgentTransport
+from rekuest.actors.types import Passport, Assignment
+
 
 logger = logging.getLogger(__name__)
 
 
-class Actor(BaseModel):
+@runtime_checkable
+class Broadcast(Protocol):
+    def __call__(
+        self,
+        assignation: Union[Assignation, Unassignation, Provision, Unprovision],
+    ) -> Awaitable[None]:
+        ...
 
-    """A definition is a descriptor of the serialization of inputs and outputs of an actor. It is a necessary element to be registered on a rekuest server"""
 
-    provision: Provision
-    """ A provision is a providing request illustrating the context of the actor. This can be provided by a governing actor or by arkitekt itself. """
+class LocalTransport(KoiledModel):
+    """Agent Transport
 
-    transport: AgentTransport
+    A Transport is a means of communicating with an Agent. It is responsible for sending
+    and receiving messages from the backend. It needs to implement the following methods:
 
-    runningAssignments: Dict[str, Assignation] = Field(default_factory=dict)
+    list_provision: Getting the list of active provisions from the backend. (depends on the backend)
+    list_assignation: Getting the list of active assignations from the backend. (depends on the backend)
 
-    _in_queue: Contextual[asyncio.Queue] = PrivateAttr(default=None)
-    _runningTasks: Dict[str, asyncio.Task] = PrivateAttr(default_factory=dict)
-    _provision_task: asyncio.Task = PrivateAttr(default=None)
+    change_assignation: Changing the status of an assignation. (depends on the backend)
+    change_provision: Changing the status of an provision. (depends on the backend)
 
-    async def on_provide(self, provision: Provision):
-        return None
+    broadcast: Configuring the callbacks for the transport on new assignation, unassignation provision and unprovison.
 
-    async def on_unprovide(self):
-        return None
+    if it is a stateful connection it can also implement the following methods:
 
-    async def on_assign(self, assignation: Assignation):
-        raise NotImplementedError(
-            "Needs to be owerwritten in Actor Subclass. Never use this class directly"
-        )
+    aconnect
+    adisconnect
+
+    """
 
-    async def apass(self, message: Union[Assignation, Unassignation]):
+    broadcast: Broadcast
 
-        assert self._in_queue, "Actor is currently not listening"
-        await self._in_queue.put(message)
+    @property
+    def connected(self):
+        return True
 
-    async def arun(self):
+    async def change_provision(
+        self,
+        id: str,
+        status: ProvisionStatus = None,
+        message: str = None,
+        mode: ProvisionMode = None,
+    ):
+        await self.broadcast(
+            ProvisionChangedMessage(
+                provision=id, status=status, message=message, mode=mode
+            )
+        )
 
-        self._in_queue = asyncio.Queue()
-        self._provision_task = asyncio.create_task(self.alisten())
-        return self._provision_task
+    async def change_assignation(
+        self,
+        id: str,
+        status: AssignationStatus = None,
+        message: str = None,
+        returns: List[Any] = None,
+        progress: int = None,
+    ):
+        await self.broadcast(
+            AssignationChangedMessage(
+                assignation=id, status=status, message=message, returns=returns
+            )
+        )
 
-    async def acancel(self):
-        """Cancel the actor and all its tasks, with its internal backoff strategy"""
-        logger.info("We are getting cancelled here?")
-        await self.astop()
+    async def log_to_provision(
+        self,
+        id: str,
+        level: LogLevelInput = None,
+        message: str = None,
+    ):
+        logger.info(f"{id} {level} {message}")
+
+    async def log_to_assignation(
+        self,
+        id: str,
+        level: LogLevelInput = None,
+        message: str = None,
+    ):
+        logger.info(f"{id} {level} {message}")
 
-    async def astop(self):
-        if not self._provision_task or self._provision_task.done():
-            return
+    async def __aenter__(self):
+        return self
 
-        self._provision_task.cancel()
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        pass
 
-        try:
-            await self._provision_task
-        except asyncio.CancelledError:
-            logger.info("Provision was cancelled")
+    class Config:
+        underscore_attrs_are_private = True
+        arbitrary_types_allowed = True
+        copy_on_model_validation = False
 
-    async def aass_log(self, id: str, message: str, level=AssignationLogLevel.INFO):
-        logging.critical(f"ASS {id} {message}")
-        await self.transport.log_to_assignation(id=id, level=level, message=message)
-        logging.critical(f"ASS SEND {message}")
 
-    async def aprov_log(self, message: str, level=ProvisionLogLevel.INFO):
-        logging.critical(f"PROV {self.provision.provision} {message}")
-        await self.transport.log_to_provision(
-            id=self.provision.provision, level=level, message=message
+class AgentActorAssignTransport(KoiledModel):
+    actor_transport: "AgentActorTransport"
+    assignment: Assignment
+
+    async def change_assignation(
+        self,
+        status: AssignationStatus = None,
+        message: str = None,
+        returns: List[Any] = None,
+        progress: int = None,
+    ):
+        await self.actor_transport.agent_transport.change_assignation(
+            id=self.assignment.assignation,
+            status=status,
+            message=message,
+            returns=returns,
+            progress=progress,
         )
 
-    async def provide(self):
-        try:
-            await self.on_provide(self.provision)
-            await self.transport.change_provision(
-                self.provision.provision,
-                status=ProvisionStatus.ACTIVE,
-            )
+    async def log_to_assignation(
+        self,
+        level: LogLevelInput = None,
+        message: str = None,
+    ):
+        await self.actor_transport.agent_transport.log_to_assignation(
+            id=self.assignment.assignation, level=level or "DEBUG", message=message
+        )
 
-        except Exception as e:
-            logging.critical(
-                f"Providing Error {self.provision.provision} {e}", exc_info=True
-            )
-            await self.transport.change_provision(
-                self.provision.provision,
-                status=ProvisionStatus.CRITICAL,
-                message=str(e),
-            )
+    class Config:
+        underscore_attrs_are_private = True
+        arbitrary_types_allowed = True
+        copy_on_model_validation = False
 
-    async def unprovide(self):
-        try:
-            await self.on_unprovide(self.provision)
-            await self.transport.change_provision(
-                self.provision.provision,
-                status=ProvisionStatus.INACTIVE,
-            )
 
-        except Exception as e:
-            logging.critical(
-                f"Unproviding Error {self.provision.provision} {e}", exc_info=True
-            )
-            await self.transport.change_provision(
-                self.provision.provision,
-                status=ProvisionStatus.CRITICAL,
-                message=str(e),
-            )
+class AgentActorTransport(KoiledModel):
+    """Agent Transport
 
-    async def process(self, message: Union[Assignation, Unassignation]):
-        logger.info(f"Actor for {self.provision}: Received {message}")
+    A Transport is a means of communicating with an Agent. It is responsible for sending
+    and receiving messages from the backend. It needs to implement the following methods:
 
-        if isinstance(message, Assignation):
-            task = asyncio.create_task(self.on_assign(message))
-            self.runningAssignments[message.assignation] = task
-            return task
-
-        elif isinstance(message, Unassignation):
-            if message.assignation in self.runningAssignments:
-                task = self.runningAssignments[message.assignation]
-                if not task.done():
-                    task.cancel()
-                else:
-                    logger.error("Task was already done")
-            else:
-                await self.transport.change_assignation(
-                    message.assignation,
-                    status=AssignationStatus.CRITICAL,
-                    message="Task was never assigned",
-                )
-        else:
-            raise UnknownMessageError(f"{message}")
-
-    async def alisten(self):
-        try:
-            await self.provide()
-            logger.info(f"Actor for {self.provision}: Is now active")
-
-            while True:
-                message = await self._in_queue.get()
-                await self.process(message)
-
-        except asyncio.CancelledError as e:
-            logger.info("Doing Whatever needs to be done to cancel!")
-
-            cancel_assignations = [i.cancel() for i in self.runningAssignments.values()]
-
-            for i in self.runningAssignments.values():
-                try:
-                    await i
-                except asyncio.CancelledError:
-                    pass
-
-            await self.unprovide()
-
-            # TODO: Maybe send back an acknoledgement that we are done cancelling.
-            # If we don't do this, arkitekt will not know if we failed to cancel our
-            # tasks or if we succeeded. If we fail to cancel arkitekt can try to
-            # kill the whole agent (maybe causing a sys.exit(1) or something)
-
-        self._in_queue = None
-
-    def _provision_task_done(self, task):
-        logger.info(f"Provision task is done: {task}")
-        if task.exception():
-            raise task.exception()
+    list_provision: Getting the list of active provisions from the backend. (depends on the backend)
+    list_assignation: Getting the list of active assignations from the backend. (depends on the backend)
 
-    async def __aenter__(self):
-        return self
+    change_assignation: Changing the status of an assignation. (depends on the backend)
+    change_provision: Changing the status of an provision. (depends on the backend)
+
+    broadcast: Configuring the callbacks for the transport on new assignation, unassignation provision and unprovison.
 
-    async def __aexit__(self, exc_type, exc, tb):
-        if self._provision_task and not self._provision_task.done():
-            await self.acancel()
+    if it is a stateful connection it can also implement the following methods:
+
+    aconnect
+    adisconnect
+
+    """
+
+    passport: Passport
+    agent_transport: AgentTransport
+
+    @property
+    def connected(self):
+        return True
+
+    async def change_provision(
+        self,
+        status: ProvisionStatus = None,
+        message: str = None,
+        mode: ProvisionMode = None,
+    ):
+        await self.agent_transport.change_provision(
+            self.passport.provision, status=status, message=message, mode=mode
+        )
+
+    async def log_to_provision(
+        self,
+        id: str,
+        level: LogLevelInput = None,
+        message: str = None,
+    ):
+        logger.info(f"{id} {level} {message}")
+        await self.agent_transport.log_to_provision(
+            id=self.passport.provision, level=level, message=message
+        )
+
+    def spawn(self, assignment: Assignment) -> AgentActorAssignTransport:
+        return AgentActorAssignTransport(actor_transport=self, assignment=assignment)
 
     class Config:
+        underscore_attrs_are_private = True
         arbitrary_types_allowed = True
+        copy_on_model_validation = False
+
+
+AgentActorAssignTransport.update_forward_refs()
+
+
+class ProxyAssignTransport(KoiledModel):
+    assignment: Assignment
+    on_change: Callable
+    on_log: Callable
+
+    async def change_assignation(self, *args, **kwargs):
+        await self.on_change(self.assignment, *args, **kwargs)
+
+    async def log_to_assignation(self, *args, **kwargs):
+        await self.on_log(self.assignment, *args, **kwargs)
+
+    class Config:
         underscore_attrs_are_private = True
+        arbitrary_types_allowed = True
         copy_on_model_validation = False
 
 
-class SerializingActor(Actor):
-    definition: DefinitionInput
-    structure_registry: StructureRegistry
-    expand_inputs: bool = True
-    shrink_outputs: bool = True
+class ProxyActorTransport(KoiledModel):
+    on_log: Callable
+    on_change: Callable
+    on_assign_change: Callable
+    on_assign_log: Callable
+
+    async def change_provision(self, *args, **kwargs):
+        await self.on_change(*args, **kwargs)
+
+    async def log_to_provision(self, *args, **kwargs):
+        await self.on_log(*args, **kwargs)
+
+    async def change_assignation(self, *args, **kwargs):
+        await self.on_assign_change(*args, **kwargs)
+
+    async def log_to_assignation(self, *args, **kwargs):
+        await self.on_assign_log(*args, **kwargs)
+
+    def spawn(self, assignment: Assignment) -> AgentActorAssignTransport:
+        return ProxyAssignTransport(
+            assignment=assignment,
+            on_change=self.change_assignation,
+            on_log=self.log_to_assignation,
+        )
```

### Comparing `rekuest-0.1.9/rekuest/actors/reactive/api.py` & `rekuest-0.2.0/rekuest/actors/reactive/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from rekuest.actors.vars import (
     get_current_assignation_helper,
     get_current_provision_helper,
 )
 from rekuest.api.schema import LogLevelInput
-from rekuest.actors.vars import (
-    get_current_assignation_helper,
-    get_current_provision_helper,
-)
 
 
 async def alog(message: str, level: LogLevelInput = LogLevelInput.DEBUG) -> None:
     await get_current_assignation_helper().alog(level, message)
 
 
+def log(message: str, level: LogLevelInput = LogLevelInput.DEBUG) -> None:
+    get_current_assignation_helper().log(level, message)
+
+
 async def plog(message: str, level: LogLevelInput = LogLevelInput.DEBUG) -> None:
     await get_current_provision_helper().alog(level, message)
 
 
 def useUser() -> str:
     """Returns the user id of the current assignation"""
     return get_current_assignation_helper().user
```

### Comparing `rekuest-0.1.9/rekuest/actors/vars.py` & `rekuest-0.2.0/rekuest/actors/vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import contextvars
 from rekuest.actors.helper import AssignationHelper, ProvisionHelper
 from rekuest.actors.errors import NotWithinAnAssignationError, NotWithinAProvisionError
 
+current_assignment = contextvars.ContextVar("current_assignment")
 current_assignation_helper = contextvars.ContextVar("current_assignation_helper")
 current_provision_helper = contextvars.ContextVar("current_provision_helper")
 
 
 def get_current_assignation_helper() -> AssignationHelper:
     try:
         return current_assignation_helper.get()
```

### Comparing `rekuest-0.1.9/rekuest/agents/transport/base.py` & `rekuest-0.2.0/rekuest/agents/transport/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     LogLevelInput,
     ProvisionMode,
     ProvisionStatus,
     AssignationStatus,
 )
 from koil.composition import KoiledModel
 from koil.types import Contextual
+from .types import TransportCallbacks
 
 
 class AgentTransport(KoiledModel):
     """Agent Transport
 
     A Transport is a means of communicating with an Agent. It is responsible for sending
     and receiving messages from the backend. It needs to implement the following methods:
@@ -29,19 +30,15 @@
     if it is a stateful connection it can also implement the following methods:
 
     aconnect
     adisconnect
 
     """
 
-    _abroadcast: Contextual[
-        Callable[
-            [Union[Assignation, Unassignation, Unprovision, Provision]], Awaitable[None]
-        ]
-    ]
+    _callback: Contextual[TransportCallbacks]
 
     @property
     def connected(self):
         return NotImplementedError("Implement this method")
 
     @abstractmethod
     async def list_provisions(
@@ -90,14 +87,17 @@
 
     @abstractmethod
     async def list_assignations(
         self, exclude: Optional[AssignationStatus] = None
     ) -> List[Assignation]:
         raise NotImplementedError("This is an abstract Base Class")
 
+    def set_callback(self, callback: TransportCallbacks):
+        self._callback = callback
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         pass
 
     class Config:
```

### Comparing `rekuest-0.1.9/rekuest/agents/transport/mock.py` & `rekuest-0.2.0/rekuest/agents/transport/mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from rekuest.agents.transport.base import AgentTransport
-from rekuest.agents.transport.protocols.agent_json import *
-from rekuest.messages import Assignation, Provision, Provision, Unprovision
+from rekuest.agents.transport.protocols.agent_json import (
+    AssignationChangedMessage,
+    ProvisionChangedMessage,
+    ProvisionMode,
+)
+from rekuest.messages import (
+    Assignation,
+    Provision,
+    Unprovision,
+    Unassignation,
+)
 from rekuest.api.schema import AssignationStatus, LogLevelInput, ProvisionStatus
 from typing import Any, List, Optional, Union
 import asyncio
 from koil import unkoil
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `rekuest-0.1.9/rekuest/agents/transport/protocols/agent_json.py` & `rekuest-0.2.0/rekuest/agents/transport/protocols/agent_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from rekuest.messages import (
     Assignation,
     AssignationLog,
     Provision,
     ProvisionLog,
     Unassignation,
     Unprovision,
+    Inquiry,
 )
 from pydantic import BaseModel, Field
 
 
 class AgentMessageTypes(str, Enum):
-
     ASSIGN_CHANGED = "ASSIGN_CHANGED"
     PROVIDE_CHANGED = "PROVIDE_CHANGED"
 
     ASSIGN_LOG = "ASSIGN_LOG"
     PROVIDE_LOG = "PROVIDE_LOG"
 
     LIST_ASSIGNATIONS = "LIST_ASSIGNATIONS"
@@ -31,18 +31,19 @@
 
     LIST_PROVISIONS = "LIST_PROVISIONS"
     LIST_PROVISIONS_REPLY = "LIST_PROVISIONS_REPLY"
     LIST_PROVISIONS_DENIED = "LIST_PROVISIONS_DENIED"
 
 
 class AgentSubMessageTypes(str, Enum):
-
+    HELLO = "HELLO"
     ASSIGN = "ASSIGN"
     UNASSIGN = "UNASSIGN"
     PROVIDE = "PROVIDE"
+    INQUIRY = "INQUIRY"
     UNPROVIDE = "UNPROVIDE"
 
 
 class JSONMeta(BaseModel):
     timestamp: datetime = Field(default_factory=datetime.utcnow)
 
 
@@ -101,14 +102,18 @@
 
 
 class AssignSubMessage(JSONMessage, Assignation):
     type: Literal[AgentSubMessageTypes.ASSIGN] = AgentSubMessageTypes.ASSIGN
     guardian: str
 
 
+class InquirySubMessage(JSONMessage, Inquiry):
+    type: Literal[AgentSubMessageTypes.INQUIRY] = AgentSubMessageTypes.INQUIRY
+
+
 class ProvideSubMessage(JSONMessage, Provision):
     type: Literal[AgentSubMessageTypes.PROVIDE] = AgentSubMessageTypes.PROVIDE
     guardian: str
 
 
 class UnassignSubMessage(JSONMessage, Unassignation):
     type: Literal[AgentSubMessageTypes.UNASSIGN] = AgentSubMessageTypes.UNASSIGN
```

### Comparing `rekuest-0.1.9/rekuest/agents/transport/websocket.py` & `rekuest-0.2.0/rekuest/postmans/transport/websocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,121 @@
-from typing import Awaitable, Callable, Dict, Any
-import websockets
-from rekuest.agents.transport.base import AgentTransport
 import asyncio
 import json
-from rekuest.agents.transport.errors import (
-    AgentTransportException,
+
+import websockets
+from rekuest.api.schema import AssignationStatus, ReservationStatus, ReserveParamsInput
+from rekuest.postmans.transport.base import PostmanTransport
+from typing import Any, Awaitable, Callable, Dict, List, Optional
+from rekuest.messages import Assignation, Reservation
+from rekuest.postmans.transport.errors import (
+    AssignDeniedError,
     AssignationListDeniedError,
-    ProvisionListDeniedError,
+    PostmanTransportException,
+    ReservationListDeniedError,
+    ReserveDeniedError,
+    UnassignDeniedError,
+    UnreserveDeniedError,
+)
+from pydantic import Field
+from rekuest.postmans.transport.protocols.postman_json import (
+    JSONMessage,
+    AssignList,
+    AssignPub,
+    AssignPubReply,
+    AssignSubUpdate,
+    AssingListReply,
+    PostmanMessageTypes,
+    PostmanSubMessageTypes,
+    ReserveList,
+    ReserveListReply,
+    ReservePub,
+    ReservePubReply,
+    ReserveSubUpdate,
+    UnassignPub,
+    UnassignPubReply,
+    UnreservePub,
+    UnreservePubReply,
 )
-from rekuest.agents.transport.protocols.agent_json import *
 import logging
 from websockets.exceptions import ConnectionClosedError, InvalidStatusCode
-from rekuest.api.schema import LogLevelInput
-import ssl
-import certifi
-from koil.types import ContextBool, Contextual
 
 logger = logging.getLogger(__name__)
 
 
 async def token_loader():
     raise NotImplementedError(
         "Websocket transport does need a defined token_loader on Connection"
     )
 
 
-class CorrectableConnectionFail(AgentTransportException):
+class CorrectableConnectionFail(PostmanTransportException):
     pass
 
 
-class DefiniteConnectionFail(AgentTransportException):
+class DefiniteConnectionFail(PostmanTransportException):
     pass
 
 
-class WebsocketAgentTransport(AgentTransport):
+class WebsocketPostmanTransport(PostmanTransport):
     endpoint_url: str
-    ssl_context: ssl.SSLContext = Field(
-        default_factory=lambda: ssl.create_default_context(cafile=certifi.where())
-    )
     token_loader: Callable[[], Awaitable[str]] = Field(exclude=True)
     max_retries = 5
-    time_between_retries = 3
+    time_between_retries = 5
     allow_reconnect = True
+
     auto_connect = True
 
-    _futures: Contextual[Dict[str, asyncio.Future]] = None
-    _connected: ContextBool = False
-    _healthy: ContextBool = False
-    _send_queue: Contextual[asyncio.Queue] = None
-    _connection_task: Contextual[asyncio.Task] = None
-
-    async def __aenter__(self):
-        assert self._abroadcast is not None, "Broadcast ss be defined"
-        self._futures = {}
-        self._send_queue = asyncio.Queue()
+    _futures: Dict[str, asyncio.Future] = {}
+    _connected = False
+    _healthy = False
+    _send_queue: Optional[asyncio.Queue] = None
+    _connection_task: Optional[asyncio.Task] = None
+
+    async def aconnect(self):
+        assert self._abroadcast is not None, (
+            "Broadcast must be defined (either overwrite abroadcast or pass this in"
+            " constructor of transport)"
+        )
 
-    async def aconnect(self, instance_id: str = "default"):
-        self._connection_task = asyncio.create_task(self.websocket_loop(instance_id))
+        assert self.instance_id, "Needs an instance id"
+        self._send_queue = asyncio.Queue()
+        self._connection_task = asyncio.create_task(self.websocket_loop())
         self._connected = True
 
-    async def websocket_loop(self, instance_id: str, retry=0, reload_token=False):
+    async def websocket_loop(self, retry=0, reload_token=False):
         send_task = None
         receive_task = None
         try:
             try:
                 token = await self.token_loader(force_refresh=reload_token)
 
                 async with websockets.connect(
-                    f"{self.endpoint_url}?token={token}&instance_id={instance_id}",
-                    ssl=self.ssl_context
-                    if self.endpoint_url.startswith("wss")
-                    else None,
+                    f"{self.endpoint_url}?token={token}&instance_id={self.instance_id}"
                 ) as client:
-
-                    logger.info("Agent on Websockets connected")
+                    logger.info("Postman on Websockets connected")
 
                     send_task = asyncio.create_task(self.sending(client))
                     receive_task = asyncio.create_task(self.receiving(client))
 
                     self._healthy = True
                     done, pending = await asyncio.wait(
                         [send_task, receive_task],
                         return_when=asyncio.FIRST_EXCEPTION,
                     )
-                    self._healthy = False
+                    self._healthy = True
 
                     for task in pending:
                         task.cancel()
 
                     for task in done:
                         raise task.exception()
 
             except InvalidStatusCode as e:
                 logger.warning(
-                    "Websocket Connect was denied. Trying to reload token",
+                    f"Websocket Connect was denied. Trying to reload token {token}",
                     exc_info=True,
                 )
                 reload_token = True
                 raise CorrectableConnectionFail from e
 
             except ConnectionClosedError as e:
                 logger.warning("Websocket was closed", exc_info=True)
@@ -106,181 +124,177 @@
             except Exception as e:
                 logger.warning("Websocket excepted. Trying to recover", exc_info=True)
                 raise CorrectableConnectionFail from e
 
         except CorrectableConnectionFail as e:
             logger.info(f"Trying to Recover from Exception {e}")
             if retry > self.max_retries or not self.allow_reconnect:
-                logger.error("Max retries reached. Giving up")
                 raise DefiniteConnectionFail("Exceeded Number of Retries")
 
             await asyncio.sleep(self.time_between_retries)
-            logger.info(f"Retrying to connect")
-            await self.websocket_loop(
-                instance_id, retry=retry + 1, reload_token=reload_token
-            )
+            logger.info("Retrying to connect")
+            await self.websocket_loop(retry=retry + 1, reload_token=reload_token)
 
         except DefiniteConnectionFail as e:
             logger.error("Websocket excepted closed definetely", exc_info=True)
             self.connection_dead = False
             raise e
 
         except asyncio.CancelledError as e:
             logger.info("Websocket got cancelled. Trying to shutdown graceully")
             if send_task and receive_task:
                 send_task.cancel()
                 receive_task.cancel()
 
-            cancellation = await asyncio.gather(
-                send_task, receive_task, return_exceptions=True
-            )
+            await asyncio.gather(send_task, receive_task, return_exceptions=True)
             raise e
 
     async def sending(self, client):
         try:
             while True:
                 message = await self._send_queue.get()
                 await client.send(message)
                 self._send_queue.task_done()
-        except asyncio.CancelledError as e:
+        except asyncio.CancelledError:
             logger.info("Sending Task sucessfully Cancelled")
 
     async def receiving(self, client):
         try:
             async for message in client:
-                logger.info(f"Receiving message {message}")
                 await self.receive(message)
-        except asyncio.CancelledError as e:
+        except asyncio.CancelledError:
             logger.info("Receiving Task sucessfully Cancelled")
 
     async def receive(self, message):
         json_dict = json.loads(message)
         if "type" in json_dict:
             type = json_dict["type"]
             id = json_dict["id"]
+            logger.debug(str(json_dict))
 
             # State Layer
-            if type == AgentSubMessageTypes.ASSIGN:
-                await self._abroadcast(AssignSubMessage(**json_dict))
+            if type == PostmanSubMessageTypes.ASSIGN_UPDATE:
+                await self._abroadcast(AssignSubUpdate(**json_dict))
 
-            if type == AgentSubMessageTypes.UNASSIGN:
-                await self._abroadcast(UnassignSubMessage(**json_dict))
+            if type == PostmanSubMessageTypes.RESERVE_UPDATE:
+                await self._abroadcast(ReserveSubUpdate(**json_dict))
 
-            if type == AgentSubMessageTypes.UNPROVIDE:
-                logger.error("RECEIVED UNPROIVDE")
-                await self._abroadcast(UnprovideSubMessage(**json_dict))
-
-            if type == AgentSubMessageTypes.PROVIDE:
-                logger.error(
-                    "OINSADOFNSÜAOEDIFNÜASIENFAPOINFPAOWINFPOWINFOIWANFPOIWNFPOIWN"
+            if type == PostmanMessageTypes.LIST_ASSIGNATION_REPLY:
+                self._futures[id].set_result(AssingListReply(**json_dict))
+            if type == PostmanMessageTypes.LIST_ASSIGNATION_DENIED:
+                self._futures[id].set_exception(
+                    AssignationListDeniedError(json_dict["error"])
                 )
-                await self._abroadcast(ProvideSubMessage(**json_dict))
 
-            if type == AgentMessageTypes.LIST_ASSIGNATIONS_REPLY:
-                self._futures[id].set_result(AssignationsListReply(**json_dict))
-            if type == AgentMessageTypes.LIST_ASSIGNATIONS_DENIED:
+            if type == PostmanMessageTypes.LIST_RESERVATION_REPLY:
+                self._futures[id].set_result(ReserveListReply(**json_dict))
+            if type == PostmanMessageTypes.LIST_RESERVATION_DENIED:
                 self._futures[id].set_exception(
-                    AssignationListDeniedError(json_dict["error"])
+                    ReservationListDeniedError(json_dict["error"])
                 )
 
-            if type == AgentMessageTypes.LIST_PROVISIONS_REPLY:
-                self._futures[id].set_result(ProvisionListReply(**json_dict))
-            if type == AgentMessageTypes.LIST_PROVISIONS_DENIED:
+            if type == PostmanMessageTypes.ASSIGN_REPLY:
+                self._futures[id].set_result(AssignPubReply(**json_dict))
+            if type == PostmanMessageTypes.ASSIGN_DENIED:
+                self._futures[id].set_exception(AssignDeniedError(json_dict["error"]))
+
+            if type == PostmanMessageTypes.UNASSIGN_REPLY:
+                self._futures[id].set_result(UnassignPubReply(**json_dict))
+            if type == PostmanMessageTypes.UNASSIGN_DENIED:
+                self._futures[id].set_exception(UnassignDeniedError(json_dict["error"]))
+
+            if type == PostmanMessageTypes.RESERVE_REPLY:
+                self._futures[id].set_result(UnreservePubReply(**json_dict))
+            if type == PostmanMessageTypes.RESERVE_DENIED:
+                self._futures[id].set_exception(ReserveDeniedError(json_dict["error"]))
+
+            if type == PostmanMessageTypes.UNRESERVE_REPLY:
+                self._futures[id].set_result(UnreservePubReply(**json_dict))
+            if type == PostmanMessageTypes.UNRESERVE_DENIED:
                 self._futures[id].set_exception(
-                    ProvisionListDeniedError(json_dict["error"])
+                    UnreserveDeniedError(json_dict["error"])
                 )
 
         else:
-            logger.error(f"Unexpected messsage: {json_dict}")
+            logger.error(f"Error {json_dict}")
 
     async def awaitaction(self, action: JSONMessage):
-
         if not self._connected:
             assert (
                 self.auto_connect
             ), "Websocket not connected, and autoconnect to false"
             await self.aconnect()
+
         if action.id in self._futures:
             raise ValueError("Action already has a future")
 
         future = asyncio.Future()
         self._futures[action.id] = future
         await self._send_queue.put(action.json())
         return await future
 
-    async def delayaction(self, action: JSONMessage):
-        if not self._connected:
-            assert (
-                self.auto_connect
-            ), "Websocket not connected, and autoconnect to false"
-            await self.aconnect()
-        await self._send_queue.put(action.json())
-
-    async def list_provisions(
-        self, exclude: Optional[ProvisionStatus] = None
-    ) -> List[Provision]:
-        action = ProvisionList(exclude=exclude)
-        prov_list_reply: ProvisionListReply = await self.awaitaction(action)
-        return prov_list_reply.provisions
-
-    async def change_provision(
-        self,
-        id: str,
-        status: ProvisionStatus = None,
-        message: str = None,
-        mode: ProvisionMode = None,
-    ):
-        action = ProvisionChangedMessage(
-            provision=id, status=status, message=message, mode=mode
+    async def alist_reservations(
+        self, exclude: Optional[ReservationStatus] = None
+    ) -> List[Reservation]:
+        prov_list_reply: ReserveListReply = await self.awaitaction(
+            ReserveList(exclude=exclude)
         )
-        await self.delayaction(action)
+        return prov_list_reply.reservations
 
-    async def change_assignation(
+    async def aassign(
         self,
-        id: str,
-        status: AssignationStatus = None,
-        message: str = None,
-        returns: List[Any] = None,
-        progress: int = None,
-    ):
-        action = AssignationChangedMessage(
-            assignation=id,
-            status=status,
-            message=message,
-            returns=returns,
-            progress=progress,
+        reservation: str,
+        args: List[Any],
+        kwargs: Dict[str, Any],
+        persist=True,
+        log=False,
+    ) -> Assignation:
+        ass_list_reply: AssignPubReply = await self.awaitaction(
+            AssignPub(
+                reservation=reservation,
+                args=args,
+                kwargs=kwargs,
+                persist=persist,
+                log=log,
+            )
         )
-        await self.delayaction(action)
+        return ass_list_reply
 
-    async def list_assignations(
+    async def areserve(
+        self, node: str, params: ReserveParamsInput = None, provision: str = None
+    ) -> Reservation:
+        action = ReservePub(node=node, params=params, provision=provision)
+        resrep: ReservePubReply = await self.awaitaction(action)
+        return resrep
+
+    async def aunreserve(self, reservation: str) -> Reservation:
+        action = UnreservePub(reservation=reservation)
+        unres: UnreservePubReply = await self.awaitaction(action)
+        return unres
+
+    async def aunassign(self, assignation: str) -> Reservation:
+        action = UnassignPub(assignation=assignation)
+        unass: UnassignPubReply = await self.awaitaction(action)
+        return unass
+
+    async def alist_assignations(
         self, exclude: Optional[AssignationStatus] = None
     ) -> List[Assignation]:
-        action = AssignationsList(exclude=exclude)
-        ass_list_reply: AssignationsListReply = await self.awaitaction(action)
+        action = AssignList(exclude=exclude)
+        ass_list_reply: AssingListReply = await self.awaitaction(action)
         return ass_list_reply.assignations
 
-    async def log_to_assignation(
-        self, id: str, level: LogLevelInput = None, message: str = None
-    ):
-        action = AssignationLogMessage(assignation=id, level=level, message=message)
-        await self.delayaction(action)
-
-    async def log_to_provision(
-        self, id: str, level: LogLevelInput = None, message: str = None
-    ):
-        action = ProvisionLogMessage(provision=id, level=level, message=message)
-        await self.delayaction(action)
-
     async def adisconnect(self):
         self._connection_task.cancel()
-        self._connected = False
 
         try:
             await self._connection_task
         except asyncio.CancelledError:
             pass
 
-        self._connection_task = None
-
     async def __aexit__(self, *args, **kwargs):
         if self._connection_task:
             await self.adisconnect()
+
+    class Config:
+        arbitrary_types_allowed = True
+        underscore_attrs_are_private = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rekuest-0.1.9/rekuest/api/schema.py` & `rekuest-0.2.0/rekuest/api/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,102 @@
 from typing_extensions import Literal
-from typing import AsyncIterator, Optional, List, Tuple, Union, Any, Iterator, Dict
+from typing import Tuple, Any, Optional, Iterator, Dict, List, AsyncIterator, Union
+from datetime import datetime
 from rekuest.traits.ports import (
-    ReturnWidgetInputTrait,
-    PortTrait,
     AnnotationInputTrait,
+    PortTrait,
+    ReturnWidgetInputTrait,
     WidgetInputTrait,
 )
 from rath.scalars import ID
-from rekuest.rath import RekuestRath
-from rekuest.scalars import Identifier, SearchQuery
+from rekuest.funcs import subscribe, aexecute, execute, asubscribe
 from rekuest.traits.node import Reserve
-from pydantic import BaseModel, Field
-from rekuest.funcs import asubscribe, aexecute, subscribe, execute
 from enum import Enum
-from datetime import datetime
-
+from rekuest.rath import RekuestRath
+from rekuest.scalars import SearchQuery, Identifier
+from pydantic import BaseModel, Field
 
-class AgentStatus(str, Enum):
-    """An enumeration."""
 
-    ACTIVE = "ACTIVE"
-    "Active"
-    DISCONNECTED = "DISCONNECTED"
-    "Disconnected"
-    VANILLA = "VANILLA"
-    "Complete Vanilla Scenario after a forced restart of"
+class CommentableModels(str, Enum):
+    FACADE_REPOSITORY = "FACADE_REPOSITORY"
+    FACADE_REGISTRY = "FACADE_REGISTRY"
+    FACADE_STRUCTURE = "FACADE_STRUCTURE"
+    FACADE_MIRRORREPOSITORY = "FACADE_MIRRORREPOSITORY"
+    FACADE_APPREPOSITORY = "FACADE_APPREPOSITORY"
+    FACADE_AGENT = "FACADE_AGENT"
+    FACADE_COLLECTION = "FACADE_COLLECTION"
+    FACADE_WAITER = "FACADE_WAITER"
+    FACADE_NODE = "FACADE_NODE"
+    FACADE_TEMPLATE = "FACADE_TEMPLATE"
+    FACADE_PROVISIONLOG = "FACADE_PROVISIONLOG"
+    FACADE_PROVISION = "FACADE_PROVISION"
+    FACADE_RESERVATIONLOG = "FACADE_RESERVATIONLOG"
+    FACADE_RESERVATION = "FACADE_RESERVATION"
+    FACADE_ASSIGNATION = "FACADE_ASSIGNATION"
+    FACADE_ASSIGNATIONLOG = "FACADE_ASSIGNATIONLOG"
+    FACADE_TESTCASE = "FACADE_TESTCASE"
+    FACADE_TESTRESULT = "FACADE_TESTRESULT"
 
 
 class NodeKind(str, Enum):
     """An enumeration."""
 
     GENERATOR = "GENERATOR"
     "Generator"
     FUNCTION = "FUNCTION"
     "Function"
 
 
+class NodeScope(str, Enum):
+    GLOBAL = "GLOBAL"
+    LOCAL = "LOCAL"
+    BRIDGE_GLOBAL_TO_LOCAL = "BRIDGE_GLOBAL_TO_LOCAL"
+    BRIDGE_LOCAL_TO_GLOBAL = "BRIDGE_LOCAL_TO_GLOBAL"
+
+
 class PortKind(str, Enum):
     INT = "INT"
     STRING = "STRING"
     STRUCTURE = "STRUCTURE"
     LIST = "LIST"
     BOOL = "BOOL"
     DICT = "DICT"
     FLOAT = "FLOAT"
+    UNION = "UNION"
+
+
+class LogicalCondition(str, Enum):
+    IS = "IS"
+    IS_NOT = "IS_NOT"
+    IN = "IN"
+
+
+class EffectKind(str, Enum):
+    HIDDEN = "HIDDEN"
+    HIGHLIGHT = "HIGHLIGHT"
+    WARN = "WARN"
+    CRAZY = "CRAZY"
+
+
+class Scope(str, Enum):
+    GLOBAL = "GLOBAL"
+    LOCAL = "LOCAL"
+
+
+class AgentStatus(str, Enum):
+    """An enumeration."""
+
+    ACTIVE = "ACTIVE"
+    "Active"
+    KICKED = "KICKED"
+    "Just kicked"
+    DISCONNECTED = "DISCONNECTED"
+    "Disconnected"
+    VANILLA = "VANILLA"
+    "Complete Vanilla Scenario after a forced restart of"
 
 
 class ProvisionMode(str, Enum):
     """An enumeration."""
 
     DEBUG = "DEBUG"
     "Debug Mode (Node might be constantly evolving)"
@@ -339,19 +388,36 @@
 
     APP = "APP"
     "Repository that is hosted by an App"
     MIRROR = "MIRROR"
     "Repository mirrors online Repository"
 
 
+class LokClientGrantType(str, Enum):
+    """An enumeration."""
+
+    CLIENT_CREDENTIALS = "CLIENT_CREDENTIALS"
+    "Backend (Client Credentials)"
+    IMPLICIT = "IMPLICIT"
+    "Implicit Grant"
+    AUTHORIZATION_CODE = "AUTHORIZATION_CODE"
+    "Authorization Code"
+    PASSWORD = "PASSWORD"
+    "Password"
+    SESSION = "SESSION"
+    "Django Session"
+
+
 class AgentStatusInput(str, Enum):
     """An enumeration."""
 
     ACTIVE = "ACTIVE"
     "Active"
+    KICKED = "KICKED"
+    "Just kicked"
     DISCONNECTED = "DISCONNECTED"
     "Disconnected"
     VANILLA = "VANILLA"
     "Complete Vanilla Scenario after a forced restart of"
 
 
 class NodeKindInput(str, Enum):
@@ -390,43 +456,49 @@
     "Ended (Reservation was ended by the the Platform and is no longer active)"
     CANCELLED = "CANCELLED"
     "Cancelled (Reservation was cancelled by user and is no longer active)"
     CRITICAL = "CRITICAL"
     "Critical (Reservation failed with an Critical Error)"
 
 
-class AvailableModels(str, Enum):
+class SharableModels(str, Enum):
+    """Sharable Models are models that can be shared amongst users and groups. They representent the models of the DB"""
+
     LOK_LOKUSER = "LOK_LOKUSER"
     LOK_LOKAPP = "LOK_LOKAPP"
     LOK_LOKCLIENT = "LOK_LOKCLIENT"
     FACADE_REPOSITORY = "FACADE_REPOSITORY"
     FACADE_REGISTRY = "FACADE_REGISTRY"
     FACADE_STRUCTURE = "FACADE_STRUCTURE"
     FACADE_MIRRORREPOSITORY = "FACADE_MIRRORREPOSITORY"
     FACADE_APPREPOSITORY = "FACADE_APPREPOSITORY"
     FACADE_AGENT = "FACADE_AGENT"
+    FACADE_COLLECTION = "FACADE_COLLECTION"
     FACADE_WAITER = "FACADE_WAITER"
     FACADE_NODE = "FACADE_NODE"
     FACADE_TEMPLATE = "FACADE_TEMPLATE"
     FACADE_PROVISIONLOG = "FACADE_PROVISIONLOG"
     FACADE_PROVISION = "FACADE_PROVISION"
     FACADE_RESERVATIONLOG = "FACADE_RESERVATIONLOG"
     FACADE_RESERVATION = "FACADE_RESERVATION"
     FACADE_ASSIGNATION = "FACADE_ASSIGNATION"
     FACADE_ASSIGNATIONLOG = "FACADE_ASSIGNATIONLOG"
+    FACADE_TESTCASE = "FACADE_TESTCASE"
+    FACADE_TESTRESULT = "FACADE_TESTRESULT"
 
 
 class PortKindInput(str, Enum):
     INT = "INT"
     STRING = "STRING"
     STRUCTURE = "STRUCTURE"
     LIST = "LIST"
     BOOL = "BOOL"
     DICT = "DICT"
     FLOAT = "FLOAT"
+    UNION = "UNION"
 
 
 class AnnotationKind(str, Enum):
     """The kind of annotation"""
 
     ValueRange = "ValueRange"
     CustomAnnotation = "CustomAnnotation"
@@ -448,100 +520,185 @@
     StringWidget = "StringWidget"
     SearchWidget = "SearchWidget"
     SliderWidget = "SliderWidget"
     LinkWidget = "LinkWidget"
     BoolWidget = "BoolWidget"
     ChoiceWidget = "ChoiceWidget"
     CustomWidget = "CustomWidget"
+    TemplateWidget = "TemplateWidget"
 
 
 class ReturnWidgetKind(str, Enum):
     """The kind of return widget"""
 
     ImageReturnWidget = "ImageReturnWidget"
     CustomReturnWidget = "CustomReturnWidget"
+    ChoiceReturnWidget = "ChoiceReturnWidget"
 
 
 class MessageKind(str, Enum):
     TERMINATE = "TERMINATE"
     CANCEL = "CANCEL"
     ASSIGN = "ASSIGN"
     TELL = "TELL"
 
 
+class DescendendInput(BaseModel):
+    children: Optional[Tuple[Optional["DescendendInput"], ...]]
+    typename: Optional[str]
+    "The type of the descendent"
+    user: Optional[str]
+    "The user that is mentioned"
+    bold: Optional[bool]
+    "Is this a bold leaf?"
+    italic: Optional[bool]
+    "Is this a italic leaf?"
+    code: Optional[bool]
+    "Is this a code leaf?"
+    text: Optional[str]
+    "The text of the leaf"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
 class DefinitionInput(BaseModel):
     """A definition for a template"""
 
     description: Optional[str]
     "A description for the Node"
+    collections: Optional[Tuple[Optional[ID], ...]]
     name: str
     "The name of this template"
-    args: Optional[Tuple[Optional["ArgPortInput"], ...]]
+    port_groups: Tuple[Optional["PortGroupInput"], ...] = Field(alias="portGroups")
+    args: Tuple[Optional["PortInput"], ...]
     "The Args"
-    returns: Optional[Tuple[Optional["ReturnPortInput"], ...]]
+    returns: Tuple[Optional["PortInput"], ...]
     "The Returns"
-    interface: Optional[str]
-    "The interface of this template"
-    interfaces: Optional[Tuple[Optional[str], ...]]
+    interfaces: Tuple[Optional[str], ...]
     "The Interfaces this node provides makes sense of the metadata"
     kind: NodeKindInput
     "The variety"
+    is_test_for: Optional[Tuple[Optional[str], ...]] = Field(alias="isTestFor")
+    "The nodes this is a test for"
     pure: Optional[bool]
     idempotent: Optional[bool]
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
+class PortGroupInput(BaseModel):
+    key: str
+    "The key of the port group"
+    hidden: Optional[bool]
+    "Is this port group hidden"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
-class ArgPortInput(PortTrait, BaseModel):
+class PortInput(PortTrait, BaseModel):
+    effects: Optional[Tuple[Optional["EffectInput"], ...]]
+    "The dependencies of this port"
     identifier: Optional[Identifier]
     "The identifier"
     key: str
     "The key of the arg"
+    scope: Scope
+    "The scope of this port"
+    variants: Optional[Tuple[Optional["ChildPortInput"], ...]]
+    "The varients of this port (only for union)"
     name: Optional[str]
     "The name of this argument"
     label: Optional[str]
     "The name of this argument"
     kind: PortKindInput
     "The type of this argument"
     description: Optional[str]
     "The description of this argument"
     child: Optional["ChildPortInput"]
     "The child of this argument"
-    widget: Optional["WidgetInput"]
+    assign_widget: Optional["WidgetInput"] = Field(alias="assignWidget")
+    "The child of this argument"
+    return_widget: Optional["ReturnWidgetInput"] = Field(alias="returnWidget")
     "The child of this argument"
     default: Optional[Any]
     "The key of the arg"
     nullable: bool
     "Is this argument nullable"
     annotations: Optional[Tuple[Optional["AnnotationInput"], ...]]
     "The annotations of this argument"
+    groups: Optional[Tuple[Optional[str], ...]]
+    "The port group of this argument"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
+class EffectInput(BaseModel):
+    dependencies: Optional[Tuple[Optional["DependencyInput"], ...]]
+    "The dependencies of this effect"
+    kind: EffectKind
+    "The condition of the dependency"
+    message: Optional[str]
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
+class DependencyInput(BaseModel):
+    key: Optional[str]
+    "The key of the port, defaults to self"
+    condition: LogicalCondition
+    "The condition of the dependency"
+    value: Any
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class ChildPortInput(PortTrait, BaseModel):
     identifier: Optional[Identifier]
     "The identifier"
+    scope: Scope
+    "The scope of this port"
     name: Optional[str]
     "The name of this port"
     kind: Optional[PortKindInput]
     "The type of this port"
-    description: Optional[str]
-    "The description of this port"
     child: Optional["ChildPortInput"]
     "The child port"
     nullable: bool
     "Is this argument nullable"
     annotations: Optional[Tuple[Optional["AnnotationInput"], ...]]
     "The annotations of this argument"
+    variants: Optional[Tuple[Optional["ChildPortInput"], ...]]
+    "The varients of this port (only for union)"
+    assign_widget: Optional["WidgetInput"] = Field(alias="assignWidget")
+    "The child of this argument"
+    return_widget: Optional["ReturnWidgetInput"] = Field(alias="returnWidget")
+    "The child of this argument"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class AnnotationInput(AnnotationInputTrait, BaseModel):
     kind: AnnotationKind
     "The kind of annotation"
     name: Optional[str]
     "The name of this annotation"
@@ -558,88 +715,100 @@
     attribute: Optional[str]
     "The attribute to check"
     annotations: Optional[Tuple[Optional["AnnotationInput"], ...]]
     "The annotation of this annotation"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class WidgetInput(WidgetInputTrait, BaseModel):
     kind: WidgetKind
     "type"
     query: Optional[SearchQuery]
     "Do we have a possible"
-    dependencies: Optional[Tuple[Optional[str], ...]]
-    "The dependencies of this port"
     choices: Optional[Tuple[Optional["ChoiceInput"], ...]]
     "The dependencies of this port"
     max: Optional[int]
     "Max value for int widget"
     min: Optional[int]
     "Max value for int widget"
     placeholder: Optional[str]
     "Placeholder for any widget"
     as_paragraph: Optional[bool] = Field(alias="asParagraph")
     "Is this a paragraph"
     hook: Optional[str]
     "A hook for the app to call"
     ward: Optional[str]
     "A ward for the app to call"
+    fields: Optional[Tuple[Optional["TemplateFieldInput"], ...]]
+    "The fields of this widget (onbly on TemplateWidget)"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class ChoiceInput(BaseModel):
     value: Any
     label: str
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
-class ReturnPortInput(PortTrait, BaseModel):
-    identifier: Optional[Identifier]
-    "The identifier"
+class TemplateFieldInput(BaseModel):
+    parent: Optional[str]
+    "The parent key (if nested)"
     key: str
-    "The key of the arg"
-    name: Optional[str]
-    "The name of this argument"
-    label: Optional[str]
-    "The name of this argument"
-    kind: PortKindInput
-    "The type of this argument"
+    "The key of the field"
+    type: str
+    "The key of the field"
     description: Optional[str]
-    "The description of this argument"
-    child: Optional[ChildPortInput]
-    "The child of this argument"
-    widget: Optional["ReturnWidgetInput"]
-    "The child of this argument"
-    nullable: bool
-    "Is this argument nullable"
-    annotations: Optional[Tuple[Optional[AnnotationInput], ...]]
-    "The annotations of this argument"
+    "A short description of the field"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class ReturnWidgetInput(ReturnWidgetInputTrait, BaseModel):
     kind: ReturnWidgetKind
     "type"
+    choices: Optional[Tuple[Optional[ChoiceInput], ...]]
+    "The dependencies of this port"
     query: Optional[str]
     "Do we have a possible"
     hook: Optional[str]
     "A hook for the app to call"
     ward: Optional[str]
     "A hook for the app to call"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
+
+
+class ReserveBindsInput(BaseModel):
+    templates: Tuple[Optional[ID], ...]
+    "The templates that we are allowed to use"
+    clients: Tuple[Optional[ID], ...]
+    "The clients that we are allowed to use"
+
+    class Config:
+        frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class ReserveParamsInput(BaseModel):
     auto_provide: Optional[bool] = Field(alias="autoProvide")
     "Do you want to autoprovide"
     auto_unprovide: Optional[bool] = Field(alias="autoUnprovide")
     "Do you want to auto_unprovide"
@@ -652,151 +821,246 @@
     desired_instances: int = Field(alias="desiredInstances")
     "The desired amount of Instances"
     minimal_instances: int = Field(alias="minimalInstances")
     "The minimal amount of Instances"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class MessageInput(BaseModel):
     kind: MessageKind
     text: str
     reference: str
     data: Any
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class GroupAssignmentInput(BaseModel):
     permissions: Tuple[Optional[str], ...]
     group: ID
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class UserAssignmentInput(BaseModel):
     permissions: Tuple[Optional[str], ...]
     user: str
-    "The user email"
+    "The user id"
 
     class Config:
         frozen = True
+        extra = "forbid"
+        use_enum_values = True
 
 
 class ProvisionFragmentTemplate(BaseModel):
-    typename: Optional[Literal["Template"]] = Field(alias="__typename")
+    typename: Optional[Literal["Template"]] = Field(alias="__typename", exclude=True)
     id: ID
     node: "NodeFragment"
     "The node this template is implementatig"
     params: Optional[Dict]
 
     class Config:
         frozen = True
 
 
 class ProvisionFragment(BaseModel):
-    typename: Optional[Literal["Provision"]] = Field(alias="__typename")
+    typename: Optional[Literal["Provision"]] = Field(alias="__typename", exclude=True)
     id: ID
     status: ProvisionStatus
     "Current lifecycle of Provision"
     template: ProvisionFragmentTemplate
 
     class Config:
         frozen = True
 
 
+class TestCaseFragmentNode(Reserve, BaseModel):
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class TestCaseFragment(BaseModel):
+    typename: Optional[Literal["TestCase"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    node: TestCaseFragmentNode
+    "The node this test belongs to"
+    key: Optional[str]
+    is_benchmark: bool = Field(alias="isBenchmark")
+    description: Optional[str]
+    name: Optional[str]
+
+    class Config:
+        frozen = True
+
+
+class TestResultFragmentCase(BaseModel):
+    typename: Optional[Literal["TestCase"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    key: Optional[str]
+
+    class Config:
+        frozen = True
+
+
+class TestResultFragment(BaseModel):
+    typename: Optional[Literal["TestResult"]] = Field(alias="__typename", exclude=True)
+    id: ID
+    case: TestResultFragmentCase
+    passed: bool
+
+    class Config:
+        frozen = True
+
+
+class AgentFragmentRegistryClient(BaseModel):
+    typename: Optional[Literal["LokClient"]] = Field(alias="__typename", exclude=True)
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class AgentFragmentRegistryUser(BaseModel):
+    """A reflection on the real User"""
+
+    typename: Optional[Literal["User"]] = Field(alias="__typename", exclude=True)
+    id: ID
+
+    class Config:
+        frozen = True
+
+
+class AgentFragmentRegistry(BaseModel):
+    typename: Optional[Literal["Registry"]] = Field(alias="__typename", exclude=True)
+    client: AgentFragmentRegistryClient
+    user: Optional[AgentFragmentRegistryUser]
+    "The Associatsed App"
+
+    class Config:
+        frozen = True
+
+
+class AgentFragment(BaseModel):
+    typename: Optional[Literal["Agent"]] = Field(alias="__typename", exclude=True)
+    registry: Optional[AgentFragmentRegistry]
+    "The provide might be limited to a instance like ImageJ belonging to a specific person. Is nullable for backend users"
+
+    class Config:
+        frozen = True
+
+
 class AssignationFragmentParent(BaseModel):
-    typename: Optional[Literal["Assignation"]] = Field(alias="__typename")
+    typename: Optional[Literal["Assignation"]] = Field(alias="__typename", exclude=True)
     id: ID
 
     class Config:
         frozen = True
 
 
 class AssignationFragment(BaseModel):
-    typename: Optional[Literal["Assignation"]] = Field(alias="__typename")
+    typename: Optional[Literal["Assignation"]] = Field(alias="__typename", exclude=True)
     args: Optional[Tuple[Optional[Any], ...]]
     kwargs: Optional[Dict]
     id: ID
     parent: Optional[AssignationFragmentParent]
     "The Assignations parent"
     id: ID
     status: AssignationStatus
     "Current lifecycle of Assignation"
     statusmessage: str
     "Clear Text status of the Assignation as for now"
     returns: Optional[Tuple[Optional[Any], ...]]
     reference: str
-    "The Unique identifier of this Assignation"
+    "The Unique identifier of this Assignation considering its parent"
     updated_at: datetime = Field(alias="updatedAt")
 
     class Config:
         frozen = True
 
 
-class TemplateFragmentRegistryApp(BaseModel):
-    typename: Optional[Literal["LokApp"]] = Field(alias="__typename")
+class TemplateFragmentAgentRegistryApp(BaseModel):
+    typename: Optional[Literal["LokApp"]] = Field(alias="__typename", exclude=True)
     version: str
     identifier: str
 
     class Config:
         frozen = True
 
 
-class TemplateFragmentRegistryUser(BaseModel):
+class TemplateFragmentAgentRegistryUser(BaseModel):
     """A reflection on the real User"""
 
-    typename: Optional[Literal["User"]] = Field(alias="__typename")
+    typename: Optional[Literal["User"]] = Field(alias="__typename", exclude=True)
     username: str
     "Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only."
 
     class Config:
         frozen = True
 
 
-class TemplateFragmentRegistry(BaseModel):
-    typename: Optional[Literal["Registry"]] = Field(alias="__typename")
+class TemplateFragmentAgentRegistry(BaseModel):
+    typename: Optional[Literal["Registry"]] = Field(alias="__typename", exclude=True)
     name: Optional[str]
     "DEPRECATED Will be replaced in the future: : None "
-    app: Optional[TemplateFragmentRegistryApp]
-    "The Associated App"
-    user: Optional[TemplateFragmentRegistryUser]
+    app: Optional[TemplateFragmentAgentRegistryApp]
     "The Associated App"
+    user: Optional[TemplateFragmentAgentRegistryUser]
+    "The Associatsed App"
+
+    class Config:
+        frozen = True
+
+
+class TemplateFragmentAgent(BaseModel):
+    typename: Optional[Literal["Agent"]] = Field(alias="__typename", exclude=True)
+    registry: Optional[TemplateFragmentAgentRegistry]
+    "The provide might be limited to a instance like ImageJ belonging to a specific person. Is nullable for backend users"
 
     class Config:
         frozen = True
 
 
 class TemplateFragment(BaseModel):
-    typename: Optional[Literal["Template"]] = Field(alias="__typename")
+    typename: Optional[Literal["Template"]] = Field(alias="__typename", exclude=True)
     id: ID
-    registry: TemplateFragmentRegistry
+    agent: TemplateFragmentAgent
     "The associated registry for this Template"
     node: "NodeFragment"
     "The node this template is implementatig"
     params: Optional[Dict]
 
     class Config:
         frozen = True
 
 
 class IsPredicateFragment(BaseModel):
-    typename: Optional[Literal["IsPredicate"]] = Field(alias="__typename")
+    typename: Optional[Literal["IsPredicate"]] = Field(alias="__typename", exclude=True)
     predicate: IsPredicateType
     "The arguments for this annotation"
 
     class Config:
         frozen = True
 
 
 class ValueRangeFragment(BaseModel):
-    typename: Optional[Literal["ValueRange"]] = Field(alias="__typename")
+    typename: Optional[Literal["ValueRange"]] = Field(alias="__typename", exclude=True)
     min: float
     "The minimum value"
     max: float
     "The maximum value"
 
     class Config:
         frozen = True
@@ -819,148 +1083,146 @@
     AnnotationFragmentBaseIsPredicate,
     AnnotationFragmentBaseValueRange,
     AnnotationFragmentBase,
 ]
 
 
 class ChildPortNestedFragmentChild(PortTrait, BaseModel):
-    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename")
-    kind: Optional[PortKind]
+    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename", exclude=True)
+    identifier: Optional[Identifier]
+    "The corresponding Model"
+    nullable: bool
+    "Is this argument nullable"
+    kind: PortKind
     "the type of input"
 
     class Config:
         frozen = True
 
 
 class ChildPortNestedFragment(PortTrait, BaseModel):
-    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename")
-    kind: Optional[PortKind]
+    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename", exclude=True)
+    kind: PortKind
     "the type of input"
     child: Optional[ChildPortNestedFragmentChild]
     "The child"
+    identifier: Optional[Identifier]
+    "The corresponding Model"
+    nullable: bool
+    "Is this argument nullable"
     annotations: Optional[Tuple[Optional[AnnotationFragment], ...]]
     "The annotations of this port"
 
     class Config:
         frozen = True
 
 
 class ChildPortFragment(PortTrait, BaseModel):
-    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename")
-    kind: Optional[PortKind]
+    typename: Optional[Literal["ChildPort"]] = Field(alias="__typename", exclude=True)
+    kind: PortKind
     "the type of input"
     identifier: Optional[Identifier]
     "The corresponding Model"
     child: Optional[ChildPortNestedFragment]
     "The child"
+    nullable: bool
+    "Is this argument nullable"
     annotations: Optional[Tuple[Optional[AnnotationFragment], ...]]
     "The annotations of this port"
 
     class Config:
         frozen = True
 
 
-class ArgPortFragment(PortTrait, BaseModel):
-    typename: Optional[Literal["ArgPort"]] = Field(alias="__typename")
+class PortFragment(PortTrait, BaseModel):
+    typename: Optional[Literal["Port"]] = Field(alias="__typename", exclude=True)
     key: str
     label: Optional[str]
     nullable: bool
     description: Optional[str]
     "A description for this Port"
     default: Optional[Any]
     kind: PortKind
     "the type of input"
     identifier: Optional[Identifier]
     "The corresponding Model"
     child: Optional[ChildPortFragment]
     "The child"
-    annotations: Optional[Tuple[Optional[AnnotationFragment], ...]]
-    "The annotations of this port"
-
-    class Config:
-        frozen = True
-
-
-class ReturnPortFragment(PortTrait, BaseModel):
-    typename: Optional[Literal["ReturnPort"]] = Field(alias="__typename")
-    label: Optional[str]
-    key: str
-    nullable: bool
-    description: Optional[str]
-    "A description for this Port"
-    identifier: Optional[Identifier]
-    "The corresponding Model"
-    kind: PortKind
-    "the type of input"
-    child: Optional[ChildPortFragment]
-    "The child"
+    variants: Optional[Tuple[Optional[ChildPortFragment], ...]]
+    "The varients of this port (only for unions)"
     annotations: Optional[Tuple[Optional[AnnotationFragment], ...]]
     "The annotations of this port"
 
     class Config:
         frozen = True
 
 
 class DefinitionFragment(Reserve, BaseModel):
-    typename: Optional[Literal["Node"]] = Field(alias="__typename")
-    args: Optional[Tuple[Optional[ArgPortFragment], ...]]
-    returns: Optional[Tuple[Optional[ReturnPortFragment], ...]]
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
+    args: Optional[Tuple[Optional[PortFragment], ...]]
+    returns: Optional[Tuple[Optional[PortFragment], ...]]
+    kind: NodeKind
+    "Function, generator? Check async Programming Textbook"
+    name: str
+    "The cleartext name of this Node"
+    description: str
+    "A description for the Node"
 
     class Config:
         frozen = True
 
 
 class NodeFragment(DefinitionFragment, Reserve, BaseModel):
-    typename: Optional[Literal["Node"]] = Field(alias="__typename")
-    name: str
-    "The cleartext name of this Node"
-    description: str
-    "A description for the Node"
-    kind: NodeKind
-    "Function, generator? Check async Programming Textbook"
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
+    hash: str
+    "The hash of the Node (completely unique)"
     id: ID
 
     class Config:
         frozen = True
 
 
 class ReserveParamsFragment(BaseModel):
-    typename: Optional[Literal["ReserveParams"]] = Field(alias="__typename")
+    typename: Optional[Literal["ReserveParams"]] = Field(
+        alias="__typename", exclude=True
+    )
     registries: Optional[Tuple[Optional[ID], ...]]
     "Registry thar are allowed"
     minimal_instances: Optional[int] = Field(alias="minimalInstances")
     "The minimal amount of Instances"
     desired_instances: Optional[int] = Field(alias="desiredInstances")
     "The desired amount of Instances"
 
     class Config:
         frozen = True
 
 
 class ReservationFragmentNode(Reserve, BaseModel):
-    typename: Optional[Literal["Node"]] = Field(alias="__typename")
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
     id: ID
+    hash: str
+    "The hash of the Node (completely unique)"
     pure: bool
     "Is this function pure. e.g can we cache the result?"
 
     class Config:
         frozen = True
 
 
 class ReservationFragmentWaiter(BaseModel):
-    typename: Optional[Literal["Waiter"]] = Field(alias="__typename")
+    typename: Optional[Literal["Waiter"]] = Field(alias="__typename", exclude=True)
     unique: str
     "The Channel we are listening to"
 
     class Config:
         frozen = True
 
 
 class ReservationFragment(BaseModel):
-    typename: Optional[Literal["Reservation"]] = Field(alias="__typename")
+    typename: Optional[Literal["Reservation"]] = Field(alias="__typename", exclude=True)
     id: ID
     statusmessage: str
     "Clear Text status of the Provision as for now"
     status: ReservationStatus
     "Current lifecycle of Reservation"
     node: ReservationFragmentNode
     "The node this reservation connects"
@@ -971,22 +1233,51 @@
     "The Unique identifier of this Assignation"
     updated_at: datetime = Field(alias="updatedAt")
 
     class Config:
         frozen = True
 
 
+class Create_testcaseMutation(BaseModel):
+    create_test_case: Optional[TestCaseFragment] = Field(alias="createTestCase")
+    "Create Repostiory"
+
+    class Arguments(BaseModel):
+        node: ID
+        key: str
+        is_benchmark: Optional[bool]
+        description: str
+        name: str
+
+    class Meta:
+        document = "fragment TestCase on TestCase {\n  id\n  node {\n    id\n  }\n  key\n  isBenchmark\n  description\n  name\n}\n\nmutation create_testcase($node: ID!, $key: String!, $is_benchmark: Boolean, $description: String!, $name: String!) {\n  createTestCase(\n    node: $node\n    key: $key\n    isBenchmark: $is_benchmark\n    description: $description\n    name: $name\n  ) {\n    ...TestCase\n  }\n}"
+
+
+class Create_testresultMutation(BaseModel):
+    create_test_result: Optional[TestResultFragment] = Field(alias="createTestResult")
+    "Create Test Result"
+
+    class Arguments(BaseModel):
+        case: ID
+        template: ID
+        passed: bool
+        result: Optional[str]
+
+    class Meta:
+        document = "fragment TestResult on TestResult {\n  id\n  case {\n    id\n    key\n  }\n  passed\n}\n\nmutation create_testresult($case: ID!, $template: ID!, $passed: Boolean!, $result: String) {\n  createTestResult(\n    case: $case\n    template: $template\n    passed: $passed\n    result: $result\n  ) {\n    ...TestResult\n  }\n}"
+
+
 class AssignMutation(BaseModel):
     assign: Optional[AssignationFragment]
 
     class Arguments(BaseModel):
         reservation: ID
         args: List[Optional[Any]]
-        reference: Optional[str] = None
-        parent: Optional[ID] = None
+        reference: Optional[str]
+        parent: Optional[ID]
 
     class Meta:
         document = "fragment Assignation on Assignation {\n  args\n  kwargs\n  id\n  parent {\n    id\n  }\n  id\n  status\n  statusmessage\n  returns\n  reference\n  updatedAt\n}\n\nmutation assign($reservation: ID!, $args: [AnyInput]!, $reference: String, $parent: ID) {\n  assign(\n    reservation: $reservation\n    args: $args\n    reference: $reference\n    parent: $parent\n  ) {\n    ...Assignation\n  }\n}"
 
 
 class UnassignMutation(BaseModel):
     unassign: Optional[AssignationFragment]
@@ -998,34 +1289,38 @@
         document = "fragment Assignation on Assignation {\n  args\n  kwargs\n  id\n  parent {\n    id\n  }\n  id\n  status\n  statusmessage\n  returns\n  reference\n  updatedAt\n}\n\nmutation unassign($assignation: ID!) {\n  unassign(assignation: $assignation) {\n    ...Assignation\n  }\n}"
 
 
 class CreateTemplateMutation(BaseModel):
     create_template: Optional[TemplateFragment] = Field(alias="createTemplate")
 
     class Arguments(BaseModel):
+        interface: str
         definition: DefinitionInput
-        params: Optional[Dict] = None
-        extensions: Optional[List[Optional[str]]] = None
+        instance_id: ID
+        params: Optional[Dict]
+        extensions: Optional[List[Optional[str]]]
 
     class Meta:
-        document = "fragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPortNested on ChildPort {\n  kind\n  child {\n    kind\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment ReturnPort on ReturnPort {\n  __typename\n  label\n  key\n  nullable\n  description\n  identifier\n  kind\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ArgPort on ArgPort {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...ArgPort\n  }\n  returns {\n    ...ReturnPort\n  }\n}\n\nfragment Node on Node {\n  name\n  description\n  kind\n  id\n  ...Definition\n}\n\nfragment Template on Template {\n  id\n  registry {\n    name\n    app {\n      version\n      identifier\n    }\n    user {\n      username\n    }\n  }\n  node {\n    ...Node\n  }\n  params\n}\n\nmutation createTemplate($definition: DefinitionInput!, $params: GenericScalar, $extensions: [String]) {\n  createTemplate(\n    definition: $definition\n    params: $params\n    extensions: $extensions\n  ) {\n    ...Template\n  }\n}"
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nfragment Template on Template {\n  id\n  agent {\n    registry {\n      name\n      app {\n        version\n        identifier\n      }\n      user {\n        username\n      }\n    }\n  }\n  node {\n    ...Node\n  }\n  params\n}\n\nmutation createTemplate($interface: String!, $definition: DefinitionInput!, $instance_id: ID!, $params: GenericScalar, $extensions: [String]) {\n  createTemplate(\n    definition: $definition\n    interface: $interface\n    params: $params\n    extensions: $extensions\n    instanceId: $instance_id\n  ) {\n    ...Template\n  }\n}"
 
 
 class SlateMutation(BaseModel):
     slate: Optional[Tuple[Optional[ID], ...]]
 
     class Arguments(BaseModel):
         identifier: str
 
     class Meta:
         document = "mutation slate($identifier: String!) {\n  slate(identifier: $identifier)\n}"
 
 
 class Reset_repositoryMutationResetrepository(BaseModel):
-    typename: Optional[Literal["ResetRepositoryReturn"]] = Field(alias="__typename")
+    typename: Optional[Literal["ResetRepositoryReturn"]] = Field(
+        alias="__typename", exclude=True
+    )
     ok: Optional[bool]
 
     class Config:
         frozen = True
 
 
 class Reset_repositoryMutation(BaseModel):
@@ -1038,15 +1333,17 @@
         pass
 
     class Meta:
         document = "mutation reset_repository {\n  resetRepository {\n    ok\n  }\n}"
 
 
 class Delete_nodeMutationDeletenode(BaseModel):
-    typename: Optional[Literal["DeleteNodeReturn"]] = Field(alias="__typename")
+    typename: Optional[Literal["DeleteNodeReturn"]] = Field(
+        alias="__typename", exclude=True
+    )
     id: Optional[str]
 
     class Config:
         frozen = True
 
 
 class Delete_nodeMutation(BaseModel):
@@ -1062,39 +1359,54 @@
         )
 
 
 class ReserveMutation(BaseModel):
     reserve: Optional[ReservationFragment]
 
     class Arguments(BaseModel):
-        node: ID
-        template: Optional[ID] = None
-        params: Optional[ReserveParamsInput] = None
-        title: Optional[str] = None
-        imitate: Optional[ID] = None
-        app_group: Optional[ID] = None
-        reference: Optional[str] = None
-        provision: Optional[ID] = None
+        node: Optional[ID]
+        hash: Optional[str]
+        params: Optional[ReserveParamsInput]
+        title: Optional[str]
+        imitate: Optional[ID]
+        app_group: Optional[ID]
+        reference: Optional[str]
+        provision: Optional[ID]
+        binds: Optional[ReserveBindsInput]
 
     class Meta:
-        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nmutation reserve($node: ID!, $template: ID, $params: ReserveParamsInput, $title: String, $imitate: ID, $appGroup: ID, $reference: String, $provision: ID) {\n  reserve(\n    node: $node\n    template: $template\n    params: $params\n    title: $title\n    imitate: $imitate\n    provision: $provision\n    appGroup: $appGroup\n    reference: $reference\n  ) {\n    ...Reservation\n  }\n}"
+        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    hash\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nmutation reserve($node: ID, $hash: String, $params: ReserveParamsInput, $title: String, $imitate: ID, $appGroup: ID, $reference: String, $provision: ID, $binds: ReserveBindsInput) {\n  reserve(\n    node: $node\n    hash: $hash\n    params: $params\n    title: $title\n    imitate: $imitate\n    provision: $provision\n    appGroup: $appGroup\n    binds: $binds\n    reference: $reference\n  ) {\n    ...Reservation\n  }\n}"
+
+
+class UnreserveMutationUnreserve(BaseModel):
+    typename: Optional[Literal["UnreserveResult"]] = Field(
+        alias="__typename", exclude=True
+    )
+    id: Optional[ID]
+
+    class Config:
+        frozen = True
 
 
 class UnreserveMutation(BaseModel):
-    unreserve: Optional[ReservationFragment]
+    unreserve: Optional[UnreserveMutationUnreserve]
 
     class Arguments(BaseModel):
         id: ID
 
     class Meta:
-        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nmutation unreserve($id: ID!) {\n  unreserve(id: $id) {\n    ...Reservation\n  }\n}"
+        document = (
+            "mutation unreserve($id: ID!) {\n  unreserve(id: $id) {\n    id\n  }\n}"
+        )
 
 
 class Watch_provisionSubscriptionProvisions(BaseModel):
-    typename: Optional[Literal["ProvisionsEvent"]] = Field(alias="__typename")
+    typename: Optional[Literal["ProvisionsEvent"]] = Field(
+        alias="__typename", exclude=True
+    )
     create: Optional[ProvisionFragment]
     delete: Optional[ID]
     update: Optional[ProvisionFragment]
 
     class Config:
         frozen = True
 
@@ -1102,19 +1414,41 @@
 class Watch_provisionSubscription(BaseModel):
     provisions: Optional[Watch_provisionSubscriptionProvisions]
 
     class Arguments(BaseModel):
         identifier: str
 
     class Meta:
-        document = "fragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPortNested on ChildPort {\n  kind\n  child {\n    kind\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment ReturnPort on ReturnPort {\n  __typename\n  label\n  key\n  nullable\n  description\n  identifier\n  kind\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ArgPort on ArgPort {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...ArgPort\n  }\n  returns {\n    ...ReturnPort\n  }\n}\n\nfragment Node on Node {\n  name\n  description\n  kind\n  id\n  ...Definition\n}\n\nfragment Provision on Provision {\n  id\n  status\n  template {\n    id\n    node {\n      ...Node\n    }\n    params\n  }\n}\n\nsubscription watch_provision($identifier: String!) {\n  provisions(identifier: $identifier) {\n    create {\n      ...Provision\n    }\n    delete\n    update {\n      ...Provision\n    }\n  }\n}"
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nfragment Provision on Provision {\n  id\n  status\n  template {\n    id\n    node {\n      ...Node\n    }\n    params\n  }\n}\n\nsubscription watch_provision($identifier: String!) {\n  provisions(identifier: $identifier) {\n    create {\n      ...Provision\n    }\n    delete\n    update {\n      ...Provision\n    }\n  }\n}"
+
+
+class Watch_myagentsSubscriptionAgentsevent(BaseModel):
+    typename: Optional[Literal["AgentEvent"]] = Field(alias="__typename", exclude=True)
+    created: Optional[AgentFragment]
+    deleted: Optional[ID]
+    updated: Optional[AgentFragment]
+
+    class Config:
+        frozen = True
+
+
+class Watch_myagentsSubscription(BaseModel):
+    agents_event: Optional[Watch_myagentsSubscriptionAgentsevent] = Field(
+        alias="agentsEvent"
+    )
+
+    class Arguments(BaseModel):
+        pass
+
+    class Meta:
+        document = "fragment Agent on Agent {\n  registry {\n    client {\n      id\n    }\n    user {\n      id\n    }\n  }\n}\n\nsubscription watch_myagents {\n  agentsEvent {\n    created {\n      ...Agent\n    }\n    deleted\n    updated {\n      ...Agent\n    }\n  }\n}"
 
 
 class Watch_todosSubscriptionTodos(BaseModel):
-    typename: Optional[Literal["TodoEvent"]] = Field(alias="__typename")
+    typename: Optional[Literal["TodoEvent"]] = Field(alias="__typename", exclude=True)
     create: Optional[AssignationFragment]
     update: Optional[AssignationFragment]
     delete: Optional[ID]
 
     class Config:
         frozen = True
 
@@ -1126,15 +1460,17 @@
         identifier: str
 
     class Meta:
         document = "fragment Assignation on Assignation {\n  args\n  kwargs\n  id\n  parent {\n    id\n  }\n  id\n  status\n  statusmessage\n  returns\n  reference\n  updatedAt\n}\n\nsubscription watch_todos($identifier: String!) {\n  todos(identifier: $identifier) {\n    create {\n      ...Assignation\n    }\n    update {\n      ...Assignation\n    }\n    delete\n  }\n}"
 
 
 class Watch_requestsSubscriptionRequests(BaseModel):
-    typename: Optional[Literal["AssignationsEvent"]] = Field(alias="__typename")
+    typename: Optional[Literal["AssignationsEvent"]] = Field(
+        alias="__typename", exclude=True
+    )
     create: Optional[AssignationFragment]
     update: Optional[AssignationFragment]
     delete: Optional[ID]
 
     class Config:
         frozen = True
 
@@ -1146,15 +1482,17 @@
         identifier: str
 
     class Meta:
         document = "fragment Assignation on Assignation {\n  args\n  kwargs\n  id\n  parent {\n    id\n  }\n  id\n  status\n  statusmessage\n  returns\n  reference\n  updatedAt\n}\n\nsubscription watch_requests($identifier: String!) {\n  requests(identifier: $identifier) {\n    create {\n      ...Assignation\n    }\n    update {\n      ...Assignation\n    }\n    delete\n  }\n}"
 
 
 class Watch_reservationsSubscriptionReservations(BaseModel):
-    typename: Optional[Literal["ReservationsEvent"]] = Field(alias="__typename")
+    typename: Optional[Literal["ReservationsEvent"]] = Field(
+        alias="__typename", exclude=True
+    )
     create: Optional[ReservationFragment]
     update: Optional[ReservationFragment]
     delete: Optional[ID]
 
     class Config:
         frozen = True
 
@@ -1162,57 +1500,117 @@
 class Watch_reservationsSubscription(BaseModel):
     reservations: Optional[Watch_reservationsSubscriptionReservations]
 
     class Arguments(BaseModel):
         identifier: str
 
     class Meta:
-        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nsubscription watch_reservations($identifier: String!) {\n  reservations(identifier: $identifier) {\n    create {\n      ...Reservation\n    }\n    update {\n      ...Reservation\n    }\n    delete\n  }\n}"
+        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    hash\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nsubscription watch_reservations($identifier: String!) {\n  reservations(identifier: $identifier) {\n    create {\n      ...Reservation\n    }\n    update {\n      ...Reservation\n    }\n    delete\n  }\n}"
 
 
 class Get_provisionQuery(BaseModel):
     provision: Optional[ProvisionFragment]
 
     class Arguments(BaseModel):
         id: ID
 
     class Meta:
-        document = "fragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPortNested on ChildPort {\n  kind\n  child {\n    kind\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment ReturnPort on ReturnPort {\n  __typename\n  label\n  key\n  nullable\n  description\n  identifier\n  kind\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ArgPort on ArgPort {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...ArgPort\n  }\n  returns {\n    ...ReturnPort\n  }\n}\n\nfragment Node on Node {\n  name\n  description\n  kind\n  id\n  ...Definition\n}\n\nfragment Provision on Provision {\n  id\n  status\n  template {\n    id\n    node {\n      ...Node\n    }\n    params\n  }\n}\n\nquery get_provision($id: ID!) {\n  provision(id: $id) {\n    ...Provision\n  }\n}"
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nfragment Provision on Provision {\n  id\n  status\n  template {\n    id\n    node {\n      ...Node\n    }\n    params\n  }\n}\n\nquery get_provision($id: ID!) {\n  provision(id: $id) {\n    ...Provision\n  }\n}"
+
+
+class Get_testcaseQuery(BaseModel):
+    testcase: Optional[TestCaseFragment]
+
+    class Arguments(BaseModel):
+        id: ID
+
+    class Meta:
+        document = "fragment TestCase on TestCase {\n  id\n  node {\n    id\n  }\n  key\n  isBenchmark\n  description\n  name\n}\n\nquery get_testcase($id: ID!) {\n  testcase(id: $id) {\n    ...TestCase\n  }\n}"
+
+
+class Get_testresultQuery(BaseModel):
+    testresult: Optional[TestResultFragment]
+
+    class Arguments(BaseModel):
+        id: ID
+
+    class Meta:
+        document = "fragment TestResult on TestResult {\n  id\n  case {\n    id\n    key\n  }\n  passed\n}\n\nquery get_testresult($id: ID!) {\n  testresult(id: $id) {\n    ...TestResult\n  }\n}"
+
+
+class Search_testcasesQueryOptions(BaseModel):
+    typename: Optional[Literal["TestCase"]] = Field(alias="__typename", exclude=True)
+    label: Optional[str]
+    value: ID
+
+    class Config:
+        frozen = True
+
+
+class Search_testcasesQuery(BaseModel):
+    options: Optional[Tuple[Optional[Search_testcasesQueryOptions], ...]]
+
+    class Arguments(BaseModel):
+        search: Optional[str]
+        values: Optional[List[Optional[ID]]]
+
+    class Meta:
+        document = "query search_testcases($search: String, $values: [ID]) {\n  options: testcases(search: $search, limit: 20, ids: $values) {\n    label: name\n    value: id\n  }\n}"
+
+
+class Search_testresultsQueryOptions(BaseModel):
+    typename: Optional[Literal["TestResult"]] = Field(alias="__typename", exclude=True)
+    label: datetime
+    value: ID
+
+    class Config:
+        frozen = True
+
+
+class Search_testresultsQuery(BaseModel):
+    options: Optional[Tuple[Optional[Search_testresultsQueryOptions], ...]]
+
+    class Arguments(BaseModel):
+        search: Optional[str]
+        values: Optional[List[Optional[ID]]]
+
+    class Meta:
+        document = "query search_testresults($search: String, $values: [ID]) {\n  options: testresults(search: $search, limit: 20, ids: $values) {\n    label: createdAt\n    value: id\n  }\n}"
 
 
 class Get_agentQueryAgentRegistry(BaseModel):
-    typename: Optional[Literal["Registry"]] = Field(alias="__typename")
+    typename: Optional[Literal["Registry"]] = Field(alias="__typename", exclude=True)
     id: ID
     name: Optional[str]
     "DEPRECATED Will be replaced in the future: : None "
 
     class Config:
         frozen = True
 
 
 class Get_agentQueryAgent(BaseModel):
-    typename: Optional[Literal["Agent"]] = Field(alias="__typename")
+    typename: Optional[Literal["Agent"]] = Field(alias="__typename", exclude=True)
     registry: Optional[Get_agentQueryAgentRegistry]
     "The provide might be limited to a instance like ImageJ belonging to a specific person. Is nullable for backend users"
     name: str
     "This providers Name"
-    identifier: str
+    instance_id: str = Field(alias="instanceId")
 
     class Config:
         frozen = True
 
 
 class Get_agentQuery(BaseModel):
     agent: Optional[Get_agentQueryAgent]
 
     class Arguments(BaseModel):
         id: ID
 
     class Meta:
-        document = "query get_agent($id: ID!) {\n  agent(id: $id) {\n    registry {\n      id\n      name\n    }\n    name\n    identifier\n  }\n}"
+        document = "query get_agent($id: ID!) {\n  agent(id: $id) {\n    registry {\n      id\n      name\n    }\n    name\n    instanceId\n  }\n}"
 
 
 class RequestsQuery(BaseModel):
     requests: Optional[Tuple[Optional[AssignationFragment], ...]]
 
     class Arguments(BaseModel):
         identifier: str
@@ -1224,96 +1622,159 @@
 class Get_templateQuery(BaseModel):
     template: Optional[TemplateFragment]
 
     class Arguments(BaseModel):
         id: ID
 
     class Meta:
-        document = "fragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPortNested on ChildPort {\n  kind\n  child {\n    kind\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment ReturnPort on ReturnPort {\n  __typename\n  label\n  key\n  nullable\n  description\n  identifier\n  kind\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ArgPort on ArgPort {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...ArgPort\n  }\n  returns {\n    ...ReturnPort\n  }\n}\n\nfragment Node on Node {\n  name\n  description\n  kind\n  id\n  ...Definition\n}\n\nfragment Template on Template {\n  id\n  registry {\n    name\n    app {\n      version\n      identifier\n    }\n    user {\n      username\n    }\n  }\n  node {\n    ...Node\n  }\n  params\n}\n\nquery get_template($id: ID!) {\n  template(id: $id) {\n    ...Template\n  }\n}"
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nfragment Template on Template {\n  id\n  agent {\n    registry {\n      name\n      app {\n        version\n        identifier\n      }\n      user {\n        username\n      }\n    }\n  }\n  node {\n    ...Node\n  }\n  params\n}\n\nquery get_template($id: ID!) {\n  template(id: $id) {\n    ...Template\n  }\n}"
+
+
+class Search_templatesQueryOptions(BaseModel):
+    typename: Optional[Literal["Template"]] = Field(alias="__typename", exclude=True)
+    label: str
+    "A name for this Template"
+    value: ID
+
+    class Config:
+        frozen = True
+
+
+class Search_templatesQuery(BaseModel):
+    options: Optional[Tuple[Optional[Search_templatesQueryOptions], ...]]
+
+    class Arguments(BaseModel):
+        search: Optional[str]
+        values: Optional[List[Optional[ID]]]
+
+    class Meta:
+        document = "query search_templates($search: String, $values: [ID]) {\n  options: templates(search: $search, limit: 20, ids: $values) {\n    label: name\n    value: id\n  }\n}"
 
 
 class FindQuery(BaseModel):
     node: Optional[NodeFragment]
     "Asss\n\n    Is A query for all of these specials in the world\n    "
 
     class Arguments(BaseModel):
-        id: Optional[ID] = None
-        template: Optional[ID] = None
-        hash: Optional[str] = None
+        id: Optional[ID]
+        template: Optional[ID]
+        hash: Optional[str]
 
     class Meta:
-        document = "fragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPortNested on ChildPort {\n  kind\n  child {\n    kind\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment ReturnPort on ReturnPort {\n  __typename\n  label\n  key\n  nullable\n  description\n  identifier\n  kind\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ArgPort on ArgPort {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...ArgPort\n  }\n  returns {\n    ...ReturnPort\n  }\n}\n\nfragment Node on Node {\n  name\n  description\n  kind\n  id\n  ...Definition\n}\n\nquery find($id: ID, $template: ID, $hash: String) {\n  node(id: $id, template: $template, hash: $hash) {\n    ...Node\n  }\n}"
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nquery find($id: ID, $template: ID, $hash: String) {\n  node(id: $id, template: $template, hash: $hash) {\n    ...Node\n  }\n}"
+
 
+class RetrieveallQuery(BaseModel):
+    allnodes: Optional[Tuple[Optional[NodeFragment], ...]]
 
-class Get_reservationQueryReservationTemplateRegistryApp(BaseModel):
-    typename: Optional[Literal["LokApp"]] = Field(alias="__typename")
+    class Arguments(BaseModel):
+        pass
+
+    class Meta:
+        document = "fragment ChildPortNested on ChildPort {\n  kind\n  child {\n    identifier\n    nullable\n    kind\n  }\n  identifier\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment ValueRange on ValueRange {\n  min\n  max\n}\n\nfragment IsPredicate on IsPredicate {\n  predicate\n}\n\nfragment ChildPort on ChildPort {\n  kind\n  identifier\n  child {\n    ...ChildPortNested\n  }\n  nullable\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Annotation on Annotation {\n  kind\n  ...IsPredicate\n  ...ValueRange\n}\n\nfragment Port on Port {\n  __typename\n  key\n  label\n  nullable\n  description\n  default\n  kind\n  identifier\n  child {\n    ...ChildPort\n  }\n  variants {\n    ...ChildPort\n  }\n  annotations {\n    ...Annotation\n  }\n}\n\nfragment Definition on Node {\n  args {\n    ...Port\n  }\n  returns {\n    ...Port\n  }\n  kind\n  name\n  description\n}\n\nfragment Node on Node {\n  hash\n  id\n  ...Definition\n}\n\nquery retrieveall {\n  allnodes {\n    ...Node\n  }\n}"
+
+
+class Search_nodesQueryOptions(Reserve, BaseModel):
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
+    label: str
+    "The cleartext name of this Node"
+    value: ID
+
+    class Config:
+        frozen = True
+
+
+class Search_nodesQuery(BaseModel):
+    options: Optional[Tuple[Optional[Search_nodesQueryOptions], ...]]
+
+    class Arguments(BaseModel):
+        search: Optional[str]
+        values: Optional[List[Optional[ID]]]
+
+    class Meta:
+        document = "query search_nodes($search: String, $values: [ID]) {\n  options: allnodes(search: $search, limit: 20, ids: $values) {\n    label: name\n    value: id\n  }\n}"
+
+
+class Get_reservationQueryReservationTemplateAgentRegistryApp(BaseModel):
+    typename: Optional[Literal["LokApp"]] = Field(alias="__typename", exclude=True)
     id: ID
     version: str
     identifier: str
 
     class Config:
         frozen = True
 
 
-class Get_reservationQueryReservationTemplateRegistryUser(BaseModel):
+class Get_reservationQueryReservationTemplateAgentRegistryUser(BaseModel):
     """A reflection on the real User"""
 
-    typename: Optional[Literal["User"]] = Field(alias="__typename")
+    typename: Optional[Literal["User"]] = Field(alias="__typename", exclude=True)
     id: ID
     email: str
 
     class Config:
         frozen = True
 
 
-class Get_reservationQueryReservationTemplateRegistry(BaseModel):
-    typename: Optional[Literal["Registry"]] = Field(alias="__typename")
-    app: Optional[Get_reservationQueryReservationTemplateRegistryApp]
-    "The Associated App"
-    user: Optional[Get_reservationQueryReservationTemplateRegistryUser]
+class Get_reservationQueryReservationTemplateAgentRegistry(BaseModel):
+    typename: Optional[Literal["Registry"]] = Field(alias="__typename", exclude=True)
+    app: Optional[Get_reservationQueryReservationTemplateAgentRegistryApp]
     "The Associated App"
+    user: Optional[Get_reservationQueryReservationTemplateAgentRegistryUser]
+    "The Associatsed App"
+
+    class Config:
+        frozen = True
+
+
+class Get_reservationQueryReservationTemplateAgent(BaseModel):
+    typename: Optional[Literal["Agent"]] = Field(alias="__typename", exclude=True)
+    instance_id: str = Field(alias="instanceId")
+    id: ID
+    registry: Optional[Get_reservationQueryReservationTemplateAgentRegistry]
+    "The provide might be limited to a instance like ImageJ belonging to a specific person. Is nullable for backend users"
 
     class Config:
         frozen = True
 
 
 class Get_reservationQueryReservationTemplate(BaseModel):
-    typename: Optional[Literal["Template"]] = Field(alias="__typename")
+    typename: Optional[Literal["Template"]] = Field(alias="__typename", exclude=True)
     id: ID
-    registry: Get_reservationQueryReservationTemplateRegistry
+    agent: Get_reservationQueryReservationTemplateAgent
     "The associated registry for this Template"
 
     class Config:
         frozen = True
 
 
 class Get_reservationQueryReservationProvisions(BaseModel):
-    typename: Optional[Literal["Provision"]] = Field(alias="__typename")
+    typename: Optional[Literal["Provision"]] = Field(alias="__typename", exclude=True)
     id: ID
     status: ProvisionStatus
     "Current lifecycle of Provision"
 
     class Config:
         frozen = True
 
 
 class Get_reservationQueryReservationNode(Reserve, BaseModel):
-    typename: Optional[Literal["Node"]] = Field(alias="__typename")
+    typename: Optional[Literal["Node"]] = Field(alias="__typename", exclude=True)
     id: ID
     kind: NodeKind
     "Function, generator? Check async Programming Textbook"
     name: str
     "The cleartext name of this Node"
 
     class Config:
         frozen = True
 
 
 class Get_reservationQueryReservation(BaseModel):
-    typename: Optional[Literal["Reservation"]] = Field(alias="__typename")
+    typename: Optional[Literal["Reservation"]] = Field(alias="__typename", exclude=True)
     id: ID
     template: Optional[Get_reservationQueryReservationTemplate]
     "The template this reservation connects"
     provisions: Tuple[Get_reservationQueryReservationProvisions, ...]
     "The Provisions this reservation connects"
     title: Optional[str]
     "A Short Hand Way to identify this reservation for you"
@@ -1332,25 +1793,153 @@
 class Get_reservationQuery(BaseModel):
     reservation: Optional[Get_reservationQueryReservation]
 
     class Arguments(BaseModel):
         id: ID
 
     class Meta:
-        document = "query get_reservation($id: ID!) {\n  reservation(id: $id) {\n    id\n    template {\n      id\n      registry {\n        app {\n          id\n          version\n          identifier\n        }\n        user {\n          id\n          email\n        }\n      }\n    }\n    provisions {\n      id\n      status\n    }\n    title\n    status\n    id\n    reference\n    node {\n      id\n      kind\n      name\n    }\n  }\n}"
+        document = "query get_reservation($id: ID!) {\n  reservation(id: $id) {\n    id\n    template {\n      id\n      agent {\n        instanceId\n        id\n        registry {\n          app {\n            id\n            version\n            identifier\n          }\n          user {\n            id\n            email\n          }\n        }\n      }\n    }\n    provisions {\n      id\n      status\n    }\n    title\n    status\n    id\n    reference\n    node {\n      id\n      kind\n      name\n    }\n  }\n}"
 
 
 class ReservationsQuery(BaseModel):
     reservations: Optional[Tuple[Optional[ReservationFragment], ...]]
 
     class Arguments(BaseModel):
         identifier: str
 
     class Meta:
-        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nquery reservations($identifier: String!) {\n  reservations(identifier: $identifier) {\n    ...Reservation\n  }\n}"
+        document = "fragment ReserveParams on ReserveParams {\n  registries\n  minimalInstances\n  desiredInstances\n}\n\nfragment Reservation on Reservation {\n  id\n  statusmessage\n  status\n  node {\n    id\n    hash\n    pure\n  }\n  params {\n    ...ReserveParams\n  }\n  waiter {\n    unique\n  }\n  reference\n  updatedAt\n}\n\nquery reservations($identifier: String!) {\n  reservations(identifier: $identifier) {\n    ...Reservation\n  }\n}"
+
+
+async def acreate_testcase(
+    node: ID,
+    key: str,
+    description: str,
+    name: str,
+    is_benchmark: Optional[bool] = None,
+    rath: RekuestRath = None,
+) -> Optional[TestCaseFragment]:
+    """create_testcase
+
+
+
+    Arguments:
+        node (ID): node
+        key (str): key
+        description (str): description
+        name (str): name
+        is_benchmark (Optional[bool], optional): is_benchmark.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestCaseFragment]"""
+    return (
+        await aexecute(
+            Create_testcaseMutation,
+            {
+                "node": node,
+                "key": key,
+                "is_benchmark": is_benchmark,
+                "description": description,
+                "name": name,
+            },
+            rath=rath,
+        )
+    ).create_test_case
+
+
+def create_testcase(
+    node: ID,
+    key: str,
+    description: str,
+    name: str,
+    is_benchmark: Optional[bool] = None,
+    rath: RekuestRath = None,
+) -> Optional[TestCaseFragment]:
+    """create_testcase
+
+
+
+    Arguments:
+        node (ID): node
+        key (str): key
+        description (str): description
+        name (str): name
+        is_benchmark (Optional[bool], optional): is_benchmark.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestCaseFragment]"""
+    return execute(
+        Create_testcaseMutation,
+        {
+            "node": node,
+            "key": key,
+            "is_benchmark": is_benchmark,
+            "description": description,
+            "name": name,
+        },
+        rath=rath,
+    ).create_test_case
+
+
+async def acreate_testresult(
+    case: ID,
+    template: ID,
+    passed: bool,
+    result: Optional[str] = None,
+    rath: RekuestRath = None,
+) -> Optional[TestResultFragment]:
+    """create_testresult
+
+
+
+    Arguments:
+        case (ID): case
+        template (ID): template
+        passed (bool): passed
+        result (Optional[str], optional): result.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestResultFragment]"""
+    return (
+        await aexecute(
+            Create_testresultMutation,
+            {"case": case, "template": template, "passed": passed, "result": result},
+            rath=rath,
+        )
+    ).create_test_result
+
+
+def create_testresult(
+    case: ID,
+    template: ID,
+    passed: bool,
+    result: Optional[str] = None,
+    rath: RekuestRath = None,
+) -> Optional[TestResultFragment]:
+    """create_testresult
+
+
+
+    Arguments:
+        case (ID): case
+        template (ID): template
+        passed (bool): passed
+        result (Optional[str], optional): result.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestResultFragment]"""
+    return execute(
+        Create_testresultMutation,
+        {"case": case, "template": template, "passed": passed, "result": result},
+        rath=rath,
+    ).create_test_result
 
 
 async def aassign(
     reservation: ID,
     args: List[Optional[Any]],
     reference: Optional[str] = None,
     parent: Optional[ID] = None,
@@ -1446,61 +2035,81 @@
 
     Returns:
         Optional[AssignationFragment]"""
     return execute(UnassignMutation, {"assignation": assignation}, rath=rath).unassign
 
 
 async def acreate_template(
+    interface: str,
     definition: DefinitionInput,
+    instance_id: ID,
     params: Optional[Dict] = None,
     extensions: Optional[List[Optional[str]]] = None,
     rath: RekuestRath = None,
 ) -> Optional[TemplateFragment]:
     """createTemplate
 
 
 
     Arguments:
+        interface (str): interface
         definition (DefinitionInput): definition
+        instance_id (ID): instance_id
         params (Optional[Dict], optional): params.
         extensions (Optional[List[Optional[str]]], optional): extensions.
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[TemplateFragment]"""
     return (
         await aexecute(
             CreateTemplateMutation,
-            {"definition": definition, "params": params, "extensions": extensions},
+            {
+                "interface": interface,
+                "definition": definition,
+                "instance_id": instance_id,
+                "params": params,
+                "extensions": extensions,
+            },
             rath=rath,
         )
     ).create_template
 
 
 def create_template(
+    interface: str,
     definition: DefinitionInput,
+    instance_id: ID,
     params: Optional[Dict] = None,
     extensions: Optional[List[Optional[str]]] = None,
     rath: RekuestRath = None,
 ) -> Optional[TemplateFragment]:
     """createTemplate
 
 
 
     Arguments:
+        interface (str): interface
         definition (DefinitionInput): definition
+        instance_id (ID): instance_id
         params (Optional[Dict], optional): params.
         extensions (Optional[List[Optional[str]]], optional): extensions.
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[TemplateFragment]"""
     return execute(
         CreateTemplateMutation,
-        {"definition": definition, "params": params, "extensions": extensions},
+        {
+            "interface": interface,
+            "definition": definition,
+            "instance_id": instance_id,
+            "params": params,
+            "extensions": extensions,
+        },
         rath=rath,
     ).create_template
 
 
 async def aslate(
     identifier: str, rath: RekuestRath = None
 ) -> Optional[List[Optional[ID]]]:
@@ -1594,128 +2203,136 @@
 
     Returns:
         Optional[Delete_nodeMutationDeletenode]"""
     return execute(Delete_nodeMutation, {"id": id}, rath=rath).delete_node
 
 
 async def areserve(
-    node: ID,
-    template: Optional[ID] = None,
+    node: Optional[ID] = None,
+    hash: Optional[str] = None,
     params: Optional[ReserveParamsInput] = None,
     title: Optional[str] = None,
     imitate: Optional[ID] = None,
     app_group: Optional[ID] = None,
     reference: Optional[str] = None,
     provision: Optional[ID] = None,
+    binds: Optional[ReserveBindsInput] = None,
     rath: RekuestRath = None,
 ) -> Optional[ReservationFragment]:
     """reserve
 
 
 
     Arguments:
-        node (ID): node
-        template (Optional[ID], optional): template.
+        node (Optional[ID], optional): node.
+        hash (Optional[str], optional): hash.
         params (Optional[ReserveParamsInput], optional): params.
         title (Optional[str], optional): title.
         imitate (Optional[ID], optional): imitate.
         app_group (Optional[ID], optional): appGroup.
         reference (Optional[str], optional): reference.
         provision (Optional[ID], optional): provision.
+        binds (Optional[ReserveBindsInput], optional): binds.
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[ReservationFragment]"""
     return (
         await aexecute(
             ReserveMutation,
             {
                 "node": node,
-                "template": template,
+                "hash": hash,
                 "params": params,
                 "title": title,
                 "imitate": imitate,
                 "appGroup": app_group,
                 "reference": reference,
                 "provision": provision,
+                "binds": binds,
             },
             rath=rath,
         )
     ).reserve
 
 
 def reserve(
-    node: ID,
-    template: Optional[ID] = None,
+    node: Optional[ID] = None,
+    hash: Optional[str] = None,
     params: Optional[ReserveParamsInput] = None,
     title: Optional[str] = None,
     imitate: Optional[ID] = None,
     app_group: Optional[ID] = None,
     reference: Optional[str] = None,
     provision: Optional[ID] = None,
+    binds: Optional[ReserveBindsInput] = None,
     rath: RekuestRath = None,
 ) -> Optional[ReservationFragment]:
     """reserve
 
 
 
     Arguments:
-        node (ID): node
-        template (Optional[ID], optional): template.
+        node (Optional[ID], optional): node.
+        hash (Optional[str], optional): hash.
         params (Optional[ReserveParamsInput], optional): params.
         title (Optional[str], optional): title.
         imitate (Optional[ID], optional): imitate.
         app_group (Optional[ID], optional): appGroup.
         reference (Optional[str], optional): reference.
         provision (Optional[ID], optional): provision.
+        binds (Optional[ReserveBindsInput], optional): binds.
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[ReservationFragment]"""
     return execute(
         ReserveMutation,
         {
             "node": node,
-            "template": template,
+            "hash": hash,
             "params": params,
             "title": title,
             "imitate": imitate,
             "appGroup": app_group,
             "reference": reference,
             "provision": provision,
+            "binds": binds,
         },
         rath=rath,
     ).reserve
 
 
-async def aunreserve(id: ID, rath: RekuestRath = None) -> Optional[ReservationFragment]:
+async def aunreserve(
+    id: ID, rath: RekuestRath = None
+) -> Optional[UnreserveMutationUnreserve]:
     """unreserve
 
 
 
     Arguments:
         id (ID): id
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
-        Optional[ReservationFragment]"""
+        Optional[UnreserveMutationUnreserve]"""
     return (await aexecute(UnreserveMutation, {"id": id}, rath=rath)).unreserve
 
 
-def unreserve(id: ID, rath: RekuestRath = None) -> Optional[ReservationFragment]:
+def unreserve(id: ID, rath: RekuestRath = None) -> Optional[UnreserveMutationUnreserve]:
     """unreserve
 
 
 
     Arguments:
         id (ID): id
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
-        Optional[ReservationFragment]"""
+        Optional[UnreserveMutationUnreserve]"""
     return execute(UnreserveMutation, {"id": id}, rath=rath).unreserve
 
 
 async def awatch_provision(
     identifier: str, rath: RekuestRath = None
 ) -> AsyncIterator[Optional[Watch_provisionSubscriptionProvisions]]:
     """watch_provision
@@ -1749,14 +2366,46 @@
         Optional[Watch_provisionSubscriptionProvisions]"""
     for event in subscribe(
         Watch_provisionSubscription, {"identifier": identifier}, rath=rath
     ):
         yield event.provisions
 
 
+async def awatch_myagents(
+    rath: RekuestRath = None,
+) -> AsyncIterator[Optional[Watch_myagentsSubscriptionAgentsevent]]:
+    """watch_myagents
+
+
+
+    Arguments:
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[Watch_myagentsSubscriptionAgentsevent]"""
+    async for event in asubscribe(Watch_myagentsSubscription, {}, rath=rath):
+        yield event.agents_event
+
+
+def watch_myagents(
+    rath: RekuestRath = None,
+) -> Iterator[Optional[Watch_myagentsSubscriptionAgentsevent]]:
+    """watch_myagents
+
+
+
+    Arguments:
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[Watch_myagentsSubscriptionAgentsevent]"""
+    for event in subscribe(Watch_myagentsSubscription, {}, rath=rath):
+        yield event.agents_event
+
+
 async def awatch_todos(
     identifier: str, rath: RekuestRath = None
 ) -> AsyncIterator[Optional[Watch_todosSubscriptionTodos]]:
     """watch_todos
 
 
 
@@ -1893,14 +2542,160 @@
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[ProvisionFragment]"""
     return execute(Get_provisionQuery, {"id": id}, rath=rath).provision
 
 
+async def aget_testcase(id: ID, rath: RekuestRath = None) -> Optional[TestCaseFragment]:
+    """get_testcase
+
+
+
+    Arguments:
+        id (ID): id
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestCaseFragment]"""
+    return (await aexecute(Get_testcaseQuery, {"id": id}, rath=rath)).testcase
+
+
+def get_testcase(id: ID, rath: RekuestRath = None) -> Optional[TestCaseFragment]:
+    """get_testcase
+
+
+
+    Arguments:
+        id (ID): id
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestCaseFragment]"""
+    return execute(Get_testcaseQuery, {"id": id}, rath=rath).testcase
+
+
+async def aget_testresult(
+    id: ID, rath: RekuestRath = None
+) -> Optional[TestResultFragment]:
+    """get_testresult
+
+
+
+    Arguments:
+        id (ID): id
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestResultFragment]"""
+    return (await aexecute(Get_testresultQuery, {"id": id}, rath=rath)).testresult
+
+
+def get_testresult(id: ID, rath: RekuestRath = None) -> Optional[TestResultFragment]:
+    """get_testresult
+
+
+
+    Arguments:
+        id (ID): id
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[TestResultFragment]"""
+    return execute(Get_testresultQuery, {"id": id}, rath=rath).testresult
+
+
+async def asearch_testcases(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_testcasesQueryOptions]]]:
+    """search_testcases
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_testcasesQueryTestcases]]]"""
+    return (
+        await aexecute(
+            Search_testcasesQuery, {"search": search, "values": values}, rath=rath
+        )
+    ).testcases
+
+
+def search_testcases(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_testcasesQueryOptions]]]:
+    """search_testcases
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_testcasesQueryTestcases]]]"""
+    return execute(
+        Search_testcasesQuery, {"search": search, "values": values}, rath=rath
+    ).testcases
+
+
+async def asearch_testresults(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_testresultsQueryOptions]]]:
+    """search_testresults
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_testresultsQueryTestresults]]]"""
+    return (
+        await aexecute(
+            Search_testresultsQuery, {"search": search, "values": values}, rath=rath
+        )
+    ).testresults
+
+
+def search_testresults(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_testresultsQueryOptions]]]:
+    """search_testresults
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_testresultsQueryTestresults]]]"""
+    return execute(
+        Search_testresultsQuery, {"search": search, "values": values}, rath=rath
+    ).testresults
+
+
 async def aget_agent(id: ID, rath: RekuestRath = None) -> Optional[Get_agentQueryAgent]:
     """get_agent
 
 
 
     Arguments:
         id (ID): id
@@ -1983,14 +2778,58 @@
         rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
 
     Returns:
         Optional[TemplateFragment]"""
     return execute(Get_templateQuery, {"id": id}, rath=rath).template
 
 
+async def asearch_templates(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_templatesQueryOptions]]]:
+    """search_templates
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_templatesQueryTemplates]]]"""
+    return (
+        await aexecute(
+            Search_templatesQuery, {"search": search, "values": values}, rath=rath
+        )
+    ).templates
+
+
+def search_templates(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_templatesQueryOptions]]]:
+    """search_templates
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_templatesQueryTemplates]]]"""
+    return execute(
+        Search_templatesQuery, {"search": search, "values": values}, rath=rath
+    ).templates
+
+
 async def afind(
     id: Optional[ID] = None,
     template: Optional[ID] = None,
     hash: Optional[str] = None,
     rath: RekuestRath = None,
 ) -> Optional[NodeFragment]:
     """find
@@ -2031,14 +2870,86 @@
     Returns:
         Optional[NodeFragment]"""
     return execute(
         FindQuery, {"id": id, "template": template, "hash": hash}, rath=rath
     ).node
 
 
+async def aretrieveall(
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[NodeFragment]]]:
+    """retrieveall
+
+
+
+    Arguments:
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[NodeFragment]]]"""
+    return (await aexecute(RetrieveallQuery, {}, rath=rath)).allnodes
+
+
+def retrieveall(rath: RekuestRath = None) -> Optional[List[Optional[NodeFragment]]]:
+    """retrieveall
+
+
+
+    Arguments:
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[NodeFragment]]]"""
+    return execute(RetrieveallQuery, {}, rath=rath).allnodes
+
+
+async def asearch_nodes(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_nodesQueryOptions]]]:
+    """search_nodes
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_nodesQueryAllnodes]]]"""
+    return (
+        await aexecute(
+            Search_nodesQuery, {"search": search, "values": values}, rath=rath
+        )
+    ).allnodes
+
+
+def search_nodes(
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: RekuestRath = None,
+) -> Optional[List[Optional[Search_nodesQueryOptions]]]:
+    """search_nodes
+
+
+
+    Arguments:
+        search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
+        rath (rekuest.rath.RekuestRath, optional): The arkitekt rath client
+
+    Returns:
+        Optional[List[Optional[Search_nodesQueryAllnodes]]]"""
+    return execute(
+        Search_nodesQuery, {"search": search, "values": values}, rath=rath
+    ).allnodes
+
+
 async def aget_reservation(
     id: ID, rath: RekuestRath = None
 ) -> Optional[Get_reservationQueryReservation]:
     """get_reservation
 
 
 
@@ -2100,14 +3011,15 @@
         Optional[List[Optional[ReservationFragment]]]"""
     return execute(
         ReservationsQuery, {"identifier": identifier}, rath=rath
     ).reservations
 
 
 AnnotationInput.update_forward_refs()
-ArgPortInput.update_forward_refs()
 ChildPortInput.update_forward_refs()
 DefinitionInput.update_forward_refs()
+DescendendInput.update_forward_refs()
+EffectInput.update_forward_refs()
+PortInput.update_forward_refs()
 ProvisionFragmentTemplate.update_forward_refs()
-ReturnPortInput.update_forward_refs()
 TemplateFragment.update_forward_refs()
 WidgetInput.update_forward_refs()
```

### Comparing `rekuest-0.1.9/rekuest/contrib/fakts/websocket_agent_transport.py` & `rekuest-0.2.0/rekuest/contrib/arkitekt/websocket_agent_transport.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from typing import Optional
 from fakts.fakt.base import Fakt
 from fakts.fakts import get_current_fakts
-from herre import current_herre
+from fakts import Fakts
+from herre import Herre
 from rekuest.agents.transport.websocket import WebsocketAgentTransport
 from pydantic import Field
 
 from typing import Any, Awaitable, Callable, Dict, Optional
 
 from pydantic import Field
-from rekuest.messages import T
 
 
 class WebsocketAgentTransportConfig(Fakt):
     endpoint_url: str
     instance_id: str = "default"
 
 
-class FaktsWebsocketAgentTransport(WebsocketAgentTransport):
+class ArkitektWebsocketAgentTransport(WebsocketAgentTransport):
     endpoint_url: Optional[str]
     instance_id: Optional[str]
     token_loader: Optional[Callable[[], Awaitable[str]]] = Field(exclude=True)
-
-    fakts_group = "arkitekt.agent"
+    fakts: Fakts
+    herre: Herre
+    fakts_group: str
     _old_fakt: Dict[str, Any] = {}
 
     def configure(self, fakt: WebsocketAgentTransportConfig) -> None:
         self.endpoint_url = fakt.endpoint_url
-        self.token_loader = self.token_loader or current_herre.get().aget_token
+        self.token_loader = self.token_loader or self.herre.aget_token
 
     async def aconnect(self, *args, **kwargs):
-        fakts = get_current_fakts()
-
-        if fakts.has_changed(self._old_fakt, self.fakts_group):
-            self._old_fakt = await fakts.aget(self.fakts_group)
+        if self.fakts.has_changed(self._old_fakt, self.fakts_group):
+            self._old_fakt = await self.fakts.aget(self.fakts_group)
             self.configure(WebsocketAgentTransportConfig(**self._old_fakt))
 
         return await super().aconnect(*args, **kwargs)
```

### Comparing `rekuest-0.1.9/rekuest/definition/define.py` & `rekuest-0.2.0/rekuest/definition/define.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,470 +1,471 @@
-from contextlib import nullcontext
 from enum import Enum
-from random import choices
-from typing import Any, Callable, List, Tuple, Type
+from typing import Callable, List, Tuple, Type, Union
+
+from rekuest.definition.guards import cls_is_union
+from .utils import get_type_hints, is_annotated
 import inflection
 from rekuest.api.schema import (
-    ArgPortInput,
+    PortInput,
     ChildPortInput,
     DefinitionInput,
     NodeKindInput,
     PortKindInput,
-    ReturnPortInput,
-    WidgetInput,
     AnnotationInput,
+    Scope,
+    WidgetInput,
+    ReturnWidgetInput,
+    PortGroupInput,
+    EffectInput,
 )
 import inspect
 from docstring_parser import parse
-from rekuest.definition.errors import DefinitionError
+from rekuest.definition.errors import DefinitionError, NonSufficientDocumentation
 
 from rekuest.structures.registry import (
     StructureRegistry,
 )
+from typing import (
+    Protocol,
+    runtime_checkable,
+    Optional,
+    List,
+    Any,
+    Dict,
+    get_origin,
+    get_args,
+)
+import types
+import typing
 
 
 def convert_child_to_childport(
     cls: Type,
     registry: StructureRegistry,
     nullable: bool = False,
-    is_return: bool = False,
     annotations: List[AnnotationInput] = None,
-) -> Tuple[ChildPortInput, WidgetInput, Callable]:
+) -> Tuple[ChildPortInput, Callable]:
     """Converts a element of a annotation to a child port
 
     Args:
         cls (Type): The type (class or annotation) of the elemtn
         registry (StructureRegistry): The structure registry to use
-        nullable (bool, optional): Is this type optional (recursive parameter). Defaults to False.
+        nullable (bool, optional): Is this type optional (recursive parameter).
+            Defaults to False.
         is_return (bool, optional): Is this a return type?. Defaults to False.
-        annotations (List[AnnotationInput], optional): The annotations for this element. Defaults to None.
+        annotations (List[AnnotationInput], optional): The annotations for this element.
+            Defaults to None.
 
     Returns:
-        Tuple[ChildPortInput, WidgetInput, Callable]: The child port, the widget and the converter for the default
+        Tuple[ChildPortInput, WidgetInput, Callable]: The child port, the widget and the
+         converter for the default
     """
 
-    if hasattr(cls, "__name__") and cls.__name__ == "Annotated":
+    if is_annotated(cls):
         real_type = cls.__args__[0]
 
-        annotations = [
-            registry.get_converter_for_annotation(i.__class__)(i)
-            for i in cls.__metadata__
-        ]
-
         return convert_child_to_childport(
             real_type,
             registry,
             nullable=nullable,
             annotations=annotations,
         )
 
     if cls.__module__ == "typing":
-
         if hasattr(cls, "_name"):
             # We are dealing with a Typing Var?
             if cls._name == "List":
-                child, insidewidget, nested_converter = convert_child_to_childport(
+                child, nested_converter = convert_child_to_childport(
                     cls.__args__[0], registry, nullable=False
                 )
 
                 return (
                     ChildPortInput(
                         kind=PortKindInput.LIST,
                         child=child,
+                        scope=Scope.GLOBAL,
                         nullable=nullable,
                         annotations=annotations,
                     ),
-                    insidewidget,
-                    lambda default: [nested_converter(ndefault) for ndefault in default]
-                    if default
-                    else None,
+                    lambda default: (
+                        [nested_converter(ndefault) for ndefault in default]
+                        if default
+                        else None
+                    ),
                 )
 
             if cls._name == "Dict":
-                child, insidewidget, nested_converter = convert_child_to_childport(
+                child, nested_converter = convert_child_to_childport(
                     cls.__args__[1], "omit", registry, nullable=False
                 )
                 return (
                     ChildPortInput(
                         kind=PortKindInput.DICT,
                         child=child,
+                        scope=Scope.GLOBAL,
                         nullable=nullable,
                         annotations=annotations,
                     ),
-                    insidewidget,
-                    lambda default: {
-                        key: item in nested_converter(item)
-                        for key, item in default.items()
-                    }
-                    if default
-                    else None,
+                    lambda default: (
+                        {
+                            key: item in nested_converter(item)
+                            for key, item in default.items()
+                        }
+                        if default
+                        else None
+                    ),
                 )
 
         if hasattr(cls, "__args__"):
             if cls.__args__[1] == type(None):
-                return convert_argument_to_port(
+                return convert_child_to_childport(
                     cls.__args__[0], registry, nullable=True
                 )
 
     if inspect.isclass(cls):
         # Generic Cases
 
         if not issubclass(cls, Enum) and issubclass(cls, bool):
             t = ChildPortInput(
                 kind=PortKindInput.BOOL,
                 nullable=nullable,
+                scope=Scope.GLOBAL,
                 annotations=annotations,
             )  # catch bool is subclass of int
-            return t, None, str
+            return t, str
 
         if not issubclass(cls, Enum) and issubclass(cls, int):
             return (
                 ChildPortInput(
                     kind=PortKindInput.INT,
                     nullable=nullable,
+                    scope=Scope.GLOBAL,
                     annotations=annotations,
                 ),
-                None,
                 int,
             )
         if not issubclass(cls, Enum) and issubclass(cls, str):
             return (
                 ChildPortInput(
                     kind=PortKindInput.STRING,
                     nullable=nullable,
+                    scope=Scope.GLOBAL,
                     annotations=annotations,
                 ),
-                None,
                 str,
             )
 
     identifier = registry.get_identifier_for_structure(cls)
+    scope = registry.get_scope_for_identifier(identifier)
     default_converter = registry.get_default_converter_for_structure(cls)
-    widget = (
-        registry.get_returnwidget_input(cls)
-        if is_return
-        else registry.get_widget_input(cls)
-    )
+    assign_widget = registry.get_widget_input(cls)
+    return_widget = registry.get_returnwidget_input(cls)
 
     return (
         ChildPortInput(
             kind=PortKindInput.STRUCTURE,
             identifier=identifier,
+            scope=scope,
             nullable=nullable,
             annotations=annotations,
+            assignWidget=assign_widget,
+            returnWidget=return_widget,
         ),
-        widget,
         default_converter,
     )
 
 
-def convert_argument_to_port(
+def convert_object_to_port(
     cls,
     key,
     registry: StructureRegistry,
     widget=None,
+    return_widget=None,
     default=None,
+    label=None,
     description=None,
     nullable=False,
+    effects: Optional[List[EffectInput]] = None,
+    groups: Optional[List[str]] = None,
     annotations=[],
-) -> ArgPortInput:
+) -> PortInput:
     """
-    Convert a class to an ArgPort
+    Convert a class to an Port
     """
-    if hasattr(cls, "__name__") and cls.__name__ == "Annotated":
+    if is_annotated(cls):
         real_type = cls.__args__[0]
 
-        annotations = [
-            registry.get_converter_for_annotation(i.__class__)(i)
-            for i in cls.__metadata__
-        ]
-
-        return convert_argument_to_port(
+        return convert_object_to_port(
             real_type,
             key,
             registry,
             widget=widget,
             default=default,
+            label=label,
+            effects=effects,
             nullable=nullable,
             annotations=annotations,
+            groups=groups,
         )
 
     if cls.__module__ == "typing":
-
         if hasattr(cls, "_name"):
             # We are dealing with a Typing Var?
             if cls._name == "List":
-                child, widget, converter = convert_child_to_childport(
+                child, converter = convert_child_to_childport(
                     cls.__args__[0], registry, nullable=False
                 )
-                return ArgPortInput(
+                return PortInput(
                     kind=PortKindInput.LIST,
-                    widget=widget,
+                    assignWidget=widget,
+                    returnWidget=return_widget,
+                    scope=Scope.GLOBAL,
                     key=key,
-                    child=child.dict(exclude={"key"}),
+                    child=child,
+                    label=label,
                     default=[converter(item) for item in default] if default else None,
                     nullable=nullable,
+                    effects=effects,
                     annotations=annotations,
                     description=description,
+                    groups=groups,
                 )
 
+            if cls_is_union(cls):
+                args = get_args(cls)
+                if len(args) == 2 and args[0] == type(None) or args[1] == type(None):
+                    if args[0] == type(None):
+                        cls = args[1]
+                    if args[1] == type(None):
+                        cls = args[0]
+
+                    return convert_object_to_port(
+                        cls,
+                        key,
+                        registry,
+                        default=default,
+                        nullable=True,
+                        widget=widget,
+                        label=label,
+                        effects=effects,
+                        return_widget=return_widget,
+                        annotations=annotations,
+                        description=description,
+                        groups=groups,
+                    )
+                else:
+                    # We are dealing with a "Real union"
+                    args = get_args(cls)
+                    nullable = False
+                    variants = []
+                    for arg in args:
+                        if arg == type(None):
+                            nullable = True
+                        child, converter = convert_child_to_childport(
+                            arg, registry, nullable=False
+                        )
+                        variants.append(child)
+
+                    return PortInput(
+                        kind=PortKindInput.UNION,
+                        assignWidget=widget,
+                        returnWidget=return_widget,
+                        scope=Scope.GLOBAL,
+                        key=key,
+                        variants=variants,
+                        label=label,
+                        default=None,
+                        nullable=nullable,
+                        effects=effects,
+                        annotations=annotations,
+                        description=description,
+                        groups=groups,
+                    )
+
             if cls._name == "Dict":
-                child, widget, converter = convert_child_to_childport(
+                child, converter = convert_child_to_childport(
                     cls.__args__[1], registry, nullable=False
                 )
-                return ArgPortInput(
+                return PortInput(
                     kind=PortKindInput.DICT,
-                    widget=widget,
+                    assignWidget=widget,
+                    scope=Scope.GLOBAL,
+                    returnWidget=return_widget,
                     key=key,
-                    child=child.dict(exclude={"key"}),
-                    default={key: converter(item) for key, item in default.items()}
-                    if default
-                    else None,
+                    child=child,
+                    label=label,
+                    default=(
+                        {key: converter(item) for key, item in default.items()}
+                        if default
+                        else None
+                    ),
                     nullable=nullable,
+                    effects=effects,
                     annotations=annotations,
                     description=description,
+                    groups=groups,
                 )
 
             if cls._name == "Union":
                 raise NotImplementedError("Union is not supported yet")
 
         if hasattr(cls, "__args__"):
             if cls.__args__[1] == type(None):
-                return convert_argument_to_port(
+                return convert_object_to_port(
                     cls.__args__[0],
                     key,
                     registry,
                     default=default,
                     nullable=True,
                     widget=widget,
+                    label=label,
+                    effects=effects,
+                    return_widget=return_widget,
                     annotations=annotations,
                     description=description,
+                    groups=groups,
                 )
 
     if inspect.isclass(cls):
         # Generic Cases
 
-        if (
-            not issubclass(cls, Enum)
-            and issubclass(cls, bool)
-            or (default is not None and isinstance(default, bool))
+        if not issubclass(cls, Enum) and (
+            issubclass(cls, bool) or (default is not None and isinstance(default, bool))
         ):
-            t = ArgPortInput(
+            t = PortInput(
                 kind=PortKindInput.BOOL,
-                widget=widget,
+                scope=Scope.GLOBAL,
+                assignWidget=widget,
+                returnWidget=return_widget,
                 key=key,
                 default=default,
+                label=label,
                 nullable=nullable,
+                effects=effects,
                 annotations=annotations,
                 description=description,
+                groups=groups,
             )  # catch bool is subclass of int
             return t
 
-        if (
-            not issubclass(cls, Enum)
-            and issubclass(cls, int)
-            or (default is not None and isinstance(default, int))
+        if not issubclass(cls, Enum) and (
+            issubclass(cls, int) or (default is not None and isinstance(default, int))
         ):
-            return ArgPortInput(
+            return PortInput(
                 kind=PortKindInput.INT,
-                widget=widget,
+                assignWidget=widget,
+                scope=Scope.GLOBAL,
+                returnWidget=return_widget,
                 key=key,
                 default=default,
+                label=label,
                 nullable=nullable,
+                effects=effects,
                 annotations=annotations,
                 description=description,
+                groups=groups,
             )
 
-        if (
-            not issubclass(cls, Enum)
-            and issubclass(cls, float)
+        if not issubclass(cls, Enum) and (
+            issubclass(cls, float)
             or (default is not None and isinstance(default, float))
         ):
-            return ArgPortInput(
+            return PortInput(
                 kind=PortKindInput.FLOAT,
-                widget=widget,
+                assignWidget=widget,
+                returnWidget=return_widget,
+                scope=Scope.GLOBAL,
                 key=key,
                 default=default,
+                label=label,
                 nullable=nullable,
+                effects=effects,
                 annotations=annotations,
                 description=description,
+                groups=groups,
             )
 
-        if (
-            not issubclass(cls, Enum)
-            and issubclass(cls, str)
-            or (default is not None and isinstance(default, str))
+        if not issubclass(cls, Enum) and (
+            issubclass(cls, str) or (default is not None and isinstance(default, str))
         ):
-            return ArgPortInput(
+            return PortInput(
                 kind=PortKindInput.STRING,
-                widget=widget,
+                assignWidget=widget,
+                returnWidget=return_widget,
+                scope=Scope.GLOBAL,
                 key=key,
                 default=default,
+                label=label,
                 nullable=nullable,
+                effects=effects,
                 annotations=annotations,
                 description=description,
+                groups=groups,
             )
 
     identifier = registry.get_identifier_for_structure(cls)
+    scope = registry.get_scope_for_identifier(identifier)
     default_converter = registry.get_default_converter_for_structure(cls)
     widget = widget or registry.get_widget_input(cls)
+    return_widget = return_widget or registry.get_returnwidget_input(cls)
 
-    return ArgPortInput(
+    return PortInput(
         kind=PortKindInput.STRUCTURE,
         identifier=identifier,
-        widget=widget,
+        assignWidget=widget,
+        scope=scope,
+        returnWidget=return_widget,
         key=key,
+        label=label,
         default=default_converter(default) if default else None,
         nullable=nullable,
+        effects=effects,
         annotations=annotations,
         description=description,
+        groups=groups,
     )
 
 
-def convert_return_to_returnport(
-    cls,
-    key: str,
-    registry: StructureRegistry,
-    description=None,
-    widget=None,
-    nullable=False,
-    annotations=None,
-) -> ReturnPortInput:
-    """
-    Convert a class to an ArgPort
-    """
-    if hasattr(cls, "__name__") and cls.__name__ == "Annotated":
-        real_type = cls.__args__[0]
-
-        annotations = [
-            registry.get_converter_for_annotation(i.__class__)(i)
-            for i in cls.__metadata__
-        ]
-
-        return convert_return_to_returnport(
-            real_type,
-            key,
-            registry,
-            widget=widget,
-            nullable=nullable,
-            annotations=annotations,
-        )
-
-    if cls.__module__ == "typing":
-
-        if hasattr(cls, "_name"):
-            # We are dealing with a Typing Var?
-            if cls._name == "List":
-                child, widget, converter = convert_child_to_childport(
-                    cls.__args__[0], registry, nullable=False, is_return=True
-                )
-                return ReturnPortInput(
-                    kind=PortKindInput.LIST,
-                    widget=widget,
-                    key=key,
-                    child=child.dict(exclude={"key"}),
-                    nullable=nullable,
-                    description=description,
-                    annotations=annotations,
-                )
-
-            if cls._name == "Dict":
-                child, widget, converter = convert_child_to_childport(
-                    cls.__args__[1], registry, nullable=False, is_return=True
-                )
-                return ReturnPortInput(
-                    kind=PortKindInput.DICT,
-                    widget=widget,
-                    key=key,
-                    child=child.dict(exclude={"key"}),
-                    nullable=nullable,
-                    description=description,
-                    annotations=annotations,
-                )
-
-        if hasattr(cls, "__args__"):
-            if cls.__args__[1] == type(None):
-                return convert_return_to_returnport(
-                    cls.__args__[0],
-                    key,
-                    registry,
-                    nullable=True,
-                    annotations=annotations,
-                    description=description,
-                )
-
-    if inspect.isclass(cls):
-        # Generic Cases
-
-        if not issubclass(cls, Enum) and issubclass(cls, bool):
-            return ReturnPortInput(
-                kind=PortKindInput.BOOL,
-                key=key,
-                nullable=nullable,
-                description=description,
-                annotations=annotations,
-            )  # catch bool is subclass of int
-        if not issubclass(cls, Enum) and issubclass(cls, int):
-            return ReturnPortInput(
-                kind=PortKindInput.INT,
-                key=key,
-                nullable=nullable,
-                description=description,
-                annotations=annotations,
-            )
-        if not issubclass(cls, Enum) and issubclass(cls, float):
-            return ReturnPortInput(
-                kind=PortKindInput.FLOAT,
-                key=key,
-                nullable=nullable,
-                description=description,
-                annotations=annotations,
-            )
-        if not issubclass(cls, Enum) and issubclass(cls, str):
-            return ReturnPortInput(
-                kind=PortKindInput.STRING,
-                key=key,
-                nullable=nullable,
-                description=description,
-                annotations=annotations,
-            )
-
-    identifier = registry.get_identifier_for_structure(cls)
-    widget = widget or registry.get_returnwidget_input(cls)
-
-    return ReturnPortInput(
-        kind=PortKindInput.STRUCTURE,
-        identifier=identifier,
-        key=key,
-        widget=widget,
-        nullable=nullable,
-        description=None,
-        annotations=annotations,
-    )
+GroupMap = Dict[str, List[str]]
+WidgetMap = Dict[str, List[WidgetInput]]
+ReturnWidgetMap = Dict[str, List[ReturnWidgetInput]]
+EffectsMap = Dict[str, List[EffectInput]]
 
 
 def prepare_definition(
     function: Callable,
     structure_registry: StructureRegistry,
-    interface=None,
-    widgets=None,
-    allow_empty_doc=False,
-    interfaces=None,
+    widgets: Optional[WidgetMap] = None,
+    return_widgets: Optional[ReturnWidgetMap] = None,
+    groups: Optional[GroupMap] = None,
+    effects: Optional[EffectsMap] = None,
+    port_groups: List[PortGroupInput] = None,
+    allow_empty_doc=True,
+    collections: List[str] = [],
+    interfaces: Optional[List[str]] = None,
+    description: str = None,
+    is_test_for: Optional[List[str]] = None,
+    port_label_map: Optional[Dict[str, str]] = None,
+    port_description_map: Optional[Dict[str, str]] = None,
+    name: str = None,
     omitfirst=None,
     omitlast=None,
     omitkeys=[],
+    allow_annotations: bool = True,
+    **kwargs,  # additional kwargs can be ignored
 ) -> DefinitionInput:
     """Define
 
     Define a callable (async function, sync function, async generator, async
     generator) in the context of arkitekt and
     return its definition(input).
 
     Attention this definition is not yet registered in the
-    arkitekt registry. This is done by the create_template function ( which will validate the definition with your local arkitekt instance
+    arkitekt registry. This is done by the create_template function ( which will
+    validate he definition with your local arkitekt instance
     and raise an error if the definition is not compatible with your arkitekt version)
 
 
     Args:
         function (): The function you want to define
     """
 
@@ -472,134 +473,228 @@
 
     is_generator = inspect.isasyncgenfunction(function) or inspect.isgeneratorfunction(
         function
     )
 
     sig = inspect.signature(function)
     widgets = widgets or {}
+    effects = effects or {}
+
+    port_groups = port_groups or []
+    port_groups_name = [i.key for i in port_groups]
+    groups = groups or {}
+    for key, grouplist in groups.items():
+        for group in grouplist:
+            if group not in port_groups_name:
+                raise DefinitionError(
+                    f"Error mapping {group} to a group in port groups for port {key}:  Please define a PortGroup for {group}"
+                )
+
+    return_widgets = return_widgets or {}
     interfaces = interfaces or []
+    collections = collections or []
     # Generate Args and Kwargs from the Annotation
-    args: List[ArgPortInput] = []
-    returns: List[ReturnPortInput] = []
+    args: List[PortInput] = []
+    returns: List[PortInput] = []
 
     # Docstring Parser to help with descriptions
     docstring = parse(function.__doc__)
-    if docstring.long_description is None:
-        assert (
-            allow_empty_doc is not False
-        ), f"We don't allow empty documentation for function {function.__name__}. Please Provide"
-
-    function_ins_annotation = sig.parameters
+    if not docstring.short_description and name is None:
+        raise NonSufficientDocumentation(
+            f"Either provide a name or better document {function.__name__}. Try docstring"
+        )
 
-    doc_param_map = {param.arg_name: param.description for param in docstring.params}
+    if not docstring.long_description and description is None and not allow_empty_doc:
+        raise NonSufficientDocumentation(
+            f"Please provide a description or better document  {function.__name__}. Try docstring"
+        )
 
-    # TODO: Update with documentatoin.... (Set description for portexample)
+    type_hints = get_type_hints(function, include_extras=allow_annotations)
+    function_ins_annotation = sig.parameters
 
-    doc_returns_map = {
-        f"return{index}": param.description
-        for index, param in enumerate(docstring.many_returns)
+    doc_param_description_map = {
+        param.arg_name: param.description for param in docstring.params
     }
+    doc_param_label_map = {param.arg_name: param.arg_name for param in docstring.params}
 
-    for index, (key, value) in enumerate(function_ins_annotation.items()):
+    if docstring.many_returns:
+        doc_param_description_map.update(
+            {
+                f"return{index}": param.description
+                for index, param in enumerate(docstring.many_returns)
+            }
+        )
+        doc_param_label_map.update(
+            {
+                f"return{index}": param.return_name
+                for index, param in enumerate(docstring.many_returns)
+            }
+        )
+    elif docstring.returns:
+        doc_param_description_map.update({"return0": docstring.returns.description})
+        doc_param_label_map.update({"return0": docstring.returns.return_name})
+
+    if port_label_map:
+        doc_param_label_map.update(port_label_map)
+    if port_description_map:
+        doc_param_description_map.update(port_description_map)
 
+    for index, (key, value) in enumerate(function_ins_annotation.items()):
         # We can skip arguments if the builder is going to provide additional arguments
         if omitfirst is not None and index < omitfirst:
             continue
         if omitlast is not None and index > omitlast:
             continue
         if key in omitkeys:
             continue
 
-        widget = widgets.get(key, None)
-        cls = value.annotation
+        widget = widgets.pop(key, None)
+        port_effects = effects.pop(key, None)
+        return_widget = return_widgets.pop(key, None)
+        default = value.default if value.default != inspect.Parameter.empty else None
+        cls = type_hints.get(key, type(default) if default is not None else None)
+        this_port_groups = groups.get(key, None)
+
+        if cls is None:
+            raise DefinitionError(
+                f"Could not find type hint for {key} in {function.__name__}. Please provide a type hint (or default) for this argument."
+            )
 
         try:
             args.append(
-                convert_argument_to_port(
+                convert_object_to_port(
                     cls,
                     key,
                     structure_registry,
                     widget=widget,
-                    default=value.default
-                    if value.default != inspect.Parameter.empty
-                    else None,
-                    description=doc_param_map.get(key, None),
+                    return_widget=return_widget,
+                    default=default,
+                    effects=port_effects,
+                    nullable=value.default != inspect.Parameter.empty,
+                    description=doc_param_description_map.pop(key, None),
+                    label=doc_param_label_map.pop(key, None),
+                    groups=this_port_groups,
                 )
             )
         except Exception as e:
             raise DefinitionError(
-                f"Could not convert Argument of function {function.__name__} to ArgPort: {value}"
+                f"Could not convert Argument of function {function.__name__} to"
+                f" ArgPort: {value}"
             ) from e
 
     function_outs_annotation = sig.return_annotation
 
     if hasattr(function_outs_annotation, "_name"):
-
         if function_outs_annotation._name == "Tuple":
             try:
                 for index, cls in enumerate(function_outs_annotation.__args__):
-                    widget = widgets.get(f"return{index}", None)
+                    key = f"return{index}"
+                    return_widget = return_widgets.pop(key, None)
+                    widget = widgets.pop(key, None)
+                    port_effects = effects.pop(key, None)
+                    this_port_groups = groups.pop(key, None)
+
                     returns.append(
-                        convert_return_to_returnport(
+                        convert_object_to_port(
                             cls,
-                            f"return{index}",
+                            key,
                             structure_registry,
-                            description=doc_returns_map.get(f"return{index}", None),
+                            return_widget=return_widget,
+                            effects=port_effects,
+                            description=doc_param_description_map.pop(key, None),
+                            label=doc_param_label_map.pop(key, None),
                             widget=widget,
+                            groups=this_port_groups,
                         )
                     )
             except Exception as e:
                 raise DefinitionError(
-                    f"Could not convert Return of function {function.__name__} to ArgPort: {cls}"
+                    f"Could not convert Return of function {function.__name__} to"
+                    f" ArgPort: {cls}"
                 ) from e
         else:
             try:
-                widget = widgets.get(f"return0", None)
+                key = "return0"
+                return_widget = return_widgets.pop(key, None)
+                widget = widgets.pop(key, None)
+                this_port_groups = groups.get(key, None)
+                port_effects = effects.pop(key, None)
                 returns.append(
-                    convert_return_to_returnport(
+                    convert_object_to_port(
                         function_outs_annotation,
-                        f"return0",
+                        key,
                         structure_registry,
+                        return_widget=return_widget,
+                        effects=port_effects,
+                        description=doc_param_description_map.pop(key, None),
+                        label=doc_param_label_map.pop(key, None),
                         widget=widget,
+                        groups=this_port_groups,
                     )
                 )  # Other types will be converted to normal lists and shit
             except Exception as e:
                 raise DefinitionError(
-                    f"Could not convert Return of function {function.__name__} to ArgPort: {function_outs_annotation}"
+                    f"Could not convert Return of function {function.__name__} to"
+                    f" ArgPort: {function_outs_annotation}"
                 ) from e
     else:
         # We are dealing with a non tuple return
         if function_outs_annotation is None:
             pass
 
         elif function_outs_annotation.__name__ != "_empty":  # Is it not empty
-            widget = widgets.get(f"return0", None)
+            key = "return0"
+            return_widget = return_widgets.pop(key, None)
+            widget = widgets.pop(key, None)
+            this_port_groups = groups.pop(key, None)
+            port_effects = effects.pop(key, None)
             returns.append(
-                convert_return_to_returnport(
+                convert_object_to_port(
                     function_outs_annotation,
                     "return0",
                     structure_registry,
                     widget=widget,
+                    effects=port_effects,
+                    description=doc_param_description_map.pop(key, None),
+                    label=doc_param_label_map.pop(key, None),
+                    return_widget=return_widget,
+                    groups=this_port_groups,
                 )
             )
 
     # Documentation Parsing
 
-    name = docstring.short_description or function.__name__
-    interface = interface or inflection.underscore(
-        function.__name__
-    )  # convert this to camelcase
-    description = docstring.long_description or "No Description"
+    name = name or docstring.short_description or function.__name__
+    description = description or docstring.long_description or "No Description"
+
+    if widgets:
+        raise DefinitionError(
+            f"Could not find the following ports for the widgets in the function {function.__name__}: {','.join(widgets.keys())}. Did you forget the type hint?"
+        )
+    if return_widgets:
+        raise DefinitionError(
+            f"Could not find the following ports for the return widgets in the function {function.__name__}: {','.join(return_widgets.keys())}. Did you forget the type hint?"
+        )
+    if port_label_map:
+        raise DefinitionError(
+            f"Could not find the following ports for the labels in the function {function.__name__}: {','.join(port_label_map.keys())}. Did you forget the type hint?"
+        )
+    if port_description_map:
+        raise DefinitionError(
+            f"Could not find the following ports for the descriptions in the function {function.__name__}: {','.join(port_description_map.keys())}. Did you forget the type hint?"
+        )
 
     x = DefinitionInput(
         **{
             "name": name,
-            "interface": interface,
             "description": description,
+            "collections": collections,
             "args": args,
             "returns": returns,
             "kind": NodeKindInput.GENERATOR if is_generator else NodeKindInput.FUNCTION,
             "interfaces": interfaces,
+            "portGroups": port_groups,
+            "isTestFor": is_test_for,
         }
     )
 
     return x
```

### Comparing `rekuest-0.1.9/rekuest/definition/registry.py` & `rekuest-0.2.0/rekuest/register.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,283 @@
-import contextvars
-from ..actors.base import Actor
-from rekuest.api.schema import DefinitionInput
-from rekuest.actors.actify import reactify, Actifier
-from rekuest.definition.define import prepare_definition
+from rekuest.actors.types import Actifier
 from rekuest.structures.registry import (
     StructureRegistry,
     get_current_structure_registry,
 )
-from rekuest.api.schema import WidgetInput
-from typing import Dict, List, Callable, Optional, Tuple
-from pydantic import Field
-from koil.composition import KoiledModel
-from typing import Protocol, runtime_checkable
-import json
-from rekuest.actors.builder import ActorBuilder
-
-
-current_definition_registry = contextvars.ContextVar(
-    "current_definition_registry", default=None
+from rekuest.structures.default import (
+    get_default_structure_registry,
+)
+from rekuest.definition.registry import (
+    DefinitionRegistry,
+    get_default_definition_registry,
+    get_current_definition_registry,
+)
+from rekuest.api.schema import (
+    WidgetInput,
+    PortGroupInput,
+    Scope,
+    ReturnWidgetInput,
+    EffectInput,
 )
-GLOBAL_DEFINITION_REGISTRY = None
+from rekuest.collection.shelve import get_current_shelve
+from typing import Dict, List, Callable, Optional, Tuple, Awaitable, Any
+import inflection
+from rekuest.definition.define import prepare_definition
+from rekuest.actors.actify import reactify
+from functools import wraps, partial
 
 
-def get_default_definition_registry():
-    global GLOBAL_DEFINITION_REGISTRY
-    if GLOBAL_DEFINITION_REGISTRY is None:
-        GLOBAL_DEFINITION_REGISTRY = DefinitionRegistry()
-    return GLOBAL_DEFINITION_REGISTRY
+def register_func(
+    function_or_actor,
+    structure_registry: StructureRegistry,
+    definition_registry: DefinitionRegistry,
+    interface: str = None,
+    actifier: Actifier = reactify,
+    port_groups: Optional[List[PortGroupInput]] = None,
+    groups: Optional[Dict[str, List[str]]] = None,
+    collections: List[str] = None,
+    is_test_for: Optional[List[str]] = None,
+    widgets: Dict[str, WidgetInput] = None,
+    effects: Dict[str, List[EffectInput]] = None,
+    interfaces: List[str] = [],
+    on_provide=None,
+    on_unprovide=None,
+    in_process: bool = False,
+    **actifier_params,
+):
+    """Register a function or actor with the definition registry
 
+    Register a function or actor with the definition registry. This will
+    create a definition for the function or actor and register it with the
+    definition registry.
+
+    If first parameter is a function, it will be wrapped in an actorBuilder
+    through the actifier. If the first parameter is an actor, it will be
+    used as the actorBuilder (needs to have the dunder __definition__) to be
+    detected as such.
 
-def get_current_definition_registry(allow_global=True):
-    return current_definition_registry.get(get_default_definition_registry())
+    Args:
+        function_or_actor (Union[Actor, Callable]): _description_
+        actifier (Actifier, optional): _description_. Defaults to None.
+        interface (str, optional): _description_. Defaults to None.
+        widgets (Dict[str, WidgetInput], optional): _description_. Defaults to {}.
+        interfaces (List[str], optional): _description_. Defaults to [].
+        on_provide (_type_, optional): _description_. Defaults to None.
+        on_unprovide (_type_, optional): _description_. Defaults to None.
+        structure_registry (StructureRegistry, optional): _description_. Defaults to None.
+    """
 
+    interface = interface or inflection.underscore(
+        function_or_actor.__name__
+    )  # convert this to camelcase
+
+    assert (
+        interface not in definition_registry.definitions
+    ), "Interface already defined. Please choose a different name"
 
-class DefinitionRegistry(KoiledModel):
-    structure_registry: Optional[StructureRegistry] = None
-    defined_nodes: List[Tuple[DefinitionInput, Callable]] = Field(
-        default_factory=list, exclude=True
+    definition, actor_builder = actifier(
+        function_or_actor,
+        structure_registry,
+        on_provide=on_provide,
+        on_unprovide=on_unprovide,
+        widgets=widgets,
+        is_test_for=is_test_for,
+        collections=collections,
+        groups=groups,
+        port_groups=port_groups,
+        effects=effects,
+        interfaces=interfaces,
+        in_process=in_process,
+        **actifier_params,
     )
-    definitions: Dict[DefinitionInput, ActorBuilder] = Field(
-        default_factory=dict, exclude=True
+
+    definition_registry.register_at_interface(
+        interface, definition, structure_registry, actor_builder
     )
-    actifier: Actifier = reactify
-    copy_from_default: bool = False
 
-    _token: contextvars.Token = None
 
-    def has_definitions(self):
-        return len(self.defined_nodes) > 0 or len(self.templated_nodes) > 0
+def register(
+    *func,
+    actifier: Actifier = reactify,
+    interface: str = None,
+    widgets: Dict[str, WidgetInput] = None,
+    interfaces: List[str] = [],
+    collections: List[str] = None,
+    port_groups: Optional[List[PortGroupInput]] = None,
+    groups: Optional[Dict[str, List[str]]] = None,
+    effects: Dict[str, List[EffectInput]] = None,
+    is_test_for: Optional[List[str]] = None,
+    on_provide=None,
+    on_unprovide=None,
+    structure_registry: StructureRegistry = None,
+    definition_registry: DefinitionRegistry = None,
+    in_process: bool = False,
+    **actifier_params,
+):
+    """Register a function or actor to the default definition registry.
 
-    def reset(self):
-        self.defined_nodes = []  # dict are queryparams for the node
-        self.templated_nodes = []
+    You can use this decorator to register a function or actor to the default
+    definition registry. There is also a function version of this decorator,
+    which is more convenient to use.
+
+    Example:
+        >>> @register
+        >>> def hello_world(string: str):
 
-    def register_actorBuilder(self, actorBuilder: ActorBuilder, **params):  # New Node
-        self.defined_nodes.append((actorBuilder.__definition__, actorBuilder, params))
-        self.definitions[actorBuilder.__definition__] = actorBuilder
+        >>> @register(interface="hello_world")
+        >>> def hello_world(string: str):
 
-    def register(
-        self,
-        function_or_actor,
-        structure_registry: StructureRegistry,
-        actifier: Actifier = None,
-        interface: str = None,
-        widgets: Dict[str, WidgetInput] = None,
-        interfaces: List[str] = [],
-        on_provide=None,
-        on_unprovide=None,
-        **actifier_params,
-    ):
-        """Register a function or actor with the definition registry
+    Args:
+        function_or_actor (Union[Callable, Actor]): The function or Actor
+        builder (ActorBuilder, optional): An actor builder (see ActorBuilder). Defaults to None.
+        package (str, optional): The package you want to register this function in. Defaults to standard app package    .
+        interface (str, optional): The name of the function. Defaults to the functions name.
+        widgets (Dict[str, WidgetInput], optional): A dictionary of parameter key and a widget. Defaults to the default widgets as registered in the structure registry .
+        interfaces (List[str], optional): Interfaces that this node adheres to. Defaults to [].
+        on_provide (Callable[[ProvisionFragment], Awaitable[dict]], optional): Function that shall be called on provide (in the async eventloop). Defaults to None.
+        on_unprovide (Callable[[], Awaitable[dict]], optional): Function that shall be called on unprovide (in the async eventloop). Defaults to None.
+        structure_registry (StructureRegistry, optional): The structure registry to use for this Actor (used to shrink and expand inputs). Defaults to None.
+    """
+    definition_registry = definition_registry or get_default_definition_registry()
+    structure_registry = structure_registry or get_default_structure_registry()
+
+    if len(func) > 1:
+        raise ValueError("You can only register one function or actor at a time.")
+    if len(func) == 1:
+        function_or_actor = func[0]
+
+        @wraps(function_or_actor)
+        def wrapped_function(*args, **kwargs):
+            return function_or_actor(*args, **kwargs)
+
+        register_func(
+            function_or_actor,
+            structure_registry=structure_registry,
+            definition_registry=definition_registry,
+            actifier=actifier,
+            interface=interface,
+            is_test_for=is_test_for,
+            widgets=widgets,
+            effects=effects,
+            collections=collections,
+            interfaces=interfaces,
+            on_provide=on_provide,
+            on_unprovide=on_unprovide,
+            port_groups=port_groups,
+            groups=groups,
+            in_process=in_process,
+            **actifier_params,
+        )
+
+        return wrapped_function
+
+    else:
+
+        def real_decorator(function_or_actor):
+            # Simple bypass for now
+            @wraps(function_or_actor)
+            def wrapped_function(*args, **kwargs):
+                return function_or_actor(*args, **kwargs)
 
-        Register a function or actor with the definition registry. This will
-        create a definition for the function or actor and register it with the
-        definition registry.
-
-        If first parameter is a function, it will be wrapped in an actorBuilder
-        through the actifier. If the first parameter is an actor, it will be
-        used as the actorBuilder (needs to have the dunder __definition__) to be
-        detected as such.
-
-        Args:
-            function_or_actor (Union[Actor, Callable]): _description_
-            actifier (Actifier, optional): _description_. Defaults to None.
-            interface (str, optional): _description_. Defaults to None.
-            widgets (Dict[str, WidgetInput], optional): _description_. Defaults to {}.
-            interfaces (List[str], optional): _description_. Defaults to [].
-            on_provide (_type_, optional): _description_. Defaults to None.
-            on_unprovide (_type_, optional): _description_. Defaults to None.
-            structure_registry (StructureRegistry, optional): _description_. Defaults to None.
-        """
-
-        if hasattr(function_or_actor, "__definition__"):
-            actorBuilder = function_or_actor
-
-        else:
-            actifier = actifier or self.actifier
-            actorBuilder = actifier(
+            register_func(
                 function_or_actor,
-                structure_registry,
+                structure_registry=structure_registry,
+                definition_registry=definition_registry,
+                actifier=actifier,
+                interface=interface,
+                is_test_for=is_test_for,
+                widgets=widgets,
+                effects=effects,
+                collections=collections,
+                interfaces=interfaces,
                 on_provide=on_provide,
                 on_unprovide=on_unprovide,
-                widgets=widgets,
+                port_groups=port_groups,
+                groups=groups,
+                in_process=in_process,
                 **actifier_params,
             )
 
-        assert hasattr(
-            actorBuilder, "__definition__"
-        ), "The actorBuilder needs to have a definition. Otherwise it is not a valid actorBuilder"
-
-        self.register_actorBuilder(actorBuilder)
-
-    async def __aenter__(self):
-        return self
-
-    def dump(self):
-        return {
-            "definitions": [
-                json.loads(x[0].json(exclude_none=True, exclude_unset=True))
-                for x in self.defined_nodes
-            ],
-            "templates": [x[0] for x in self.templated_nodes],
-        }
+            return wrapped_function
 
-    async def __exit__(self, *args, **kwargs):
-        current_definition_registry.set(None)
+        return real_decorator
 
 
-def register(
-    widgets: Dict[str, WidgetInput] = {},
-    interfaces: List[str] = [],
-    on_provide=None,
-    on_unprovide=None,
-    definition_registry: DefinitionRegistry = None,
-    structure_registry: StructureRegistry = None,
-    **params,
+def register_structure(
+    *cls,
+    identifier: str = None,
+    scope: Scope = Scope.LOCAL,
+    aexpand: Callable[
+        [
+            str,
+        ],
+        Awaitable[Any],
+    ] = None,
+    ashrink: Callable[
+        [
+            any,
+        ],
+        Awaitable[str],
+    ] = None,
+    acollect: Callable[
+        [
+            str,
+        ],
+        Awaitable[Any],
+    ] = None,
+    convert_default: Callable[[Any], str] = None,
+    default_widget: WidgetInput = None,
+    default_returnwidget: ReturnWidgetInput = None,
+    registry: StructureRegistry = None,
+    **kwargs,
 ):
-    """Take a function and register it as a node.
+    """Register a structure to the default structure registry.
 
-    This function is used to register a node. Use it as a decorator. You can specify
-    specific widgets for every paramer in a dictionary {argument_key: widget}. By default
-    this function will use the default defintion registry to store the nodes inputdata.
-    This definition registry will then be used by an agent to create, and provide the node.
+    Args:
+        cls (Structure): The structure class
+        name (str, optional): The name of the structure. Defaults to the class name.
+    """
+    if len(cls) > 1:
+        raise ValueError("You can only register one function or actor at a time.")
+    if len(cls) == 1:
+        function_or_actor = cls[0]
+
+        sregistry = registry or get_default_structure_registry()
+
+        sregistry.register_as_structure(
+            function_or_actor,
+            identifier=identifier,
+            scope=scope,
+            ashrink=ashrink,
+            aexpand=aexpand,
+            acollect=acollect,
+            convert_default=convert_default,
+            default_widget=default_widget,
+            default_returnwidget=default_returnwidget,
+            **kwargs,
+        )
 
-    If your function has specific inputs that need custom rules for expansion and shrinking
-     , you can pass a structure registry to the function. This registry will then be used.
+        return cls
 
-    This decorator is non intrusive. You can still call this function as a normal function from
-    your code
+    else:
 
-    Args:
-        widgets (Dict[str, WidgetInput], optional): _description_. Defaults to {}.
-        interfaces (List[str], optional): _description_. Defaults to [].
-        on_provide (_type_, optional): _description_. Defaults to None.
-        on_unprovide (_type_, optional): _description_. Defaults to None.
-        definition_registry (DefinitionRegistry, optional): _description_. Defaults to None.
-        structure_registry (StructureRegistry, optional): _description_. Defaults to None.
+        def real_decorator(cls):
+            # Simple bypass for now
 
-    Returns:
-        Callable: A wrapped function that just returns the original function.
-    """
-    definition_registry = definition_registry or get_current_definition_registry()
-    structure_registry = structure_registry or get_current_structure_registry()
+            sregistry = registry or get_default_structure_registry()
 
-    def real_decorator(function):
-        # Simple bypass for now
-        def wrapped_function(*args, **kwargs):
-            return function(*args, **kwargs)
+            sregistry.register_as_structure(
+                cls,
+                identifier=identifier,
+                scope=scope,
+                ashrink=ashrink,
+                aexpand=aexpand,
+                acollect=acollect,
+                convert_default=convert_default,
+                default_widget=default_widget,
+                default_returnwidget=default_returnwidget,
+                **kwargs,
+            )
 
-        definition_registry.register(
-            function,
-            widgets=widgets,
-            interfaces=interfaces,
-            structure_registry=structure_registry,
-            on_provide=on_provide,
-            on_unprovide=on_unprovide,
-            **params,
-        )
+            return cls
 
-    return real_decorator
+        return real_decorator
```

### Comparing `rekuest-0.1.9/rekuest/definition/validate.py` & `rekuest-0.2.0/rekuest/definition/validate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from rekuest.api.schema import DefinitionInput, DefinitionFragment
-import random
+import json
+import hashlib
 
 
 def auto_validate(defintion: DefinitionInput) -> DefinitionFragment:
     """Validates a definition against its own schema
 
     This should always be the first step in the validation process
     but does not guarantee that the definition is valid on the connected
     arkitekt service. That means that the definition might be valid
     within this client (e.g. you can access and assign to actors in this
     context, but the arkitekt service might not be able to adress your actor
     or assign to it.)
 
     """
 
-    return DefinitionFragment(**defintion.dict())
+    return DefinitionFragment(**defintion.dict(by_alias=True))
+
+
+def hash_definition(definition: DefinitionInput):
+    hashable_definition = {
+        key: value
+        for key, value in dict(definition.dict()).items()
+        if key not in ["meta", "interface"]
+    }
+    return hashlib.sha256(
+        json.dumps(hashable_definition, sort_keys=True).encode()
+    ).hexdigest()
```

### Comparing `rekuest-0.1.9/rekuest/funcs.py` & `rekuest-0.2.0/rekuest/funcs.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.9/rekuest/messages.py` & `rekuest-0.2.0/rekuest/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import Any, List, Optional, TypeVar
 from pydantic import BaseModel
 from rekuest.api.schema import (
     LogLevelInput,
     ProvisionStatus,
     ReservationStatus,
     AssignationStatus,
 )
@@ -14,15 +14,15 @@
     pass
 
     def update(self: T, use: BaseModel = None, in_place=True, **kwargs) -> Optional[T]:
         if in_place:
             if use:
                 for key, value in use.dict().items():
                     if key in self.__fields__:
-                        if value != None:  # None is not a valid update!
+                        if value is not None:  # None is not a valid update!
                             setattr(self, key, value)
             if kwargs:
                 for key in kwargs:
                     setattr(self, key, kwargs[key])
 
             return self
         else:
@@ -54,14 +54,18 @@
 class Provision(UpdatableModel):
     provision: str
     guardian: str
     template: Optional[str]
     status: Optional[ProvisionStatus]
 
 
+class Inquiry(UpdatableModel):
+    assignations: List[Assignation]
+
+
 class Unprovision(UpdatableModel):
     provision: str
     message: Optional[str]
 
 
 class Reservation(UpdatableModel):
     reference: Optional[str]
```

### Comparing `rekuest-0.1.9/rekuest/postmans/graphql.py` & `rekuest-0.2.0/rekuest/postmans/graphql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Union
 import uuid
 from rekuest.api.schema import (
-    AssignationStatus,
-    ReservationStatus,
     AssignationFragment,
     ReservationFragment,
     ReserveParamsInput,
     aassign,
     areserve,
     awatch_requests,
     awatch_reservations,
     aunassign,
     aunreserve,
+    ReserveBindsInput,
 )
 
 from rekuest.postmans.base import BasePostman
 import asyncio
 from pydantic import Field
 import logging
-from .transport.base import PostmanTransport
+from .errors import PostmanException
+from .vars import current_postman
 
 logger = logging.getLogger(__name__)
 
 
 class GraphQLPostman(BasePostman):
     assignations: Dict[str, AssignationFragment] = Field(default_factory=dict)
     reservations: Dict[str, ReservationFragment] = Field(default_factory=dict)
@@ -33,57 +33,67 @@
     _res_update_queue: asyncio.Queue = None
     _ass_update_queue: asyncio.Queue = None
 
     _watch_resraces_task: asyncio.Task = None
     _watch_assraces_task: asyncio.Task = None
     _watch_reservations_task: asyncio.Task = None
     _watch_assignations_task: asyncio.Task = None
-    _watching = False
 
-    _lock = None
+    _watching: bool = None
+    _lock: asyncio.Lock = None
 
     async def aconnect(self):
-
-        self._lock = asyncio.Lock()
         await super().aconnect()
 
         data = {}  # await self.transport.alist_reservations()
         self.reservations = {res.reservation: res for res in data}
 
         data = {}  # await self.transport.alist_assignations()
         self.assignations = {ass.assignation: ass for ass in data}
 
     async def areserve(
         self,
-        node: str,
+        hash: str = None,
         params: ReserveParamsInput = None,
         provision: str = None,
         reference: str = "default",
+        binds: ReserveBindsInput = None,
     ) -> asyncio.Queue:
         async with self._lock:
             if not self._watching:
-                await self.start_watching()
+                self.start_watching()
 
-        unique_identifier = node + reference
+        unique_identifier = hash + reference
 
         self.reservations[unique_identifier] = None
         self._res_update_queues[unique_identifier] = asyncio.Queue()
-        reservation = await areserve(
-            node=node, params=params, provision=provision, reference=reference
-        )
+        try:
+            reservation = await areserve(
+                hash=hash,
+                params=params,
+                provision=provision,
+                reference=reference,
+                binds=binds,
+            )
+        except Exception as e:
+            raise PostmanException("Cannot Reserve") from e
+
         await self._res_update_queue.put(reservation)
         return self._res_update_queues[unique_identifier]
 
     async def aunreserve(self, reservation_id: str):
         async with self._lock:
             if not self._watching:
                 await self.start_watching()
 
-        unreservation = await aunreserve(reservation_id)
-        self.reservations[unreservation.id] = unreservation
+        try:
+            unreservation = await aunreserve(reservation_id)
+            self.reservations[unreservation.id] = unreservation
+        except Exception as e:
+            raise PostmanException("Cannot Unreserve") from e
 
     async def aassign(
         self,
         reservation: str,
         args: List[Any],
         persist=True,
         log=False,
@@ -95,29 +105,35 @@
                 await self.start_watching()
 
         if not reference:
             reference = str(uuid.uuid4())
 
         self.assignations[reference] = None
         self._ass_update_queues[reference] = asyncio.Queue()
-        assignation = await aassign(
-            reservation=reservation, args=args, reference=reference, parent=parent
-        )
+        try:
+            assignation = await aassign(
+                reservation=reservation, args=args, reference=reference, parent=parent
+            )
+        except Exception as e:
+            raise PostmanException("Cannot Assign") from e
         await self._ass_update_queue.put(assignation)
         return self._ass_update_queues[reference]
 
     async def aunassign(
         self,
         assignation: str,
     ) -> AssignationFragment:
         async with self._lock:
             if not self._watching:
                 await self.start_watching()
 
-        unassignation = await aunassign(assignation)
+        try:
+            unassignation = await aunassign(assignation)
+        except Exception as e:
+            raise PostmanException("Cannot Unassign") from e
         self.assignations[unassignation.id] = unassignation
         return unassignation
 
     def register_reservation_queue(
         self, node: str, reference: str, queue: asyncio.Queue
     ):
         self._res_update_queues[node + reference] = queue
@@ -128,98 +144,103 @@
     def unregister_reservation_queue(self, node: str, reference: str):
         del self._res_update_queues[node + reference]
 
     def unregister_assignation_queue(self, ass_id: str):
         del self._ass_update_queues[ass_id]
 
     async def watch_reservations(self):
-
         async for e in awatch_reservations("default"):
             res = e.update or e.create
             await self._res_update_queue.put(res)
 
     async def watch_assignations(self):
-
         async for assignation in awatch_requests("default"):
             ass = assignation.update or assignation.create
             await self._ass_update_queue.put(ass)
 
     async def watch_resraces(self):
         try:
             while True:
                 res: ReservationFragment = await self._res_update_queue.get()
-                self._res_update_queue.task_done()
 
-                unique_identifier = res.node.id + res.reference
+                unique_identifier = res.node.hash + res.reference
 
                 if unique_identifier not in self._res_update_queues:
                     logger.info(
-                        "Reservation update for unknown reservation received. Probably old stuf"
+                        "Reservation update for unknown reservation received. Probably"
+                        " old stuf"
                     )
-                    continue
-
-                if self.reservations[unique_identifier] is None:
-                    self.reservations[unique_identifier] = res
-                    await self._res_update_queues[unique_identifier].put(res)
-                    continue
-
                 else:
-                    if self.reservations[unique_identifier].updated_at < res.updated_at:
+                    if self.reservations[unique_identifier] is None:
                         self.reservations[unique_identifier] = res
                         await self._res_update_queues[unique_identifier].put(res)
+                        continue
+
                     else:
-                        logger.info(
-                            "Reservation update for reservation {} is older than current state. Ignoring".format(
-                                unique_identifier
+                        if (
+                            self.reservations[unique_identifier].updated_at
+                            < res.updated_at
+                        ):
+                            self.reservations[unique_identifier] = res
+                            await self._res_update_queues[unique_identifier].put(res)
+                        else:
+                            logger.info(
+                                "Reservation update for reservation {} is older than"
+                                " current state. Ignoring".format(unique_identifier)
                             )
-                        )
-                        continue
+
+                self._res_update_queue.task_done()
+
         except Exception:
             logger.error("Error in watch_resraces", exc_info=True)
 
     async def watch_assraces(self):
         try:
             while True:
                 ass: AssignationFragment = await self._ass_update_queue.get()
                 self._ass_update_queue.task_done()
 
                 unique_identifier = ass.reference
 
                 if unique_identifier not in self._ass_update_queues:
                     logger.info(
-                        f"Assignation update for unknown assignation received. Probably old stuf {ass}"
+                        "Assignation update for unknown assignation received. Probably"
+                        f" old stuf {ass}"
                     )
                     continue
 
                 if self.assignations[unique_identifier] is None:
                     self.assignations[unique_identifier] = ass
                     await self._ass_update_queues[unique_identifier].put(ass)
                     continue
 
                 else:
                     if self.assignations[unique_identifier].updated_at < ass.updated_at:
                         self.assignations[unique_identifier] = ass
                         await self._ass_update_queues[unique_identifier].put(ass)
                     else:
                         logger.info(
-                            f"Assignation update for assignation {ass} is older than current state. Ignoring"
+                            f"Assignation update for assignation {ass} is older than"
+                            " current state. Ignoring"
                         )
                         continue
 
         except Exception:
             logger.error("Error in watch_resraces", exc_info=True)
 
-    async def start_watching(self):
+    def start_watching(self):
+        logger.error("Starting watching")
         self._res_update_queue = asyncio.Queue()
         self._ass_update_queue = asyncio.Queue()
         self._watch_reservations_task = asyncio.create_task(self.watch_reservations())
         self._watch_assignations_task = asyncio.create_task(self.watch_assignations())
         self._watch_resraces_task = asyncio.create_task(self.watch_resraces())
         self._watch_assraces_task = asyncio.create_task(self.watch_assraces())
         self._watching = True
+        logger.error("Started watching")
 
     async def stop_watching(self):
         self._watch_reservations_task.cancel()
         self._watch_assignations_task.cancel()
         self._watch_resraces_task.cancel()
         self._watch_assraces_task.cancel()
 
@@ -234,16 +255,18 @@
         except asyncio.CancelledError:
             pass
 
         self._watching = False
 
     async def __aenter__(self):
         self._lock = asyncio.Lock()
+        current_postman.set(self)
         return await super().__aenter__()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if self._watching:
             await self.stop_watching()
+        current_postman.set(None)
         return await super().__aexit__(exc_type, exc_val, exc_tb)
 
     class Config:
         underscore_attrs_are_private = True
```

### Comparing `rekuest-0.1.9/rekuest/postmans/stateful.py` & `rekuest-0.2.0/rekuest/postmans/stateful.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 
 from rekuest.messages import Assignation, Reservation
 from rekuest.postmans.base import BasePostman
 import asyncio
 from pydantic import Field
 import logging
 from .transport.base import PostmanTransport
-import uuid
 
 logger = logging.getLogger(__name__)
 
 
 class StatefulPostman(BasePostman):
-
     transport: PostmanTransport
     assignations: Dict[str, Assignation] = Field(default_factory=dict)
     reservations: Dict[str, Reservation] = Field(default_factory=dict)
 
     _res_update_queues: Dict[str, asyncio.Queue] = {}
     _ass_update_queues: Dict[str, asyncio.Queue] = {}
 
@@ -86,25 +84,29 @@
             if message.assignation in self._ass_update_queues:
                 self.assignations[message.assignation].update(message)
                 await self._ass_update_queues[message.assignation].put(
                     self.assignations[message.assignation]
                 )
             else:
                 logger.warning(
-                    "Received Assignation Update without having knowingly queued it. Most likely because client crashed before receiving updates.  We will omit!"
+                    "Received Assignation Update without having knowingly queued it."
+                    " Most likely because client crashed before receiving updates.  We"
+                    " will omit!"
                 )
         elif isinstance(message, Reservation):
             if message.reservation in self._res_update_queues:
                 self.reservations[message.reservation].update(message)
                 await self._res_update_queues[message.reservation].put(
                     self.reservations[message.reservation]
                 )
             else:
                 logger.warning(
-                    "Received Reservation Update without having knowingly queued it. Most likely because client crashed before receiving updates. We will omit!"
+                    "Received Reservation Update without having knowingly queued it."
+                    " Most likely because client crashed before receiving updates. We"
+                    " will omit!"
                 )
 
         else:
             raise Exception("Unknown message type")
 
     def unregister_reservation_queue(self, node: str, reference: str):
         del self._res_update_queues[node + reference]
```

### Comparing `rekuest-0.1.9/rekuest/postmans/transport/base.py` & `rekuest-0.2.0/rekuest/postmans/transport/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from typing import (
-    Awaitable,
-    Callable,
     List,
     Optional,
     Dict,
     Any,
-    Union,
     Protocol,
     runtime_checkable,
 )
 
 from rekuest.messages import Assignation, Reservation, Unassignation, Unreservation
 from rekuest.api.schema import AssignationStatus, ReservationStatus, ReserveParamsInput
-from koil.composition import KoiledModel
 
 
 @runtime_checkable
 class PostmanTransport(Protocol):
     connected = False
 
     async def aassign(
```

### Comparing `rekuest-0.1.9/rekuest/postmans/transport/errors.py` & `rekuest-0.2.0/rekuest/postmans/transport/errors.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.9/rekuest/postmans/transport/mock.py` & `rekuest-0.2.0/rekuest/postmans/transport/mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         self,
         reservation: str,
         args: List[Any],
         kwargs: Dict[str, Any],
         persist=True,
         log=False,
     ) -> Assignation:
-
         assignation = Assignation(
             assignation=str(len(self.assignationState) + 1),
             reservation=reservation,
             args=args,
             kwargs=kwargs,
             status=AssignationStatus.PENDING,
         )
@@ -92,17 +91,15 @@
     async def aunassign(self, assignation: str) -> Unassignation:
         self.assignationState[assignation].update(
             Assignation(assignation=assignation, status=AssignationStatus.CANCELLED)
         )
         return assignation
 
     async def aresolve_reservations(self):
-
         while True:
-
             await asyncio.sleep(0.1)
 
             ress = [
                 res
                 for key, res in self.reservationState.items()
                 if res.status == ReservationStatus.ROUTING
             ]
@@ -128,15 +125,15 @@
                 await self._abroadcast(ass)
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         self._task.cancel()
 
         try:
             await self._task
-        except asyncio.CancelledError as e:
+        except asyncio.CancelledError:
             pass
 
     class Config:
         underscore_attrs_are_private = True
 
 
 class MockPostmanTransport(KoiledModel):
@@ -157,15 +154,14 @@
 
     async def alist_reservations(
         self, exclude: Optional[ReservationStatus] = None
     ) -> List[Reservation]:
         return []
 
     async def aconnect(self):
-
         self._in_queue = asyncio.Queue()
         self.connected = True
 
     async def __aenter__(self):
         await self.aconnect()
         pass
 
@@ -197,15 +193,14 @@
     async def areserve(
         self,
         node: str,
         params: ReserveParamsInput = None,
         provision: str = None,
         reference: str = "default",
     ) -> Reservation:
-
         assert self.connected, "Not connected"
 
         unique_identifier = node + reference
 
         self.reservationState[unique_identifier] = None
         self._res_update_queues[unique_identifier] = asyncio.Queue()
 
@@ -215,45 +210,41 @@
             status=ReservationStatus.ROUTING,
         )
 
         await self._in_queue.put(reservation)
         return self._res_update_queues[unique_identifier]
 
     async def aunreserve(self, reservation: str) -> Unreservation:
-
         assert self.connected, "Not connected"
 
         unreservation = Unreservation(reservation=reservation)
         await self._in_queue.put(unreservation)
         return unreservation
 
     async def aunassign(self, assignation: str) -> Unassignation:
-
         assert self.connected, "Not connected"
 
         unassignation = Unassignation(assignation=assignation)
         await self._in_queue.put(Unassignation(assignation=assignation))
         return unassignation
 
     async def adelay(
         self, message: Union[Assignation, Reservation, Unreservation, Unassignation]
     ):
-
         if isinstance(message, ReserveSubUpdate):
             unique_identifier = message.node + message.reference
             return await self._res_update_queues[unique_identifier].put(message)
 
         if isinstance(message, AssignSubUpdate):
             unique_identifier = message.reference
             return await self._ass_update_queues[unique_identifier].put(message)
 
         raise NotImplementedError()
 
     async def areceive(self, timeout=None):
-
         if timeout:
             return await asyncio.wait_for(self._in_queue.get(), timeout)
         return await self._in_queue.get()
 
     def delay(
         self, message: Union[Assignation, Reservation, Unreservation, Unassignation]
     ):
```

### Comparing `rekuest-0.1.9/rekuest/postmans/transport/protocols/postman_json.py` & `rekuest-0.2.0/rekuest/postmans/transport/protocols/postman_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 import uuid
 from typing_extensions import Literal
 
 
 from pydantic import BaseModel, Field
 from datetime import datetime
 from rekuest.messages import Assignation, Reservation, Unassignation, Unreservation
 from rekuest.api.schema import ReservationStatus, AssignationStatus, ReserveParamsInput
 from enum import Enum
 
 
 class PostmanMessageTypes(str, Enum):
-
     LIST_RESERVATION = "RESERVE_LIST"
     LIST_RESERVATION_REPLY = "RESERVE_LIST_REPLY"
     LIST_RESERVATION_DENIED = "RESERVE_LIST_DENIED"
 
     RESERVE = "RESERVE"
     RESERVE_REPLY = "RESERVE_REPLY"
     RESERVE_DENIED = "RESERVE_DENIED"
@@ -34,15 +33,14 @@
 
     UNASSIGN = "UNASSIGN"
     UNASSIGN_REPLY = "UNASSIGN_REPLY"
     UNASSIGN_DENIED = "UNASSIGN_DENIED"
 
 
 class PostmanSubMessageTypes(str, Enum):
-
     ASSIGN_UPDATE = "ASSIGN_UPDATE"
     RESERVE_UPDATE = "RESERVE_UPDATE"
 
 
 class JSONMeta(BaseModel):
     timestamp: datetime = Field(default_factory=datetime.utcnow)
```

### Comparing `rekuest-0.1.9/rekuest/postmans/transport/websocket.py` & `rekuest-0.2.0/rekuest/actors/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,283 +1,291 @@
-import asyncio
-import json
+from typing import Dict, Union
 
-import websockets
-from rekuest.postmans.transport.base import PostmanTransport
-from typing import Any, Awaitable, Callable, Dict, List, Optional
-from rekuest.messages import Assignation, Reservation
-from rekuest.postmans.transport.errors import (
-    AssignDeniedError,
-    AssignationListDeniedError,
-    PostmanTransportException,
-    ReservationListDeniedError,
-    ReserveDeniedError,
-    UnassignDeniedError,
-    UnreserveDeniedError,
+from pydantic import BaseModel, Field, PrivateAttr
+from rekuest.structures.registry import (
+    StructureRegistry,
 )
-from pydantic import Field
-from .protocols.postman_json import *
+import asyncio
 import logging
-from websockets.exceptions import ConnectionClosedError, InvalidStatusCode
+from rekuest.api.schema import (
+    AssignationLogLevel,
+    AssignationStatus,
+    ProvisionLogLevel,
+    ProvisionStatus,
+    ProvisionMode,
+    LogLevelInput,
+)
+from rekuest.messages import Assignation, Provision, Unassignation
+from rekuest.actors.errors import UnknownMessageError, ProvisionDelegateException
+from koil.types import Contextual
+from rekuest.definition.define import DefinitionInput
+from typing import Protocol, runtime_checkable, Optional, List, Any
+from rekuest.actors.transport.types import ActorTransport, AssignTransport
+from rekuest.collection.collector import ActorCollector, AssignationCollector
+from rekuest.definition.registry import (
+    DefinitionRegistry,
+)
+from rekuest.actors.types import Assignment, Passport, Unassignment
+import uuid
+from rekuest.collection.collector import Collector
 
 logger = logging.getLogger(__name__)
 
 
-async def token_loader():
-    raise NotImplementedError(
-        "Websocket transport does need a defined token_loader on Connection"
-    )
+class Actor(BaseModel):
+    passport: Passport
+    transport: ActorTransport
+    collector: Collector
+    definition_registry: DefinitionRegistry
+    managed_actors: Dict[str, "Actor"] = Field(default_factory=dict)
+    running_assignments: Dict[str, Assignment] = Field(default_factory=dict)
+
+    _in_queue: Contextual[asyncio.Queue] = PrivateAttr(default=None)
+    _running_asyncio_tasks: Dict[str, asyncio.Task] = PrivateAttr(default_factory=dict)
+    _running_transports: Dict[str, AssignTransport] = PrivateAttr(default_factory=dict)
+    _provision_task: asyncio.Task = PrivateAttr(default=None)
+    _status: ProvisionStatus = PrivateAttr(default=ProvisionStatus.PENDING)
 
+    async def on_provide(self, passport: Passport):
+        return None
 
-class CorrectableConnectionFail(PostmanTransportException):
-    pass
+    async def on_unprovide(self):
+        return None
 
+    async def on_assign(
+        self,
+        assignment: Assignment,
+        collector: AssignationCollector,
+        transport: AssignTransport,
+    ):
+        raise NotImplementedError(
+            "Needs to be owerwritten in Actor Subclass. Never use this class directly"
+        )
 
-class DefiniteConnectionFail(PostmanTransportException):
-    pass
+    async def apass(self, message: Union[Unassignment, Assignment]):
+        assert self._in_queue, "Actor is currently not listening"
+        await self._in_queue.put(message)
+
+    async def arun(self):
+        self._in_queue = asyncio.Queue()
+        self._provision_task = asyncio.create_task(self.alisten())
+        return self._provision_task
+
+    async def aset_status(self, status: ProvisionStatus, message: str = None):
+        self._status = status
+        await self.transport.change_provision(
+            status=status,
+            message=message or "No message provided",
+        )
 
+    async def aget_status(self):
+        return self._status
 
-class WebsocketPostmanTransport(PostmanTransport):
-    endpoint_url: str
-    token_loader: Callable[[], Awaitable[str]] = Field(exclude=True)
-    max_retries = 5
-    time_between_retries = 5
-    allow_reconnect = True
+    async def acancel(self):
+        # Cancel Mnaged actors
+        logger.info(f"Cancelling Actor {self.passport.id}")
+        if self.managed_actors:
+            logger.info("Cancelling Actors")
+            for actor in self.managed_actors.values():
+                logger.info(
+                    f"Cancelling managed actor with passport {actor.passport.id}"
+                )
+                await actor.acancel()
 
-    auto_connect = True
+        if not self._provision_task or self._provision_task.done():
+            # Race condition
+            return
 
-    _futures: Dict[str, asyncio.Future] = {}
-    _connected = False
-    _healthy = False
-    _send_queue: Optional[asyncio.Queue] = None
-    _connection_task: Optional[asyncio.Task] = None
+        self._provision_task.cancel()
 
-    async def aconnect(self):
-        assert (
-            self._abroadcast is not None
-        ), "Broadcast must be defined (either overwrite abroadcast or pass this in constructor of transport)"
+        try:
+            await self._provision_task
+        except asyncio.CancelledError:
+            logger.info(f"Actor {self.passport.id} was cancelled")
 
-        assert self.instance_id, "Needs an instance id"
-        self._send_queue = asyncio.Queue()
-        self._connection_task = asyncio.create_task(self.websocket_loop())
-        self._connected = True
+    async def aass_log(self, id: str, message: str, level=AssignationLogLevel.INFO):
+        logging.critical(f"ASS {id} {message}")
+        await self.transport.log_to_assignation(id=id, level=level, message=message)
+        logging.critical(f"ASS SEND {message}")
+
+    async def aprov_log(self, message: str, level=ProvisionLogLevel.INFO):
+        logging.critical(f"PROV {self.passport} {message}")
+        await self.transport.log_to_provision(
+            id=self.passport, level=level, message=message
+        )
 
-    async def websocket_loop(self, retry=0, reload_token=False):
-        send_task = None
-        receive_task = None
+    async def provide(self):
         try:
-            try:
-                token = await self.token_loader(force_refresh=reload_token)
+            logging.info(f"Providing {self.passport}")
+            await self.on_provide(self.passport)
+            await self.aset_status(
+                status=ProvisionStatus.ACTIVE,
+            )
 
-                async with websockets.connect(
-                    f"{self.endpoint_url}?token={token}&instance_id={self.instance_id}"
-                ) as client:
-
-                    logger.info("Postman on Websockets connected")
-
-                    send_task = asyncio.create_task(self.sending(client))
-                    receive_task = asyncio.create_task(self.receiving(client))
-
-                    self._healthy = True
-                    done, pending = await asyncio.wait(
-                        [send_task, receive_task],
-                        return_when=asyncio.FIRST_EXCEPTION,
-                    )
-                    self._healthy = True
+        except Exception as e:
+            logging.critical(f"Providing Error {self.passport} {e}", exc_info=True)
+            await self.aset_status(
+                status=ProvisionStatus.CRITICAL,
+                message=str(e),
+            )
 
-                    for task in pending:
-                        task.cancel()
+    async def unprovide(self):
+        try:
+            await self.on_unprovide()
+            await self.aset_status(
+                status=ProvisionStatus.INACTIVE,
+            )
 
-                    for task in done:
-                        raise task.exception()
+        except Exception as e:
+            logging.critical(f"Unproviding Error {self.passport} {e}", exc_info=True)
+            await self.aset_status(
+                status=ProvisionStatus.CRITICAL,
+                message=str(e),
+            )
 
-            except InvalidStatusCode as e:
-                logger.warning(
-                    f"Websocket Connect was denied. Trying to reload token {token}",
-                    exc_info=True,
-                )
-                reload_token = True
-                raise CorrectableConnectionFail from e
+    async def aprocess(self, message: Union[Assignment, Unassignment]):
+        logger.info(f"Actor for {self.passport}: Received {message}")
 
-            except ConnectionClosedError as e:
-                logger.warning("Websocket was closed", exc_info=True)
-                raise CorrectableConnectionFail from e
-
-            except Exception as e:
-                logger.warning("Websocket excepted. Trying to recover", exc_info=True)
-                raise CorrectableConnectionFail from e
-
-        except CorrectableConnectionFail as e:
-            logger.info(f"Trying to Recover from Exception {e}")
-            if retry > self.max_retries or not self.allow_reconnect:
-                raise DefiniteConnectionFail("Exceeded Number of Retries")
-
-            await asyncio.sleep(self.time_between_retries)
-            logger.info(f"Retrying to connect")
-            await self.websocket_loop(retry=retry + 1, reload_token=reload_token)
-
-        except DefiniteConnectionFail as e:
-            logger.error("Websocket excepted closed definetely", exc_info=True)
-            self.connection_dead = False
-            raise e
-
-        except asyncio.CancelledError as e:
-            logger.info("Websocket got cancelled. Trying to shutdown graceully")
-            if send_task and receive_task:
-                send_task.cancel()
-                receive_task.cancel()
+        if isinstance(message, Assignment):
+            transport = self.transport.spawn(message)
 
-            cancellation = await asyncio.gather(
-                send_task, receive_task, return_exceptions=True
+            task = asyncio.create_task(
+                self.on_assign(
+                    message,
+                    collector=self.collector,
+                    transport=transport,
+                )
             )
-            raise e
 
-    async def sending(self, client):
-        try:
-            while True:
-                message = await self._send_queue.get()
-                await client.send(message)
-                self._send_queue.task_done()
-        except asyncio.CancelledError as e:
-            logger.info("Sending Task sucessfully Cancelled")
+            self._running_transports[message.id] = transport
+            self._running_asyncio_tasks[message.id] = task
 
-    async def receiving(self, client):
-        try:
-            async for message in client:
-                await self.receive(message)
-        except asyncio.CancelledError as e:
-            logger.info("Receiving Task sucessfully Cancelled")
-
-    async def receive(self, message):
-        json_dict = json.loads(message)
-        if "type" in json_dict:
-            type = json_dict["type"]
-            id = json_dict["id"]
-            logger.debug(str(json_dict))
-
-            # State Layer
-            if type == PostmanSubMessageTypes.ASSIGN_UPDATE:
-                await self._abroadcast(AssignSubUpdate(**json_dict))
-
-            if type == PostmanSubMessageTypes.RESERVE_UPDATE:
-                await self._abroadcast(ReserveSubUpdate(**json_dict))
-
-            if type == PostmanMessageTypes.LIST_ASSIGNATION_REPLY:
-                self._futures[id].set_result(AssingListReply(**json_dict))
-            if type == PostmanMessageTypes.LIST_ASSIGNATION_DENIED:
-                self._futures[id].set_exception(
-                    AssignationListDeniedError(json_dict["error"])
-                )
+        elif isinstance(message, Unassignment):
+            if message.id in self._running_asyncio_tasks:
+                task = self._running_asyncio_tasks[message.id]
+                transport = self._running_transports[message.id]
+
+                if not task.done():
+                    task.cancel()
+                    try:
+                        await task
+                    except asyncio.CancelledError:
+                        logger.info(
+                            f"Task {transport.assignment} was cancelled through arkitekt. Setting Cancelled"
+                        )
+                        await transport.change_assignation(
+                            status=AssignationStatus.CANCELLED,
+                            message="Cancelled by Actor",
+                        )
+
+                        del self._running_asyncio_tasks[message.id]
+                        del self._running_transports[message.id]
+
+                else:
+                    logger.warning(
+                        f"Race Condition: Task was already done before cancellation"
+                    )
 
-            if type == PostmanMessageTypes.LIST_RESERVATION_REPLY:
-                self._futures[id].set_result(ReserveListReply(**json_dict))
-            if type == PostmanMessageTypes.LIST_RESERVATION_DENIED:
-                self._futures[id].set_exception(
-                    ReservationListDeniedError(json_dict["error"])
+            else:
+                logger.warning(
+                    f"Actor for {self.passport}: Received unassignment for unknown assignation {message.id}"
                 )
+        else:
+            raise UnknownMessageError(f"{message}")
 
-            if type == PostmanMessageTypes.ASSIGN_REPLY:
-                self._futures[id].set_result(AssignPubReply(**json_dict))
-            if type == PostmanMessageTypes.ASSIGN_DENIED:
-                self._futures[id].set_exception(AssignDeniedError(json_dict["error"]))
-
-            if type == PostmanMessageTypes.UNASSIGN_REPLY:
-                self._futures[id].set_result(UnassignPubReply(**json_dict))
-            if type == PostmanMessageTypes.UNASSIGN_DENIED:
-                self._futures[id].set_exception(UnassignDeniedError(json_dict["error"]))
-
-            if type == PostmanMessageTypes.RESERVE_REPLY:
-                self._futures[id].set_result(ReservePubReply(**json_dict))
-            if type == PostmanMessageTypes.RESERVE_DENIED:
-                self._futures[id].set_exception(ReserveDeniedError(json_dict["error"]))
-
-            if type == PostmanMessageTypes.UNRESERVE_REPLY:
-                self._futures[id].set_result(UnreservePubReply(**json_dict))
-            if type == PostmanMessageTypes.UNRESERVE_DENIED:
-                self._futures[id].set_exception(
-                    UnreserveDeniedError(json_dict["error"])
-                )
+    async def alisten(self):
+        try:
+            await self.provide()
+            logger.info(f"Actor for {self.passport}: Is now active")
 
-        else:
-            logger.error(f"Error {json_dict}")
+            while True:
+                message = await self._in_queue.get()
+                try:
+                    await self.aprocess(message)
+                except Exception as e:
+                    logger.critical(
+                        "Processing unknown message should never happen", exc_info=True
+                    )
 
-    async def awaitaction(self, action: JSONMessage):
-        if not self._connected:
-            assert (
-                self.auto_connect
-            ), "Websocket not connected, and autoconnect to false"
-            await self.aconnect()
-
-        if action.id in self._futures:
-            raise ValueError("Action already has a future")
-
-        future = asyncio.Future()
-        self._futures[action.id] = future
-        await self._send_queue.put(action.json())
-        return await future
-
-    async def alist_reservations(
-        self, exclude: Optional[ReservationStatus] = None
-    ) -> List[Reservation]:
-        prov_list_reply: ReserveListReply = await self.awaitaction(
-            ReserveList(exclude=exclude)
-        )
-        return prov_list_reply.reservations
+        except asyncio.CancelledError:
+            logger.info("Doing Whatever needs to be done to cancel!")
 
-    async def aassign(
-        self,
-        reservation: str,
-        args: List[Any],
-        kwargs: Dict[str, Any],
-        persist=True,
-        log=False,
-    ) -> Assignation:
-        ass_list_reply: AssignPubReply = await self.awaitaction(
-            AssignPub(
-                reservation=reservation,
-                args=args,
-                kwargs=kwargs,
-                persist=persist,
-                log=log,
-            )
-        )
-        return ass_list_reply
+            [i.cancel() for i in self._running_asyncio_tasks.values()]
+
+            for task, transport in zip(
+                self._running_asyncio_tasks.values(), self._running_transports.values()
+            ):
+                try:
+                    await task
+                except asyncio.CancelledError:
+                    logger.info(
+                        f"Task {transport.assignment} was cancelled through applicaction. Setting Critical"
+                    )
+                    await transport.change_assignation(
+                        status=AssignationStatus.CRITICAL,
+                        message="Cancelled by Application",
+                    )
 
-    async def areserve(
-        self, node: str, params: ReserveParamsInput = None, provision: str = None
-    ) -> Reservation:
-        action = ReservePub(node=node, params=params, provision=provision)
-        resrep: ReservePubReply = await self.awaitaction(action)
-        return resrep
-
-    async def aunreserve(self, reservation: str) -> Reservation:
-        action = UnreservePub(reservation=reservation)
-        unres: UnreservePubReply = await self.awaitaction(action)
-        return unres
-
-    async def aunassign(self, assignation: str) -> Reservation:
-        action = UnassignPub(assignation=assignation)
-        unass: UnassignPubReply = await self.awaitaction(action)
-        return unass
-
-    async def alist_assignations(
-        self, exclude: Optional[AssignationStatus] = None
-    ) -> List[Assignation]:
-        action = AssignList(exclude=exclude)
-        ass_list_reply: AssingListReply = await self.awaitaction(action)
-        return ass_list_reply.assignations
+            await self.unprovide()
 
-    async def adisconnect(self):
-        self._connection_task.cancel()
+        except Exception as e:
+            logger.critical("Unhandled exception", exc_info=True)
 
+            # TODO: Maybe send back an acknoledgement that we are done cancelling.
+            # If we don't do this, arkitekt will not know if we failed to cancel our
+            # tasks or if we succeeded. If we fail to cancel arkitekt can try to
+            # kill the whole agent (maybe causing a sys.exit(1) or something)
+
+        self._in_queue = None
+
+    def _provision_task_done(self, task):
+        logger.info(f"Provision task is done: {task}")
+        if task.exception():
+            raise task.exception()
+
+    async def __aenter__(self):
+        return self
+
+    async def aspawn_actor(
+        self, interface: str, transport: ActorTransport
+    ) -> "SerializingActor":
+        """Spawns an Actor from the definition of the given interface"""
         try:
-            await self._connection_task
-        except asyncio.CancelledError:
-            pass
+            actor_builder = self.definition_registry.get_builder_for_interface(
+                interface
+            )
 
-    async def __aexit__(self, *args, **kwargs):
-        if self._connection_task:
-            await self.adisconnect()
+        except KeyError as e:
+            raise ProvisionDelegateException(
+                "No Actor Builder found for interface"
+            ) from e
+
+        passport = Passport(provision=self.passport.provision, parent=self.passport.id)
+
+        actor = actor_builder(
+            passport=passport,
+            transport=transport,
+            definition_registry=self.definition_registry,
+            collector=self.collector,
+        )
+        self.managed_actors[passport.id] = actor
+        return actor
+
+    async def __aexit__(self, exc_type, exc, tb):
+        if self._provision_task and not self._provision_task.done():
+            await self.acancel()
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
+        copy_on_model_validation = "none"
+
+
+class SerializingActor(Actor):
+    definition: DefinitionInput
+    structure_registry: StructureRegistry
+    expand_inputs: bool = True
+    shrink_outputs: bool = True
+
+
+Actor.update_forward_refs()
+SerializingActor.update_forward_refs()
```

### Comparing `rekuest-0.1.9/rekuest/postmans/utils.py` & `rekuest-0.2.0/rekuest/postmans/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,482 +1,662 @@
-from ast import Assign
-from random import Random, random
-from typing import Awaitable, Callable, Optional, Union, TypeVar
+from random import random
+from typing import (
+    Awaitable,
+    Callable,
+    Optional,
+    Union,
+    TypeVar,
+    runtime_checkable,
+    Protocol,
+    Any,
+    Dict,
+    List,
+    Tuple,
+    AsyncIterator,
+)
 import uuid
-
+from rekuest.scalars import Interface
 from pydantic import Field
-from rekuest.messages import Assignation, Reservation
-from rekuest.postmans.vars import current_postman
+from rekuest.messages import Assignation, Reservation, Unassignation
 from rekuest.structures.registry import get_current_structure_registry
 from koil.composition import KoiledModel
 from koil.helpers import unkoil_gen
 from koil.types import ContextBool
-from .stateful import StatefulPostman
 from rekuest.api.schema import (
     AssignationFragment,
     AssignationLogLevel,
     AssignationStatus,
+    ProvisionStatus,
     ReservationFragment,
     ReservationStatus,
     ReserveParamsInput,
     NodeFragment,
 )
+import uuid
 import asyncio
-from rekuest.traits.node import Reserve
 from koil import unkoil
 import logging
-from rekuest.structures.serialization.postman import shrink_inputs, expand_outputs
+from rekuest.structures.serialization.postman import (
+    shrink_inputs,
+    expand_outputs,
+    serialize_inputs,
+    deserialize_outputs,
+)
 from rekuest.structures.registry import StructureRegistry
-from rekuest.api.schema import DefinitionFragment, DefinitionInput
+from rekuest.api.schema import (
+    DefinitionFragment,
+    DefinitionInput,
+    ReserveBindsInput,
+    afind,
+)
+from .errors import (
+    AssignException,
+    IncorrectReserveState,
+    PostmanException,
+    RecoverableAssignException,
+)
 from rekuest.agents.base import BaseAgent
-from rekuest.agents.transport.mock import MockAgentTransport
+from rekuest.actors.base import Actor, SerializingActor
+from rekuest.agents.transport.base import AgentTransport
+from rekuest.actors.transport.local_transport import (
+    LocalTransport,
+    ProxyActorTransport,
+    ProxyAssignTransport,
+)
 from rekuest.definition.validate import auto_validate
+from .base import BasePostman
+from rekuest.messages import Provision
+import asyncio
+from rekuest.agents.transport.protocols.agent_json import (
+    AssignationChangedMessage,
+    ProvisionChangedMessage,
+    ProvisionMode,
+)
+from rekuest.actors.transport.types import ActorTransport, AssignTransport
+from rekuest.definition.registry import DefinitionRegistry
+from rekuest.actors.types import Passport, Assignment, Unassignment, AssignmentUpdate
+from rekuest.structures.serialization.postman import (
+    serialize_inputs,
+    deserialize_outputs,
+)
+from enum import Enum
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
-class RPCContract(KoiledModel):
+class ContractStatus(str, Enum):
+    ACTIVE = "ACTIVE"
+    INACTIVE = "INACTIVE"
+
+
+@runtime_checkable
+class ContractStateHook(Protocol):
+    async def __call__(
+        self, state: ContractStatus = None, reference: str = None
+    ) -> None:
+        ...
+
+
+@runtime_checkable
+class RPCContract(Protocol):
+    async def __aenter__(self: Any) -> Any:
+        ...
+
+    async def __aexit__(self, exc_type, exc, tb):
+        ...
+
+    async def change_state(self, state: ContractStatus):
+        ...
+
+    async def aassign(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        assign_timeout: float = 10,
+    ) -> Dict[str, Any]:
+        ...
+
+    async def aassign_retry(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        assign_timeout: float = 10,
+        retry: int = 0,
+    ) -> Dict[str, Any]:
+        ...
+
+    async def astream(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        yield_timeout: float = 10,
+    ) -> AsyncIterator[List[Any]]:
+        ...
+
+    async def astream_retry(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        yield_timeout: float = 10,
+        retry: int = 0,
+    ) -> Dict[str, Any]:
+        ...
+
+
+class RPCContractBase(KoiledModel):
+    max_retries: int = 3
+    retry_delay_ms: float = 1000
+    reference: Optional[str]
     active: ContextBool = Field(default=False)
-    shrink_inputs: bool = True
-    expand_outputs: bool = True
+    state: ContractStatus = Field(default=ContractStatus.INACTIVE)
+    state_hook: Optional[ContractStateHook] = None
+    timeout_is_recoverable: bool = True
 
     async def aenter(self):
         raise NotImplementedError("Should be implemented by subclass")
 
     async def aexit(self):
         raise NotImplementedError("Should be implemented by subclass")
 
+    async def change_state(self, state: ContractStatus):
+        self.state = state
+        if self.state_hook:
+            await self.state_hook(state=state, reference=self.reference)
+
     async def aassign(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        reference: str = None,
+        assign_timeout: Optional[int] = None,
     ):
         raise NotImplementedError("Should be implemented by subclass")
 
     async def astream(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        reference: str = None,
+        yield_timeout: Optional[int] = None,
     ):
         raise NotImplementedError("Should be implemented by subclass")
 
-    def assign(self, *args, **kwargs):
-        return unkoil(self.aassign, *args, **kwargs)
+    async def astream_retry(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        yield_timeout: Optional[int] = None,
+        retry: int = 0,
+        reference: str = None,
+        retry_delay_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        try:
+            async for i in self.astream(
+                kwargs={**kwargs},
+                parent=parent,
+                reference=reference,
+                yield_timeout=yield_timeout,
+            ):
+                yield i
+        except RecoverableAssignException as e:
+            logger.warning(f"Stream failed with {e}")
+            if retry < self.max_retries:
+                await asyncio.sleep((retry_delay_ms or self.retry_delay_ms) * 0.001)
+                async for i in self.astream_retry(
+                    kwargs=kwargs,
+                    parent=parent,
+                    reference=reference,
+                    yield_timeout=yield_timeout,
+                    retry=retry + 1,
+                    retry_delay_ms=retry_delay_ms,
+                ):
+                    yield i
+            else:
+                raise e
 
-    def stream(self, *args, **kwargs):
-        return unkoil_gen(self.astream, *args, **kwargs)
+    async def aassign_retry(
+        self,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        assign_timeout: Optional[int] = None,
+        retry: int = 0,
+        reference: str = None,
+        retry_delay_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        try:
+            return await self.aassign(
+                kwargs={**kwargs},
+                parent=parent,
+                reference=reference,
+                assign_timeout=assign_timeout,
+            )
+        except RecoverableAssignException as e:
+            logger.warning(f"Assign failed with {e}")
+            if retry < self.max_retries:
+                logger.info(f"Retrying in {retry_delay_ms or self.retry_delay_ms}ms")
+                await asyncio.sleep((retry_delay_ms or self.retry_delay_ms) * 0.001)
+                return await self.aassign_retry(
+                    kwargs=kwargs,
+                    parent=parent,
+                    reference=reference,
+                    assign_timeout=assign_timeout,
+                    retry=retry + 1,
+                    retry_delay_ms=retry_delay_ms,
+                )
+            else:
+                raise e
 
     async def __aenter__(self: T) -> T:
         await self.aenter()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.aexit()
 
 
-class ReservationContract(RPCContract):
-    # TODO:Assert that we can actually assign to this? validating that all of the nodes inputs are
-    # registered in the structure registry?
-    definition: NodeFragment
-    provision: Optional[str] = None
-    reference: str = "default"
-    params: Optional[ReserveParamsInput] = None
-    auto_unreserve: bool = False
-    shrink_inputs: bool = True
-    expand_outputs: bool = True
-    res_log: Optional[
-        Callable[[Reservation, AssignationLogLevel, str], Awaitable[None]]
-    ] = Field(default=None, exclude=True)
-    on_reservation_change: Optional[
-        Callable[[ReservationFragment], Awaitable[None]]
-    ] = Field(default=None, exclude=True)
-
-    active: ContextBool = False
-    _reservation: Reservation = None
-
-    async def aassign(
-        self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
-    ):
-        raise NotImplementedError("Should be implemented by subclass")
-
-    async def astream(
-        self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
-    ):
-        raise NotImplementedError("Should be implemented by subclass")
-
-    async def _alog(self, assignation, level, msg):
-        if self.ass_log:  # pragma: no branch
-            await self.ass_log(assignation, level, msg)
-
-    async def _rlog(self, level, msg):
-        if self.res_log:  # pragma: no branch
-            await self.res_log(self._reservation, level, msg)
-
-    def assign(self, *args, **kwargs):
-        return unkoil(self.aassign, *args, **kwargs)
-
-    def stream(self, *args, **kwargs):
-        return unkoil_gen(self.astream, *args, **kwargs)
-
-    class Config:
-        arbitrary_types_allowed = True
-        json_encoders = {
-            callable: lambda q: repr(q),
-        }
-
+class actoruse(RPCContractBase):
+    interface: Interface
+    supervisor: Actor
+    reference: Optional[str]
+    "The governing actor"
+    assign_timeout: Optional[float] = 36000
+    yield_timeout: Optional[float] = 2000
 
-class localuse(RPCContract):
-    template: str
-    structure_registry: StructureRegistry
-    agent: BaseAgent
-    provide_timeout: Optional[float] = 2
-    assign_timeout: Optional[float] = 2
-    yield_timeout: Optional[float] = 2
-
-    _definition: DefinitionFragment = None
+    _transport: AgentTransport = None
+    _actor: SerializingActor
+    _enter_future: asyncio.Future = None
+    _exit_future: asyncio.Future = None
+    _updates_queue: asyncio.Queue[
+        Union[AssignationChangedMessage, ProvisionChangedMessage]
+    ] = None
+    _updates_watcher: asyncio.Task = None
+    _assign_queues = {}
 
     async def aassign(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        parent: Optional[Union[str, AssignationFragment]] = None,
-        assign_timeout: Optional[float] = 4,
-        **kwargs,
-    ):
-        assert self._reservation, "We never entered the context manager"
-        assert (
-            self._reservation.status == ReservationStatus.ACTIVE
-        ), "Reservation is not active"
-
-        structure_registry = structure_registry or self.structure_registry
-        inputs = await shrink_inputs(
-            self.definition,
-            args,
-            kwargs,
-            structure_registry=structure_registry,
-            skip_shrinking=not self.shrink_inputs,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        assign_timeout: Optional[float] = None,
+        reference: str = None,
+    ) -> Dict[str, Any]:
+        assignment = Assignment(
+            assignation=parent.assignation,
+            parent=parent.id,
+            args=serialize_inputs(self._actor.definition, kwargs),
+            status=AssignationStatus.ASSIGNED,
+            user=parent.user,
+            reference=reference,
         )
 
-        _ass_queue = await self.postman.aassign(
-            self._reservation.id, inputs, parent=parent
-        )
+        _ass_queue = asyncio.Queue[AssignmentUpdate]()
+        self._assign_queues[assignment.id] = _ass_queue
+
+        await self._actor.apass(assignment)
         try:
             while True:  # Waiting for assignation
                 ass = await asyncio.wait_for(
                     _ass_queue.get(), timeout=assign_timeout or self.assign_timeout
                 )
-                logger.info(f"Reservation Context: {ass}")
                 if ass.status == AssignationStatus.RETURNED:
-                    outputs = await expand_outputs(
-                        self.definition,
-                        ass.returns,
-                        structure_registry=structure_registry,
-                        skip_expanding=not self.expand_outputs,
-                    )
-                    return outputs
+                    return deserialize_outputs(self._actor.definition, ass.returns)
 
                 if ass.status in [AssignationStatus.CRITICAL, AssignationStatus.ERROR]:
-                    raise Exception(f"Critical error: {ass.statusmessage}")
+                    raise AssignException(f"Critical error: {ass.message}")
         except asyncio.CancelledError as e:
-            await self.postman.aunassign(ass.id)
+            await self._actor.apass(
+                Unassignation(
+                    assignation=id,
+                )
+            )
 
             ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
             if ass.status == AssignationStatus.CANCELING:
                 logger.info("Wonderfully cancelled that assignation!")
                 raise e
 
-            raise Exception(f"Critical error: {ass}")
+            raise AssignException(f"Critical error: {ass}")
+
+        except asyncio.TimeoutError as e:
+            exc_class = (
+                RecoverableAssignException
+                if self.timeout_is_recoverable
+                else AssignException
+            )
+
+            raise exc_class("Timeout error for assignation") from e
+
+    async def on_actor_log(self, *args, **kwargs):
+        logger.info(f"ActorLog: {args} {kwargs}")
+
+    async def on_assign_log(self, *args, **kwargs):
+        logger.info(f"AssingLog: {args} {kwargs}")
+
+    async def on_actor_change(self, status: ProvisionStatus, **kwargs):
+        if status == ProvisionStatus.ACTIVE:
+            await self.change_state(ContractStatus.ACTIVE)
+            if self._enter_future and not self._enter_future.done():
+                self._enter_future.set_result(True)
+
+        else:
+            await self.change_state(ContractStatus.INACTIVE)
+            if self._enter_future and not self._enter_future.done():
+                self._enter_future.set_exception(Exception("Error on provision"))
 
     async def astream(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        parent: Optional[Union[str, AssignationFragment]] = None,
-        yield_timeout: Optional[float] = 4,
-        **kwargs,
-    ):
-        assert self._reservation, "We never entered the context manager"
-        assert (
-            self._reservation.status == ReservationStatus.ACTIVE
-        ), "Reservation is not active"
-
-        structure_registry = structure_registry or get_current_structure_registry()
-
-        inputs = await shrink_inputs(
-            self.definition,
-            args,
-            kwargs,
-            structure_registry=structure_registry,
-            skip_shrinking=not self.shrink_inputs,
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        yield_timeout: Optional[float] = None,
+        reference: str = None,
+    ) -> AsyncIterator[Dict[str, Any]]:
+        inputs = serialize_inputs(self._actor.definition, kwargs)
+        assignment = Assignment(
+            assignation=parent.assignation,
+            parent=parent.id,
+            args=inputs,
+            status=AssignationStatus.ASSIGNED,
+            reference=reference,
         )
 
-        _ass_queue = await self.postman.aassign(
-            self._reservation.id,
-            inputs,
-            parent=parent,
-        )
+        _ass_queue = asyncio.Queue[AssignmentUpdate]()
+        self._assign_queues[assignment.id] = _ass_queue
+
+        await self._actor.apass(assignment)
+
         try:
             while True:  # Waiting for assignation
                 ass = await asyncio.wait_for(
                     _ass_queue.get(), timeout=yield_timeout or self.yield_timeout
                 )
-                logger.info(f"Reservation Context: {ass}")
                 if ass.status == AssignationStatus.YIELD:
-                    outputs = await expand_outputs(
-                        self.definition,
-                        ass.returns,
-                        structure_registry=structure_registry,
-                        skip_expanding=not self.expand_outputs,
-                    )
-                    yield outputs
+                    yield deserialize_outputs(self._actor.definition, ass.returns)
 
                 if ass.status == AssignationStatus.DONE:
+                    print("Done")
                     return
 
                 if ass.status in [AssignationStatus.CRITICAL, AssignationStatus.ERROR]:
-                    raise Exception(f"Critical error: {ass.statusmessage}")
+                    raise AssignException(f"Critical error: {ass.message}")
 
         except asyncio.CancelledError as e:
-            logger.warning(f"Cancelling this assignation {ass}")
-            await self.postman.aunassign(ass.id)
+            await self._actor.apass(
+                Unassignment(assignation=assignment.id, id=assignment.id)
+            )
 
             ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
             if ass.status == AssignationStatus.CANCELING:
                 logger.info("Wonderfully cancelled that assignation!")
                 raise e
 
             raise e
 
-    async def watch_updates(self):
+        except asyncio.TimeoutError as e:
+            exc_class = (
+                RecoverableAssignException
+                if self.timeout_is_recoverable
+                else AssignException
+            )
 
-        logger.info("Waiting for updates")
-        try:
-            while True:
-                self._reservation = await self._updates_queue.get()
-                logger.info(f"Updated Reservation {self._reservation}")
-                if self._reservation.status == ReservationStatus.ACTIVE:
-                    if self._enter_future and not self._enter_future.done():
-                        logger.info("Entering future")
-                        self._enter_future.set_result(True)
+            raise exc_class("Timeout error for assignation") from e
 
-                if self.on_reservation_change:
-                    await self.on_reservation_change(self._reservation)
+    async def on_assign_change(
+        self, assignment: Assignment, status=None, returns=None, progress=None
+    ):
+        await self._assign_queues[assignment.id].put(
+            AssignmentUpdate(
+                assignment=assignment.id,
+                status=status,
+                returns=returns,
+                progress=progress,
+            )
+        )
 
-        except asyncio.CancelledError:
-            pass
+        return
 
     async def aenter(self):
-        logger.info(f"Trying to reserve {self.definition}")
-
         self._enter_future = asyncio.Future()
+        self._updates_queue = asyncio.Queue[AssignationChangedMessage]()
 
-        self.transport = MockAgentTransport()
-
-        self._updates_queue = await self.agent.aspawn_actor(
-            node=self.definition.id,
-            params=self.params,
-            provision=self.provision,
-            reference=self.reference,
+        self._actor = await self.supervisor.aspawn_actor(
+            self.interface,
+            ProxyActorTransport(
+                on_log=self.on_actor_log,
+                on_change=self.on_actor_change,
+                on_assign_change=self.on_assign_change,
+                on_assign_log=self.on_assign_log,
+            ),
         )
-        try:
-            self._updates_watcher = asyncio.create_task(self.watch_updates())
-            await asyncio.wait_for(
-                self._enter_future, self.reserve_timeout
-            )  # Waiting to enter
 
-            self.active = True
+        await self._actor.arun()
+        await self._enter_future
 
-        except asyncio.TimeoutError:
-            logger.warning("Reservation timeout")
-            self._updates_watcher.cancel()
-
-            try:
-                await self._updates_watcher
-            except asyncio.CancelledError:
-                pass
-
-            self.active = False
-
-            raise
+    async def aexit(self):
+        if self._actor:
+            await self._actor.acancel()
 
-        return self
+    class Config:
+        arbitrary_types_allowed = True
+        underscore_attrs_are_private = True
+        copy_on_model_validation = False
 
 
-class arkiuse(ReservationContract):
-    postman: StatefulPostman
-    structure_registry: StructureRegistry
-    reserve_timeout: Optional[float] = 2
-    assign_timeout: Optional[float] = 2
-    yield_timeout: Optional[float] = 2
+class arkiuse(RPCContractBase):
+    hash: Optional[str] = None
+    provision: Optional[str] = None
+    reference: str = "default"
+    binds: Optional[ReserveBindsInput] = None
+    params: Optional[ReserveParamsInput] = None
+    postman: BasePostman
+    reserve_timeout: Optional[int] = 100000
+    assign_timeout: Optional[int] = 100000
+    yield_timeout: Optional[int] = 100000
+    auto_unreserve: bool = False
 
     _reservation: ReservationFragment = None
     _enter_future: asyncio.Future = None
     _exit_future: asyncio.Future = None
     _updates_queue: asyncio.Queue = None
     _updates_watcher: asyncio.Task = None
+    _definition: Optional[DefinitionFragment] = None
 
     async def aassign(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        parent: Optional[Union[str, AssignationFragment]] = None,
-        assign_timeout: Optional[float] = 4,
-        **kwargs,
-    ):
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        assign_timeout: Optional[int] = None,
+        reference: str = None,
+    ) -> Dict[str, Any]:
         assert self._reservation, "We never entered the context manager"
-        assert (
-            self._reservation.status == ReservationStatus.ACTIVE
-        ), "Reservation is not active"
-
-        structure_registry = structure_registry or self.structure_registry
-        inputs = await shrink_inputs(
-            self.definition,
-            args,
-            kwargs,
-            structure_registry=structure_registry,
-            skip_shrinking=not self.shrink_inputs,
-        )
+        if self.state != ContractStatus.ACTIVE:
+            raise IncorrectReserveState(
+                f"Contract is not active at the moment: {self.state}"
+            )
+
+        inputs = serialize_inputs(self._definition, kwargs)
 
-        _ass_queue = await self.postman.aassign(
-            self._reservation.id, inputs, parent=parent
-        )
+        try:
+            _ass_queue = await self.postman.aassign(
+                self._reservation.id,
+                inputs,
+                parent=parent.assignation,
+                reference=reference,
+            )
+        except PostmanException as e:
+            raise AssignException("Cannot do initial assignment") from e
+
+        ass = None
         try:
             while True:  # Waiting for assignation
                 ass = await asyncio.wait_for(
                     _ass_queue.get(), timeout=assign_timeout or self.assign_timeout
                 )
-                logger.info(f"Reservation Context: {ass}")
+                logger.info(f"Assign Context: {ass}")
                 if ass.status == AssignationStatus.RETURNED:
-                    outputs = await expand_outputs(
-                        self.definition,
-                        ass.returns,
-                        structure_registry=structure_registry,
-                        skip_expanding=not self.expand_outputs,
+                    return deserialize_outputs(self._definition, ass.returns)
+
+                if ass.status in [AssignationStatus.ERROR]:
+                    raise RecoverableAssignException(
+                        f"Recoverable Exception: {ass.statusmessage}"
                     )
-                    return outputs
 
-                if ass.status in [AssignationStatus.CRITICAL, AssignationStatus.ERROR]:
-                    raise Exception(f"Critical error: {ass.statusmessage}")
+                if ass.status in [AssignationStatus.CRITICAL]:
+                    raise AssignException(f"Critical error: {ass.statusmessage}")
+
+                if ass.status in [AssignationStatus.CANCELLED]:
+                    raise AssignException("Was cancelled from the outside")
+
         except asyncio.CancelledError as e:
-            await self.postman.aunassign(ass.id)
+            if ass:
+                await self.postman.aunassign(ass.id)
 
-            ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
-            if ass.status == AssignationStatus.CANCELING:
-                logger.info("Wonderfully cancelled that assignation!")
-                raise e
+                ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
+                if ass.status == AssignationStatus.CANCELING:
+                    logger.info("Wonderfully cancelled that assignation!")
+                    raise e
+
+                raise PostmanException(
+                    f"Unexpected Arkitekt repsonse while trying to cancel exception: {ass}"
+                )
+
+        except asyncio.TimeoutError as e:
+            if ass:
+                logger.warning(
+                    f"Cancelling this assignation but not wait for request {ass}"
+                )
+                await self.postman.aunassign(ass.id)
+
+            exc_class = (
+                RecoverableAssignException
+                if self.timeout_is_recoverable
+                else AssignException
+            )
 
-            raise Exception(f"Critical error: {ass}")
+            raise exc_class("Timeout error for assignation") from e
 
     async def astream(
         self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        parent: Optional[Union[str, AssignationFragment]] = None,
-        yield_timeout: Optional[float] = 4,
-        **kwargs,
-    ):
+        kwargs: Dict[str, Any],
+        parent: Assignment,
+        yield_timeout: Optional[int] = None,
+        reference: str = None,
+    ) -> AsyncIterator[Dict[str, Any]]:
         assert self._reservation, "We never entered the context manager"
-        assert (
-            self._reservation.status == ReservationStatus.ACTIVE
-        ), "Reservation is not active"
-
-        structure_registry = structure_registry or get_current_structure_registry()
-
-        inputs = await shrink_inputs(
-            self.definition,
-            args,
-            kwargs,
-            structure_registry=structure_registry,
-            skip_shrinking=not self.shrink_inputs,
-        )
+        if self.state != ContractStatus.ACTIVE:
+            raise IncorrectReserveState(
+                f"Contract is not active at the moment: {self.state}"
+            )
+
+        try:
+            _ass_queue = await self.postman.aassign(
+                self._reservation.id,
+                serialize_inputs(self._definition, kwargs),
+                parent=parent.assignation,
+                reference=reference,
+            )
+        except PostmanException as e:
+            raise AssignException("Cannot do initial assignment") from e
+        ass = None
 
-        _ass_queue = await self.postman.aassign(
-            self._reservation.id,
-            inputs,
-            parent=parent,
-        )
         try:
             while True:  # Waiting for assignation
                 ass = await asyncio.wait_for(
                     _ass_queue.get(), timeout=yield_timeout or self.yield_timeout
                 )
-                logger.info(f"Reservation Context: {ass}")
+                logger.info(f"Stream Context: {ass}")
                 if ass.status == AssignationStatus.YIELD:
-                    outputs = await expand_outputs(
-                        self.definition,
-                        ass.returns,
-                        structure_registry=structure_registry,
-                        skip_expanding=not self.expand_outputs,
-                    )
-                    yield outputs
+                    yield deserialize_outputs(self._definition, ass.returns)
 
-                if ass.status == AssignationStatus.DONE:
+                if ass.status in [AssignationStatus.DONE]:
                     return
 
-                if ass.status in [AssignationStatus.CRITICAL, AssignationStatus.ERROR]:
-                    raise Exception(f"Critical error: {ass.statusmessage}")
+                if ass.status in [AssignationStatus.ERROR]:
+                    raise RecoverableAssignException(
+                        f"Recoverable Exception: {ass.statusmessage}"
+                    )
+
+                if ass.status in [AssignationStatus.CRITICAL]:
+                    raise AssignException(f"Critical error: {ass.statusmessage}")
+
+                if ass.status in [AssignationStatus.CANCELLED]:
+                    raise AssignException("Was cancelled from the outside")
 
         except asyncio.CancelledError as e:
-            logger.warning(f"Cancelling this assignation {ass}")
-            await self.postman.aunassign(ass.id)
+            if ass:
+                logger.warning(f"Cancelling this assignation {ass}")
+                await self.postman.aunassign(ass.id)
+
+                ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
+                if ass.status == AssignationStatus.CANCELING:
+                    logger.info("Wonderfully cancelled that assignation!")
+                    raise e
 
-            ass = await asyncio.wait_for(_ass_queue.get(), timeout=2)
-            if ass.status == AssignationStatus.CANCELING:
-                logger.info("Wonderfully cancelled that assignation!")
-                raise e
+                raise PostmanException(
+                    f"Unexpected Arkitekt repsonse while trying to cancel exception: {ass}"
+                )
 
-            raise e
+        except asyncio.TimeoutError as e:
+            if ass:
+                logger.warning(
+                    f"Cancelling this assignation but not wait for request {ass}"
+                )
+                await self.postman.aunassign(ass.id)
 
-    async def watch_updates(self):
+            exc_class = (
+                RecoverableAssignException
+                if self.timeout_is_recoverable
+                else AssignException
+            )
 
+            raise exc_class("Timeout error for assignation") from e
+
+    async def watch_updates(self):
         logger.info("Waiting for updates")
         try:
             while True:
                 self._reservation = await self._updates_queue.get()
                 logger.info(f"Updated Reservation {self._reservation}")
                 if self._reservation.status == ReservationStatus.ACTIVE:
                     if self._enter_future and not self._enter_future.done():
                         logger.info("Entering future")
                         self._enter_future.set_result(True)
 
-                if self.on_reservation_change:
-                    await self.on_reservation_change(self._reservation)
+                    await self.change_state(ContractStatus.ACTIVE)
+
+                elif self._reservation.status == ReservationStatus.DISCONNECT:
+                    if self._enter_future and not self._enter_future.done():
+                        logger.info("Entering future")
+                        self._enter_future.set_result(True)
+
+                    await self.change_state(ContractStatus.INACTIVE)
+
+                else:
+                    logger.error(
+                        f"Currently unhandled status {self._reservation.status}"
+                    )
+                    if self._enter_future and not self._enter_future.done():
+                        self._enter_future.set_exception(True)
+
+                    await self.change_state(ContractStatus.INACTIVE)
 
         except asyncio.CancelledError:
             pass
 
     async def aenter(self):
-        logger.info(f"Trying to reserve {self.definition}")
-        assert self.postman.transport.connected, "Postman is not connected"
+        logger.info(f"Trying to reserve {self.hash}")
 
         self._enter_future = asyncio.Future()
-
+        self._definition = await afind(hash=self.hash)
         self._updates_queue = await self.postman.areserve(
-            node=self.definition.id,
+            hash=self.hash,
             params=self.params,
             provision=self.provision,
             reference=self.reference,
+            binds=self.binds,
         )
         try:
             self._updates_watcher = asyncio.create_task(self.watch_updates())
             await asyncio.wait_for(
                 self._enter_future, self.reserve_timeout
             )  # Waiting to enter
 
@@ -492,32 +672,31 @@
             raise
 
         return self
 
     async def aexit(self):
         self.active = False
 
-        if self.auto_unreserve:
-
-            unreservation = await asyncio.wait_for(
-                self.postman.aunreserve(self._reservation.id), timeout=1
-            )
-            logger.info(f"Unreserved {unreservation}")
+        if self._reservation:
+            if self.auto_unreserve:
+                logger.info(f"Unreserving {self.hash}")
+                await self.postman.aunreserve(self._reservation.id)
 
         if self._updates_watcher:
             self._updates_watcher.cancel()
 
             try:
                 await self._updates_watcher
             except asyncio.CancelledError:
                 pass
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
+        copy_on_model_validation = False
 
 
 class mockuse(RPCContract):
     returns: tuple = (1,)
     streamevents: int = 3
     assign_sleep: float = Field(default_factory=random)
     reserve_sleep: float = Field(default_factory=random)
@@ -526,15 +705,14 @@
 
     async def aenter(self):
         await asyncio.sleep(self.reserve_sleep)
         self.active = True
         return self
 
     async def aexit(self):
-
         self.active = False
         await asyncio.sleep(self.unreserve_sleep)
 
     async def aassign(
         self,
         *args,
         structure_registry=None,
@@ -562,81 +740,13 @@
         if alog:
             await alog(
                 Assignation(assignation=str(uuid.uuid4())),
                 AssignationLogLevel.INFO,
                 "Mock assignation",
             )
         for i in range(self.streamevents):
-            await asyncio.sleep(self.stream_sleep)
-            yield self.returns
-
-    class Config:
-        arbitrary_types_allowed = True
-        underscore_attrs_are_private = True
-
-
-class definitionmockuse(RPCContract):
-    definition: Union[DefinitionFragment, DefinitionInput]
-    should_assert: bool = True
-    returns: tuple = (1,)
-    streamevents: int = 3
-    assign_sleep: float = Field(default_factory=random)
-    reserve_sleep: float = Field(default_factory=random)
-    unreserve_sleep: float = Field(default_factory=random)
-    stream_sleep: float = Field(default_factory=random)
-
-    _active = False
-
-    async def aenter(self):
-        if isinstance(self.definition, DefinitionInput):
-            self.definition = auto_validate(self.definition)
-
-        self._active = True
-        await asyncio.sleep(self.reserve_sleep)
-        return self
-
-    async def aexit(self):
-        await asyncio.sleep(self.unreserve_sleep)
-        self._active = False
-
-    async def aassign(
-        self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
-    ):
-        assert self._active, "We never entered the context manager"
-        if self.should_assert:
-            assert len(args) == len(self.definition.args), "Wrong number of arguments"
-
-        if alog:
-            await alog(
-                Assignation(assignation=str(uuid.uuid4())),
-                AssignationLogLevel.INFO,
-                "Mock assignation",
-            )
-        await asyncio.sleep(self.assign_sleep)
-
-        return tuple(p.mock() for p in self.definition.returns)
-
-    async def astream(
-        self,
-        *args,
-        structure_registry=None,
-        alog: Callable[[Assignation, AssignationLogLevel, str], Awaitable[None]] = None,
-        **kwargs,
-    ):
-        assert self._active, "We never entered the context manager"
-        if alog:
-            await alog(
-                Assignation(assignation=str(uuid.uuid4())),
-                AssignationLogLevel.INFO,
-                "Mock assignation",
-            )
-        for i in range(self.streamevents):
             await asyncio.sleep(self.stream_sleep)
             yield self.returns
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
```

### Comparing `rekuest-0.1.9/rekuest/qt/builders.py` & `rekuest-0.2.0/rekuest/qt/builders.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,131 +1,171 @@
-from typing import Any
+from typing import Any, Tuple
 from qtpy import QtCore
 from rekuest.agents.transport.base import AgentTransport
-from rekuest.api.schema import TemplateFragment
 from rekuest.messages import Provision
 from koil.qt import QtCoro
 from rekuest.actors.functional import FunctionalFuncActor
-from rekuest.rath import RekuestRath
 from qtpy import QtWidgets
 from rekuest.definition.registry import ActorBuilder
 from rekuest.definition.define import prepare_definition, DefinitionInput
+from rekuest.actors.types import ActorBuilder, Passport
+from rekuest.collection.collector import ActorCollector
+from rekuest.actors.transport.types import ActorTransport
 
 
 class QtInLoopBuilder(QtCore.QObject):
     """A function that takes a provision and an actor transport and returns an actor.
 
     The actor produces by this builder will be running in the same thread as the
     koil instance (aka, the thread that called the builder).
 
     Args:
         QtCore (_type_): _description_
     """
 
-    def __init__(self, assign=None, *args, parent=None, **actor_kwargs) -> None:
+    def __init__(
+        self,
+        assign=None,
+        *args,
+        parent=None,
+        structure_registry=None,
+        definition=None,
+        **actor_kwargs
+    ) -> None:
         super().__init__(*args, parent=parent)
         self.coro = QtCoro(
-            lambda f, *args, **kwargs: assign(*args, **kwargs), autoresolve=True
+            lambda *args, **kwargs: assign(*args, **kwargs), autoresolve=True
         )
         self.provisions = {}
+        self.structure_registry = structure_registry
         self.actor_kwargs = actor_kwargs
+        self.definition = definition
 
     async def on_assign(self, *args, **kwargs) -> None:
         return await self.coro.acall(*args, **kwargs)
 
-    def build(
-        self,
-        provision: Provision,
-        transport: AgentTransport,
-        definition: DefinitionInput,
-    ) -> Any:
+    async def on_provide(self, provision: Provision) -> Any:
+        return None
+
+    async def on_unprovide(self) -> Any:
+        return None
+
+    def build(self, *args, **kwargs) -> Any:
         try:
             ac = FunctionalFuncActor(
-                definition=definition,
-                provision=provision,
-                transport=transport,
+                *args,
+                **kwargs,
+                structure_registry=self.structure_registry,
                 assign=self.on_assign,
-                **self.actor_kwargs,
+                on_provide=self.on_provide,
+                on_unprovide=self.on_unprovide,
+                definition=self.definition,
             )
             return ac
         except Exception as e:
             raise e
 
 
-class QtInLoopBuilder(QtCore.QObject):
+class QtFutureBuilder(QtCore.QObject):
     """A function that takes a provision and an actor transport and returns an actor.
 
     The actor produces by this builder will be running in the same thread as the
     koil instance (aka, the thread that called the builder).
 
     Args:
         QtCore (_type_): _description_
     """
 
     def __init__(
-        self, assign=None, *args, parent=None, structure_registry=None, **actor_kwargs
+        self,
+        assign=None,
+        *args,
+        parent=None,
+        structure_registry=None,
+        definition=None,
+        **actor_kwargs
     ) -> None:
         super().__init__(*args, parent=parent)
         self.coro = QtCoro(
-            lambda f, *args, **kwargs: assign(*args, **kwargs), autoresolve=True
+            lambda *args, **kwargs: assign(*args, **kwargs), autoresolve=False
         )
         self.provisions = {}
         self.structure_registry = structure_registry
         self.actor_kwargs = actor_kwargs
+        self.definition = definition
 
     async def on_assign(self, *args, **kwargs) -> None:
         return await self.coro.acall(*args, **kwargs)
 
     async def on_provide(self, provision: Provision) -> Any:
         return None
 
-    async def on_unprovide(self, provision: Provision) -> Any:
+    async def on_unprovide(self) -> Any:
         return None
 
-    def build(
-        self,
-        provision: Provision,
-        transport: AgentTransport,
-        definition: DefinitionInput,
-    ) -> Any:
+    def build(self, *args, **kwargs) -> Any:
         try:
             ac = FunctionalFuncActor(
-                definition=definition,
-                provision=provision,
+                *args,
+                **kwargs,
                 structure_registry=self.structure_registry,
-                transport=transport,
                 assign=self.on_assign,
                 on_provide=self.on_provide,
                 on_unprovide=self.on_unprovide,
+                definition=self.definition,
             )
             return ac
         except Exception as e:
             raise e
 
 
 def qtinloopactifier(
     function, structure_registry, parent: QtWidgets.QWidget = None, **kwargs
-) -> ActorBuilder:
+) -> Tuple[DefinitionInput, ActorBuilder]:
     """Qt Actifier
 
     The qt actifier wraps a function and returns a builder that will create an actor
     that runs in the same thread as the Qt instance, enabling the use of Qt widgets
     and signals.
     """
 
+    definition = prepare_definition(function, structure_registry, **kwargs)
+
     in_loop_instance = QtInLoopBuilder(
-        parent=parent, assign=function, structure_registry=structure_registry
+        parent=parent,
+        assign=function,
+        structure_registry=structure_registry,
+        definition=definition,
     )
-    definition = prepare_definition(function, structure_registry)
-
-    def builder(
-        provision: Provision,
-        transport: AgentTransport,
-    ) -> Any:
 
+    def builder(*args, **kwargs) -> Any:
         return in_loop_instance.build(
-            provision, transport, definition
+            *args, **kwargs
         )  # build an actor for this inloop instance
 
-    builder.__definition__ = definition
+    return definition, builder
+
+
+def qtwithfutureactifier(
+    function, structure_registry, parent: QtWidgets.QWidget = None, **kwargs
+) -> ActorBuilder:
+    """Qt Actifier
+
+    The qt actifier wraps a function and returns a build that calls the function with
+    its first parameter being a future that can be resolved within the qt loop
+    """
+
+    definition = prepare_definition(function, structure_registry, omitfirst=1, **kwargs)
+
+    in_loop_instance = QtFutureBuilder(
+        parent=parent,
+        assign=function,
+        structure_registry=structure_registry,
+        definition=definition,
+    )
+
+    def builder(*args, **kwargs) -> Any:
+        return in_loop_instance.build(
+            *args, **kwargs
+        )  # build an actor for this inloop instance
 
-    return builder
+    return definition, builder
```

### Comparing `rekuest-0.1.9/rekuest/rath.py` & `rekuest-0.2.0/rekuest/rath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from graphql import OperationType
 from pydantic import Field
 from rath import rath
 import contextvars
-from rath.links.aiohttp import AIOHttpLink
 from rath.links.auth import AuthTokenLink
 
-from rath.links.base import TerminatingLink
-from rath.links.compose import TypedComposedLink, compose
+from rath.links.compose import TypedComposedLink
 from rath.links.dictinglink import DictingLink
 from rath.links.shrink import ShrinkingLink
 from rath.links.split import SplitLink
 from rath.links.retry import RetryLink
-from rath.links.websockets import WebSocketLink
 
 current_rekuest_rath = contextvars.ContextVar("current_rekuest_rath", default=None)
 
 
 class RekuestLinkComposition(TypedComposedLink):
     shrink: ShrinkingLink = Field(default_factory=ShrinkingLink)
     dicting: DictingLink = Field(default_factory=DictingLink)
     auth: AuthTokenLink
     retry: RetryLink = Field(default_factory=RetryLink)
     split: SplitLink
 
+    def _repr_html_inline_(self):
+        return f"<table><tr><td>auth</td><td>{self.auth.maximum_refresh_attempts}</td></tr></table>"
+
 
 class RekuestRath(rath.Rath):
     link: RekuestLinkComposition = Field(default_factory=RekuestLinkComposition)
 
     async def __aenter__(self):
         await super().__aenter__()
         current_rekuest_rath.set(self)
         return self
 
+    def _repr_html_inline_(self):
+        return f"<table><tr><td>link</td><td>{self.link._repr_html_inline_()}</td></tr></table>"
+
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await super().__aexit__(exc_type, exc_val, exc_tb)
         current_rekuest_rath.set(None)
```

### Comparing `rekuest-0.1.9/rekuest/rekuest.py` & `rekuest-0.2.0/rekuest/rekuest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,69 @@
-from textwrap import wrap
-from typing import Any, Awaitable, Callable, Dict, List
+from typing import Dict
 from pydantic import Field
-from rekuest.agents.stateful import StatefulAgent
-from rekuest.api.schema import TemplateFragment, WidgetInput
+from rekuest.api.schema import TemplateFragment
 from rekuest.postmans.graphql import GraphQLPostman
-from rekuest.postmans.stateful import StatefulPostman
 from rekuest.rath import RekuestRath
-from rekuest.messages import Provision
 from rekuest.structures.default import get_default_structure_registry
 from rekuest.structures.registry import (
     StructureRegistry,
 )
 
 from rekuest.definition.registry import (
     DefinitionRegistry,
     get_current_definition_registry,
+    get_default_definition_registry,
 )
 from rekuest.agents.base import BaseAgent
 from rekuest.postmans.base import BasePostman
 from koil import unkoil
 from koil.composition import Composition
 from koil.decorators import koilable
-from rekuest.api.schema import acreate_template
-from rekuest.actors.builder import ActorBuilder
+from rekuest.register import register
 
 
 @koilable(fieldname="koil", add_connectors=True)
 class Rekuest(Composition):
     rath: RekuestRath = Field(default_factory=RekuestRath)
     structure_registry: StructureRegistry = Field(
         default_factory=get_default_structure_registry
     )
-    definition_registry: DefinitionRegistry = Field(
-        default_factory=get_current_definition_registry
-    )
-    agent: BaseAgent = Field(default_factory=StatefulAgent)
+    agent: BaseAgent = Field(default_factory=BaseAgent)
     postman: BasePostman = Field(default_factory=GraphQLPostman)
 
     registered_templates: Dict[str, TemplateFragment] = Field(default_factory=dict)
 
     def register(self, *args, **kwargs) -> None:
         """
         Register a new function
         """
-        structure_registry = kwargs.get("structure_registry", self.structure_registry)
-
-        def real_decorator(function_or_actor):
-
-            self.definition_registry.register(
-                function_or_actor,
-                *args,
-                structure_registry=structure_registry,
-                **kwargs
-            )
-
-            return function_or_actor
-
-        return real_decorator
+        structure_registry = kwargs.pop("structure_registry", self.structure_registry)
+        definition_registry = kwargs.pop(
+            "definition_registry", self.agent.definition_registry
+        )
+
+        return register(
+            *args,
+            definition_registry=definition_registry,
+            structure_registry=structure_registry,
+            **kwargs,
+        )
 
     def run(self, *args, **kwargs) -> None:
         """
         Run the application.
         """
         return unkoil(self.arun, *args, **kwargs)
 
-    async def arun(self, instance_id: str = "default") -> None:
+    async def arun(self) -> None:
         """
         Run the application.
         """
-        assert self.agent.transport.connected, "Transport is not connected"
-        await self.agent.aprovide(instance_id=instance_id)
+        await self.agent.aprovide()
+
+    def _repr_html_inline_(self):
+        return f"<table><tr><td>rath</td><td>{self.rath._repr_html_inline_()}</td></tr></table>"
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
         extra = "forbid"
```

### Comparing `rekuest-0.1.9/rekuest/scalars.py` & `rekuest-0.2.0/rekuest/scalars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,153 @@
-from datetime import date
 from graphql import (
     DocumentNode,
     parse,
     OperationDefinitionNode,
     OperationType,
     print_ast,
+    print_source_location,
+    print_location,
+    GraphQLError,
 )
+from graphql.language.print_location import print_prefixed_lines
+import inspect
 
 
 class QString(str):
     pass
 
 
-class Identifier(str):
+class Interface(str):
+    @classmethod
+    def validate(cls, v):
+        if not isinstance(v, str):
+            if hasattr(v, "__name__"):
+                return v.__name__
+            else:
+                raise ValueError("Interface must be either a str or function")
+        return v
 
+    pass
+
+
+class Identifier(str):
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str):
             raise TypeError("Identifier must be a string")
-        if "@" in v and not "/" in v:
+        if "@" in v and "/" not in v:
             raise ValueError(
-                "Identifier must contain follow '@package/module' when trying to mimic a global module "
+                "Identifier must contain follow '@package/module' when trying to mimic"
+                " a global module "
             )
         return v
 
     def __repr__(self):
         return f"Identifier({repr(self)})"
 
 
+def parse_or_raise(v: str):
+    try:
+        return parse(v)
+    except GraphQLError as e:
+        x = repr(e)
+        x += "\n" + v + "\n"
+        for l in e.locations:
+            x += "\n" + print_source_location(e.source, l)
+        raise ValueError("Could not parse to graphql: \n" + x)
+
+
 class SearchQuery(str):
-    
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str) and not isinstance(v, DocumentNode):
             raise TypeError(
                 "Search query must be either a str or a graphql DocumentNode"
             )
         if isinstance(v, str):
-            try:
-                v = parse(v)
-            except Exception as e:
-                raise ValueError("Could not parse to graphql: " + repr(e))
+            v = parse_or_raise(v)
 
         if not v.definitions or len(v.definitions) > 1:
             raise ValueError("Only one definintion allowed")
 
         if not isinstance(v.definitions[0], OperationDefinitionNode):
             raise ValueError("Needs an operation")
 
         definition = v.definitions[0]
         if not definition:
             raise ValueError("Specify an operation")
 
         if not definition.operation == OperationType.QUERY:
             raise ValueError("Needs to be operation")
 
+        assert len(definition.variable_definitions) >= 2, (
+            "At least two arguments should be provided ($search: String, $values:"
+            f" [ID])): Was given: {print_ast(v)}"
+        )
+
+        if (
+            definition.variable_definitions[0].variable.name.value != "search"
+            or definition.variable_definitions[0].type.kind != "named_type"
+        ):
+            raise ValueError(
+                "First parameter of search function should be '$search: String' if you"
+                " provide arguments for your options. This parameter will be filled"
+                f" with userinput: Was given: {print_ast(v)}"
+            )
+
         if (
-            len(definition.variable_definitions) > 0
-            and definition.variable_definitions[0].variable.name.value != "search"
+            definition.variable_definitions[1].variable.name.value != "values"
+            or definition.variable_definitions[0].type.kind != "named_type"
         ):
             raise ValueError(
-                "First parameter of search function should be '$search: String' if you provide arguments for your options. This parameter will be filled with userinput"
+                "Seconrd parameter of search function should be '$values: [ID]' if you"
+                " provide arguments for your options. This parameter will be filled"
+                f" with the default values: Was given: {print_ast(v)}"
             )
 
         wrapped_query = definition.selection_set.selections[0]
 
         options_value = (
             wrapped_query.alias.value
             if wrapped_query.alias
             else wrapped_query.name.value
         )
         if options_value != "options":
-            raise ValueError("First element of query should be 'options'")
+            raise ValueError(
+                "First element of query should be 'options':  Was given:"
+                f" {print_ast(v)}"
+            )
 
         wrapped_selection = wrapped_query.selection_set.selections
         aliases = [
             field.alias.value if field.alias else field.name.value
             for field in wrapped_selection
         ]
-        if not "value" in aliases:
+        if "value" not in aliases:
             raise ValueError(
-                "Searched query needs to contain a 'value' not that corresponds to the selected value"
+                "Searched query needs to contain a 'value' not that corresponds to the"
+                " selected value"
             )
-        if not "label" in aliases:
+        if "label" not in aliases:
             raise ValueError(
-                "Searched query needs to contain a 'label' that corresponds to the displayed value to the user"
+                "Searched query needs to contain a 'label' that corresponds to the"
+                " displayed value to the user"
             )
 
         return print_ast(v)
 
     def __repr__(self):
         return f"SearchQuery({repr(self)})"
```

### Comparing `rekuest-0.1.9/rekuest/structures/annotations.py` & `rekuest-0.2.0/rekuest/structures/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pydantic import BaseModel
 from rekuest.api.schema import AnnotationInput, AnnotationKind, IsPredicateType
 from annotated_types import (
     Gt,
     Ge,
     Le,
     Lt,
     Interval,
```

### Comparing `rekuest-0.1.9/rekuest/structures/errors.py` & `rekuest-0.2.0/rekuest/structures/errors.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.9/rekuest/structures/registry.py` & `rekuest-0.2.0/rekuest/structures/registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,59 @@
 import contextvars
 from enum import Enum
-from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union, TypeVar
+from typing import Any, Awaitable, Callable, Dict, Optional, Type, TypeVar
 
 from rekuest.api.schema import (
     ChoiceInput,
     ReturnWidgetInput,
     WidgetInput,
     AnnotationInput,
+    Scope,
+    PortInput,
 )
 from pydantic import BaseModel, Field
-
+import inspect
+from rekuest.collection.shelve import get_current_shelve
 from .errors import (
     StructureDefinitionError,
     StructureOverwriteError,
     StructureRegistryError,
 )
+from .types import PortBuilder
 
 current_structure_registry = contextvars.ContextVar("current_structure_registry")
 
 
 async def id_shrink(self):
     return self.id
 
 
+async def shelve_ashrink(cls: Type):
+    shelve = get_current_shelve()
+    return await shelve.aput(cls)
+
+
+async def shelve_aexpand(id: str):
+    shelve = get_current_shelve()
+    return await shelve.aget(id)
+
+
+async def shelve_acollect(id: str):
+    shelve = get_current_shelve()
+    return await shelve.adelete(id)
+
+
+async def void_acollect(id: str):
+    return None
+
+
+def build_instance_predicate(cls: Type):
+    return lambda x: isinstance(x, cls)
+
+
 def build_enum_shrink_expand(cls: Type[Enum]):
     async def shrink(s):
         return s._name_
 
     async def expand(v):
         return cls.__members__[v].value
 
@@ -37,160 +64,217 @@
 
 Identifier = str
 """ A unique identifier of this structure on the arkitekt platform"""
 
 
 class StructureRegistry(BaseModel):
     copy_from_default: bool = False
-    allow_overwrites: bool = True
+    allow_overwrites: bool = False
     allow_auto_register: bool = True
 
     identifier_structure_map: Dict[str, Type] = Field(
         default_factory=dict, exclude=True
     )
+    identifier_scope_map: Dict[str, Scope] = Field(default_factory=dict, exclude=True)
     _identifier_expander_map: Dict[str, Callable[[str], Awaitable[Any]]] = {}
     _identifier_shrinker_map: Dict[str, Callable[[Any], Awaitable[str]]] = {}
+    _identifier_collecter_map: Dict[str, Callable[[Any], Awaitable[None]]] = {}
+    _identifier_predicate_map: Dict[str, Callable[[Any], bool]] = {}
+    _identifier_builder_map: Dict[str, PortBuilder] = {}
 
     _structure_convert_default_map: Dict[str, Callable[[Any], str]] = {}
     _structure_identifier_map: Dict[Type, str] = {}
     _structure_default_widget_map: Dict[Type, WidgetInput] = {}
     _structure_default_returnwidget_map: Dict[Type, ReturnWidgetInput] = {}
     _structure_annotation_map: Dict[Type, Type] = {}
 
     _token: contextvars.Token = None
 
     def get_expander_for_identifier(self, key):
         try:
             return self._identifier_expander_map[key]
         except KeyError as e:
-            raise StructureRegistryError(f"{key} is not registered") from e
+            raise StructureRegistryError(f"Expander for {key} is not registered") from e
+
+    def get_collector_for_identifier(self, key):
+        try:
+            return self._identifier_collecter_map[key]
+        except KeyError as e:
+            raise StructureRegistryError(
+                f"Collector for {key} is not registered"
+            ) from e
 
     def get_shrinker_for_identifier(self, key):
         try:
             return self._identifier_shrinker_map[key]
         except KeyError as e:
-            raise StructureRegistryError(f"{key} is not registered") from e
+            raise StructureRegistryError(f"Shrinker for {key} is not registered") from e
 
     def register_expander(self, key, expander):
         self._identifier_expander_map[key] = expander
 
     def get_widget_input(self, cls) -> Optional[WidgetInput]:
         return self._structure_default_widget_map.get(cls, None)
 
     def get_returnwidget_input(self, cls) -> Optional[ReturnWidgetInput]:
         return self._structure_default_returnwidget_map.get(cls, None)
 
+    def get_predicator_for_identifier(
+        self, identifier: str
+    ) -> Optional[Callable[[Any], bool]]:
+        return self._identifier_predicate_map[identifier]
+
     def get_identifier_for_structure(self, cls):
         try:
             return self._structure_identifier_map[cls]
         except KeyError as e:
             if self.allow_auto_register:
                 try:
                     self.register_as_structure(cls)
                     return self._structure_identifier_map[cls]
                 except StructureDefinitionError as e:
                     raise StructureDefinitionError(
-                        f"{cls} was not registered and could not be registered automatically"
+                        f"{cls} was not registered and could not be registered"
+                        " automatically"
                     ) from e
             else:
                 raise StructureRegistryError(
-                    f"{cls} is not registered and allow_auto_register is set to False. Please make sure to register this type beforehand or set allow_auto_register to True"
+                    f"{cls} is not registered and allow_auto_register is set to False."
+                    " Please make sure to register this type beforehand or set"
+                    " allow_auto_register to True"
                 ) from e
 
+    def get_scope_for_identifier(self, identifier: str):
+        return self.identifier_scope_map[identifier]
+
     def get_default_converter_for_structure(self, cls):
         try:
             return self._structure_convert_default_map[cls]
         except KeyError as e:
             if self.allow_auto_register:
                 try:
                     self.register_as_structure(cls)
                     return self._structure_convert_default_map[cls]
                 except StructureDefinitionError as e:
                     raise StructureDefinitionError(
-                        f"{cls} was not registered and not be no default converter could be registered automatically."
+                        f"{cls} was not registered and not be no default converter"
+                        " could be registered automatically."
                     ) from e
             else:
                 raise StructureRegistryError(
-                    f"{cls} is not registered and allow_auto_register is set to False. Please register a 'conver_default' function for this type beforehand or set allow_auto_register to True. Otherwise you cant use this type with a default"
+                    f"{cls} is not registered and allow_auto_register is set to False."
+                    " Please register a 'conver_default' function for this type"
+                    " beforehand or set allow_auto_register to True. Otherwise you"
+                    " cant use this type with a default"
                 ) from e
 
     def register_as_structure(
         self,
         cls: Type,
         identifier: str = None,
-        expand: Callable[
+        scope: Scope = Scope.LOCAL,
+        aexpand: Callable[
             [
                 str,
             ],
             Awaitable[Any],
         ] = None,
-        shrink: Callable[
+        ashrink: Callable[
             [
                 any,
             ],
             Awaitable[str],
         ] = None,
+        acollect: Callable[
+            [
+                str,
+            ],
+            Awaitable[Any],
+        ] = None,
+        predicate: Callable[[Any], bool] = None,
         convert_default: Callable[[Any], str] = None,
-        default_widget: WidgetInput = None,
-        default_returnwidget: ReturnWidgetInput = None,
+        default_widget: Optional[WidgetInput] = None,
+        default_returnwidget: Optional[ReturnWidgetInput] = None,
     ):
-        if issubclass(cls, Enum):
-            identifier = "cls/" + cls.__name__.lower()
-            shrink, expand = build_enum_shrink_expand(cls)
-            convert_default = lambda x: x._name_
-            default_widget = WidgetInput(
-                kind="ChoiceWidget",
-                choices=[
-                    ChoiceInput(label=key, value=key)
-                    for key, value in cls.__members__.items()
-                ],
-            )
+        if inspect.isclass(cls):
+            if issubclass(cls, Enum):
+                identifier = "cls/" + cls.__name__.lower()
+                shrink, expand = build_enum_shrink_expand(cls)
+                ashrink = ashrink or shrink
+                aexpand = aexpand or expand
+                scope = Scope.GLOBAL
+
+                def convert_default(x):
+                    return x._name_
+
+                default_widget = default_widget or WidgetInput(
+                    kind="ChoiceWidget",
+                    choices=[
+                        ChoiceInput(label=key, value=key)
+                        for key, value in cls.__members__.items()
+                    ],
+                )
+                default_returnwidget = default_returnwidget or ReturnWidgetInput(
+                    kind="ChoiceReturnWidget",
+                    choices=[
+                        ChoiceInput(label=key, value=key)
+                        for key, value in cls.__members__.items()
+                    ],
+                )
 
         if convert_default is None:
             if hasattr(cls, "convert_default"):
                 convert_default = cls.convert_default
 
-        if expand is None:
-            if not hasattr(cls, "aexpand"):
+        if aexpand is None:
+            if not hasattr(cls, "aexpand") and scope == Scope.GLOBAL:
                 raise StructureDefinitionError(
-                    f"You need to pass 'aexpand' method or {cls} needs to implement a aexpand method"
+                    f"You need to pass 'expand' method or {cls} needs to implement a"
+                    " aexpand method if it wants to become a GLOBAL structure"
                 )
-            expand = cls.aexpand
+            aexpand = getattr(cls, "aexpand", shelve_aexpand)
 
-        if shrink is None:
-            if not hasattr(cls, "ashrink"):
-                if issubclass(cls, BaseModel):
-                    if "id" in cls.__fields__:
-                        shrink = id_shrink
-                    else:
-                        raise StructureDefinitionError(
-                            f"You need to pass 'ashrink' method or {cls} needs to implement a ashrink method. A BaseModel can be automatically shrinked by providing an id field"
-                        )
-                else:
-                    raise StructureDefinitionError(
-                        f"You need to pass 'ashrink' method or {cls} needs to implement a ashrink method"
-                    )
+        if ashrink is None:
+            if not hasattr(cls, "ashrink") and scope == Scope.GLOBAL:
+                raise StructureDefinitionError(
+                    f"You need to pass 'ashrink' method or {cls} needs to implement a"
+                    " ashrink method if it wants to become a GLOBAL structure"
+                )
+            ashrink = getattr(cls, "ashrink", shelve_ashrink)
+
+        if acollect is None:
+            if scope == Scope.GLOBAL:
+                acollect = void_acollect
             else:
-                shrink = cls.ashrink
+                acollect = getattr(cls, "acollect", shelve_acollect)
+
+        if predicate is None:
+            predicate = build_instance_predicate(cls)
 
         if identifier is None:
             if not hasattr(cls, "get_identifier"):
                 raise StructureDefinitionError(
-                    f"You need to pass 'identifier' or  {cls} needs to implement a get_identifier method"
+                    f"You need to pass 'identifier' or  {cls} needs to implement a"
+                    " get_identifier method"
                 )
             identifier = cls.get_identifier()
 
         if identifier in self.identifier_structure_map and not self.allow_overwrites:
             raise StructureOverwriteError(
-                f"{identifier} is already registered. Previously registered {self.identifier_structure_map[identifier]}"
+                f"{identifier} is already registered. Previously registered"
+                f" {self.identifier_structure_map[identifier]}"
             )
 
-        self._identifier_expander_map[identifier] = expand
-        self._identifier_shrinker_map[identifier] = shrink
+        self._identifier_expander_map[identifier] = aexpand
+        self._identifier_collecter_map[identifier] = acollect
+        self._identifier_shrinker_map[identifier] = ashrink
+        self._identifier_predicate_map[identifier] = predicate
+
         self.identifier_structure_map[identifier] = cls
+        self.identifier_scope_map[identifier] = scope
         self._structure_identifier_map[cls] = identifier
         self._structure_default_widget_map[cls] = default_widget
         self._structure_default_returnwidget_map[cls] = default_returnwidget
         self._structure_convert_default_map[cls] = convert_default
 
     def get_converter_for_annotation(self, annotation):
         try:
@@ -202,15 +286,16 @@
         self,
         annotation: T,
         converter: Callable[[Type[T]], AnnotationInput],
         overwrite=False,
     ):
         if annotation in self._structure_annotation_map and not overwrite:
             raise StructureRegistryError(
-                f"{annotation} is already registered: Specify overwrite=True to overwrite"
+                f"{annotation} is already registered: Specify overwrite=True to"
+                " overwrite"
             )
 
         self._structure_annotation_map[annotation] = converter
 
     async def __aenter__(self):
         current_structure_registry.set(self)
         return self
@@ -224,43 +309,7 @@
 
 
 DEFAULT_STRUCTURE_REGISTRY = None
 
 
 def get_current_structure_registry(allow_default=True):
     return current_structure_registry.get()
-
-
-def register_structure(
-    identifier: str = None,
-    expand: Callable[
-        [
-            str,
-        ],
-        Awaitable[Any],
-    ] = None,
-    shrink: Callable[
-        [
-            any,
-        ],
-        Awaitable[str],
-    ] = None,
-    default_widget: WidgetInput = None,
-    registry: StructureRegistry = None,
-):
-    """A Decorator for registering a structure
-
-    Args:
-        identifier ([type], optional): [description]. Defaults to None.
-        expand ([type], optional): [description]. Defaults to None.
-        shrink ([type], optional): [description]. Defaults to None.
-        default_widget ([type], optional): [description]. Defaults to None.
-    """
-
-    registry = registry or get_current_structure_registry()
-
-    def func(cls):
-
-        registry.register_as_structure(cls, identifier, expand, shrink, default_widget)
-        return cls
-
-    return func
```

### Comparing `rekuest-0.1.9/rekuest/structures/serialization/actor.py` & `rekuest-0.2.0/rekuest/structures/serialization/actor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,101 @@
-from typing import Any, Dict, List, Optional, Tuple
-from rekuest.api.schema import NodeFragment
+from typing import Any, List, Tuple
 import asyncio
 from rekuest.structures.errors import ExpandingError, ShrinkingError
 from rekuest.structures.registry import StructureRegistry
 import asyncio
 from typing import Any, Union
 from rekuest.api.schema import (
-    ArgPortFragment,
+    PortFragment,
     PortKind,
-    ReturnPortFragment,
     ChildPortFragment,
     DefinitionInput,
     DefinitionFragment,
 )
 from rekuest.structures.errors import (
     PortShrinkingError,
     StructureShrinkingError,
-    PortExpandingError,
     StructureExpandingError,
 )
 from rekuest.definition.validate import auto_validate
+from .predication import predicate_port
 
 
 async def aexpand_arg(
-    port: Union[ArgPortFragment, ChildPortFragment],
+    port: Union[PortFragment, ChildPortFragment],
     value: Union[str, int, float, dict, list],
     structure_registry,
 ) -> Any:
     """Expand a value through a port
 
     Args:
         port (ArgPortFragment): Port to expand to
         value (Any): Value to expand
     Returns:
         Any: Expanded value
 
     """
     if value is None:
+        value = port.default
+
+    if value is None:
         if port.nullable:
             return None
         else:
             raise ExpandingError(
-                f"{port.key} is not nullable (optional) but your provided None"
+                f"{port.key} is not nullable (optional) but received None"
             )
 
     if not isinstance(value, (str, int, float, dict, list)):
         raise ExpandingError(
-            f"Can't expand {value} of type {type(value)} to {port.kind}. We only accept strings, ints and floats (json serializable)"
+            f"Can't expand {value} of type {type(value)} to {port.kind}. We only accept"
+            " strings, ints and floats (json serializable) and null values"
         ) from None
 
     if port.kind == PortKind.DICT:
         if not isinstance(value, dict):
             raise ExpandingError(
-                f"Can't expand {value} of type {type(value)} to {port.kind}. We only accept dicts"
+                f"Can't expand {value} of type {type(value)} to {port.kind}. We only"
+                " accept dicts"
             ) from None
 
         return {
             key: await aexpand_arg(port.child, value, structure_registry)
             for key, value in value.items()
         }
 
+    if port.kind == PortKind.UNION:
+        if not isinstance(value, dict):
+            raise ExpandingError(
+                f"Can't expand {value} of type {type(value)} to {port.kind}. We only"
+                " accept dicts in unions"
+            )
+        assert "use" in value, "No use in vaalue"
+        index = value["use"]
+        true_value = value["value"]
+        return await aexpand_arg(
+            port.variants[index], true_value, structure_registry=structure_registry
+        )
+
     if port.kind == PortKind.LIST:
         if not isinstance(value, list):
             raise ExpandingError(
-                f"Can't expand {value} of type {type(value)} to {port.kind}. We only accept lists"
+                f"Can't expand {value} of type {type(value)} to {port.kind}. Only"
+                " accept lists"
             ) from None
 
         return await asyncio.gather(
             *[aexpand_arg(port.child, item, structure_registry) for item in value]
         )
 
     if port.kind == PortKind.INT:
-        return int(value) if value is not None else int(port.default)
+        return int(value)
 
     if port.kind == PortKind.FLOAT:
-        return float(value) if value is not None else float(port.default)
+        return float(value)
 
     if port.kind == PortKind.STRUCTURE:
         try:
             expander = structure_registry.get_expander_for_identifier(port.identifier)
         except KeyError:
             raise StructureExpandingError(
                 f"Couldn't find expander for {port.identifier}"
@@ -86,29 +103,27 @@
 
         try:
             expand = await expander(value)
             return expand
         except Exception as e:
             raise StructureExpandingError(
                 f"Error expanding {repr(value)} with Structure {port.identifier}"
-            ) from None
+            ) from e
 
     if port.kind == PortKind.BOOL:
-
-        return bool(value) if value is not None else bool(port.default)
+        return bool(value)
 
     if port.kind == PortKind.STRING:
-
-        return str(value) if value is not None else str(port.default)
+        return str(value)
 
     raise NotImplementedError("Should be implemented by subclass")
 
 
 async def expand_inputs(
-    definition: DefinitionInput | DefinitionFragment,
+    definition: Union[DefinitionInput, DefinitionFragment],
     args: List[Union[str, int, float, dict, list]],
     structure_registry: StructureRegistry,
     skip_expanding: bool = False,
 ):
     """Expand
 
     Args:
@@ -135,47 +150,59 @@
             )
 
             expandend_params = {
                 port.key: val for port, val in zip(node.args, expanded_args)
             }
 
         except Exception as e:
-            raise ExpandingError(f"Couldn't expand Arguments {args} ") from e
+            raise ExpandingError(f"Couldn't expand Arguments {args}") from e
     else:
-        expandend_params = {port.key: arg for port, arg in zip(node.args, args)}
+        expandend_params = {
+            port.key: arg for port, arg in zip(node.args, args) if arg is not None
+        }
 
     return expandend_params
 
 
 async def ashrink_return(
-    port: Union[ReturnPortFragment, ChildPortFragment],
+    port: Union[PortFragment, ChildPortFragment],
     value: Any,
     structure_registry=None,
 ) -> Union[str, int, float, dict, list, None]:
     """Expand a value through a port
 
     Args:
         port (ArgPortFragment): Port to expand to
         value (Any): Value to expand
     Returns:
         Any: Expanded value
 
     """
     try:
-
         if value is None:
             if port.nullable:
                 return None
             else:
                 raise ValueError(
                     f"{port} is not nullable (optional) but your provided None"
                 )
 
-        if port.kind == PortKind.DICT:
+        if port.kind == PortKind.UNION:
+            for index, x in enumerate(port.variants):
+                if predicate_port(x, value, structure_registry):
+                    return {
+                        "use": index,
+                        "value": await ashrink_return(x, value, structure_registry),
+                    }
 
+            raise ShrinkingError(
+                f"Port is union butn none of the predicated for this port held true {port.variants}"
+            )
+
+        if port.kind == PortKind.DICT:
             return {
                 key: await ashrink_return(port.child, value, structure_registry)
                 for key, value in value.items()
             }
 
         if port.kind == PortKind.LIST:
             return await asyncio.gather(
@@ -186,14 +213,17 @@
                     for item in value
                 ]
             )
 
         if port.kind == PortKind.INT:
             return int(value) if value is not None else None
 
+        if port.kind == PortKind.FLOAT:
+            return float(value) if value is not None else None
+
         if port.kind == PortKind.STRUCTURE:
             # We always convert structures returns to strings
             try:
                 shrinker = structure_registry.get_shrinker_for_identifier(
                     port.identifier
                 )
             except KeyError:
@@ -202,15 +232,15 @@
                 ) from None
             try:
                 shrink = await shrinker(value)
                 return str(shrink)
             except Exception as e:
                 raise StructureShrinkingError(
                     f"Error shrinking {repr(value)} with Structure {port.identifier}"
-                ) from None
+                ) from e
 
         if port.kind == PortKind.BOOL:
             return bool(value) if value is not None else None
 
         if port.kind == PortKind.STRING:
             return str(value) if value is not None else None
 
@@ -219,33 +249,35 @@
     except Exception as e:
         raise PortShrinkingError(
             f"Couldn't shrink value {value} with port {port}"
         ) from e
 
 
 async def shrink_outputs(
-    definition: DefinitionInput | DefinitionFragment,
+    definition: Union[DefinitionInput, DefinitionFragment],
     returns: List[Any],
     structure_registry: StructureRegistry,
     skip_shrinking: bool = False,
 ) -> Tuple[Union[str, int, float, dict, list, None]]:
-
     node = (
         auto_validate(definition)
         if isinstance(definition, DefinitionInput)
         else definition
     )
 
     if returns is None:
-        returns = ()
-    if not isinstance(returns, tuple):
+        returns = []
+    elif not isinstance(returns, tuple):
         returns = [returns]
+
     assert len(node.returns) == len(
         returns
-    ), "Missmatch in Return Length"  # We are dealing with a single output, convert it to a proper port like structure
+    ), (  # We are dealing with a single output, convert it to a proper port like structure
+        f"Mismatch in Return Length: expected {len(node.returns)} got {len(returns)}"
+    )
 
     if not skip_shrinking:
         shrinked_returns_future = [
             ashrink_return(port, val, structure_registry)
             for port, val in zip(node.returns, returns)
         ]
         try:
```

### Comparing `rekuest-0.1.9/rekuest/structures/serialization/postman.py` & `rekuest-0.2.0/rekuest/structures/serialization/postman.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 from rekuest.api.schema import NodeFragment
 import asyncio
 from rekuest.structures.errors import ExpandingError, ShrinkingError
 from rekuest.structures.registry import StructureRegistry
-import asyncio
-from typing import Any, Union
 from rekuest.api.schema import (
-    ArgPortFragment,
+    PortFragment,
     PortKind,
-    ReturnPortFragment,
+    DefinitionInput,
+    DefinitionFragment,
     ChildPortFragment,
 )
 from rekuest.structures.errors import (
     PortShrinkingError,
     StructureShrinkingError,
     PortExpandingError,
     StructureExpandingError,
 )
+from .predication import predicate_port
 
 
 async def ashrink_arg(
-    port: Union[ArgPortFragment, ChildPortFragment], value: Any, structure_registry=None
+    port: Union[PortFragment, ChildPortFragment], value: Any, structure_registry=None
 ) -> Any:
     """Expand a value through a port
 
     Args:
         port (ArgPortFragment): Port to expand to
         value (Any): Value to expand
     Returns:
         Any: Expanded value
 
     """
     try:
-
         if value is None:
             if port.nullable:
                 return None
             else:
                 raise ValueError(
                     "{port} is not nullable (optional) but your provided None"
                 )
 
         if port.kind == PortKind.DICT:
-
             return {
                 key: await ashrink_arg(port.child, value, structure_registry)
                 for key, value in value.items()
             }
 
         if port.kind == PortKind.LIST:
             return await asyncio.gather(
@@ -55,28 +53,40 @@
                     for item in value
                 ]
             )
 
         if port.kind == PortKind.INT:
             return int(value) if value is not None else None
 
+        if port.kind == PortKind.UNION:
+            for index, x in enumerate(port.variants):
+                if predicate_port(x, value, structure_registry):
+                    return {
+                        "use": index,
+                        "value": await ashrink_arg(x, value, structure_registry),
+                    }
+
+            raise ShrinkingError(
+                f"Port is union butn none of the predicated for this port held true {port.variants}"
+            )
+
         if port.kind == PortKind.STRUCTURE:
             # We always convert structures returns to strings
             try:
                 shrinker = structure_registry.get_shrinker_for_identifier(
                     port.identifier
                 )
             except KeyError:
                 raise StructureShrinkingError(
                     f"Couldn't find shrinker for {port.identifier}"
                 ) from None
             try:
                 shrink = await shrinker(value)
                 return str(shrink)
-            except Exception as e:
+            except Exception:
                 raise StructureShrinkingError(
                     f"Error shrinking {repr(value)} with Structure {port.identifier}"
                 ) from None
 
         if port.kind == PortKind.BOOL:
             return bool(value) if value is not None else None
 
@@ -149,30 +159,29 @@
                 asyncio.create_task(ashrink_arg(port, arg, structure_registry))
             )
 
         try:
             shrinked_args = await asyncio.gather(*shrinked_args_futures)
 
         except Exception as e:
-
             for future in shrinked_args_futures:
                 future.cancel()
 
             await asyncio.gather(*shrinked_args_futures, return_exceptions=True)
 
-            raise ShrinkingError(f"Couldn't shrink Arguments") from e
+            raise ShrinkingError("Couldn't shrink Arguments") from e
 
     else:
         shrinked_args = args_list
 
     return tuple(shrinked_args)
 
 
 async def aexpand_return(
-    port: Union[ReturnPortFragment, ChildPortFragment],
+    port: Union[PortFragment, ChildPortFragment],
     value: Any,
     structure_registry=None,
 ) -> Any:
     """Expand a value through a port
 
     Args:
         port (ArgPortFragment): Port to expand to
@@ -199,14 +208,23 @@
         return await asyncio.gather(
             *[
                 aexpand_return(port.child, item, structure_registry=structure_registry)
                 for item in value
             ]
         )
 
+    if port.kind == PortKind.UNION:
+        assert isinstance(value, dict), "Union value needs to be a dict"
+        assert "use" in value, "No use in vaalue"
+        index = value["use"]
+        true_value = value["value"]
+        return await aexpand_return(
+            port.variants[index], true_value, structure_registry=structure_registry
+        )
+
     if port.kind == PortKind.INT:
         return int(value)
 
     if port.kind == PortKind.FLOAT:
         return float(value)
 
     if port.kind == PortKind.STRUCTURE:
@@ -219,27 +237,24 @@
             expander = structure_registry.get_expander_for_identifier(port.identifier)
         except KeyError:
             raise StructureExpandingError(
                 f"Couldn't find expander for {port.identifier}"
             ) from None
 
         try:
-
             return await expander(value)
-        except Exception as e:
+        except Exception:
             raise StructureExpandingError(
                 f"Error expanding {repr(value)} with Structure {port.identifier}"
             ) from None
 
     if port.kind == PortKind.BOOL:
-
         return bool(value)
 
     if port.kind == PortKind.STRING:
-
         return str(value)
 
     raise NotImplementedError("Should be implemented by subclass")
 
 
 async def expand_outputs(
     node: NodeFragment,
@@ -261,37 +276,104 @@
 
     Returns:
         List[Any]: The Expanded Returns
     """
     assert returns is not None, "Returns can't be empty"
     if len(node.returns) != len(returns):
         raise ExpandingError(
-            f"Missmatch in Return Length. Node requires {len(node.returns)} returns, but got {len(returns)}"
+            f"Missmatch in Return Length. Node requires {len(node.returns)} returns,"
+            f" but got {len(returns)}"
         )
     if len(returns) == 0:
         return None
 
     if not skip_expanding:
-
         expanded_returns_futures = [
             asyncio.create_task(aexpand_return(port, value, structure_registry))
             for port, value in zip(node.returns, returns)
         ]
 
         try:
-
             expanded_returns = await asyncio.gather(*expanded_returns_futures)
 
         except Exception as e:
-
             for future in expanded_returns_futures:
                 future.cancel()
 
             await asyncio.gather(*expanded_returns_futures, return_exceptions=True)
 
-            raise ExpandingError(f"Couldn't expand Returns") from e
+            raise ExpandingError("Couldn't expand Returns") from e
 
     else:
-
         expanded_returns = returns
 
     return tuple(expanded_returns)
+
+
+def serialize_inputs(
+    definition: Union[DefinitionFragment, DefinitionInput],
+    kwargs: Dict[str, Any],
+) -> Tuple[Any]:
+    """Shrinks args and kwargs
+
+    Shrinks the inputs according to the Node Definition
+
+    Args:
+        node (Node): The Node
+
+    Raises:
+        ShrinkingError: If args are not Shrinkable
+        ShrinkingError: If kwargs are not Shrinkable
+
+    Returns:
+        Tuple[List[Any], Dict[str, Any]]: Parsed Args as a List, Parsed Kwargs as a dict
+    """
+
+    args_list = []
+
+    # Extract to Argslist
+
+    for port in definition.args:
+        value = kwargs.pop(port.key, None)
+        if value is None and not port.nullable:
+            raise ShrinkingError(
+                f"Couldn't find value for nonnunllable port {port.key}"
+            )
+        args_list.append(value)
+
+    shrinked_args = args_list
+
+    return tuple(shrinked_args)
+
+
+def deserialize_outputs(
+    definition: Union[DefinitionFragment, DefinitionInput],
+    returns: List[Any],
+) -> Dict[str, Any]:
+    """Expands Returns
+
+    Expands the Returns according to the Node definition
+
+
+    Args:
+        node (Node): Node definition
+        returns (List[any]): The returns
+
+    Raises:
+        ExpandingError: if they are not expandable
+
+    Returns:
+        Dcit[str, Any]: The Expanded Returns
+    """
+    assert returns is not None, "Returns can't be empty"
+    if len(definition.returns) != len(returns):
+        raise ExpandingError(
+            f"Missmatch in Return Length. Node requires {len(definition.returns)} returns,"
+            f" but got {len(returns)}"
+        )
+
+    values = {}
+
+    for port, value in zip(definition.returns, returns):
+        values[port.key] = value
+
+    return values
```

### Comparing `rekuest-0.1.9/rekuest/structures/serialization/utils.py` & `rekuest-0.2.0/rekuest/structures/serialization/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,21 @@
             return None
 
         return await structure_registry.get_expander_for_identifier(port.identifier)(
             value
         )
 
     if port.kind == PortKind.BOOL:
-        if value == None:
+        if value is None:
             value = port.default
 
         return bool(value) if value is not None else None
 
     if port.kind == PortKind.STRING:
-        if value == None:
+        if value is None:
             value = port.default
 
         return str(value) if value is not None else None
 
     raise NotImplementedError("Should be implemented by subclass")
 
 
@@ -67,25 +67,23 @@
         port (ArgPortFragment): Port to expand to
         value (Any): Value to expand
     Returns:
         Any: Expanded value
 
     """
     try:
-
         if value is None:
             if port.nullable:
                 return None
             else:
                 raise ValueError(
                     "{port} is not nullable (optional) but your provided None"
                 )
 
         if port.kind == PortKind.DICT:
-
             return {
                 key: await ashrink(port.child, value, structure_registry)
                 for key, value in value.items()
             }
 
         if port.kind == PortKind.LIST:
             return await asyncio.gather(
@@ -107,15 +105,15 @@
             except KeyError:
                 raise StructureShrinkingError(
                     f"Couldn't find shrinker for {port.identifier}"
                 ) from None
             try:
                 shrink = await shrinker(value)
                 return str(shrink)
-            except Exception as e:
+            except Exception:
                 raise StructureShrinkingError(
                     f"Error shrinking {repr(value)} with Structure {port.identifier}"
                 ) from None
 
         if port.kind == PortKind.BOOL:
             return bool(value) if value is not None else None
```

### Comparing `rekuest-0.1.9/rekuest/traits/node.py` & `rekuest-0.2.0/rekuest/traits/node.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def __rich_repr__(self):
         yield self.name
         yield "args", self.args
         yield "kwargs", self.kwargs
         yield "returns", self.returns
 
     def __rich__(self):
-
         from rich.table import Table
 
         my_table = Table(title=f"Node: {self.name}", show_header=False)
 
         my_table.add_row("ID", str(self.id))
         my_table.add_row("Package", self.package)
         my_table.add_row("Interface", self.interface)
@@ -34,11 +33,12 @@
         return my_table
 
     def _repr_html_(self):
         return f"""
         <div class="container" style="border:1px solid #00000f;padding: 4px;">
             <div class="item item-1 font-xl">{self.name}</div>
             <div class="item item-2">{self.package}/{self.interface}</div>
-            <div class="item item-3">Args: {" ".join([port._repr_html_list() for port in self.args])}</div>
+            <div class="item item-3">Args:{" ".join([port._repr_html_list() for port in self.args])}
+            </div>
             <div class="item item-3">Kwargs: {" ".join([port.key for port in self.kwargs])}</div>
             <div class="item item-3">Returns: {" ".join([port.key for port in self.returns])}</div>
         </div>"""
```

### Comparing `rekuest-0.1.9/rekuest/traits/ports.py` & `rekuest-0.2.0/rekuest/traits/ports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from abc import abstractmethod
-import asyncio
-from typing import Dict, Optional, Callable
+from typing import Callable
 from pydantic import BaseModel, root_validator
-from graphql import parse
 import uuid
 import random
 
 
 class PortTrait(BaseModel):
     """
     Class for validating port input
@@ -22,15 +19,16 @@
 
         if kind is None:
             raise ValueError("kind is required")
 
         if kind == PortKind.STRUCTURE:
             if values.get("identifier") is None:
                 raise ValueError(
-                    "When specifying a structure you need to provide an arkitekt identifier"
+                    "When specifying a structure you need to provide an arkitekt"
+                    " identifier got:" + str(values)
                 )
 
         if kind == PortKind.LIST:
             if values.get("child") is None:
                 raise ValueError(
                     "When specifying a list you need to provide a wrapped 'child' port"
                 )
@@ -85,30 +83,31 @@
 
         kind = values.get("kind")
 
         if kind is None:
             raise ValueError("kind is required")
 
         if kind == WidgetKind.SearchWidget:
-
             if values.get("query") is None:
                 raise ValueError(
-                    "When specifying a SearchWidget you need to provide an query parameter"
+                    "When specifying a SearchWidget you need to provide an query"
+                    " parameter"
                 )
 
         if kind == WidgetKind.SliderWidget:
-
             if values.get("min") is None or values.get("max") is None:
                 raise ValueError(
-                    "When specifying a Slider you need to provide an 'max and 'min' parameter"
+                    "When specifying a Slider you need to provide an 'max and 'min'"
+                    f" parameter {values}"
                 )
 
             if values.get("min") > values.get("max"):
                 raise ValueError(
-                    "When specifying a Slider you need to provide an 'max' greater than 'min'"
+                    "When specifying a Slider you need to provide an 'max' greater than"
+                    " 'min'"
                 )
 
         return values
 
 
 class ReturnWidgetInputTrait(BaseModel):
     """
@@ -123,18 +122,18 @@
 
         kind = values.get("kind")
 
         if kind is None:
             raise ValueError("kind is required")
 
         if kind == ReturnWidgetKind.CustomReturnWidget:
-
             if values.get("hook") is None:
                 raise ValueError(
-                    "When specifying a CustomReturnWidget you need to provide a 'hook' parameter, corresponding to the desired reigstered hook"
+                    "When specifying a CustomReturnWidget you need to provide a 'hook'"
+                    " parameter, corresponding to the desired reigstered hook"
                 )
 
         return values
 
 
 class AnnotationInputTrait(BaseModel):
     """
@@ -170,11 +169,12 @@
                 raise ValueError("hook is required when using CustomAnnotation")
 
         if kind == AnnotationKind.AttributePredicate:
             if values.get("attribute") is None:
                 raise ValueError("atrribute is required when using AttributePredicate")
             if values.get("annotations") is None:
                 raise ValueError(
-                    "annotations on the predicate is required when using AttributePredicate"
+                    "annotations on the predicate is required when using"
+                    " AttributePredicate"
                 )
 
         return values
```

### Comparing `rekuest-0.1.9/PKG-INFO` & `rekuest-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: rekuest
-Version: 0.1.9
+Version: 0.2.0
 Summary: rpc and node backbone
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: annotated-types (>=0.4.0,<0.5.0)
 Requires-Dist: docstring-parser (>=0.11)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: koil (>=0.2.10)
 Requires-Dist: pydantic (>=1.9.0)
-Requires-Dist: pytest-aiohttp (>=1.0.4,<2.0.0)
-Requires-Dist: pytest-asyncio (>=0.20.2,<0.21.0)
-Requires-Dist: rath (>=0.3.4)
+Requires-Dist: rath (>=0.4.0)
 Requires-Dist: websockets (>=10.0,<11.0)
```

