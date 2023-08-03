# Comparing `tmp/tlslite-ng-0.8.0a45.tar.gz` & `tmp/tlslite-ng-0.8.0a46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlslite-ng-0.8.0a45.tar", last modified: Tue Aug  1 15:43:28 2023, max compression
+gzip compressed data, was "tlslite-ng-0.8.0a46.tar", last modified: Thu Aug  3 17:25:16 2023, max compression
```

## Comparing `tlslite-ng-0.8.0a45.tar` & `tlslite-ng-0.8.0a46.tar`

### file list

```diff
@@ -1,503 +1,503 @@
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       34 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.checkignore
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      715 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/.codeclimate.yml
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.142925 tlslite-ng-0.8.0a45/.github/
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.148925 tlslite-ng-0.8.0a45/.github/workflows/
--rw-r--r--   0 hkario   (20970) hkario   (20970)    23071 2023-07-11 11:45:08.000000 tlslite-ng-0.8.0a45/.github/workflows/ci.yml
--rw-r--r--   0 hkario   (20970) hkario   (20970)      128 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/.gitignore
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.landscape.yaml
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       28 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.pep257
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6804 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/.travis.yml
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5749 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/CONTRIBUTING.md
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    27882 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/LICENSE
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      131 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/MANIFEST.in
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4231 2021-07-27 19:18:05.000000 tlslite-ng-0.8.0a45/Makefile
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/PKG-INFO
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2099 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/README
--rw-r--r--   0 hkario   (20970) hkario   (20970)    39629 2023-08-01 15:39:53.000000 tlslite-ng-0.8.0a45/README.md
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2199 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/SECURITY.md
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-2.6.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      149 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-2.7.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-3.3.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      140 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-3.4.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       79 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.155925 tlslite-ng-0.8.0a45/docs/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7622 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/Makefile
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.142925 tlslite-ng-0.8.0a45/docs/_build/
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.164925 tlslite-ng-0.8.0a45/docs/_build/html/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      230 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/.buildinfo
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.171925 tlslite-ng-0.8.0a45/docs/_build/html/_sources/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.api.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.basedb.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.bufferedsocket.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.checker.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.constants.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.defragmenter.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.dh.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.errors.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.extensions.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakehashes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakehelpers.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakesettings.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.asyncstatemachine.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.clienthelper.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.httptlsconnection.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.imap4_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.pop3_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.smtp_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.tlsasyncdispatchermixin.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.tlssocketservermixin.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.xmlrpcserver.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.xmlrpctransport.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.keyexchange.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.mathtls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.messages.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.messagesocket.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.recordlayer.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.session.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.sessioncache.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.tlsconnection.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.tlsrecordlayer.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.asn1parser.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.chacha.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.chacha20_poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.cipherfactory.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.codec.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.compat.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.constanttime.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.cryptomath.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.datefuncs.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.deprecations.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.dns_utils.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.ecc.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.ecdsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.keyfactory.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.lists.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pem.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_chacha20_poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rijndael.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tackwrapper.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tlshashlib.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.x25519.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.verifierdb.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.x509.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.x509certchain.rst.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.172925 tlslite-ng-0.8.0a45/docs/_build/html/_static/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4418 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15180 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.172925 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2922 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)   128848 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8171 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/doctools.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)      429 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)      286 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/file.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)   288580 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    89501 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.173925 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      934 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5023 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4758 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/language_data.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/minus.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/plus.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4846 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/pygments.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)    17088 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    68420 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19530 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)   252791 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/genindex.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4704 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/index.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7955 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/modules.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11369 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/objects.inv
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21834 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/py-modindex.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3593 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/search.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   161631 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/searchindex.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7635 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.api.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14507 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.basedb.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15038 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.bufferedsocket.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12591 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.checker.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   278477 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.constants.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12414 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.defragmenter.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     9820 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.dh.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    40595 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.errors.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   164652 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.extensions.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13049 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehashes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14256 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehelpers.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    33544 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakesettings.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19608 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15981 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.asyncstatemachine.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13925 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.clienthelper.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6874 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15108 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.httptlsconnection.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14811 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.imap4_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12135 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.pop3_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11674 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.smtp_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    20642 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12512 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlssocketservermixin.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11939 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpcserver.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15905 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpctransport.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    58370 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.keyexchange.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    67608 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.mathtls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   143539 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messages.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18129 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messagesocket.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    35655 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.recordlayer.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    20952 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.session.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11817 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.sessioncache.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    47436 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsconnection.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    43739 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsrecordlayer.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7786 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8459 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13626 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.asn1parser.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12725 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10067 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha20_poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18141 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cipherfactory.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    33216 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.codec.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16967 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.compat.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18018 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.constanttime.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    34260 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cryptomath.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10078 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.datefuncs.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14255 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.deprecations.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6466 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.dns_utils.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7761 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecc.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21776 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecdsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10584 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19234 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.keyfactory.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     9265 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.lists.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16689 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    17482 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11632 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14357 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pem.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8842 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10515 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7817 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10063 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14657 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10746 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8560 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5897 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6017 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10047 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14650 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7538 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11634 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rijndael.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    38486 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5238 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tackwrapper.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6794 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tlshashlib.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7979 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.x25519.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15655 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.verifierdb.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14761 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15974 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509certchain.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10006 2023-08-01 15:39:03.000000 tlslite-ng-0.8.0a45/docs/conf.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/index.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7740 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/make.bat
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/modules.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.api.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.basedb.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.bufferedsocket.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.checker.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.constants.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.defragmenter.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.dh.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.errors.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.extensions.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakehashes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakehelpers.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakesettings.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.asyncstatemachine.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.clienthelper.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.httptlsconnection.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.imap4_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.pop3_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.smtp_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.tlsasyncdispatchermixin.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.tlssocketservermixin.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.xmlrpcserver.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.xmlrpctransport.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.keyexchange.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.mathtls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.messages.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.messagesocket.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.recordlayer.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.session.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.sessioncache.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.tlsconnection.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.tlsrecordlayer.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.asn1parser.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.chacha.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.chacha20_poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.cipherfactory.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.codec.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.compat.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.constanttime.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.cryptomath.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.datefuncs.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.deprecations.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.dns_utils.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.ecc.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.ecdsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.keyfactory.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.lists.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pem.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_chacha20_poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rijndael.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tackwrapper.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tlshashlib.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.x25519.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.verifierdb.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.x509.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.x509certchain.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10645 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/pylintrc
--rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/requirements.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.173925 tlslite-ng-0.8.0a45/scripts/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1903 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/scripts/speed.py
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)    25679 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/scripts/tls.py
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)     3774 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/scripts/tlsdb.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)       38 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/setup.cfg
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)     1931 2023-08-01 15:40:02.000000 tlslite-ng-0.8.0a45/setup.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.185925 tlslite-ng-0.8.0a45/tests/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      124 2015-10-14 14:17:40.000000 tlslite-ng-0.8.0a45/tests/.coverage
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK1.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK2.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK_Key1.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK_Key2.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      650 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/TACKs.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/TACKunrelated.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/clientECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/clientECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      485 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/clientEd25519Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/clientEd25519Key.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      924 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/clientX509Cert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      891 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/clientX509Key.pem
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)      327 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/httpsclient.py
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)      113 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/httpsserver.sh
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      152 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/index.html
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      292 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      757 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      361 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6628 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverDSACert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverDSAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      554 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2261 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECDSANonCACert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECDSANonCAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      489 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd25519Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd25519Key.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      591 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd448Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      156 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd448Key.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      660 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP384ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      306 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP384ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      761 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP521ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      384 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP521ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverRSANonCACert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1675 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverRSANonCAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1700 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1229 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSSigCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSSigKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1094 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/serverX509Cert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/serverX509Key.pem
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)   114602 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tests/tlstest.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    24576 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/verifierDB
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.188925 tlslite-ng-0.8.0a45/tlslite/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      878 2021-08-06 12:04:22.000000 tlslite-ng-0.8.0a45/tlslite/__init__.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1400 2023-08-01 15:39:10.000000 tlslite-ng-0.8.0a45/tlslite/api.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4092 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/basedb.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2836 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/bufferedsocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2725 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/checker.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    66261 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/constants.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4430 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/defragmenter.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      914 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/dh.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6838 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/errors.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    68800 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/extensions.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4137 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/handshakehashes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6725 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/handshakehelpers.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    32163 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/handshakesettings.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.189925 tlslite-ng-0.8.0a45/tlslite/integration/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      396 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/integration/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7202 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a45/tlslite/integration/asyncstatemachine.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/clienthelper.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4514 2018-07-30 10:15:07.000000 tlslite-ng-0.8.0a45/tlslite/integration/httptlsconnection.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3680 2021-01-14 12:41:41.000000 tlslite-ng-0.8.0a45/tlslite/integration/imap4_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3199 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/pop3_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3026 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/smtp_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4964 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/tlsasyncdispatchermixin.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2320 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/tlssocketservermixin.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1909 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/xmlrpcserver.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5332 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/xmlrpctransport.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    43331 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/keyexchange.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    45528 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/mathtls.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    78203 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/messages.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6250 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/messagesocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5933 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/ocsp.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    51706 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/recordlayer.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6906 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/session.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3552 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/sessioncache.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3545 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/signed.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   212380 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/tlsconnection.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    60589 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/tlsrecordlayer.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.194925 tlslite-ng-0.8.0a45/tlslite/utils/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      837 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1222 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4966 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6866 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3802 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/asn1parser.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4821 2017-02-17 16:14:00.000000 tlslite-ng-0.8.0a45/tlslite/utils/chacha.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3123 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/chacha20_poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5957 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/cipherfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    15543 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/codec.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7229 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/compat.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6399 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/constanttime.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12585 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/cryptomath.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2278 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/datefuncs.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     8742 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/deprecations.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1468 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/dns_utils.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3144 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/dsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/ecc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5590 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/ecdsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4766 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/eddsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      483 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/format_output.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10460 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/keyfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1549 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/lists.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4539 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      733 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      709 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7156 2023-07-11 11:45:08.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1801 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/pem.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1504 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      840 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      446 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      764 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rc4.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2644 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      872 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      271 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      268 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      316 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_chacha20_poly1305.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3777 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_dsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3388 2023-07-10 15:01:18.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_ecdsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2101 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_eddsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11034 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_key.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1073 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4691 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    16932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      561 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/tlslite/utils/rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    53143 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/rijndael.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    26348 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      334 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tlslite/utils/tackwrapper.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1024 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/tlslite/utils/tlshashlib.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3079 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/tlshmac.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      870 2018-02-01 13:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3255 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/x25519.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3702 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/verifierdb.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10386 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/x509.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3323 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/x509certchain.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.194925 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/PKG-INFO
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18045 2023-08-01 15:43:28.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/SOURCES.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)        1 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/dependency_links.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/requires.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)        8 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/top_level.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/unit_tests/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)        0 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/unit_tests/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3336 2018-06-29 15:54:59.000000 tlslite-ng-0.8.0a45/unit_tests/mocksock.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    18932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tls1_3_vectors.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4414 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_bufferedsocket.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12726 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_constants.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6979 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_defragmenter.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2245 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_dh.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    95334 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_extensions.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3383 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehashes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    17133 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehelpers.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15363 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakesettings.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   126491 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_keyexchange.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     9991 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_mathtls.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   150116 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messages.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    12586 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messagesocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    25676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_ocsp.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)   117035 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_recordlayer.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1834 2016-04-14 13:26:36.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_session.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1275 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_sessioncache.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2611 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_signed.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19118 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsconnection.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    36862 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsrecordlayer.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2931 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aes_split.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10191 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aescbc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    22930 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10558 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesctr.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    14665 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2143 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_asn1.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    15890 2016-01-07 16:34:17.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5662 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha20_poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    11423 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_codec.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      789 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_compat.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16432 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_constanttime.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    26699 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3442 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    16100 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_deprecations.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1286 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_dns_utils.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     8381 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2228 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecdsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    13810 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_keyfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1694 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_lists.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7573 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_poly1305.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21266 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_dsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3998 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_ecdsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7738 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_key.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6754 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rijndael.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   170557 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      765 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tlshashlib.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    20642 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3178 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes_split.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    14421 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_x25519.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6997 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_x509.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.701641 tlslite-ng-0.8.0a46/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       34 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/.checkignore
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      715 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/.codeclimate.yml
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.631640 tlslite-ng-0.8.0a46/.github/
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.636640 tlslite-ng-0.8.0a46/.github/workflows/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    23796 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/.github/workflows/ci.yml
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      128 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/.gitignore
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/.landscape.yaml
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       28 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/.pep257
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6804 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/.travis.yml
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5749 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/CONTRIBUTING.md
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    27882 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a46/LICENSE
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      131 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/MANIFEST.in
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4231 2021-07-27 19:18:05.000000 tlslite-ng-0.8.0a46/Makefile
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3508 2023-08-03 17:25:16.701641 tlslite-ng-0.8.0a46/PKG-INFO
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2117 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/README
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    39778 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/README.md
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2199 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/SECURITY.md
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/build-requirements-2.6.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      149 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/build-requirements-2.7.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/build-requirements-3.3.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      140 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/build-requirements-3.4.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       79 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/build-requirements.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.644640 tlslite-ng-0.8.0a46/docs/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7622 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/Makefile
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.631640 tlslite-ng-0.8.0a46/docs/_build/
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.654641 tlslite-ng-0.8.0a46/docs/_build/html/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      230 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/.buildinfo
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.661641 tlslite-ng-0.8.0a46/docs/_build/html/_sources/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.api.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.basedb.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.bufferedsocket.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.checker.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.constants.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.defragmenter.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.dh.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.errors.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.extensions.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.handshakehashes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.handshakehelpers.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.handshakesettings.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.asyncstatemachine.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.clienthelper.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.httptlsconnection.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.imap4_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.pop3_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.smtp_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.tlsasyncdispatchermixin.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.tlssocketservermixin.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.xmlrpcserver.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.xmlrpctransport.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.keyexchange.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.mathtls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.messages.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.messagesocket.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.recordlayer.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.session.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.sessioncache.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.tlsconnection.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.tlsrecordlayer.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.asn1parser.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.chacha.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.chacha20_poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.cipherfactory.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.codec.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.compat.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.constanttime.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.cryptomath.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.datefuncs.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.deprecations.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.dns_utils.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.ecc.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.ecdsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.keyfactory.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.lists.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.openssl_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.openssl_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.openssl_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.openssl_tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pem.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pycrypto_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pycrypto_aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pycrypto_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pycrypto_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.pycrypto_tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.python_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.python_aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.python_chacha20_poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.python_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.python_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.rijndael.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.tackwrapper.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.tlshashlib.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.x25519.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.verifierdb.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.x509.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.x509certchain.rst.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.663641 tlslite-ng-0.8.0a46/docs/_build/html/_static/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4418 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15180 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.663641 tlslite-ng-0.8.0a46/docs/_build/html/_static/css/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2922 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   128848 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8171 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      429 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      286 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/file.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   288580 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    89501 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.664641 tlslite-ng-0.8.0a46/docs/_build/html/_static/js/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      934 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5023 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4758 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/minus.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/plus.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4846 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    17088 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    68420 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19530 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a46/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   255727 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/genindex.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4704 2023-08-03 17:25:11.000000 tlslite-ng-0.8.0a46/docs/_build/html/index.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7955 2023-08-03 17:25:11.000000 tlslite-ng-0.8.0a46/docs/_build/html/modules.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11473 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/objects.inv
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21834 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/py-modindex.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3593 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/search.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   162778 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/searchindex.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7635 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.api.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14507 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.basedb.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15038 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.bufferedsocket.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12591 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.checker.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   282446 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.constants.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12836 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.defragmenter.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     9820 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.dh.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    40595 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.errors.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   169749 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.extensions.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13049 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakehashes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14256 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakehelpers.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    34028 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakesettings.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19608 2023-08-03 17:25:11.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15981 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.asyncstatemachine.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13925 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.clienthelper.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6874 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15108 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.httptlsconnection.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14811 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.imap4_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12135 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.pop3_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11674 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.smtp_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    20642 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12512 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.tlssocketservermixin.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11939 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.xmlrpcserver.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15905 2023-08-03 17:25:12.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.xmlrpctransport.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    58370 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.keyexchange.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    67608 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.mathtls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   147651 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.messages.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18129 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.messagesocket.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    35655 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.recordlayer.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    25249 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.session.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11817 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.sessioncache.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    47436 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.tlsconnection.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    43739 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.tlsrecordlayer.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7786 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8459 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13626 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.asn1parser.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12725 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.chacha.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10067 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.chacha20_poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18141 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.cipherfactory.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    33216 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.codec.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16967 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.compat.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18018 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.constanttime.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    34260 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.cryptomath.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10078 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.datefuncs.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14255 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.deprecations.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6466 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.dns_utils.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7761 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.ecc.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21776 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.ecdsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10584 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19234 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.keyfactory.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     9265 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.lists.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16689 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    17482 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11632 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14357 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pem.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8842 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10515 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7817 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10063 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14657 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10746 2023-08-03 17:25:13.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8560 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5897 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6017 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10047 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14650 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7538 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11634 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rijndael.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    38486 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5238 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tackwrapper.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6794 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tlshashlib.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7979 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.x25519.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15655 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.verifierdb.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14761 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.x509.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15974 2023-08-03 17:25:14.000000 tlslite-ng-0.8.0a46/docs/_build/html/tlslite.x509certchain.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10006 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/docs/conf.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/index.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7740 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/make.bat
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/modules.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.api.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.basedb.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.bufferedsocket.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.checker.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.constants.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.defragmenter.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.dh.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.errors.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.extensions.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.handshakehashes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.handshakehelpers.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.handshakesettings.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.asyncstatemachine.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.clienthelper.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.httptlsconnection.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.imap4_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.pop3_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.smtp_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.tlsasyncdispatchermixin.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.tlssocketservermixin.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.xmlrpcserver.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.integration.xmlrpctransport.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.keyexchange.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.mathtls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.messages.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.messagesocket.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.recordlayer.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.session.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.sessioncache.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.tlsconnection.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.tlsrecordlayer.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.asn1parser.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.chacha.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.chacha20_poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.cipherfactory.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.codec.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.compat.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.constanttime.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.cryptomath.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.datefuncs.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.deprecations.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.dns_utils.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.ecc.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.ecdsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.keyfactory.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.lists.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.openssl_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.openssl_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.openssl_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.openssl_tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pem.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pycrypto_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pycrypto_aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pycrypto_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pycrypto_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.pycrypto_tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.python_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.python_aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.python_chacha20_poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.python_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.python_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.rijndael.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.tackwrapper.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.tlshashlib.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.utils.x25519.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.verifierdb.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.x509.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/docs/tlslite.x509certchain.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10645 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/pylintrc
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/requirements.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.664641 tlslite-ng-0.8.0a46/scripts/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1903 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/scripts/speed.py
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)    25742 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/scripts/tls.py
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)     3774 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/scripts/tlsdb.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       38 2023-08-03 17:25:16.701641 tlslite-ng-0.8.0a46/setup.cfg
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)     2093 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/setup.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.675640 tlslite-ng-0.8.0a46/tests/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      124 2015-10-14 14:17:40.000000 tlslite-ng-0.8.0a46/tests/.coverage
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/TACK1.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/TACK2.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/TACK_Key1.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/TACK_Key2.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      650 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a46/tests/TACKs.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a46/tests/TACKunrelated.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/clientECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/clientECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      485 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/clientEd25519Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/clientEd25519Key.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      924 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a46/tests/clientX509Cert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      891 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a46/tests/clientX509Key.pem
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)      327 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/httpsclient.py
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)      113 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/httpsserver.sh
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      152 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/index.html
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP256r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP256r1ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP384r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      292 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP384r1ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      757 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP512r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      361 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverBrainpoolP512r1ECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6628 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverDSACert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverDSAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      554 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2261 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverECDSANonCACert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverECDSANonCAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      489 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverEd25519Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverEd25519Key.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      591 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverEd448Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      156 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tests/serverEd448Key.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      660 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverP384ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      306 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverP384ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      761 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverP521ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      384 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverP521ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverRSANonCACert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1675 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tests/serverRSANonCAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tests/serverRSAPSSCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1700 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tests/serverRSAPSSKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1229 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tests/serverRSAPSSSigCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tests/serverRSAPSSSigKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1094 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/serverX509Cert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/serverX509Key.pem
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)   120979 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tests/tlstest.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    24576 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tests/verifierDB
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.679641 tlslite-ng-0.8.0a46/tlslite/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      878 2021-08-06 12:04:22.000000 tlslite-ng-0.8.0a46/tlslite/__init__.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1666 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/tlslite/api.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4092 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/basedb.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2836 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/bufferedsocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2725 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/checker.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    67117 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/constants.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4564 2023-08-03 11:21:38.000000 tlslite-ng-0.8.0a46/tlslite/defragmenter.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      914 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/dh.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6838 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/errors.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    70188 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/extensions.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4137 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/handshakehashes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6725 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/handshakehelpers.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    32463 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/handshakesettings.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.680641 tlslite-ng-0.8.0a46/tlslite/integration/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      396 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tlslite/integration/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7202 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a46/tlslite/integration/asyncstatemachine.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/integration/clienthelper.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4514 2018-07-30 10:15:07.000000 tlslite-ng-0.8.0a46/tlslite/integration/httptlsconnection.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3680 2021-01-14 12:41:41.000000 tlslite-ng-0.8.0a46/tlslite/integration/imap4_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3199 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/integration/pop3_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3026 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/integration/smtp_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4964 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/integration/tlsasyncdispatchermixin.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2320 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/integration/tlssocketservermixin.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1909 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/integration/xmlrpcserver.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5332 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/integration/xmlrpctransport.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    43331 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/keyexchange.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    45528 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/mathtls.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    80761 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/messages.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6250 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/messagesocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5933 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/ocsp.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    51923 2023-08-03 17:22:09.000000 tlslite-ng-0.8.0a46/tlslite/recordlayer.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8581 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/session.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3552 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/sessioncache.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3545 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/signed.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   219811 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/tlsconnection.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    62199 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/tlslite/tlsrecordlayer.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.686641 tlslite-ng-0.8.0a46/tlslite/utils/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      837 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1222 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4966 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6866 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3802 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/asn1parser.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4821 2017-02-17 16:14:00.000000 tlslite-ng-0.8.0a46/tlslite/utils/chacha.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3123 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/chacha20_poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5957 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/cipherfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    15543 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/codec.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7229 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/compat.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6399 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/constanttime.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12585 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/cryptomath.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2278 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a46/tlslite/utils/datefuncs.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     8742 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/deprecations.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1468 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/utils/dns_utils.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3144 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/dsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/ecc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5590 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/ecdsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4766 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/eddsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      483 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/format_output.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10460 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/keyfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1549 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/lists.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4539 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      733 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      709 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7156 2023-07-11 11:45:08.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1801 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/openssl_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a46/tlslite/utils/pem.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1504 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/utils/poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      840 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      446 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      764 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_rc4.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2644 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      872 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      271 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      268 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      316 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_chacha20_poly1305.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3777 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_dsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3388 2023-07-10 15:01:18.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_ecdsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2101 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_eddsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11034 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_key.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1073 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4691 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    16932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/python_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      561 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a46/tlslite/utils/rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    53143 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/rijndael.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    26348 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/utils/rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      334 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a46/tlslite/utils/tackwrapper.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1024 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a46/tlslite/utils/tlshashlib.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3079 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/utils/tlshmac.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      870 2018-02-01 13:32:10.000000 tlslite-ng-0.8.0a46/tlslite/utils/tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3255 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/utils/x25519.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3702 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/tlslite/verifierdb.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10386 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/tlslite/x509.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3323 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/tlslite/x509certchain.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.686641 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3508 2023-08-03 17:25:15.000000 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/PKG-INFO
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18045 2023-08-03 17:25:16.000000 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)        1 2023-08-03 17:25:16.000000 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-08-03 17:25:16.000000 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/requires.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)        8 2023-08-03 17:25:16.000000 tlslite-ng-0.8.0a46/tlslite_ng.egg-info/top_level.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-03 17:25:16.701641 tlslite-ng-0.8.0a46/unit_tests/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)        0 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/unit_tests/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3336 2018-06-29 15:54:59.000000 tlslite-ng-0.8.0a46/unit_tests/mocksock.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    18932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tls1_3_vectors.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4414 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_bufferedsocket.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12726 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_constants.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6979 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_defragmenter.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2245 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_dh.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    98752 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_extensions.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3383 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakehashes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    17133 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakehelpers.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15363 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakesettings.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   126491 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_keyexchange.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     9991 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_mathtls.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   154757 2023-08-03 17:14:04.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_messages.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    12586 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_messagesocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    25676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_ocsp.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)   117035 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_recordlayer.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1834 2016-04-14 13:26:36.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_session.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1275 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_sessioncache.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2611 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_signed.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19118 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_tlsconnection.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    36862 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_tlsrecordlayer.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2931 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aes_split.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10191 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aescbc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    22930 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10558 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesctr.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    14665 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2143 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_asn1.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    15890 2016-01-07 16:34:17.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_chacha.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5662 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_chacha20_poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    11423 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_codec.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      789 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_compat.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16432 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_constanttime.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    26699 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_cryptomath.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3442 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    16100 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_deprecations.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1286 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_dns_utils.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     8381 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_ecc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2228 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_ecdsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    13810 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_keyfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1694 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_lists.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7573 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_poly1305.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21266 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_dsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3998 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_ecdsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7738 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_key.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6754 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_rijndael.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   170557 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      765 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tlshashlib.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    20642 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3178 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tripledes_split.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    14421 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_x25519.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6997 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a46/unit_tests/test_tlslite_x509.py
```

### Comparing `tlslite-ng-0.8.0a45/.codeclimate.yml` & `tlslite-ng-0.8.0a46/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/.github/workflows/ci.yml` & `tlslite-ng-0.8.0a46/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,20 @@
             python-version: 3.8
           - name: py3.9
             os: ubuntu-latest
             python-version: 3.9
           - name: py3.10
             os: ubuntu-latest
             python-version: '3.10'
+          - name: py3.11
+            os: ubuntu-latest
+            python-version: '3.11'
+          - name: py3.12
+            os: ubuntu-latest
+            python-version: '3.12.0-beta.4'
           - name: py2.6
             os: ubuntu-latest
             container: centos:6
             python-version: 2.6
           # then test with the different optional dependencies installed
           - name: py3.6 with tackpy
             os: ubuntu-20.04
@@ -66,14 +72,18 @@
             os: ubuntu-latest
             python-version: 3.9
             opt-deps: ['m2crypto']
           - name: py3.10 with m2crypto
             os: ubuntu-latest
             python-version: '3.10'
             opt-deps: ['m2crypto']
+          - name: py3.11 with m2crypto
+            os: ubuntu-latest
+            python-version: '3.11'
+            opt-deps: ['m2crypto']
           - name: py2.7 with pycrypto
             os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['pycrypto']
           - name: py3.6 with pycrypto
             os: ubuntu-20.04
             # note: 3.6 is the last version where pycrypto is installable
@@ -103,14 +113,15 @@
             opt-deps: ['gmpy']
           - name: py3.9 with gmpy
             os: ubuntu-latest
             python-version: 3.9
             opt-deps: ['gmpy']
           - name: py3.10 with gmpy
             os: ubuntu-latest
+            # 3.10 is the last version gmpy builds with
             python-version: '3.10'
             opt-deps: ['gmpy']
           - name: py2.7 with gmpy2
             os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['gmpy2']
           - name: py3.6 with gmpy2
@@ -129,14 +140,18 @@
             os: ubuntu-latest
             python-version: 3.9
             opt-deps: ['gmpy2']
           - name: py3.10 with gmpy2
             os: ubuntu-latest
             python-version: '3.10'
             opt-deps: ['gmpy2']
+          - name: py3.11 with gmpy2
+            os: ubuntu-latest
+            python-version: '3.11'
+            opt-deps: ['gmpy2']
           # finally test with multiple dependencies installed at the same time
           - name: py2.7 with m2crypto, pycrypto, gmpy, and gmpy2
             os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['m2crypto', 'pycrypto', 'gmpy', 'gmpy2']
           - name: py3.6 with m2crypto, pycrypto, gmpy, and gmpy2
             os: ubuntu-20.04
@@ -153,16 +168,21 @@
           - name: py3.9 with m2crypto, gmpy, and gmpy2
             os: ubuntu-latest
             python-version: 3.9
             opt-deps: ['m2crypto', 'gmpy', 'gmpy2']
           - name: py3.10 with m2crypto, gmpy, and gmpy2
             os: ubuntu-latest
             python-version: '3.10'
+            opt-deps: ['m2crypto', 'gmpy', 'gmpy2']
+          - name: py3.11 with m2crypto, gmpy, and gmpy2
+            os: ubuntu-latest
+            python-version: '3.11'
+            # gmpy doesn't build with 3.11
             # coverage to codeclimate can be submitted just once
-            opt-deps: ['m2crypto', 'gmpy', 'gmpy2', 'codeclimate']
+            opt-deps: ['m2crypto', 'gmpy2', 'codeclimate']
     steps:
       - uses: actions/checkout@v2
         if: ${{ !matrix.container }}
         with:
           fetch-depth: 50
       - uses: actions/checkout@v1
         # centos 6 doesn't have glibc new enough for the nodejs used by v2
```

### Comparing `tlslite-ng-0.8.0a45/.travis.yml` & `tlslite-ng-0.8.0a46/.travis.yml`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/CONTRIBUTING.md` & `tlslite-ng-0.8.0a46/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/LICENSE` & `tlslite-ng-0.8.0a46/LICENSE`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/Makefile` & `tlslite-ng-0.8.0a46/Makefile`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/PKG-INFO` & `tlslite-ng-0.8.0a46/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlslite-ng
-Version: 0.8.0a45
+Version: 0.8.0a46
 Summary: Pure python implementation of SSL and TLS.
 Home-page: https://github.com/tlsfuzzer/tlslite-ng
 Author: Hubert Kario
 Author-email: hkario@redhat.com
 License: LGPLv2
 Keywords: ssl,tls,pure-python
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Obsoletes: tlslite
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
 
@@ -50,16 +53,16 @@
  - secp256r1, secp384r1, secp521r1, secp256k1, secp224r1 and secp192r1 curves
    for ECDHE key exchange (support for last two depends on the version of ecdsa
    library used)
  - x25519 and x448 curves for ECDHE key exchage (RFC 7748. RFC 4492bis)
  - anonymous DHE key exchange
  - anonymous ECDH key exchange
  - PSK and PSK-DH key exchange in TLS 1.3
- - session ticket based resumption in TLS 1.3
- - post-handshake key authentication in TLS 1.3
+ - session ticket based resumption (RFC 5077) and in TLS 1.3
+ - post-handshake client authentication in TLS 1.3
  - NULL encryption ciphersuites
  - FALLBACK_SCSV (RFC 7507)
  - encrypt-then-MAC mode of operation for CBC ciphersuites (RFC 7366)
  - TACK certificate pinning
  - SRP_SHA_RSA and SRP_SHA ciphersuites (RFC 5054)
  - Extended Master Secret calculation for TLS connections (RFC 7627)
  - padding extension (RFC 7685)
```

### Comparing `tlslite-ng-0.8.0a45/README` & `tlslite-ng-0.8.0a46/README`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
  - secp256r1, secp384r1, secp521r1, secp256k1, secp224r1 and secp192r1 curves
    for ECDHE key exchange (support for last two depends on the version of ecdsa
    library used)
  - x25519 and x448 curves for ECDHE key exchage (RFC 7748. RFC 4492bis)
  - anonymous DHE key exchange
  - anonymous ECDH key exchange
  - PSK and PSK-DH key exchange in TLS 1.3
- - session ticket based resumption in TLS 1.3
- - post-handshake key authentication in TLS 1.3
+ - session ticket based resumption (RFC 5077) and in TLS 1.3
+ - post-handshake client authentication in TLS 1.3
  - NULL encryption ciphersuites
  - FALLBACK_SCSV (RFC 7507)
  - encrypt-then-MAC mode of operation for CBC ciphersuites (RFC 7366)
  - TACK certificate pinning
  - SRP_SHA_RSA and SRP_SHA ciphersuites (RFC 5054)
  - Extended Master Secret calculation for TLS connections (RFC 7627)
  - padding extension (RFC 7685)
```

### Comparing `tlslite-ng-0.8.0a45/README.md` & `tlslite-ng-0.8.0a46/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tlslite-ng version 0.8.0-alpha45 (2023-08-01)
+tlslite-ng version 0.8.0-alpha46 (2023-08-03)
 
 [![Build Status](https://github.com/tlsfuzzer/tlslite-ng/workflows/GitHub%20CI/badge.svg?branch=master)](https://github.com/tlsfuzzer/tlslite-ng/actions?query=workflow%3A%22GitHub+CI%22+branch%3Amaster)
 [![Read the Docs](https://img.shields.io/readthedocs/tlslite-ng)](https://tlslite-ng.readthedocs.io/en/latest/)
 [![Coverage Status](https://coveralls.io/repos/tlsfuzzer/tlslite-ng/badge.svg?branch=master)](https://coveralls.io/r/tlsfuzzer/tlslite-ng?branch=master)
 [![Code Climate](https://codeclimate.com/github/tlsfuzzer/tlslite-ng/badges/gpa.svg)](https://codeclimate.com/github/tlsfuzzer/tlslite-ng)
 
 Table of Contents
@@ -58,15 +58,15 @@
 * Secure Renegotiation
 * Encrypt Then MAC extension
 * TLS_FALLBACK_SCSV
 * Extended master secret
 * padding extension
 * keying material exporter
 * RSA, RSA-PSS, ECDSA, and EdDSA certificates
-* ticket based session resumption in TLSv1.3
+* ticket based session resumption
 * 1-RTT handshake, Hello Retry Request, middlebox compatibility mode,
   cookie extension, post-handshake authentication and KeyUpdate
   (TLS 1.3)
 * FFDHE supported_groups extension
 * X25519 and X448 ECDHE key exchange
 * Ed25519 and Ed448 EdDSA signatures
 * (experimental) TACK extension
@@ -682,23 +682,25 @@
 * fix wrong error message in AES implementation (Bernt Røskar Brenna)
 * migrate to Github Action for CI
 * fix API break caused by the workaround for Bleichenbacher; RSA keys generated
   in-memory with m2crypto wouldn't work for decryption/encryption
 * handle too short RSA ciphertexts for the key size consistently between
   backends
 * strict handling of CCS in TLS 1.3 (don't allow it post handshake)
+* detect and reject multi-byte CCS messages
 * improved RSA key generation - don't generate biased primes
 * support for both encodings of RSA-PSS algorithm identifier in X.509
 * Support for EdDSA (Ed25519 and Ed448) in TLS 1.2 and TLS 1.3, both
   for server and client certificates
 * Support for echo server in the example tls.py script
 * Better handling of HMACs in FIPS mode
 * Generate RSA keys with 65537 as public exponent with m2crypto (as with
   other backends)
-
+* Ticket based session resumption in TLS 1.2 and earlier
+* strict size checking of `session_id` field in ClientHello
 
 0.7.0 - 2017-07-31
 
 * enable and add missing definitions of TLS_ECDHE_RSA_WITH_RC4_128_SHA and
   TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA
 * add definitions of some ECDHE_ECDSA, ECDH_ECDSA and ECDH_RSA ciphersuites,
   they remain unsupported, but IDs are useful for other projects
```

### Comparing `tlslite-ng-0.8.0a45/SECURITY.md` & `tlslite-ng-0.8.0a46/SECURITY.md`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/Makefile` & `tlslite-ng-0.8.0a46/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.rst.txt` & `tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.integration.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.rst.txt` & `tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rst.txt` & `tlslite-ng-0.8.0a46/docs/_build/html/_sources/tlslite.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/basic.css` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/css/badge_only.css` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/css/theme.css` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/doctools.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery-3.6.0.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/js/badge_only.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/js/theme.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/language_data.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/pygments.css` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/searchtools.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore-1.13.1.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore.js` & `tlslite-ng-0.8.0a46/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/genindex.html` & `tlslite-ng-0.8.0a46/docs/_build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>Index &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -188,14 +188,16 @@
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.RenegotiationInfoExtension.__init__">(tlslite.extensions.RenegotiationInfoExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerCertTypeExtension.__init__">(tlslite.extensions.ServerCertTypeExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerKeyShareExtension.__init__">(tlslite.extensions.ServerKeyShareExtension method)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension.__init__">(tlslite.extensions.SessionTicketExtension method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SignatureAlgorithmsCertExtension.__init__">(tlslite.extensions.SignatureAlgorithmsCertExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SignatureAlgorithmsExtension.__init__">(tlslite.extensions.SignatureAlgorithmsExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.__init__">(tlslite.extensions.SNIExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SRPExtension.__init__">(tlslite.extensions.SRPExtension method)</a>
@@ -306,14 +308,16 @@
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.KeyUpdate.__init__">(tlslite.messages.KeyUpdate method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.Message.__init__">(tlslite.messages.Message method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket.__init__">(tlslite.messages.NewSessionTicket method)</a>
 </li>
+        <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket1_0.__init__">(tlslite.messages.NewSessionTicket1_0 method)</a>
+</li>
         <li><a href="tlslite.messages.html#tlslite.messages.NextProtocol.__init__">(tlslite.messages.NextProtocol method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader.__init__">(tlslite.messages.RecordHeader method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader2.__init__">(tlslite.messages.RecordHeader2 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader3.__init__">(tlslite.messages.RecordHeader3 method)</a>
@@ -338,14 +342,16 @@
 </li>
         <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.RecordLayer.__init__">(tlslite.recordlayer.RecordLayer method)</a>
 </li>
         <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.RecordSocket.__init__">(tlslite.recordlayer.RecordSocket method)</a>
 </li>
         <li><a href="tlslite.session.html#tlslite.session.Session.__init__">(tlslite.session.Session method)</a>
 </li>
+        <li><a href="tlslite.session.html#tlslite.session.Ticket.__init__">(tlslite.session.Ticket method)</a>
+</li>
         <li><a href="tlslite.sessioncache.html#tlslite.sessioncache.SessionCache.__init__">(tlslite.sessioncache.SessionCache method)</a>
 </li>
         <li><a href="tlslite.tlsconnection.html#tlslite.tlsconnection.TLSConnection.__init__">(tlslite.tlsconnection.TLSConnection method)</a>
 </li>
         <li><a href="tlslite.tlsrecordlayer.html#tlslite.tlsrecordlayer.TLSRecordLayer.__init__">(tlslite.tlsrecordlayer.TLSRecordLayer method)</a>
 </li>
         <li><a href="tlslite.utils.aes.html#tlslite.utils.aes.AES.__init__">(tlslite.utils.aes.AES method)</a>
@@ -432,14 +438,16 @@
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.KeyShareEntry.__repr__">(tlslite.extensions.KeyShareEntry method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ListExtension.__repr__">(tlslite.extensions.ListExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.NPNExtension.__repr__">(tlslite.extensions.NPNExtension method)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension.__repr__">(tlslite.extensions.SessionTicketExtension method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.__repr__">(tlslite.extensions.SNIExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.ServerName.__repr__">(tlslite.extensions.SNIExtension.ServerName method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SRPExtension.__repr__">(tlslite.extensions.SRPExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SrvSupportedVersionsExtension.__repr__">(tlslite.extensions.SrvSupportedVersionsExtension method)</a>
@@ -929,18 +937,18 @@
 </li>
       <li><a href="tlslite.utils.compat.html#tlslite.utils.compat.compat_b2a">compat_b2a() (in module tlslite.utils.compat)</a>
 </li>
       <li><a href="tlslite.utils.compat.html#tlslite.utils.compat.compatAscii2Bytes">compatAscii2Bytes() (in module tlslite.utils.compat)</a>
 </li>
       <li><a href="tlslite.utils.compat.html#tlslite.utils.compat.compatHMAC">compatHMAC() (in module tlslite.utils.compat)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.utils.compat.html#tlslite.utils.compat.compatLong">compatLong() (in module tlslite.utils.compat)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.integration.xmlrpctransport.html#tlslite.integration.xmlrpctransport.XMLRPCTransport.conn_class_is_http">conn_class_is_http (tlslite.integration.xmlrpctransport.XMLRPCTransport attribute)</a>
 </li>
       <li><a href="tlslite.integration.httptlsconnection.html#tlslite.integration.httptlsconnection.HTTPTLSConnection.connect">connect() (tlslite.integration.httptlsconnection.HTTPTLSConnection method)</a>
 </li>
       <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.ConnectionState">ConnectionState (class in tlslite.recordlayer)</a>
 </li>
       <li><a href="tlslite.utils.chacha.html#tlslite.utils.chacha.ChaCha.constants">constants (tlslite.utils.chacha.ChaCha attribute)</a>
@@ -980,14 +988,16 @@
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.PreSharedKeyExtension.create">(tlslite.extensions.PreSharedKeyExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.PskIdentity.create">(tlslite.extensions.PskIdentity method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerKeyShareExtension.create">(tlslite.extensions.ServerKeyShareExtension method)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension.create">(tlslite.extensions.SessionTicketExtension method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.create">(tlslite.extensions.SNIExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SRPExtension.create">(tlslite.extensions.SRPExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SrvSupportedVersionsExtension.create">(tlslite.extensions.SrvSupportedVersionsExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.StatusRequestExtension.create">(tlslite.extensions.StatusRequestExtension method)</a>
@@ -1028,14 +1038,16 @@
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.HelloRequest.create">(tlslite.messages.HelloRequest method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.KeyUpdate.create">(tlslite.messages.KeyUpdate method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket.create">(tlslite.messages.NewSessionTicket method)</a>
 </li>
+        <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket1_0.create">(tlslite.messages.NewSessionTicket1_0 method)</a>
+</li>
         <li><a href="tlslite.messages.html#tlslite.messages.NextProtocol.create">(tlslite.messages.NextProtocol method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader2.create">(tlslite.messages.RecordHeader2 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader3.create">(tlslite.messages.RecordHeader3 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.ServerHello.create">(tlslite.messages.ServerHello method)</a>
@@ -1351,14 +1363,16 @@
 </li>
       <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.RecordLayer.encryptThenMAC">encryptThenMAC (tlslite.recordlayer.RecordLayer property)</a>
 
       <ul>
         <li><a href="tlslite.tlsrecordlayer.html#tlslite.tlsrecordlayer.TLSRecordLayer.encryptThenMAC">(tlslite.tlsrecordlayer.TLSRecordLayer property)</a>
 </li>
       </ul></li>
+      <li><a href="tlslite.constants.html#tlslite.constants.HandshakeType.end_of_early_data">end_of_early_data (tlslite.constants.HandshakeType attribute)</a>
+</li>
       <li><a href="tlslite.constants.html#tlslite.constants.SSL2HandshakeType.error">error (tlslite.constants.SSL2HandshakeType attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.ECCurveType.explicit_char2">explicit_char2 (tlslite.constants.ECCurveType attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.ECCurveType.explicit_prime">explicit_prime (tlslite.constants.ECCurveType attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.AlertDescription.export_restriction">export_restriction (tlslite.constants.AlertDescription attribute)</a>
@@ -1380,14 +1394,16 @@
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.PaddingExtension.extData">(tlslite.extensions.PaddingExtension property)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.PreSharedKeyExtension.extData">(tlslite.extensions.PreSharedKeyExtension property)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerKeyShareExtension.extData">(tlslite.extensions.ServerKeyShareExtension property)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension.extData">(tlslite.extensions.SessionTicketExtension property)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.extData">(tlslite.extensions.SNIExtension property)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SRPExtension.extData">(tlslite.extensions.SRPExtension property)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SrvSupportedVersionsExtension.extData">(tlslite.extensions.SrvSupportedVersionsExtension property)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.StatusRequestExtension.extData">(tlslite.extensions.StatusRequestExtension property)</a>
@@ -1431,22 +1447,24 @@
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.GroupName.ffdhe6144">ffdhe6144 (tlslite.constants.GroupName attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.GroupName.ffdhe8192">ffdhe8192 (tlslite.constants.GroupName attribute)</a>
 </li>
       <li><a href="tlslite.mathtls.html#tlslite.mathtls.FFDHE_PARAMETERS">FFDHE_PARAMETERS (in module tlslite.mathtls)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.keyexchange.html#tlslite.keyexchange.FFDHKeyExchange">FFDHKeyExchange (class in tlslite.keyexchange)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.tlsrecordlayer.html#tlslite.tlsrecordlayer.TLSRecordLayer.fileno">fileno() (tlslite.tlsrecordlayer.TLSRecordLayer method)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.filter_for_certificate">filter_for_certificate() (tlslite.constants.CipherSuite static method)</a>
 </li>
+      <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.filter_for_prfs">filter_for_prfs() (tlslite.constants.CipherSuite static method)</a>
+</li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.filterForVersion">filterForVersion() (tlslite.constants.CipherSuite static method)</a>
 </li>
       <li><a href="tlslite.integration.tlssocketservermixin.html#tlslite.integration.tlssocketservermixin.TLSSocketServerMixIn.finish_request">finish_request() (tlslite.integration.tlssocketservermixin.TLSSocketServerMixIn method)</a>
 </li>
       <li><a href="tlslite.messages.html#tlslite.messages.Finished">Finished (class in tlslite.messages)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.HandshakeType.finished">finished (tlslite.constants.HandshakeType attribute)</a>
@@ -1741,14 +1759,16 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.i">i (tlslite.constants.CipherSuite attribute)</a>
+</li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.ietfNames">ietfNames (tlslite.constants.CipherSuite attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.AlertDescription.illegal_parameter">illegal_parameter (tlslite.constants.AlertDescription attribute)</a>
 </li>
       <li><a href="tlslite.integration.imap4_tls.html#tlslite.integration.imap4_tls.IMAP4_TLS">IMAP4_TLS (class in tlslite.integration.imap4_tls)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.AlertDescription.inappropriate_fallback">inappropriate_fallback (tlslite.constants.AlertDescription attribute)</a>
@@ -1769,14 +1789,16 @@
 </li>
       <li><a href="tlslite.errors.html#tlslite.errors.InvalidSignature">InvalidSignature</a>
 </li>
       <li><a href="tlslite.utils.cryptomath.html#tlslite.utils.cryptomath.invMod">invMod() (in module tlslite.utils.cryptomath)</a>
 </li>
       <li><a href="tlslite.integration.asyncstatemachine.html#tlslite.integration.asyncstatemachine.AsyncStateMachine.inWriteEvent">inWriteEvent() (tlslite.integration.asyncstatemachine.AsyncStateMachine method)</a>
 </li>
+      <li><a href="tlslite.defragmenter.html#tlslite.defragmenter.Defragmenter.is_empty">is_empty() (tlslite.defragmenter.Defragmenter method)</a>
+</li>
       <li><a href="tlslite.utils.dns_utils.html#tlslite.utils.dns_utils.is_valid_hostname">is_valid_hostname() (in module tlslite.utils.dns_utils)</a>
 </li>
       <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.RecordLayer.isCBCMode">isCBCMode() (tlslite.recordlayer.RecordLayer method)</a>
 </li>
       <li><a href="tlslite.utils.datefuncs.html#tlslite.utils.datefuncs.isDateClassBefore">isDateClassBefore() (in module tlslite.utils.datefuncs)</a>
 </li>
       <li><a href="tlslite.utils.datefuncs.html#tlslite.utils.datefuncs.isDateClassExpired">isDateClassExpired() (in module tlslite.utils.datefuncs)</a>
@@ -2108,20 +2130,22 @@
         <li><a href="tlslite.utils.python_chacha20_poly1305.html#tlslite.utils.python_chacha20_poly1305.new">(in module tlslite.utils.python_chacha20_poly1305)</a>
 </li>
         <li><a href="tlslite.utils.python_rc4.html#tlslite.utils.python_rc4.new">(in module tlslite.utils.python_rc4)</a>
 </li>
         <li><a href="tlslite.utils.tlshashlib.html#tlslite.utils.tlshashlib.new">(in module tlslite.utils.tlshashlib)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.constants.html#tlslite.constants.HandshakeType.new_session_ticket">new_session_ticket (tlslite.constants.HandshakeType attribute)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket">NewSessionTicket (class in tlslite.messages)</a>
 </li>
+      <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket1_0">NewSessionTicket1_0 (class in tlslite.messages)</a>
+</li>
       <li><a href="tlslite.constants.html#tlslite.constants.HandshakeType.next_protocol">next_protocol (tlslite.constants.HandshakeType attribute)</a>
 </li>
       <li><a href="tlslite.messages.html#tlslite.messages.ServerHello.next_protos">next_protos (tlslite.messages.ServerHello property)</a>
 </li>
       <li><a href="tlslite.messages.html#tlslite.messages.ServerHello.next_protos_advertised">next_protos_advertised (tlslite.messages.ServerHello property)</a>
 </li>
       <li><a href="tlslite.messages.html#tlslite.messages.NextProtocol">NextProtocol (class in tlslite.messages)</a>
@@ -2253,14 +2277,16 @@
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.PskIdentity.parse">(tlslite.extensions.PskIdentity method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerCertTypeExtension.parse">(tlslite.extensions.ServerCertTypeExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ServerKeyShareExtension.parse">(tlslite.extensions.ServerKeyShareExtension method)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension.parse">(tlslite.extensions.SessionTicketExtension method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.parse">(tlslite.extensions.SNIExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SRPExtension.parse">(tlslite.extensions.SRPExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SrvSupportedVersionsExtension.parse">(tlslite.extensions.SrvSupportedVersionsExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.StatusRequestExtension.parse">(tlslite.extensions.StatusRequestExtension method)</a>
@@ -2307,14 +2333,16 @@
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.HelloRequest.parse">(tlslite.messages.HelloRequest method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.KeyUpdate.parse">(tlslite.messages.KeyUpdate method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket.parse">(tlslite.messages.NewSessionTicket method)</a>
 </li>
+        <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket1_0.parse">(tlslite.messages.NewSessionTicket1_0 method)</a>
+</li>
         <li><a href="tlslite.messages.html#tlslite.messages.NextProtocol.parse">(tlslite.messages.NextProtocol method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader2.parse">(tlslite.messages.RecordHeader2 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader3.parse">(tlslite.messages.RecordHeader3 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.ServerHello.parse">(tlslite.messages.ServerHello method)</a>
@@ -2710,16 +2738,20 @@
 </li>
       <li><a href="tlslite.messages.html#tlslite.messages.ServerKeyExchange">ServerKeyExchange (class in tlslite.messages)</a>
 </li>
       <li><a href="tlslite.extensions.html#tlslite.extensions.ServerKeyShareExtension">ServerKeyShareExtension (class in tlslite.extensions)</a>
 </li>
       <li><a href="tlslite.session.html#tlslite.session.Session">Session (class in tlslite.session)</a>
 </li>
+      <li><a href="tlslite.constants.html#tlslite.constants.ExtensionType.session_ticket">session_ticket (tlslite.constants.ExtensionType attribute)</a>
+</li>
       <li><a href="tlslite.sessioncache.html#tlslite.sessioncache.SessionCache">SessionCache (class in tlslite.sessioncache)</a>
 </li>
+      <li><a href="tlslite.extensions.html#tlslite.extensions.SessionTicketExtension">SessionTicketExtension (class in tlslite.extensions)</a>
+</li>
       <li><a href="tlslite.messages.html#tlslite.messages.SessionTicketPayload">SessionTicketPayload (class in tlslite.messages)</a>
 </li>
       <li><a href="tlslite.integration.asyncstatemachine.html#tlslite.integration.asyncstatemachine.AsyncStateMachine.setCloseOp">setCloseOp() (tlslite.integration.asyncstatemachine.AsyncStateMachine method)</a>
 </li>
       <li><a href="tlslite.integration.asyncstatemachine.html#tlslite.integration.asyncstatemachine.AsyncStateMachine.setHandshakeOp">setHandshakeOp() (tlslite.integration.asyncstatemachine.AsyncStateMachine method)</a>
 </li>
       <li><a href="tlslite.utils.codec.html#tlslite.utils.codec.Parser.setLengthCheck">setLengthCheck() (tlslite.utils.codec.Parser method)</a>
@@ -2738,24 +2770,26 @@
         <li><a href="tlslite.tlsrecordlayer.html#tlslite.tlsrecordlayer.TLSRecordLayer.settimeout">(tlslite.tlsrecordlayer.TLSRecordLayer method)</a>
 </li>
       </ul></li>
       <li><a href="tlslite.integration.xmlrpcserver.html#tlslite.integration.xmlrpcserver.TLSXMLRPCRequestHandler.setup">setup() (tlslite.integration.xmlrpcserver.TLSXMLRPCRequestHandler method)</a>
 </li>
       <li><a href="tlslite.integration.asyncstatemachine.html#tlslite.integration.asyncstatemachine.AsyncStateMachine.setWriteOp">setWriteOp() (tlslite.integration.asyncstatemachine.AsyncStateMachine method)</a>
 </li>
-      <li><a href="tlslite.constants.html#tlslite.constants.HashAlgorithm.sha1">sha1 (tlslite.constants.HashAlgorithm attribute)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="tlslite.constants.html#tlslite.constants.HashAlgorithm.sha1">sha1 (tlslite.constants.HashAlgorithm attribute)</a>
+</li>
       <li><a href="tlslite.utils.cryptomath.html#tlslite.utils.cryptomath.SHA1">SHA1() (in module tlslite.utils.cryptomath)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.HashAlgorithm.sha224">sha224 (tlslite.constants.HashAlgorithm attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.HashAlgorithm.sha256">sha256 (tlslite.constants.HashAlgorithm attribute)</a>
 </li>
+      <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.sha256PrfSuites">sha256PrfSuites (tlslite.constants.CipherSuite attribute)</a>
+</li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.sha256Suites">sha256Suites (tlslite.constants.CipherSuite attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.HashAlgorithm.sha384">sha384 (tlslite.constants.HashAlgorithm attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.sha384PrfSuites">sha384PrfSuites (tlslite.constants.CipherSuite attribute)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.sha384Suites">sha384Suites (tlslite.constants.CipherSuite attribute)</a>
@@ -2908,14 +2942,16 @@
 </li>
       <li><a href="tlslite.extensions.html#tlslite.extensions.TACKExtension">TACKExtension (class in tlslite.extensions)</a>
 </li>
       <li><a href="tlslite.extensions.html#tlslite.extensions.TACKExtension.TACK">TACKExtension.TACK (class in tlslite.extensions)</a>
 </li>
       <li><a href="tlslite.utils.rijndael.html#tlslite.utils.rijndael.test">test() (in module tlslite.utils.rijndael)</a>
 </li>
+      <li><a href="tlslite.session.html#tlslite.session.Ticket">Ticket (class in tlslite.session)</a>
+</li>
       <li><a href="tlslite.utils.compat.html#tlslite.utils.compat.time_stamp">time_stamp() (in module tlslite.utils.compat)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.tls12Suites">tls12Suites (tlslite.constants.CipherSuite attribute)</a>
 </li>
       <li><a href="tlslite.recordlayer.html#tlslite.recordlayer.RecordLayer.tls13record">tls13record (tlslite.recordlayer.RecordLayer property)</a>
 </li>
       <li><a href="tlslite.constants.html#tlslite.constants.CipherSuite.tls13Suites">tls13Suites (tlslite.constants.CipherSuite attribute)</a>
@@ -3828,15 +3864,19 @@
   </ul></td>
 </tr></table>
 
 <h2 id="V">V</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="tlslite.session.html#tlslite.session.Session.valid">valid() (tlslite.session.Session method)</a>
+
+      <ul>
+        <li><a href="tlslite.session.html#tlslite.session.Ticket.valid">(tlslite.session.Ticket method)</a>
 </li>
+      </ul></li>
       <li><a href="tlslite.handshakesettings.html#tlslite.handshakesettings.HandshakeSettings.validate">validate() (tlslite.handshakesettings.HandshakeSettings method)</a>
 
       <ul>
         <li><a href="tlslite.handshakesettings.html#tlslite.handshakesettings.Keypair.validate">(tlslite.handshakesettings.Keypair method)</a>
 </li>
         <li><a href="tlslite.handshakesettings.html#tlslite.handshakesettings.VirtualHost.validate">(tlslite.handshakesettings.VirtualHost method)</a>
 </li>
@@ -3928,14 +3968,16 @@
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.KeyUpdate.write">(tlslite.messages.KeyUpdate method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.Message.write">(tlslite.messages.Message method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket.write">(tlslite.messages.NewSessionTicket method)</a>
 </li>
+        <li><a href="tlslite.messages.html#tlslite.messages.NewSessionTicket1_0.write">(tlslite.messages.NewSessionTicket1_0 method)</a>
+</li>
         <li><a href="tlslite.messages.html#tlslite.messages.NextProtocol.write">(tlslite.messages.NextProtocol method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader2.write">(tlslite.messages.RecordHeader2 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.RecordHeader3.write">(tlslite.messages.RecordHeader3 method)</a>
 </li>
         <li><a href="tlslite.messages.html#tlslite.messages.ServerHello.write">(tlslite.messages.ServerHello method)</a>
```

#### html2text {}

```diff
@@ -55,14 +55,15 @@
           o (tlslite.extensions.PreSharedKeyExtension_method)
           o (tlslite.extensions.PskIdentity_method)
           o (tlslite.extensions.PskKeyExchangeModesExtension_method)
           o (tlslite.extensions.RecordSizeLimitExtension_method)
           o (tlslite.extensions.RenegotiationInfoExtension_method)
           o (tlslite.extensions.ServerCertTypeExtension_method)
           o (tlslite.extensions.ServerKeyShareExtension_method)
+          o (tlslite.extensions.SessionTicketExtension_method)
           o (tlslite.extensions.SignatureAlgorithmsCertExtension_method)
           o (tlslite.extensions.SignatureAlgorithmsExtension_method)
           o (tlslite.extensions.SNIExtension_method)
           o (tlslite.extensions.SRPExtension_method)
           o (tlslite.extensions.SrvPreSharedKeyExtension_method)
           o (tlslite.extensions.SrvSupportedVersionsExtension_method)
           o (tlslite.extensions.StatusRequestExtension_method)
@@ -80,49 +81,50 @@
           o (tlslite.handshakesettings.VirtualHost_method)                           * __repr__()_(tlslite.extensions.ALPNExtension_method)
           o (tlslite.integration.asyncstatemachine.AsyncStateMachine_method)               o (tlslite.extensions.ClientKeyShareExtension
           o (tlslite.integration.clienthelper.ClientHelper_method)                           method)
           o (tlslite.integration.httptlsconnection.HTTPTLSConnection_method)               o (tlslite.extensions.IntExtension_method)
           o (tlslite.integration.imap4_tls.IMAP4_TLS_method)                               o (tlslite.extensions.KeyShareEntry_method)
           o (tlslite.integration.pop3_tls.POP3_TLS_method)                                 o (tlslite.extensions.ListExtension_method)
           o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn           o (tlslite.extensions.NPNExtension_method)
-            method)                                                                        o (tlslite.extensions.SNIExtension_method)
-          o (tlslite.integration.xmlrpcserver.MultiPathTLSXMLRPCServer_method)             o (tlslite.extensions.SNIExtension.ServerName
-          o (tlslite.integration.xmlrpcserver.TLSXMLRPCServer_method)                        method)
-          o (tlslite.integration.xmlrpctransport.XMLRPCTransport_method)                   o (tlslite.extensions.SRPExtension_method)
-          o (tlslite.keyexchange.ADHKeyExchange_method)                                    o (tlslite.extensions.SrvSupportedVersionsExtension
-          o (tlslite.keyexchange.AECDHKeyExchange_method)                                    method)
-          o (tlslite.keyexchange.DHE_RSAKeyExchange_method)                                o (tlslite.extensions.StatusRequestExtension_method)
-          o (tlslite.keyexchange.ECDHE_RSAKeyExchange_method)                              o (tlslite.extensions.TACKExtension_method)
-          o (tlslite.keyexchange.ECDHKeyExchange_method)                                   o (tlslite.extensions.TACKExtension.TACK_method)
-          o (tlslite.keyexchange.FFDHKeyExchange_method)                                   o (tlslite.extensions.TLSExtension_method)
-          o (tlslite.keyexchange.KeyExchange_method)                                       o (tlslite.extensions.VarBytesExtension_method)
-          o (tlslite.keyexchange.RawDHKeyExchange_method)                                  o (tlslite.messages.Alert_method)
-          o (tlslite.keyexchange.RSAKeyExchange_method)                                    o (tlslite.messages.Certificate_method)
-          o (tlslite.keyexchange.SRPKeyExchange_method)                                    o (tlslite.messages.CertificateEntry_method)
-          o (tlslite.messages.Alert_method)                                                o (tlslite.messages.ClientHello_method)
-          o (tlslite.messages.ApplicationData_method)                                      o (tlslite.messages.RecordHeader3_method)
-          o (tlslite.messages.Certificate_method)                                          o (tlslite.messages.ServerHello_method)
-          o (tlslite.messages.CertificateEntry_method)                                     o (tlslite.messages.ServerHelloDone_method)
-          o (tlslite.messages.CertificateRequest_method)                                   o (tlslite.messages.ServerKeyExchange_method)
-          o (tlslite.messages.CertificateStatus_method)                              * __setitem__()_(tlslite.basedb.BaseDB_method)
-          o (tlslite.messages.CertificateVerify_method)                                    o (tlslite.sessioncache.SessionCache_method)
-          o (tlslite.messages.ChangeCipherSpec_method)                                     o (tlslite.verifierdb.VerifierDB_method)
-          o (tlslite.messages.ClientFinished_method)                                 * __str__()_(tlslite.errors.TLSError_method)
-          o (tlslite.messages.ClientHello_method)                                          o (tlslite.errors.TLSLocalAlert_method)
-          o (tlslite.messages.ClientKeyExchange_method)                                    o (tlslite.errors.TLSRemoteAlert_method)
-          o (tlslite.messages.ClientMasterKey_method)                                      o (tlslite.messages.Alert_method)
-          o (tlslite.messages.EncryptedExtensions_method)                                  o (tlslite.messages.ClientHello_method)
-          o (tlslite.messages.Finished_method)                                             o (tlslite.messages.Heartbeat_method)
-          o (tlslite.messages.HandshakeMsg_method)                                         o (tlslite.messages.RecordHeader3_method)
-          o (tlslite.messages.Heartbeat_method)                                            o (tlslite.messages.ServerHello_method)
-          o (tlslite.messages.HelloMessage_method)
+            method)                                                                        o (tlslite.extensions.SessionTicketExtension_method)
+          o (tlslite.integration.xmlrpcserver.MultiPathTLSXMLRPCServer_method)             o (tlslite.extensions.SNIExtension_method)
+          o (tlslite.integration.xmlrpcserver.TLSXMLRPCServer_method)                      o (tlslite.extensions.SNIExtension.ServerName
+          o (tlslite.integration.xmlrpctransport.XMLRPCTransport_method)                     method)
+          o (tlslite.keyexchange.ADHKeyExchange_method)                                    o (tlslite.extensions.SRPExtension_method)
+          o (tlslite.keyexchange.AECDHKeyExchange_method)                                  o (tlslite.extensions.SrvSupportedVersionsExtension
+          o (tlslite.keyexchange.DHE_RSAKeyExchange_method)                                  method)
+          o (tlslite.keyexchange.ECDHE_RSAKeyExchange_method)                              o (tlslite.extensions.StatusRequestExtension_method)
+          o (tlslite.keyexchange.ECDHKeyExchange_method)                                   o (tlslite.extensions.TACKExtension_method)
+          o (tlslite.keyexchange.FFDHKeyExchange_method)                                   o (tlslite.extensions.TACKExtension.TACK_method)
+          o (tlslite.keyexchange.KeyExchange_method)                                       o (tlslite.extensions.TLSExtension_method)
+          o (tlslite.keyexchange.RawDHKeyExchange_method)                                  o (tlslite.extensions.VarBytesExtension_method)
+          o (tlslite.keyexchange.RSAKeyExchange_method)                                    o (tlslite.messages.Alert_method)
+          o (tlslite.keyexchange.SRPKeyExchange_method)                                    o (tlslite.messages.Certificate_method)
+          o (tlslite.messages.Alert_method)                                                o (tlslite.messages.CertificateEntry_method)
+          o (tlslite.messages.ApplicationData_method)                                      o (tlslite.messages.ClientHello_method)
+          o (tlslite.messages.Certificate_method)                                          o (tlslite.messages.RecordHeader3_method)
+          o (tlslite.messages.CertificateEntry_method)                                     o (tlslite.messages.ServerHello_method)
+          o (tlslite.messages.CertificateRequest_method)                                   o (tlslite.messages.ServerHelloDone_method)
+          o (tlslite.messages.CertificateStatus_method)                                    o (tlslite.messages.ServerKeyExchange_method)
+          o (tlslite.messages.CertificateVerify_method)                              * __setitem__()_(tlslite.basedb.BaseDB_method)
+          o (tlslite.messages.ChangeCipherSpec_method)                                     o (tlslite.sessioncache.SessionCache_method)
+          o (tlslite.messages.ClientFinished_method)                                       o (tlslite.verifierdb.VerifierDB_method)
+          o (tlslite.messages.ClientHello_method)                                    * __str__()_(tlslite.errors.TLSError_method)
+          o (tlslite.messages.ClientKeyExchange_method)                                    o (tlslite.errors.TLSLocalAlert_method)
+          o (tlslite.messages.ClientMasterKey_method)                                      o (tlslite.errors.TLSRemoteAlert_method)
+          o (tlslite.messages.EncryptedExtensions_method)                                  o (tlslite.messages.Alert_method)
+          o (tlslite.messages.Finished_method)                                             o (tlslite.messages.ClientHello_method)
+          o (tlslite.messages.HandshakeMsg_method)                                         o (tlslite.messages.Heartbeat_method)
+          o (tlslite.messages.Heartbeat_method)                                            o (tlslite.messages.RecordHeader3_method)
+          o (tlslite.messages.HelloMessage_method)                                         o (tlslite.messages.ServerHello_method)
           o (tlslite.messages.HelloRequest_method)
           o (tlslite.messages.KeyUpdate_method)
           o (tlslite.messages.Message_method)
           o (tlslite.messages.NewSessionTicket_method)
+          o (tlslite.messages.NewSessionTicket1_0_method)
           o (tlslite.messages.NextProtocol_method)
           o (tlslite.messages.RecordHeader_method)
           o (tlslite.messages.RecordHeader2_method)
           o (tlslite.messages.RecordHeader3_method)
           o (tlslite.messages.ServerFinished_method)
           o (tlslite.messages.ServerHello_method)
           o (tlslite.messages.ServerHello2_method)
@@ -131,14 +133,15 @@
           o (tlslite.messages.SessionTicketPayload_method)
           o (tlslite.messages.SSL2Finished_method)
           o (tlslite.messagesocket.MessageSocket_method)
           o (tlslite.recordlayer.ConnectionState_method)
           o (tlslite.recordlayer.RecordLayer_method)
           o (tlslite.recordlayer.RecordSocket_method)
           o (tlslite.session.Session_method)
+          o (tlslite.session.Ticket_method)
           o (tlslite.sessioncache.SessionCache_method)
           o (tlslite.tlsconnection.TLSConnection_method)
           o (tlslite.tlsrecordlayer.TLSRecordLayer_method)
           o (tlslite.utils.aes.AES_method)
           o (tlslite.utils.aesgcm.AESGCM_method)
           o (tlslite.utils.asn1parser.ASN1Parser_method)
           o (tlslite.utils.asn1parser.ASN1Type_method)
@@ -273,44 +276,44 @@
     * brainpoolP512r1_(tlslite.constants.GroupName            o (in_module_tlslite.x509certchain)
       attribute)                                        * bytesToNumber()_(in_module
     * BufferedSocket_(class_in                            tlslite.utils.cryptomath)
       tlslite.bufferedsocket)
     * byte_length()_(in_module
       tlslite.utils.compat)
 ***** C *****
-                                                                                     * compatLong()_(in_module_tlslite.utils.compat)
                                                                                      * conn_class_is_http_
                                                                                        (tlslite.integration.xmlrpctransport.XMLRPCTransport
                                                                                        attribute)
-    * calc_key()_(in_module_tlslite.mathtls)                                         * connect()_
-    * calc_public_value()_(tlslite.keyexchange.ECDHKeyExchange_method)                 (tlslite.integration.httptlsconnection.HTTPTLSConnection
-          o (tlslite.keyexchange.FFDHKeyExchange_method)                               method)
-          o (tlslite.keyexchange.RawDHKeyExchange_method)                            * ConnectionState_(class_in_tlslite.recordlayer)
-    * calc_res_binder_psk()_(tlslite.handshakehelpers.HandshakeHelpers_static        * constants_(tlslite.utils.chacha.ChaCha_attribute)
-      method)                                                                        * ContentType_(class_in_tlslite.constants)
-    * calc_shared_key()_(tlslite.keyexchange.ECDHKeyExchange_method)                 * cookie_(tlslite.constants.ExtensionType_attribute)
-          o (tlslite.keyexchange.FFDHKeyExchange_method)                             * CookieExtension_(class_in_tlslite.extensions)
-          o (tlslite.keyexchange.RawDHKeyExchange_method)                            * copy()_(tlslite.handshakehashes.HandshakeHashes_method)
-    * calcExtendedMasterSecret()_(in_module_tlslite.mathtls)                               o (tlslite.mathtls.MAC_SSL_method)
-    * calcFinished()_(in_module_tlslite.mathtls)                                     * counter_(tlslite.utils.openssl_aes.OpenSSL_CTR_property)
-    * calcMasterSecret()_(in_module_tlslite.mathtls)                                 * create()_(tlslite.basedb.BaseDB_method)
-    * calcPendingStates()_(tlslite.recordlayer.RecordLayer_method)                         o (tlslite.extensions.ALPNExtension_method)
-    * calcSSL2PendingStates()_(tlslite.recordlayer.RecordLayer_method)                     o (tlslite.extensions.CertificateStatusExtension
-    * calcTLS1_3KeyUpdate_reciever()_(tlslite.recordlayer.RecordLayer_method)                method)
-    * calcTLS1_3KeyUpdate_sender()_(tlslite.recordlayer.RecordLayer_method)                o (tlslite.extensions.ClientKeyShareExtension
-    * calcTLS1_3PendingState()_(tlslite.recordlayer.RecordLayer_method)                      method)
-    * calculateMAC()_(tlslite.recordlayer.RecordLayer_method)                              o (tlslite.extensions.CustomNameExtension_method)
-    * calcVerifyBytes()_(tlslite.keyexchange.KeyExchange_static_method)                    o (tlslite.extensions.HRRKeyShareExtension_method)
-    * canonicalCipherName()_(tlslite.constants.CipherSuite_static_method)                  o (tlslite.extensions.KeyShareEntry_method)
-    * canonicalMacName()_(tlslite.constants.CipherSuite_static_method)                     o (tlslite.extensions.NPNExtension_method)
-    * cert_chain_(tlslite.messages.Certificate_property)                                   o (tlslite.extensions.PaddingExtension_method)
-    * cert_type_(tlslite.constants.ExtensionType_attribute)                                o (tlslite.extensions.PreSharedKeyExtension_method)
-    * certAllSuites_(tlslite.constants.CipherSuite_attribute)                              o (tlslite.extensions.PskIdentity_method)
-    * Certificate_(class_in_tlslite.messages)                                              o (tlslite.extensions.ServerKeyShareExtension
-    * certificate_(tlslite.constants.HandshakeType_attribute)                                method)
+                                                                                     * connect()_
+    * calc_key()_(in_module_tlslite.mathtls)                                           (tlslite.integration.httptlsconnection.HTTPTLSConnection
+    * calc_public_value()_(tlslite.keyexchange.ECDHKeyExchange_method)                 method)
+          o (tlslite.keyexchange.FFDHKeyExchange_method)                             * ConnectionState_(class_in_tlslite.recordlayer)
+          o (tlslite.keyexchange.RawDHKeyExchange_method)                            * constants_(tlslite.utils.chacha.ChaCha_attribute)
+    * calc_res_binder_psk()_(tlslite.handshakehelpers.HandshakeHelpers_static        * ContentType_(class_in_tlslite.constants)
+      method)                                                                        * cookie_(tlslite.constants.ExtensionType_attribute)
+    * calc_shared_key()_(tlslite.keyexchange.ECDHKeyExchange_method)                 * CookieExtension_(class_in_tlslite.extensions)
+          o (tlslite.keyexchange.FFDHKeyExchange_method)                             * copy()_(tlslite.handshakehashes.HandshakeHashes_method)
+          o (tlslite.keyexchange.RawDHKeyExchange_method)                                  o (tlslite.mathtls.MAC_SSL_method)
+    * calcExtendedMasterSecret()_(in_module_tlslite.mathtls)                         * counter_(tlslite.utils.openssl_aes.OpenSSL_CTR_property)
+    * calcFinished()_(in_module_tlslite.mathtls)                                     * create()_(tlslite.basedb.BaseDB_method)
+    * calcMasterSecret()_(in_module_tlslite.mathtls)                                       o (tlslite.extensions.ALPNExtension_method)
+    * calcPendingStates()_(tlslite.recordlayer.RecordLayer_method)                         o (tlslite.extensions.CertificateStatusExtension
+    * calcSSL2PendingStates()_(tlslite.recordlayer.RecordLayer_method)                       method)
+    * calcTLS1_3KeyUpdate_reciever()_(tlslite.recordlayer.RecordLayer_method)              o (tlslite.extensions.ClientKeyShareExtension
+    * calcTLS1_3KeyUpdate_sender()_(tlslite.recordlayer.RecordLayer_method)                  method)
+    * calcTLS1_3PendingState()_(tlslite.recordlayer.RecordLayer_method)                    o (tlslite.extensions.CustomNameExtension_method)
+    * calculateMAC()_(tlslite.recordlayer.RecordLayer_method)                              o (tlslite.extensions.HRRKeyShareExtension_method)
+    * calcVerifyBytes()_(tlslite.keyexchange.KeyExchange_static_method)                    o (tlslite.extensions.KeyShareEntry_method)
+    * canonicalCipherName()_(tlslite.constants.CipherSuite_static_method)                  o (tlslite.extensions.NPNExtension_method)
+    * canonicalMacName()_(tlslite.constants.CipherSuite_static_method)                     o (tlslite.extensions.PaddingExtension_method)
+    * cert_chain_(tlslite.messages.Certificate_property)                                   o (tlslite.extensions.PreSharedKeyExtension_method)
+    * cert_type_(tlslite.constants.ExtensionType_attribute)                                o (tlslite.extensions.PskIdentity_method)
+    * certAllSuites_(tlslite.constants.CipherSuite_attribute)                              o (tlslite.extensions.ServerKeyShareExtension
+    * Certificate_(class_in_tlslite.messages)                                                method)
+    * certificate_(tlslite.constants.HandshakeType_attribute)                              o (tlslite.extensions.SessionTicketExtension_method)
     * certificate_expired_(tlslite.constants.AlertDescription_attribute)                   o (tlslite.extensions.SNIExtension_method)
     * certificate_request_(tlslite.constants.HandshakeType_attribute)                      o (tlslite.extensions.SRPExtension_method)
     * certificate_required_(tlslite.constants.AlertDescription_attribute)                  o (tlslite.extensions.SrvSupportedVersionsExtension
     * certificate_revoked_(tlslite.constants.AlertDescription_attribute)                     method)
     * certificate_status_(tlslite.constants.HandshakeType_attribute)                       o (tlslite.extensions.StatusRequestExtension_method)
     * certificate_type_(tlslite.messages.ServerHello_property)                             o (tlslite.extensions.TACKExtension_method)
     * certificate_types_(tlslite.messages.ClientHello_property)                            o (tlslite.extensions.TACKExtension.TACK_method)
@@ -328,52 +331,53 @@
     * ChaCha_(class_in_tlslite.utils.chacha)                                               o (tlslite.messages.ClientMasterKey_method)
     * CHACHA20_POLY1305_(class_in_tlslite.utils.chacha20_poly1305)                         o (tlslite.messages.EncryptedExtensions_method)
     * chacha20draft00Suites_(tlslite.constants.CipherSuite_attribute)                      o (tlslite.messages.Finished_method)
     * chacha20Suites_(tlslite.constants.CipherSuite_attribute)                             o (tlslite.messages.Heartbeat_method)
     * chacha_block()_(tlslite.utils.chacha.ChaCha_static_method)                           o (tlslite.messages.HelloRequest_method)
     * change_cipher_spec_(tlslite.constants.ContentType_attribute)                         o (tlslite.messages.KeyUpdate_method)
     * ChangeCipherSpec_(class_in_tlslite.messages)                                         o (tlslite.messages.NewSessionTicket_method)
-    * changeReadState()_(tlslite.recordlayer.RecordLayer_method)                           o (tlslite.messages.NextProtocol_method)
-    * changeWriteState()_(tlslite.recordlayer.RecordLayer_method)                          o (tlslite.messages.RecordHeader2_method)
-    * check()_(tlslite.basedb.BaseDB_method)                                               o (tlslite.messages.RecordHeader3_method)
-    * Checker_(class_in_tlslite.checker)                                                   o (tlslite.messages.ServerHello_method)
-    * checkTack()_(tlslite.x509certchain.X509CertChain_method)                             o (tlslite.messages.ServerHello2_method)
-    * CipherSuite_(class_in_tlslite.constants)                                             o (tlslite.messages.ServerHelloDone_method)
-    * clear_buffers()_(tlslite.defragmenter.Defragmenter_method)                           o (tlslite.messages.SessionTicketPayload_method)
-    * clearReadBuffer()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                     o (tlslite.messages.SSL2Finished_method)
-    * clearWriteBuffer()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                    o (tlslite.session.Session_method)
-    * client_cert_chain_(tlslite.messages.SessionTicketPayload_property)             * create_response()_(tlslite.messages.Heartbeat_method)
-    * client_certificate_(tlslite.constants.SSL2HandshakeType_attribute)             * create_tag()_(tlslite.utils.poly1305.Poly1305_method)
-    * client_finished_(tlslite.constants.SSL2HandshakeType_attribute)                * createAES()_(in_module_tlslite.utils.cipherfactory)
-    * client_hello_(tlslite.constants.HandshakeType_attribute)                       * createAESCCM()_(in_module_tlslite.utils.cipherfactory)
-          o (tlslite.constants.SSL2HandshakeType_attribute)                          * createAESCCM_8()_(in_module_tlslite.utils.cipherfactory)
-    * client_hello_padding_(tlslite.constants.ExtensionType_attribute)               * createAESCTR()_(in_module_tlslite.utils.cipherfactory)
-    * client_key_exchange_(tlslite.constants.HandshakeType_attribute)                * createAESGCM()_(in_module_tlslite.utils.cipherfactory)
-    * client_master_key_(tlslite.constants.SSL2HandshakeType_attribute)              * createCHACHA20()_(in_module_tlslite.utils.cipherfactory)
-    * clientCertFaults_(tlslite.constants.Fault_attribute)                           * createDateClass()_(in_module_tlslite.utils.datefuncs)
-    * ClientCertificateType_(class_in_tlslite.constants)                             * createDH()_(tlslite.messages.ClientKeyExchange_method)
-    * ClientCertTypeExtension_(class_in_tlslite.extensions)                                o (tlslite.messages.ServerKeyExchange_method)
-    * ClientFinished_(class_in_tlslite.messages)                                     * createECDH()_(tlslite.messages.ClientKeyExchange_method)
-    * ClientHello_(class_in_tlslite.messages)                                              o (tlslite.messages.ServerKeyExchange_method)
-    * ClientHelper_(class_in_tlslite.integration.clienthelper)                       * createHMAC()_(in_module_tlslite.mathtls)
-    * ClientKeyExchange_(class_in_tlslite.messages)                                  * createMAC_SSL()_(in_module_tlslite.mathtls)
-    * ClientKeyShareExtension_(class_in_tlslite.extensions)                          * createRC4()_(in_module_tlslite.utils.cipherfactory)
-    * ClientMasterKey_(class_in_tlslite.messages)                                    * createRSA()_(tlslite.messages.ClientKeyExchange_method)
-    * clientNoAuthFaults_(tlslite.constants.Fault_attribute)                         * createSRP()_(tlslite.messages.ClientKeyExchange_method)
-    * clientSrpFaults_(tlslite.constants.Fault_attribute)                                  o (tlslite.messages.ServerKeyExchange_method)
-    * close()_(tlslite.bufferedsocket.BufferedSocket_method)                         * createTripleDES()_(in_module
-          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn       tlslite.utils.cipherfactory)
-            method)                                                                  * cswap()_(in_module_tlslite.utils.x25519)
-          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * ct_check_cbc_mac_and_pad()_(in_module
-    * close_notify_(tlslite.constants.AlertDescription_attribute)                      tlslite.utils.constanttime)
-    * closeAsync()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                    * ct_eq_u32()_(in_module_tlslite.utils.constanttime)
-    * compat26Str()_(in_module_tlslite.utils.compat)                                 * ct_gt_u32()_(in_module_tlslite.utils.constanttime)
-    * compat_b2a()_(in_module_tlslite.utils.compat)                                  * ct_isnonzero_u32()_(in_module
-    * compatAscii2Bytes()_(in_module_tlslite.utils.compat)                             tlslite.utils.constanttime)
-    * compatHMAC()_(in_module_tlslite.utils.compat)                                  * ct_le_u32()_(in_module_tlslite.utils.constanttime)
+    * changeReadState()_(tlslite.recordlayer.RecordLayer_method)                           o (tlslite.messages.NewSessionTicket1_0_method)
+    * changeWriteState()_(tlslite.recordlayer.RecordLayer_method)                          o (tlslite.messages.NextProtocol_method)
+    * check()_(tlslite.basedb.BaseDB_method)                                               o (tlslite.messages.RecordHeader2_method)
+    * Checker_(class_in_tlslite.checker)                                                   o (tlslite.messages.RecordHeader3_method)
+    * checkTack()_(tlslite.x509certchain.X509CertChain_method)                             o (tlslite.messages.ServerHello_method)
+    * CipherSuite_(class_in_tlslite.constants)                                             o (tlslite.messages.ServerHello2_method)
+    * clear_buffers()_(tlslite.defragmenter.Defragmenter_method)                           o (tlslite.messages.ServerHelloDone_method)
+    * clearReadBuffer()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                     o (tlslite.messages.SessionTicketPayload_method)
+    * clearWriteBuffer()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                    o (tlslite.messages.SSL2Finished_method)
+    * client_cert_chain_(tlslite.messages.SessionTicketPayload_property)                   o (tlslite.session.Session_method)
+    * client_certificate_(tlslite.constants.SSL2HandshakeType_attribute)             * create_response()_(tlslite.messages.Heartbeat_method)
+    * client_finished_(tlslite.constants.SSL2HandshakeType_attribute)                * create_tag()_(tlslite.utils.poly1305.Poly1305_method)
+    * client_hello_(tlslite.constants.HandshakeType_attribute)                       * createAES()_(in_module_tlslite.utils.cipherfactory)
+          o (tlslite.constants.SSL2HandshakeType_attribute)                          * createAESCCM()_(in_module_tlslite.utils.cipherfactory)
+    * client_hello_padding_(tlslite.constants.ExtensionType_attribute)               * createAESCCM_8()_(in_module_tlslite.utils.cipherfactory)
+    * client_key_exchange_(tlslite.constants.HandshakeType_attribute)                * createAESCTR()_(in_module_tlslite.utils.cipherfactory)
+    * client_master_key_(tlslite.constants.SSL2HandshakeType_attribute)              * createAESGCM()_(in_module_tlslite.utils.cipherfactory)
+    * clientCertFaults_(tlslite.constants.Fault_attribute)                           * createCHACHA20()_(in_module_tlslite.utils.cipherfactory)
+    * ClientCertificateType_(class_in_tlslite.constants)                             * createDateClass()_(in_module_tlslite.utils.datefuncs)
+    * ClientCertTypeExtension_(class_in_tlslite.extensions)                          * createDH()_(tlslite.messages.ClientKeyExchange_method)
+    * ClientFinished_(class_in_tlslite.messages)                                           o (tlslite.messages.ServerKeyExchange_method)
+    * ClientHello_(class_in_tlslite.messages)                                        * createECDH()_(tlslite.messages.ClientKeyExchange_method)
+    * ClientHelper_(class_in_tlslite.integration.clienthelper)                             o (tlslite.messages.ServerKeyExchange_method)
+    * ClientKeyExchange_(class_in_tlslite.messages)                                  * createHMAC()_(in_module_tlslite.mathtls)
+    * ClientKeyShareExtension_(class_in_tlslite.extensions)                          * createMAC_SSL()_(in_module_tlslite.mathtls)
+    * ClientMasterKey_(class_in_tlslite.messages)                                    * createRC4()_(in_module_tlslite.utils.cipherfactory)
+    * clientNoAuthFaults_(tlslite.constants.Fault_attribute)                         * createRSA()_(tlslite.messages.ClientKeyExchange_method)
+    * clientSrpFaults_(tlslite.constants.Fault_attribute)                            * createSRP()_(tlslite.messages.ClientKeyExchange_method)
+    * close()_(tlslite.bufferedsocket.BufferedSocket_method)                               o (tlslite.messages.ServerKeyExchange_method)
+          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn     * createTripleDES()_(in_module
+            method)                                                                    tlslite.utils.cipherfactory)
+          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * cswap()_(in_module_tlslite.utils.x25519)
+    * close_notify_(tlslite.constants.AlertDescription_attribute)                    * ct_check_cbc_mac_and_pad()_(in_module
+    * closeAsync()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)                      tlslite.utils.constanttime)
+    * compat26Str()_(in_module_tlslite.utils.compat)                                 * ct_eq_u32()_(in_module_tlslite.utils.constanttime)
+    * compat_b2a()_(in_module_tlslite.utils.compat)                                  * ct_gt_u32()_(in_module_tlslite.utils.constanttime)
+    * compatAscii2Bytes()_(in_module_tlslite.utils.compat)                           * ct_isnonzero_u32()_(in_module
+    * compatHMAC()_(in_module_tlslite.utils.compat)                                    tlslite.utils.constanttime)
+    * compatLong()_(in_module_tlslite.utils.compat)                                  * ct_le_u32()_(in_module_tlslite.utils.constanttime)
                                                                                      * ct_lsb_prop_u16()_(in_module_tlslite.utils.constanttime)
                                                                                      * ct_lsb_prop_u8()_(in_module_tlslite.utils.constanttime)
                                                                                      * ct_lt_u32()_(in_module_tlslite.utils.constanttime)
                                                                                      * ct_neq_u32()_(in_module_tlslite.utils.constanttime)
                                                                                      * CustomNameExtension_(class_in_tlslite.extensions)
 ***** D *****
                                                                      * dePem()_(in_module_tlslite.utils.pem)
@@ -410,25 +414,25 @@
     * decryption_failed_(tlslite.constants.AlertDescription          * dsa_sha512_(tlslite.constants.SignatureScheme_attribute)
       attribute)                                                     * dss_fixed_dh_(tlslite.constants.ClientCertificateType
     * Defragmenter_(class_in_tlslite.defragmenter)                     attribute)
                                                                      * dss_sign_(tlslite.constants.ClientCertificateType
                                                                        attribute)
 ***** E *****
     * early_data_(tlslite.constants.ExtensionType_attribute)
-    * early_data_ok_(tlslite.recordlayer.RecordLayer_property)
-    * ec_point_formats_(tlslite.constants.ExtensionType
-      attribute)                                                     * encrypt_then_mac_(tlslite.constants.ExtensionType
+    * early_data_ok_(tlslite.recordlayer.RecordLayer_property)       * encrypt_then_mac_(tlslite.constants.ExtensionType
+    * ec_point_formats_(tlslite.constants.ExtensionType                attribute)
+      attribute)                                                     * encrypted_extensions_(tlslite.constants.HandshakeType
     * ECCurveType_(class_in_tlslite.constants)                         attribute)
-    * ecdhAllSuites_(tlslite.constants.CipherSuite_attribute)        * encrypted_extensions_(tlslite.constants.HandshakeType
-    * ecdhAnonSuites_(tlslite.constants.CipherSuite_attribute)         attribute)
-    * ECDHE_RSAKeyExchange_(class_in_tlslite.keyexchange)            * EncryptedExtensions_(class_in_tlslite.messages)
-    * ecdheCertSuites_(tlslite.constants.CipherSuite_attribute)      * EncryptionError
-    * ecdheEcdsaSuites_(tlslite.constants.CipherSuite_attribute)     * encryptThenMAC_(tlslite.recordlayer.RecordLayer
-    * ECDHKeyExchange_(class_in_tlslite.keyexchange)                   property)
-    * ecdsa_(tlslite.constants.SignatureAlgorithm_attribute)               o (tlslite.tlsrecordlayer.TLSRecordLayer_property)
+    * ecdhAllSuites_(tlslite.constants.CipherSuite_attribute)        * EncryptedExtensions_(class_in_tlslite.messages)
+    * ecdhAnonSuites_(tlslite.constants.CipherSuite_attribute)       * EncryptionError
+    * ECDHE_RSAKeyExchange_(class_in_tlslite.keyexchange)            * encryptThenMAC_(tlslite.recordlayer.RecordLayer
+    * ecdheCertSuites_(tlslite.constants.CipherSuite_attribute)        property)
+    * ecdheEcdsaSuites_(tlslite.constants.CipherSuite_attribute)           o (tlslite.tlsrecordlayer.TLSRecordLayer_property)
+    * ECDHKeyExchange_(class_in_tlslite.keyexchange)                 * end_of_early_data_(tlslite.constants.HandshakeType
+    * ecdsa_(tlslite.constants.SignatureAlgorithm_attribute)           attribute)
     * ecdsa_fixed_ecdh_(tlslite.constants.ClientCertificateType      * error_(tlslite.constants.SSL2HandshakeType_attribute)
       attribute)                                                     * explicit_char2_(tlslite.constants.ECCurveType
     * ecdsa_secp256r1_sha256_(tlslite.constants.SignatureScheme        attribute)
       attribute)                                                     * explicit_prime_(tlslite.constants.ECCurveType
     * ecdsa_secp384r1_sha384_(tlslite.constants.SignatureScheme        attribute)
       attribute)                                                     * export_restriction_(tlslite.constants.AlertDescription
     * ecdsa_secp521r1_sha512_(tlslite.constants.SignatureScheme        attribute)
@@ -443,62 +447,64 @@
     * ed25519_(tlslite.constants.SignatureAlgorithm_attribute)             o (tlslite.extensions.IntExtension_property)
           o (tlslite.constants.SignatureScheme_attribute)                  o (tlslite.extensions.NPNExtension_property)
     * ed448_(tlslite.constants.SignatureAlgorithm_attribute)               o (tlslite.extensions.PaddingExtension_property)
           o (tlslite.constants.SignatureScheme_attribute)                  o (tlslite.extensions.PreSharedKeyExtension
     * EMSA_PSS_encode()_(tlslite.utils.rsakey.RSAKey_method)                 property)
     * EMSA_PSS_verify()_(tlslite.utils.rsakey.RSAKey_method)               o (tlslite.extensions.ServerKeyShareExtension
     * encodeX962Point()_(in_module_tlslite.utils.ecc)                        property)
-    * EncodingError                                                        o (tlslite.extensions.SNIExtension_property)
-    * encrypt()_(in_module_tlslite.utils.rijndael)                         o (tlslite.extensions.SRPExtension_property)
-          o (tlslite.utils.aes.AES_method)                                 o (tlslite.extensions.SrvSupportedVersionsExtension
-          o (tlslite.utils.chacha.ChaCha_method)                             property)
-          o (tlslite.utils.openssl_aes.OpenSSL_AES_method)                 o (tlslite.extensions.StatusRequestExtension
+    * EncodingError                                                        o (tlslite.extensions.SessionTicketExtension
+    * encrypt()_(in_module_tlslite.utils.rijndael)                           property)
+          o (tlslite.utils.aes.AES_method)                                 o (tlslite.extensions.SNIExtension_property)
+          o (tlslite.utils.chacha.ChaCha_method)                           o (tlslite.extensions.SRPExtension_property)
+          o (tlslite.utils.openssl_aes.OpenSSL_AES_method)                 o (tlslite.extensions.SrvSupportedVersionsExtension
           o (tlslite.utils.openssl_aes.OpenSSL_CTR_method)                   property)
-          o (tlslite.utils.openssl_rc4.OpenSSL_RC4_method)                 o (tlslite.extensions.TACKExtension_property)
-          o (tlslite.utils.openssl_tripledes.OpenSSL_TripleDES             o (tlslite.extensions.TLSExtension_property)
-            method)                                                        o (tlslite.extensions.VarBytesExtension_property)
-          o (tlslite.utils.pycrypto_aes.PyCrypto_AES_method)               o (tlslite.extensions.VarListExtension_property)
-          o (tlslite.utils.pycrypto_rc4.PyCrypto_RC4_method)               o (tlslite.extensions.VarSeqListExtension_property)
-          o (tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES     * extended_master_secret_(tlslite.constants.ExtensionType
-            method)                                                    attribute)
-          o (tlslite.utils.python_aes.Python_AES_method)             * extended_random_(tlslite.constants.ExtensionType
+          o (tlslite.utils.openssl_rc4.OpenSSL_RC4_method)                 o (tlslite.extensions.StatusRequestExtension
+          o (tlslite.utils.openssl_tripledes.OpenSSL_TripleDES               property)
+            method)                                                        o (tlslite.extensions.TACKExtension_property)
+          o (tlslite.utils.pycrypto_aes.PyCrypto_AES_method)               o (tlslite.extensions.TLSExtension_property)
+          o (tlslite.utils.pycrypto_rc4.PyCrypto_RC4_method)               o (tlslite.extensions.VarBytesExtension_property)
+          o (tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES           o (tlslite.extensions.VarListExtension_property)
+            method)                                                        o (tlslite.extensions.VarSeqListExtension_property)
+          o (tlslite.utils.python_aes.Python_AES_method)             * extended_master_secret_(tlslite.constants.ExtensionType
           o (tlslite.utils.python_rc4.Python_RC4_method)               attribute)
-          o (tlslite.utils.rc4.RC4_method)                           * ExtensionType_(class_in_tlslite.constants)
-          o (tlslite.utils.rijndael.Rijndael_method)
-          o (tlslite.utils.rsakey.RSAKey_method)
+          o (tlslite.utils.rc4.RC4_method)                           * extended_random_(tlslite.constants.ExtensionType
+          o (tlslite.utils.rijndael.Rijndael_method)                   attribute)
+          o (tlslite.utils.rsakey.RSAKey_method)                     * ExtensionType_(class_in_tlslite.constants)
           o (tlslite.utils.tripledes.TripleDES_method)
 ***** F *****
     * fatal_
       (tlslite.constants.AlertLevel
       attribute)
     * Fault_(class_in
       tlslite.constants)
     * faultAlerts_
-      (tlslite.constants.Fault          * FFDHKeyExchange_(class_in_tlslite.keyexchange)
+      (tlslite.constants.Fault
       attribute)                        * fileno()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)
     * faultNames_                       * filter_for_certificate()_(tlslite.constants.CipherSuite_static
       (tlslite.constants.Fault            method)
-      attribute)                        * filterForVersion()_(tlslite.constants.CipherSuite_static
+      attribute)                        * filter_for_prfs()_(tlslite.constants.CipherSuite_static
     * ffdhe2048_                          method)
-      (tlslite.constants.GroupName      * finish_request()_
-      attribute)                          (tlslite.integration.tlssocketservermixin.TLSSocketServerMixIn
-    * ffdhe3072_                          method)
-      (tlslite.constants.GroupName      * Finished_(class_in_tlslite.messages)
-      attribute)                        * finished_(tlslite.constants.HandshakeType_attribute)
-    * ffdhe4096_                        * flush()_(tlslite.bufferedsocket.BufferedSocket_method)
-      (tlslite.constants.GroupName            o (tlslite.messagesocket.MessageSocket_method)
-      attribute)                        * flushBlocking()_(tlslite.messagesocket.MessageSocket_method)
-    * ffdhe6144_                        * formatExceptionTrace()_(in_module_tlslite.utils.compat)
-      (tlslite.constants.GroupName
-      attribute)
+      (tlslite.constants.GroupName      * filterForVersion()_(tlslite.constants.CipherSuite_static
+      attribute)                          method)
+    * ffdhe3072_                        * finish_request()_
+      (tlslite.constants.GroupName        (tlslite.integration.tlssocketservermixin.TLSSocketServerMixIn
+      attribute)                          method)
+    * ffdhe4096_                        * Finished_(class_in_tlslite.messages)
+      (tlslite.constants.GroupName      * finished_(tlslite.constants.HandshakeType_attribute)
+      attribute)                        * flush()_(tlslite.bufferedsocket.BufferedSocket_method)
+    * ffdhe6144_                              o (tlslite.messagesocket.MessageSocket_method)
+      (tlslite.constants.GroupName      * flushBlocking()_(tlslite.messagesocket.MessageSocket_method)
+      attribute)                        * formatExceptionTrace()_(in_module_tlslite.utils.compat)
     * ffdhe8192_
       (tlslite.constants.GroupName
       attribute)
     * FFDHE_PARAMETERS_(in_module
       tlslite.mathtls)
+    * FFDHKeyExchange_(class_in
+      tlslite.keyexchange)
 ***** G *****
                                                                * getFirstMatching()_(in_module
                                                                  tlslite.utils.lists)
                                                                * getFixBytes()_(tlslite.utils.codec.Parser
                                                                  method)
                                                                * getFixList()_(tlslite.utils.codec.Parser
                                                                  method)
@@ -618,21 +624,22 @@
                                                                                  (tlslite.extensions.SNIExtension
                                                                                  property)
                                                                                * HRRKeyShareExtension_(class_in
                                                                                  tlslite.extensions)
                                                                                * HTTPTLSConnection_(class_in
                                                                                  tlslite.integration.httptlsconnection)
 ***** I *****
-    * ietfNames_(tlslite.constants.CipherSuite_attribute)
-    * illegal_parameter_(tlslite.constants.AlertDescription        * intrinsic_(tlslite.constants.HashAlgorithm_attribute)
-      attribute)                                                   * InvalidSignature
-    * IMAP4_TLS_(class_in_tlslite.integration.imap4_tls)           * invMod()_(in_module_tlslite.utils.cryptomath)
-    * inappropriate_fallback_                                      * inWriteEvent()_
-      (tlslite.constants.AlertDescription_attribute)                 (tlslite.integration.asyncstatemachine.AsyncStateMachine
-    * inReadEvent()_                                                 method)
+    * i_(tlslite.constants.CipherSuite_attribute)
+    * ietfNames_(tlslite.constants.CipherSuite_attribute)          * intrinsic_(tlslite.constants.HashAlgorithm_attribute)
+    * illegal_parameter_(tlslite.constants.AlertDescription        * InvalidSignature
+      attribute)                                                   * invMod()_(in_module_tlslite.utils.cryptomath)
+    * IMAP4_TLS_(class_in_tlslite.integration.imap4_tls)           * inWriteEvent()_
+    * inappropriate_fallback_                                        (tlslite.integration.asyncstatemachine.AsyncStateMachine
+      (tlslite.constants.AlertDescription_attribute)                 method)
+    * inReadEvent()_                                               * is_empty()_(tlslite.defragmenter.Defragmenter_method)
       (tlslite.integration.asyncstatemachine.AsyncStateMachine     * is_valid_hostname()_(in_module_tlslite.utils.dns_utils)
       method)                                                      * isCBCMode()_(tlslite.recordlayer.RecordLayer_method)
     * insufficient_security_                                       * isDateClassBefore()_(in_module_tlslite.utils.datefuncs)
       (tlslite.constants.AlertDescription_attribute)               * isDateClassExpired()_(in_module_tlslite.utils.datefuncs)
     * int_to_bytes()_(in_module_tlslite.utils.compat)              * isPrime()_(in_module_tlslite.utils.cryptomath)
     * internal_error_(tlslite.constants.AlertDescription           * IV_(tlslite.utils.openssl_aes.OpenSSL_AES_property)
       attribute)
@@ -776,45 +783,45 @@
           o tlslite.utils.tlshashlib
           o tlslite.utils.tripledes
           o tlslite.utils.x25519
           o tlslite.verifierdb
           o tlslite.x509
           o tlslite.x509certchain
 ***** N *****
-                                                        * new_session_ticket_
-                                                          (tlslite.constants.HandshakeType_attribute)
                                                         * NewSessionTicket_(class_in_tlslite.messages)
+                                                        * NewSessionTicket1_0_(class_in
+                                                          tlslite.messages)
                                                         * next_protocol_
-                                                          (tlslite.constants.HandshakeType_attribute)
-    * name_                                             * next_protos_(tlslite.messages.ServerHello
-      (tlslite.extensions.SNIExtension.ServerName         property)
-      attribute)                                        * next_protos_advertised_
-    * name_type_                                          (tlslite.messages.ServerHello_property)
-      (tlslite.extensions.SNIExtension.ServerName       * NextProtocol_(class_in_tlslite.messages)
-      attribute)                                        * no_application_protocol_
-    * named_curve_(tlslite.constants.ECCurveType          (tlslite.constants.AlertDescription
-      attribute)                                          attribute)
-    * NameType_(class_in_tlslite.constants)             * no_certificate_
-    * new()_(in_module_tlslite.utils.openssl_aes)         (tlslite.constants.AlertDescription
-          o (in_module_tlslite.utils.openssl_rc4)         attribute)
-          o (in_module                                        o (tlslite.constants.SSL2ErrorDescription
-            tlslite.utils.openssl_tripledes)                    attribute)
-          o (in_module_tlslite.utils.pycrypto_aes)      * no_cipher_
-          o (in_module                                    (tlslite.constants.SSL2ErrorDescription
-            tlslite.utils.pycrypto_aesgcm)                attribute)
-          o (in_module_tlslite.utils.pycrypto_rc4)      * no_renegotiation_
-          o (in_module                                    (tlslite.constants.AlertDescription
-            tlslite.utils.pycrypto_tripledes)             attribute)
-          o (in_module_tlslite.utils.python_aes)        * none_(tlslite.constants.HashAlgorithm
-          o (in_module_tlslite.utils.python_aesgcm)       attribute)
-          o (in_module                                  * NPNExtension_(class_in_tlslite.extensions)
-            tlslite.utils.python_chacha20_poly1305)     * nullSuites_(tlslite.constants.CipherSuite
-          o (in_module_tlslite.utils.python_rc4)          attribute)
-          o (in_module_tlslite.utils.tlshashlib)        * num_to_16_le_bytes()_
-                                                          (tlslite.utils.poly1305.Poly1305_static
+    * name_                                               (tlslite.constants.HandshakeType_attribute)
+      (tlslite.extensions.SNIExtension.ServerName       * next_protos_(tlslite.messages.ServerHello
+      attribute)                                          property)
+    * name_type_                                        * next_protos_advertised_
+      (tlslite.extensions.SNIExtension.ServerName         (tlslite.messages.ServerHello_property)
+      attribute)                                        * NextProtocol_(class_in_tlslite.messages)
+    * named_curve_(tlslite.constants.ECCurveType        * no_application_protocol_
+      attribute)                                          (tlslite.constants.AlertDescription
+    * NameType_(class_in_tlslite.constants)               attribute)
+    * new()_(in_module_tlslite.utils.openssl_aes)       * no_certificate_
+          o (in_module_tlslite.utils.openssl_rc4)         (tlslite.constants.AlertDescription
+          o (in_module                                    attribute)
+            tlslite.utils.openssl_tripledes)                  o (tlslite.constants.SSL2ErrorDescription
+          o (in_module_tlslite.utils.pycrypto_aes)              attribute)
+          o (in_module                                  * no_cipher_
+            tlslite.utils.pycrypto_aesgcm)                (tlslite.constants.SSL2ErrorDescription
+          o (in_module_tlslite.utils.pycrypto_rc4)        attribute)
+          o (in_module                                  * no_renegotiation_
+            tlslite.utils.pycrypto_tripledes)             (tlslite.constants.AlertDescription
+          o (in_module_tlslite.utils.python_aes)          attribute)
+          o (in_module_tlslite.utils.python_aesgcm)     * none_(tlslite.constants.HashAlgorithm
+          o (in_module                                    attribute)
+            tlslite.utils.python_chacha20_poly1305)     * NPNExtension_(class_in_tlslite.extensions)
+          o (in_module_tlslite.utils.python_rc4)        * nullSuites_(tlslite.constants.CipherSuite
+          o (in_module_tlslite.utils.tlshashlib)          attribute)
+    * new_session_ticket_                               * num_to_16_le_bytes()_
+      (tlslite.constants.HandshakeType_attribute)         (tlslite.utils.poly1305.Poly1305_static
                                                           method)
                                                         * numberToByteArray()_(in_module
                                                           tlslite.utils.cryptomath)
                                                         * numberToMPI()_(in_module
                                                           tlslite.utils.cryptomath)
 ***** O *****
                                                                    * OpenSSL_RSAKey_(class_in_tlslite.utils.openssl_rsakey)
@@ -836,42 +843,42 @@
                                                                          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn
                                                                            method)
 ***** P *****
                                                                   * parseAsPublicKey()_(in_module
                                                                     tlslite.utils.keyfactory)
                                                                   * parseBinary()_(in_module_tlslite.dh)
                                                                         o (tlslite.x509.X509_method)
-                                                                  * parseDateClass()_(in_module
-                                                                    tlslite.utils.datefuncs)
-    * P_(tlslite.utils.poly1305.Poly1305_attribute)               * parsePEM()_
-    * P_hash()_(in_module_tlslite.mathtls)                          (tlslite.utils.python_rsakey.Python_RSAKey_static
-    * PAD()_(in_module_tlslite.mathtls)                             method)
-    * pad16()_                                                    * parsePEMKey()_(in_module_tlslite.utils.keyfactory)
-      (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305          * parsePemList()_
-      static_method)                                                (tlslite.x509certchain.X509CertChain_method)
-    * PaddingExtension_(class_in_tlslite.extensions)              * parsePrivateKey()_(in_module
-    * paramStrength()_(in_module_tlslite.mathtls)                   tlslite.utils.keyfactory)
-    * parse()_(in_module_tlslite.dh)                              * Parser_(class_in_tlslite.utils.codec)
-          o (tlslite.extensions.ALPNExtension_method)             * password_callback()_(in_module
-          o (tlslite.extensions.CertificateStatusExtension          tlslite.utils.openssl_rsakey)
+    * P_(tlslite.utils.poly1305.Poly1305_attribute)               * parseDateClass()_(in_module
+    * P_hash()_(in_module_tlslite.mathtls)                          tlslite.utils.datefuncs)
+    * PAD()_(in_module_tlslite.mathtls)                           * parsePEM()_
+    * pad16()_                                                      (tlslite.utils.python_rsakey.Python_RSAKey_static
+      (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305            method)
+      static_method)                                              * parsePEMKey()_(in_module_tlslite.utils.keyfactory)
+    * PaddingExtension_(class_in_tlslite.extensions)              * parsePemList()_
+    * paramStrength()_(in_module_tlslite.mathtls)                   (tlslite.x509certchain.X509CertChain_method)
+    * parse()_(in_module_tlslite.dh)                              * parsePrivateKey()_(in_module
+          o (tlslite.extensions.ALPNExtension_method)               tlslite.utils.keyfactory)
+          o (tlslite.extensions.CertificateStatusExtension        * Parser_(class_in_tlslite.utils.codec)
+            method)                                               * password_callback()_(in_module
+          o (tlslite.extensions.ClientKeyShareExtension             tlslite.utils.openssl_rsakey)
             method)                                               * PEER_ALLOWED_TO_SEND_
-          o (tlslite.extensions.ClientKeyShareExtension             (tlslite.constants.HeartbeatMode_attribute)
-            method)                                               * PEER_NOT_ALLOWED_TO_SEND_
           o (tlslite.extensions.CustomNameExtension_method)         (tlslite.constants.HeartbeatMode_attribute)
-          o (tlslite.extensions.HeartbeatExtension_method)        * pem()_(in_module_tlslite.utils.pem)
-          o (tlslite.extensions.HRRKeyShareExtension_method)      * pemSniff()_(in_module_tlslite.utils.pem)
-          o (tlslite.extensions.IntExtension_method)              * Poly1305_(class_in_tlslite.utils.poly1305)
-          o (tlslite.extensions.KeyShareEntry_method)             * poly1305_key_gen()_
-          o (tlslite.extensions.NPNExtension_method)                (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305
-          o (tlslite.extensions.PaddingExtension_method)            static_method)
-          o (tlslite.extensions.PreSharedKeyExtension_method)     * POP3_TLS_(class_in_tlslite.integration.pop3_tls)
-          o (tlslite.extensions.PskIdentity_method)               * post_handshake_auth_
-          o (tlslite.extensions.ServerCertTypeExtension             (tlslite.constants.ExtensionType_attribute)
+          o (tlslite.extensions.HeartbeatExtension_method)        * PEER_NOT_ALLOWED_TO_SEND_
+          o (tlslite.extensions.HRRKeyShareExtension_method)        (tlslite.constants.HeartbeatMode_attribute)
+          o (tlslite.extensions.IntExtension_method)              * pem()_(in_module_tlslite.utils.pem)
+          o (tlslite.extensions.KeyShareEntry_method)             * pemSniff()_(in_module_tlslite.utils.pem)
+          o (tlslite.extensions.NPNExtension_method)              * Poly1305_(class_in_tlslite.utils.poly1305)
+          o (tlslite.extensions.PaddingExtension_method)          * poly1305_key_gen()_
+          o (tlslite.extensions.PreSharedKeyExtension_method)       (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305
+          o (tlslite.extensions.PskIdentity_method)                 static_method)
+          o (tlslite.extensions.ServerCertTypeExtension           * POP3_TLS_(class_in_tlslite.integration.pop3_tls)
+            method)                                               * post_handshake_auth_
+          o (tlslite.extensions.ServerKeyShareExtension             (tlslite.constants.ExtensionType_attribute)
             method)                                               * postWrite()_(tlslite.messages.HandshakeMsg_method)
-          o (tlslite.extensions.ServerKeyShareExtension           * powMod()_(in_module_tlslite.utils.cryptomath)
+          o (tlslite.extensions.SessionTicketExtension            * powMod()_(in_module_tlslite.utils.cryptomath)
             method)                                               * pre_shared_key_(tlslite.constants.ExtensionType
           o (tlslite.extensions.SNIExtension_method)                attribute)
           o (tlslite.extensions.SRPExtension_method)              * PreSharedKeyExtension_(class_in
           o (tlslite.extensions.SrvSupportedVersionsExtension       tlslite.extensions)
             method)                                               * PRF()_(in_module_tlslite.mathtls)
           o (tlslite.extensions.StatusRequestExtension            * PRF_1_2()_(in_module_tlslite.mathtls)
             method)                                               * PRF_1_2_SHA384()_(in_module_tlslite.mathtls)
@@ -894,27 +901,27 @@
           o (tlslite.messages.ClientMasterKey_method)                   o (tlslite.keyexchange.SRPKeyExchange_method)
           o (tlslite.messages.EncryptedExtensions_method)         * protocol_version_
           o (tlslite.messages.Finished_method)                      (tlslite.constants.AlertDescription_attribute)
           o (tlslite.messages.Heartbeat_method)                   * psk_dhe_ke_(tlslite.constants.PskKeyExchangeMode
           o (tlslite.messages.HelloRequest_method)                  attribute)
           o (tlslite.messages.KeyUpdate_method)                   * psk_ke_(tlslite.constants.PskKeyExchangeMode
           o (tlslite.messages.NewSessionTicket_method)              attribute)
-          o (tlslite.messages.NextProtocol_method)                * psk_key_exchange_modes_
-          o (tlslite.messages.RecordHeader2_method)                 (tlslite.constants.ExtensionType_attribute)
-          o (tlslite.messages.RecordHeader3_method)               * psk_truncate()_(tlslite.messages.ClientHello
-          o (tlslite.messages.ServerHello_method)                   method)
-          o (tlslite.messages.ServerHello2_method)                * PskIdentity_(class_in_tlslite.extensions)
-          o (tlslite.messages.ServerHelloDone_method)             * PskKeyExchangeMode_(class_in_tlslite.constants)
-          o (tlslite.messages.ServerKeyExchange_method)           * PskKeyExchangeModesExtension_(class_in
-          o (tlslite.messages.SessionTicketPayload_method)          tlslite.extensions)
-          o (tlslite.messages.SSL2Finished_method)                * PyCrypto_AES_(class_in_tlslite.utils.pycrypto_aes)
-          o (tlslite.utils.openssl_rsakey.OpenSSL_RSAKey          * PyCrypto_RC4_(class_in_tlslite.utils.pycrypto_rc4)
-            static_method)                                        * PyCrypto_RSAKey_(class_in
-          o (tlslite.x509.X509_method)                              tlslite.utils.pycrypto_rsakey)
-                                                                  * PyCrypto_TripleDES_(class_in
+          o (tlslite.messages.NewSessionTicket1_0_method)         * psk_key_exchange_modes_
+          o (tlslite.messages.NextProtocol_method)                  (tlslite.constants.ExtensionType_attribute)
+          o (tlslite.messages.RecordHeader2_method)               * psk_truncate()_(tlslite.messages.ClientHello
+          o (tlslite.messages.RecordHeader3_method)                 method)
+          o (tlslite.messages.ServerHello_method)                 * PskIdentity_(class_in_tlslite.extensions)
+          o (tlslite.messages.ServerHello2_method)                * PskKeyExchangeMode_(class_in_tlslite.constants)
+          o (tlslite.messages.ServerHelloDone_method)             * PskKeyExchangeModesExtension_(class_in
+          o (tlslite.messages.ServerKeyExchange_method)             tlslite.extensions)
+          o (tlslite.messages.SessionTicketPayload_method)        * PyCrypto_AES_(class_in_tlslite.utils.pycrypto_aes)
+          o (tlslite.messages.SSL2Finished_method)                * PyCrypto_RC4_(class_in_tlslite.utils.pycrypto_rc4)
+          o (tlslite.utils.openssl_rsakey.OpenSSL_RSAKey          * PyCrypto_RSAKey_(class_in
+            static_method)                                          tlslite.utils.pycrypto_rsakey)
+          o (tlslite.x509.X509_method)                            * PyCrypto_TripleDES_(class_in
                                                                     tlslite.utils.pycrypto_tripledes)
                                                                   * Python_AES_(class_in_tlslite.utils.python_aes)
                                                                   * Python_RC4_(class_in_tlslite.utils.python_rc4)
                                                                   * Python_RSAKey_(class_in
                                                                     tlslite.utils.python_rsakey)
 ***** Q *****
                                        * queueMessage()_
@@ -998,19 +1005,23 @@
                                                                                      * RSAKeyExchange_(class_in
                                                                                        tlslite.keyexchange)
                                                                                      * RSASSA_PSS_sign()_
                                                                                        (tlslite.utils.rsakey.RSAKey_method)
                                                                                      * RSASSA_PSS_verify()_
                                                                                        (tlslite.utils.rsakey.RSAKey_method)
 ***** S *****
+                                                                                     * sha1_(tlslite.constants.HashAlgorithm
+                                                                                       attribute)
                                                                                      * SHA1()_(in_module_tlslite.utils.cryptomath)
                                                                                      * sha224_(tlslite.constants.HashAlgorithm
                                                                                        attribute)
                                                                                      * sha256_(tlslite.constants.HashAlgorithm
                                                                                        attribute)
+                                                                                     * sha256PrfSuites_
+                                                                                       (tlslite.constants.CipherSuite_attribute)
                                                                                      * sha256Suites_(tlslite.constants.CipherSuite
                                                                                        attribute)
                                                                                      * sha384_(tlslite.constants.HashAlgorithm
                                                                                        attribute)
                                                                                      * sha384PrfSuites_
                                                                                        (tlslite.constants.CipherSuite_attribute)
                                                                                      * sha384Suites_(tlslite.constants.CipherSuite
@@ -1026,92 +1037,92 @@
                                                                                        method)
                                                                                            o (tlslite.recordlayer.RecordLayer
                                                                                              method)
                                                                                            o (tlslite.tlsrecordlayer.TLSRecordLayer
                                                                                              method)
                                                                                      * sign()_(tlslite.utils.ecdsakey.ECDSAKey
                                                                                        method)
-                                                                                           o (tlslite.utils.rsakey.RSAKey_method)
-                                                                                     * signature_algorithms_
-                                                                                       (tlslite.constants.ExtensionType_attribute)
-    * seal()_(tlslite.utils.aesgcm.AESGCM_method)                                    * signature_algorithms_cert_
-          o (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305_method)                 (tlslite.constants.ExtensionType_attribute)
-    * secp160k1_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithm_(class_in
-    * secp160r1_(tlslite.constants.GroupName_attribute)                                tlslite.constants)
-    * secp160r2_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithmsCertExtension_(class_in
-    * secp192k1_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
-    * secp192r1_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithmsExtension_(class_in
-    * secp224k1_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
-    * secp224r1_(tlslite.constants.GroupName_attribute)                              * SignatureScheme_(class_in_tlslite.constants)
-    * secp256k1_(tlslite.constants.GroupName_attribute)                              * signServerKeyExchange()_
-    * secp256r1_(tlslite.constants.GroupName_attribute)                                (tlslite.keyexchange.KeyExchange_method)
-    * secp384r1_(tlslite.constants.GroupName_attribute)                              * skip_bytes()_(tlslite.utils.codec.Parser
-    * secp521r1_(tlslite.constants.GroupName_attribute)                                method)
-    * sect163k1_(tlslite.constants.GroupName_attribute)                              * SMTP_TLS_(class_in
-    * sect163r1_(tlslite.constants.GroupName_attribute)                                tlslite.integration.smtp_tls)
-    * sect163r2_(tlslite.constants.GroupName_attribute)                              * SNIExtension_(class_in_tlslite.extensions)
-    * sect193r1_(tlslite.constants.GroupName_attribute)                              * SNIExtension.ServerName_(class_in
-    * sect193r2_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
-    * sect233k1_(tlslite.constants.GroupName_attribute)                              * splitFirstByte()_
-    * sect233r1_(tlslite.constants.GroupName_attribute)                                (tlslite.messages.ApplicationData_method)
-    * sect239k1_(tlslite.constants.GroupName_attribute)                              * srp_(tlslite.constants.ExtensionType
-    * sect283k1_(tlslite.constants.GroupName_attribute)                                attribute)
-    * sect283r1_(tlslite.constants.GroupName_attribute)                              * srp_username_(tlslite.messages.ClientHello
-    * sect409k1_(tlslite.constants.GroupName_attribute)                                property)
-    * sect409r1_(tlslite.constants.GroupName_attribute)                              * srpAllSuites_(tlslite.constants.CipherSuite
-    * sect571k1_(tlslite.constants.GroupName_attribute)                                attribute)
-    * sect571r1_(tlslite.constants.GroupName_attribute)                              * srpCertSuites_(tlslite.constants.CipherSuite
-    * secureHash()_(in_module_tlslite.utils.cryptomath)                                attribute)
-    * secureHMAC()_(in_module_tlslite.utils.cryptomath)                              * srpDsaSuites_(tlslite.constants.CipherSuite
-    * send()_(tlslite.bufferedsocket.BufferedSocket_method)                            attribute)
-          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn     * SRPExtension_(class_in_tlslite.extensions)
-            method)                                                                  * SRPKeyExchange_(class_in
-          o (tlslite.recordlayer.RecordSocket_method)                                  tlslite.keyexchange)
-          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * srpSuites_(tlslite.constants.CipherSuite
-    * send_heartbeat_request()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)          attribute)
-    * send_keyupdate_request()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)        * SrvPreSharedKeyExtension_(class_in
-    * sendall()_(tlslite.bufferedsocket.BufferedSocket_method)                         tlslite.extensions)
-          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * SrvSupportedVersionsExtension_(class_in
-    * sendMessage()_(tlslite.messagesocket.MessageSocket_method)                       tlslite.extensions)
-    * sendMessageBlocking()_(tlslite.messagesocket.MessageSocket_method)             * ssl2_128Key_(tlslite.constants.CipherSuite
-    * sendRecord()_(tlslite.recordlayer.RecordLayer_method)                            attribute)
-    * server_finished_(tlslite.constants.SSL2HandshakeType_attribute)                * ssl2_192Key_(tlslite.constants.CipherSuite
-    * server_hello_(tlslite.constants.HandshakeType_attribute)                         attribute)
-          o (tlslite.constants.SSL2HandshakeType_attribute)                          * ssl2_3des_(tlslite.constants.CipherSuite
-    * server_hello_done_(tlslite.constants.HandshakeType_attribute)                    attribute)
-    * server_key_exchange_(tlslite.constants.HandshakeType_attribute)                * ssl2_64Key_(tlslite.constants.CipherSuite
-    * server_name_(tlslite.constants.ExtensionType_attribute)                          attribute)
-          o (tlslite.messages.ClientHello_property)                                  * ssl2des_(tlslite.constants.CipherSuite
-    * server_verify_(tlslite.constants.SSL2HandshakeType_attribute)                    attribute)
-    * ServerCertTypeExtension_(class_in_tlslite.extensions)                          * SSL2ErrorDescription_(class_in
-    * serverFaults_(tlslite.constants.Fault_attribute)                                 tlslite.constants)
-    * ServerFinished_(class_in_tlslite.messages)                                     * ssl2export_(tlslite.constants.CipherSuite
-    * ServerHello_(class_in_tlslite.messages)                                          attribute)
-    * ServerHello2_(class_in_tlslite.messages)                                       * SSL2Finished_(class_in_tlslite.messages)
-    * ServerHelloDone_(class_in_tlslite.messages)                                    * SSL2HandshakeType_(class_in
-    * ServerKeyExchange_(class_in_tlslite.messages)                                    tlslite.constants)
-    * ServerKeyShareExtension_(class_in_tlslite.extensions)                          * ssl2idea_(tlslite.constants.CipherSuite
-    * Session_(class_in_tlslite.session)                                               attribute)
-    * SessionCache_(class_in_tlslite.sessioncache)                                   * ssl2rc2_(tlslite.constants.CipherSuite
-    * SessionTicketPayload_(class_in_tlslite.messages)                                 attribute)
-    * setCloseOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine          * ssl2rc4_(tlslite.constants.CipherSuite
-      method)                                                                          attribute)
-    * setHandshakeOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine      * ssl3Suites_(tlslite.constants.CipherSuite
-      method)                                                                          attribute)
-    * setLengthCheck()_(tlslite.utils.codec.Parser_method)                           * SSL_CK_DES_192_EDE3_CBC_WITH_MD5_
-    * setServerHandshakeOp()_                                                          (tlslite.constants.CipherSuite_attribute)
-      (tlslite.integration.asyncstatemachine.AsyncStateMachine_method)               * SSL_CK_DES_64_CBC_WITH_MD5_
-    * setsockopt()_(tlslite.bufferedsocket.BufferedSocket_method)                      (tlslite.constants.CipherSuite_attribute)
-          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * SSL_CK_IDEA_128_CBC_WITH_MD5_
-    * settimeout()_(tlslite.bufferedsocket.BufferedSocket_method)                      (tlslite.constants.CipherSuite_attribute)
-          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * SSL_CK_RC2_128_CBC_EXPORT40_WITH_MD5_
-    * setup()_(tlslite.integration.xmlrpcserver.TLSXMLRPCRequestHandler_method)        (tlslite.constants.CipherSuite_attribute)
-    * setWriteOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine          * SSL_CK_RC2_128_CBC_WITH_MD5_
-      method)                                                                          (tlslite.constants.CipherSuite_attribute)
-    * sha1_(tlslite.constants.HashAlgorithm_attribute)                               * SSL_CK_RC4_128_EXPORT40_WITH_MD5_
+    * seal()_(tlslite.utils.aesgcm.AESGCM_method)                                          o (tlslite.utils.rsakey.RSAKey_method)
+          o (tlslite.utils.chacha20_poly1305.CHACHA20_POLY1305_method)               * signature_algorithms_
+    * secp160k1_(tlslite.constants.GroupName_attribute)                                (tlslite.constants.ExtensionType_attribute)
+    * secp160r1_(tlslite.constants.GroupName_attribute)                              * signature_algorithms_cert_
+    * secp160r2_(tlslite.constants.GroupName_attribute)                                (tlslite.constants.ExtensionType_attribute)
+    * secp192k1_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithm_(class_in
+    * secp192r1_(tlslite.constants.GroupName_attribute)                                tlslite.constants)
+    * secp224k1_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithmsCertExtension_(class_in
+    * secp224r1_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
+    * secp256k1_(tlslite.constants.GroupName_attribute)                              * SignatureAlgorithmsExtension_(class_in
+    * secp256r1_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
+    * secp384r1_(tlslite.constants.GroupName_attribute)                              * SignatureScheme_(class_in_tlslite.constants)
+    * secp521r1_(tlslite.constants.GroupName_attribute)                              * signServerKeyExchange()_
+    * sect163k1_(tlslite.constants.GroupName_attribute)                                (tlslite.keyexchange.KeyExchange_method)
+    * sect163r1_(tlslite.constants.GroupName_attribute)                              * skip_bytes()_(tlslite.utils.codec.Parser
+    * sect163r2_(tlslite.constants.GroupName_attribute)                                method)
+    * sect193r1_(tlslite.constants.GroupName_attribute)                              * SMTP_TLS_(class_in
+    * sect193r2_(tlslite.constants.GroupName_attribute)                                tlslite.integration.smtp_tls)
+    * sect233k1_(tlslite.constants.GroupName_attribute)                              * SNIExtension_(class_in_tlslite.extensions)
+    * sect233r1_(tlslite.constants.GroupName_attribute)                              * SNIExtension.ServerName_(class_in
+    * sect239k1_(tlslite.constants.GroupName_attribute)                                tlslite.extensions)
+    * sect283k1_(tlslite.constants.GroupName_attribute)                              * splitFirstByte()_
+    * sect283r1_(tlslite.constants.GroupName_attribute)                                (tlslite.messages.ApplicationData_method)
+    * sect409k1_(tlslite.constants.GroupName_attribute)                              * srp_(tlslite.constants.ExtensionType
+    * sect409r1_(tlslite.constants.GroupName_attribute)                                attribute)
+    * sect571k1_(tlslite.constants.GroupName_attribute)                              * srp_username_(tlslite.messages.ClientHello
+    * sect571r1_(tlslite.constants.GroupName_attribute)                                property)
+    * secureHash()_(in_module_tlslite.utils.cryptomath)                              * srpAllSuites_(tlslite.constants.CipherSuite
+    * secureHMAC()_(in_module_tlslite.utils.cryptomath)                                attribute)
+    * send()_(tlslite.bufferedsocket.BufferedSocket_method)                          * srpCertSuites_(tlslite.constants.CipherSuite
+          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn       attribute)
+            method)                                                                  * srpDsaSuites_(tlslite.constants.CipherSuite
+          o (tlslite.recordlayer.RecordSocket_method)                                  attribute)
+          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                           * SRPExtension_(class_in_tlslite.extensions)
+    * send_heartbeat_request()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)        * SRPKeyExchange_(class_in
+    * send_keyupdate_request()_(tlslite.tlsrecordlayer.TLSRecordLayer_method)          tlslite.keyexchange)
+    * sendall()_(tlslite.bufferedsocket.BufferedSocket_method)                       * srpSuites_(tlslite.constants.CipherSuite
+          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                             attribute)
+    * sendMessage()_(tlslite.messagesocket.MessageSocket_method)                     * SrvPreSharedKeyExtension_(class_in
+    * sendMessageBlocking()_(tlslite.messagesocket.MessageSocket_method)               tlslite.extensions)
+    * sendRecord()_(tlslite.recordlayer.RecordLayer_method)                          * SrvSupportedVersionsExtension_(class_in
+    * server_finished_(tlslite.constants.SSL2HandshakeType_attribute)                  tlslite.extensions)
+    * server_hello_(tlslite.constants.HandshakeType_attribute)                       * ssl2_128Key_(tlslite.constants.CipherSuite
+          o (tlslite.constants.SSL2HandshakeType_attribute)                            attribute)
+    * server_hello_done_(tlslite.constants.HandshakeType_attribute)                  * ssl2_192Key_(tlslite.constants.CipherSuite
+    * server_key_exchange_(tlslite.constants.HandshakeType_attribute)                  attribute)
+    * server_name_(tlslite.constants.ExtensionType_attribute)                        * ssl2_3des_(tlslite.constants.CipherSuite
+          o (tlslite.messages.ClientHello_property)                                    attribute)
+    * server_verify_(tlslite.constants.SSL2HandshakeType_attribute)                  * ssl2_64Key_(tlslite.constants.CipherSuite
+    * ServerCertTypeExtension_(class_in_tlslite.extensions)                            attribute)
+    * serverFaults_(tlslite.constants.Fault_attribute)                               * ssl2des_(tlslite.constants.CipherSuite
+    * ServerFinished_(class_in_tlslite.messages)                                       attribute)
+    * ServerHello_(class_in_tlslite.messages)                                        * SSL2ErrorDescription_(class_in
+    * ServerHello2_(class_in_tlslite.messages)                                         tlslite.constants)
+    * ServerHelloDone_(class_in_tlslite.messages)                                    * ssl2export_(tlslite.constants.CipherSuite
+    * ServerKeyExchange_(class_in_tlslite.messages)                                    attribute)
+    * ServerKeyShareExtension_(class_in_tlslite.extensions)                          * SSL2Finished_(class_in_tlslite.messages)
+    * Session_(class_in_tlslite.session)                                             * SSL2HandshakeType_(class_in
+    * session_ticket_(tlslite.constants.ExtensionType_attribute)                       tlslite.constants)
+    * SessionCache_(class_in_tlslite.sessioncache)                                   * ssl2idea_(tlslite.constants.CipherSuite
+    * SessionTicketExtension_(class_in_tlslite.extensions)                             attribute)
+    * SessionTicketPayload_(class_in_tlslite.messages)                               * ssl2rc2_(tlslite.constants.CipherSuite
+    * setCloseOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine            attribute)
+      method)                                                                        * ssl2rc4_(tlslite.constants.CipherSuite
+    * setHandshakeOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine        attribute)
+      method)                                                                        * ssl3Suites_(tlslite.constants.CipherSuite
+    * setLengthCheck()_(tlslite.utils.codec.Parser_method)                             attribute)
+    * setServerHandshakeOp()_                                                        * SSL_CK_DES_192_EDE3_CBC_WITH_MD5_
+      (tlslite.integration.asyncstatemachine.AsyncStateMachine_method)                 (tlslite.constants.CipherSuite_attribute)
+    * setsockopt()_(tlslite.bufferedsocket.BufferedSocket_method)                    * SSL_CK_DES_64_CBC_WITH_MD5_
+          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                             (tlslite.constants.CipherSuite_attribute)
+    * settimeout()_(tlslite.bufferedsocket.BufferedSocket_method)                    * SSL_CK_IDEA_128_CBC_WITH_MD5_
+          o (tlslite.tlsrecordlayer.TLSRecordLayer_method)                             (tlslite.constants.CipherSuite_attribute)
+    * setup()_(tlslite.integration.xmlrpcserver.TLSXMLRPCRequestHandler_method)      * SSL_CK_RC2_128_CBC_EXPORT40_WITH_MD5_
+    * setWriteOp()_(tlslite.integration.asyncstatemachine.AsyncStateMachine            (tlslite.constants.CipherSuite_attribute)
+      method)                                                                        * SSL_CK_RC2_128_CBC_WITH_MD5_
+                                                                                       (tlslite.constants.CipherSuite_attribute)
+                                                                                     * SSL_CK_RC4_128_EXPORT40_WITH_MD5_
                                                                                        (tlslite.constants.CipherSuite_attribute)
                                                                                      * SSL_CK_RC4_128_WITH_MD5_
                                                                                        (tlslite.constants.CipherSuite_attribute)
                                                                                      * startLengthCheck()_
                                                                                        (tlslite.utils.codec.Parser_method)
                                                                                      * starttls()_
                                                                                        (tlslite.integration.smtp_tls.SMTP_TLS
@@ -1144,14 +1155,15 @@
       attribute)
           o (tlslite.messages.ClientHello_property)
     * tackExt_(tlslite.messages.ServerHello_property)
     * TACKExtension_(class_in_tlslite.extensions)
     * TACKExtension.TACK_(class_in
       tlslite.extensions)
     * test()_(in_module_tlslite.utils.rijndael)
+    * Ticket_(class_in_tlslite.session)
     * time_stamp()_(in_module_tlslite.utils.compat)
     * tls12Suites_(tlslite.constants.CipherSuite
       attribute)
     * tls13record_(tlslite.recordlayer.RecordLayer
       property)
     * tls13Suites_(tlslite.constants.CipherSuite
       attribute)
@@ -1444,16 +1456,16 @@
     * unrecognized_name_                         * update_requested_
       (tlslite.constants.AlertDescription          (tlslite.constants.KeyUpdateMessageType
       attribute)                                   attribute)
     * unsupported_certificate_                   * user_canceled_
       (tlslite.constants.AlertDescription          (tlslite.constants.AlertDescription
       attribute)                                   attribute)
 ***** V *****
-                                                       * VerifierDB_(class_in_tlslite.verifierdb)
-    * valid()_(tlslite.session.Session_method)         * verify()_(tlslite.utils.ecdsakey.ECDSAKey
+    * valid()_(tlslite.session.Session_method)         * VerifierDB_(class_in_tlslite.verifierdb)
+          o (tlslite.session.Ticket_method)            * verify()_(tlslite.utils.ecdsakey.ECDSAKey
     * validate()_                                        method)
       (tlslite.handshakesettings.HandshakeSettings           o (tlslite.utils.rsakey.RSAKey_method)
       method)                                          * verify_binder()_
           o (tlslite.handshakesettings.Keypair           (tlslite.handshakehelpers.HandshakeHelpers
             method)                                      static_method)
           o (tlslite.handshakesettings.VirtualHost     * verifyServerKeyExchange()_
             method)                                      (tlslite.keyexchange.KeyExchange_static
@@ -1477,30 +1489,31 @@
     * write()_(tlslite.extensions.KeyShareEntry_method)
           o (tlslite.extensions.PskIdentity_method)
           o (tlslite.extensions.SNIExtension_method)
           o (tlslite.extensions.TACKExtension.TACK_method)
           o (tlslite.extensions.TLSExtension_method)
           o (tlslite.messages.Alert_method)
           o (tlslite.messages.ApplicationData_method)
-          o (tlslite.messages.Certificate_method)                              * write_heartbeat()_
-          o (tlslite.messages.CertificateEntry_method)                           (tlslite.tlsrecordlayer.TLSRecordLayer
-          o (tlslite.messages.CertificateRequest_method)                         method)
-          o (tlslite.messages.CertificateStatus_method)                        * writeAsync()_
-          o (tlslite.messages.CertificateVerify_method)                          (tlslite.tlsrecordlayer.TLSRecordLayer
-          o (tlslite.messages.ChangeCipherSpec_method)                           method)
-          o (tlslite.messages.ClientHello_method)                              * writeBytes()_(tlslite.x509.X509
-          o (tlslite.messages.ClientKeyExchange_method)                          method)
-          o (tlslite.messages.ClientMasterKey_method)                          * writeParams()_
-          o (tlslite.messages.EncryptedExtensions_method)                        (tlslite.messages.ServerKeyExchange
-          o (tlslite.messages.Finished_method)                                   method)
-          o (tlslite.messages.Heartbeat_method)                                * Writer_(class_in_tlslite.utils.codec)
-          o (tlslite.messages.HelloRequest_method)
+          o (tlslite.messages.Certificate_method)
+          o (tlslite.messages.CertificateEntry_method)                         * write_heartbeat()_
+          o (tlslite.messages.CertificateRequest_method)                         (tlslite.tlsrecordlayer.TLSRecordLayer
+          o (tlslite.messages.CertificateStatus_method)                          method)
+          o (tlslite.messages.CertificateVerify_method)                        * writeAsync()_
+          o (tlslite.messages.ChangeCipherSpec_method)                           (tlslite.tlsrecordlayer.TLSRecordLayer
+          o (tlslite.messages.ClientHello_method)                                method)
+          o (tlslite.messages.ClientKeyExchange_method)                        * writeBytes()_(tlslite.x509.X509
+          o (tlslite.messages.ClientMasterKey_method)                            method)
+          o (tlslite.messages.EncryptedExtensions_method)                      * writeParams()_
+          o (tlslite.messages.Finished_method)                                   (tlslite.messages.ServerKeyExchange
+          o (tlslite.messages.Heartbeat_method)                                  method)
+          o (tlslite.messages.HelloRequest_method)                             * Writer_(class_in_tlslite.utils.codec)
           o (tlslite.messages.KeyUpdate_method)
           o (tlslite.messages.Message_method)
           o (tlslite.messages.NewSessionTicket_method)
+          o (tlslite.messages.NewSessionTicket1_0_method)
           o (tlslite.messages.NextProtocol_method)
           o (tlslite.messages.RecordHeader2_method)
           o (tlslite.messages.RecordHeader3_method)
           o (tlslite.messages.ServerHello_method)
           o (tlslite.messages.ServerHello2_method)
           o (tlslite.messages.ServerHelloDone_method)
           o (tlslite.messages.ServerKeyExchange_method)
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/index.html` & `tlslite-ng-0.8.0a46/docs/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to tlslite-ng’s documentation! &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>Welcome to tlslite-ng’s documentation! &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/modules.html` & `tlslite-ng-0.8.0a46/docs/_build/html/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/py-modindex.html` & `tlslite-ng-0.8.0a46/docs/_build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>Python Module Index &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/search.html` & `tlslite-ng-0.8.0a46/docs/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>Search &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/searchindex.js` & `tlslite-ng-0.8.0a46/docs/_build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
         "handshakehelp": [1, 2],
         "handshakeset": [1, 2, 17, 18, 19, 20, 21, 25, 33, 34],
         "keyexchang": [1, 2],
         "mathtl": [1, 2],
         "messag": [1, 2, 7, 8, 10, 11, 12, 13, 14, 26, 27, 29, 30, 33, 34, 45, 47, 71],
         "messagesocket": [1, 2],
         "recordlay": [1, 2, 29],
-        "session": [1, 2, 6, 14, 21, 28, 32, 33, 34],
+        "session": [1, 2, 6, 11, 14, 21, 28, 32, 33, 34],
         "sessioncach": [1, 2, 23, 33],
         "tlsconnect": [1, 2, 6, 10, 17, 18, 19, 20, 21, 22, 23, 25, 31, 34],
         "tlsrecordlay": [1, 2, 33],
         "verifierdb": [1, 2, 4, 26, 33],
         "x509": [1, 2, 7, 14, 22, 23, 28, 78],
         "x509certchain": [1, 2, 17, 18, 19, 20, 21, 22, 23, 25, 28, 31, 33],
         "tl": [2, 7, 8, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 27, 28, 29, 30, 31, 32, 33, 34, 40, 42, 44, 51],
@@ -140,21 +140,21 @@
         "filenam": [4, 76],
         "type": [4, 7, 8, 9, 10, 11, 12, 14, 16, 17, 18, 19, 20, 21, 25, 26, 28, 29, 30, 31, 33, 34, 38, 41, 42, 44, 45, 48, 50, 51, 52, 55, 62, 71, 75, 76, 77, 78],
         "__contains__": 4,
         "usernam": [4, 7, 17, 18, 19, 20, 21, 25, 27, 28, 31, 33, 34, 76],
         "check": [4, 6, 8, 11, 14, 30, 33, 42, 44, 48, 52, 71],
         "databas": [4, 33, 76],
         "contain": [4, 11, 22, 28, 30, 31, 45, 50, 51, 52, 55, 57, 68, 71, 78],
-        "specifi": [4, 10, 11, 14, 18, 26, 27, 28, 30, 47, 50, 51, 55, 62, 71, 76],
+        "specifi": [4, 7, 10, 11, 14, 18, 26, 27, 28, 30, 47, 50, 51, 55, 62, 71, 76],
         "paramet": [4, 6, 7, 9, 10, 11, 12, 13, 14, 16, 17, 18, 19, 20, 21, 25, 26, 27, 28, 29, 30, 32, 33, 34, 38, 41, 42, 44, 45, 47, 48, 50, 51, 52, 55, 62, 71, 75, 76, 77, 78],
         "str": [4, 6, 10, 11, 12, 14, 16, 17, 18, 19, 20, 21, 23, 25, 26, 28, 30, 31, 33, 34, 41, 45, 47, 48, 50, 51, 52, 55, 62, 71, 76, 77, 78],
         "The": [4, 6, 7, 9, 10, 11, 14, 16, 17, 18, 19, 20, 21, 22, 25, 27, 28, 30, 31, 32, 33, 34, 42, 43, 45, 47, 50, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "return": [4, 5, 7, 8, 9, 11, 12, 14, 16, 23, 26, 27, 28, 29, 30, 31, 33, 34, 37, 38, 40, 41, 42, 43, 44, 45, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 66, 67, 68, 71, 75, 76, 77, 78],
-        "bool": [4, 6, 11, 14, 16, 17, 18, 25, 30, 31, 33, 34, 50, 51, 55, 62, 71],
-        "true": [4, 13, 14, 16, 17, 22, 23, 27, 30, 31, 33, 34, 41, 42, 44, 50, 51, 55, 68, 71],
+        "bool": [4, 6, 11, 14, 16, 17, 18, 25, 28, 30, 31, 33, 34, 50, 51, 55, 62, 71],
+        "true": [4, 8, 13, 14, 16, 17, 22, 23, 27, 30, 31, 33, 34, 41, 42, 44, 50, 51, 55, 68, 71],
         "fals": [4, 5, 6, 11, 14, 17, 18, 23, 25, 27, 28, 30, 31, 33, 34, 42, 43, 44, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "otherwis": [4, 7, 11, 22, 28, 44],
         "__delitem__": 4,
         "__getitem__": [4, 32],
         "__init__": [4, 5, 6, 8, 10, 11, 12, 14, 16, 17, 18, 19, 20, 22, 24, 25, 26, 28, 29, 30, 31, 32, 33, 34, 36, 37, 38, 39, 40, 42, 50, 53, 54, 55, 56, 58, 59, 61, 62, 63, 64, 67, 68, 69, 70, 71, 74, 76, 77, 78],
         "__setitem__": [4, 32, 76],
         "valu": [4, 5, 7, 11, 12, 13, 14, 26, 27, 28, 29, 30, 31, 33, 34, 38, 42, 43, 44, 45, 50, 51, 52, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 75, 76, 77, 78],
@@ -176,15 +176,15 @@
         "around": 5,
         "interfac": [5, 28, 70],
         "provid": [5, 7, 11, 13, 26, 27, 28, 29, 30, 33, 34, 71],
         "buffer": [5, 8, 11, 22, 27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "read": [5, 16, 19, 22, 23, 28, 29, 30, 33, 34, 42],
         "write": [5, 11, 16, 22, 28, 29, 30, 33, 34, 42, 50, 55, 71],
         "real": 5,
-        "when": [5, 6, 10, 11, 14, 16, 17, 18, 22, 25, 27, 28, 30, 32, 33, 34, 51],
+        "when": [5, 6, 10, 11, 14, 16, 17, 18, 22, 25, 27, 28, 30, 31, 32, 33, 34, 51],
         "buffer_writ": 5,
         "enabl": [5, 14],
         "won": [5, 11, 17, 22, 34, 47],
         "t": [5, 6, 7, 10, 11, 14, 17, 22, 26, 33, 34, 42, 47, 50, 71],
         "pass": [5, 6, 10, 11, 16, 22, 25, 29, 30, 32, 33, 43, 50, 51, 55, 62, 71, 76],
         "until": [5, 33, 34],
         "flush": [5, 29],
@@ -197,19 +197,19 @@
         "whether": [5, 11, 14, 16, 27, 28, 30, 31, 33, 34, 42, 43, 45, 50, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "data": [5, 7, 8, 9, 10, 11, 12, 14, 16, 28, 29, 30, 31, 33, 34, 37, 39, 40, 42, 44, 45, 49, 50, 58, 68, 70, 71],
         "default": [5, 6, 7, 14, 26, 27, 28, 29, 31, 32, 33, 34, 42, 43, 45, 51, 52, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 70, 71, 76, 77, 78],
         "associ": [5, 13, 14, 28, 33, 34, 40, 68, 76],
         "close": [5, 10, 16, 22, 30, 33, 34, 39, 44],
         "underli": [5, 10, 16, 30, 34],
         "send": [5, 11, 14, 18, 19, 22, 26, 28, 29, 30, 33, 34],
-        "all": [5, 7, 8, 10, 11, 12, 14, 22, 26, 27, 28, 34, 42, 43, 44, 47, 55, 57, 62, 70, 71],
+        "all": [5, 7, 8, 10, 11, 12, 14, 22, 26, 27, 28, 31, 34, 42, 43, 44, 47, 55, 57, 62, 70, 71],
         "getpeernam": [5, 34],
         "remot": [5, 7, 10, 11, 19, 26, 34],
         "address": [5, 17, 34],
-        "which": [5, 6, 7, 8, 11, 13, 14, 17, 18, 19, 20, 21, 22, 25, 26, 27, 29, 33, 34, 38, 42, 45, 50, 57, 71, 76],
+        "which": [5, 6, 7, 8, 11, 13, 14, 17, 18, 19, 20, 21, 22, 25, 26, 27, 29, 31, 33, 34, 38, 42, 45, 50, 57, 71, 76],
         "connect": [5, 6, 10, 11, 14, 17, 18, 19, 20, 21, 22, 23, 24, 25, 27, 28, 30, 31, 33, 34],
         "emul": [5, 34],
         "getsocknam": [5, 34],
         "own": [5, 34],
         "gettimeout": [5, 34],
         "timeout": [5, 18, 19, 20, 21, 34],
         "recv": [5, 22, 30, 34],
@@ -239,20 +239,20 @@
         "complet": [6, 8, 10, 11, 16, 22, 23, 28, 33, 34],
         "successfulli": 6,
         "judg": 6,
         "miss": 6,
         "inadequ": [6, 10],
         "subclass": [6, 10, 11, 16, 22, 34],
         "tlsauthenticationerror": [6, 10, 33],
-        "current": [6, 14, 26, 30, 42, 47],
+        "current": [6, 14, 26, 30, 31, 42, 47],
         "an": [6, 7, 10, 11, 14, 16, 17, 18, 19, 20, 21, 22, 25, 27, 28, 30, 31, 33, 34, 38, 41, 42, 43, 44, 45, 50, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 66, 67, 68, 71, 76, 77, 78],
         "x": [6, 27, 33, 39, 42, 43, 77, 78],
         "509": [6, 33, 45, 77, 78],
         "__call__": 6,
-        "end": [6, 11, 27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
+        "end": [6, 7, 11, 27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "examin": [6, 33],
         "bad": [6, 7, 10, 30, 42],
         "instanc": [6, 11, 12, 22, 25, 28, 30, 32, 33, 47, 76, 78],
         "must": [6, 10, 11, 14, 22, 27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 70, 71, 76, 77, 78],
         "argument": [6, 11, 16, 17, 18, 19, 20, 21, 23, 25, 27, 28, 31, 33, 34, 42, 43, 45, 47, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "combin": [6, 17, 18, 19, 20, 21, 22, 25, 33],
         "A": [6, 7, 10, 16, 17, 27, 31, 33, 34, 41, 50, 51, 55, 70, 71, 76, 77, 78],
@@ -262,17 +262,17 @@
         "fingerprint": [6, 10, 77, 78],
         "match": [6, 7, 10, 11, 14, 28, 33, 42, 50, 52, 71],
         "resum": [6, 31, 33, 34],
         "should": [6, 8, 10, 11, 13, 14, 16, 17, 18, 19, 20, 21, 25, 27, 28, 30, 33, 34, 51, 75],
         "theori": 6,
         "wa": [6, 7, 10, 11, 28, 29, 30, 31, 33, 34, 42, 47, 50],
         "onc": [6, 10, 30],
-        "we": [6, 8, 14, 28, 30, 34],
+        "we": [6, 8, 14, 28, 30, 31, 34],
         "don": [6, 11, 14, 26, 42, 50, 71],
-        "need": [6, 8, 11, 14, 17, 18, 25, 26, 27, 29, 30],
+        "need": [6, 8, 11, 14, 17, 18, 25, 26, 27, 29, 30, 31],
         "bother": 6,
         "re": [6, 33, 34],
         "alertdescript": [7, 10],
         "tlsenum": [7, 11],
         "bad_record_mac": 7,
         "record": [7, 10, 11, 14, 16, 22, 28, 29, 30, 31, 34, 42],
         "fail": [7, 10, 30, 34, 71],
@@ -310,15 +310,15 @@
         "exampl": [7, 11, 16, 22, 23, 27, 28, 31, 33, 34, 42, 43, 45, 47, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "protocol_vers": [7, 14, 28],
         "version": [7, 11, 12, 14, 17, 18, 19, 20, 21, 25, 26, 27, 28, 30, 33, 34, 43, 44],
         "unaccept": 7,
         "couldn": 7,
         "agre": 7,
         "user_cancel": 7,
-        "being": [7, 34, 42],
+        "being": [7, 14, 34, 42],
         "cancel": 7,
         "reason": 7,
         "access_deni": 7,
         "49": 7,
         "bad_certif": 7,
         "42": 7,
         "bad_certificate_hash_valu": 7,
@@ -381,21 +381,21 @@
         "unsupported_extens": 7,
         "110": 7,
         "90": 7,
         "alertlevel": [7, 10],
         "enumer": [7, 42, 52],
         "protocol": [7, 11, 12, 14, 26, 27, 28, 29, 30, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 75, 76, 77, 78],
         "fatal": 7,
-        "2": [7, 11, 14, 26, 27, 28, 29, 30, 34, 38, 42, 45],
+        "2": [7, 11, 14, 26, 27, 28, 29, 30, 31, 34, 38, 42, 45],
         "warn": [7, 47],
         "1": [7, 9, 11, 13, 14, 27, 28, 29, 30, 31, 33, 34, 38, 42, 44, 45, 71, 77],
         "algorithmoid": 7,
         "algorithm": [7, 10, 11, 14, 26, 27, 28, 41, 45, 50, 71, 77],
         "oid": 7,
-        "defin": [7, 11, 23, 27, 28, 33],
+        "defin": [7, 11, 23, 27, 28, 31, 33],
         "rfc5758": 7,
         "ecdsa": [7, 14, 50, 77],
         "rfc5754": 7,
         "sha": [7, 14],
         "rfc3447": 7,
         "rss": 7,
         "pss": [7, 14, 55, 62, 68, 71, 77],
@@ -762,14 +762,15 @@
         "maxvers": [7, 14],
         "copi": [7, 12, 14, 27],
         "without": [7, 10, 11, 26, 28, 31, 33, 34],
         "incompat": [7, 47],
         "filter_for_certif": 7,
         "cert_chain": [7, 22, 23, 28],
         "cert": [7, 11, 14, 78],
+        "filter_for_prf": 7,
         "classmethod": [7, 39, 71],
         "getanonsuit": 7,
         "getcertsuit": 7,
         "getdhecertsuit": 7,
         "getdhedsasuit": 7,
         "getecdhanonsuit": 7,
         "getecdhecertsuit": 7,
@@ -777,40 +778,44 @@
         "getsrpallsuit": 7,
         "getsrpcertsuit": 7,
         "getsrpdsasuit": 7,
         "getsrpsuit": 7,
         "gettls13suit": 7,
         "ar": [7, 8, 10, 11, 13, 14, 26, 27, 28, 30, 31, 33, 34, 42, 43, 45, 50, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 70, 71, 76, 77, 78],
         "specif": [7, 8, 10, 11, 17, 18, 19, 20, 21, 25, 30, 38, 42],
+        "i": [7, 11, 16, 27, 32, 33, 45, 51, 71, 77],
         "nullsuit": 7,
         "encrypt": [7, 10, 11, 14, 21, 28, 30, 31, 34, 36, 37, 39, 40, 50, 51, 53, 54, 55, 56, 59, 61, 63, 64, 67, 68, 69, 70, 71, 74],
         "stream": 7,
-        "tls1": [7, 11, 27, 28, 31, 45],
+        "sha256prfsuit": 7,
+        "up": [7, 8, 14, 28, 30, 34, 45],
+        "later": [7, 17, 18, 25, 26, 28],
         "sha384suit": 7,
         "384": 7,
         "srpdsasuit": 7,
         "ssl2_128kei": 7,
         "ssl2": [7, 28, 30],
         "ssl2_192kei": 7,
         "192": [7, 70],
         "ssl2_3de": 7,
         "ssl2_64kei": 7,
         "ssl2de": 7,
         "singl": [7, 11, 14, 22, 28, 29, 30, 33, 34, 39, 42, 44, 70],
         "de": 7,
         "ssl2export": 7,
-        "onli": [7, 10, 11, 14, 17, 18, 22, 25, 26, 28, 30, 33, 34, 47, 51, 55, 62, 68, 71],
+        "onli": [7, 10, 11, 14, 17, 18, 22, 25, 26, 28, 30, 31, 33, 34, 47, 51, 55, 62, 68, 71],
         "part": [7, 11, 26, 28, 68],
         "ssl2idea": 7,
         "idea": 7,
         "ssl2rc2": 7,
         "rc2": 7,
         "ssl2rc4": 7,
         "ssl3suit": 7,
         "ssl3": 7,
+        "tls1": [7, 11, 27, 28, 31, 45],
         "streamsuit": 7,
         "construct": [7, 34, 38],
         "tls12suit": 7,
         "tls13suit": 7,
         "clientcertificatetyp": 7,
         "dss_fixed_dh": 7,
         "dss_sign": 7,
@@ -852,28 +857,30 @@
         "cert_typ": [7, 11],
         "9": [7, 11, 57],
         "client_hello_pad": 7,
         "cooki": [7, 11],
         "early_data": [7, 14, 30],
         "ec_point_format": 7,
         "11": [7, 45],
-        "encrypt_then_mac": 7,
-        "extended_master_secret": 7,
+        "encrypt_then_mac": [7, 28],
+        "extended_master_secret": [7, 28],
         "extended_random": 7,
         "15": [7, 27],
         "key_shar": 7,
         "max_fragment_length": 7,
         "post_handshake_auth": 7,
         "pre_shared_kei": 7,
         "psk_key_exchange_mod": 7,
         "record_size_limit": [7, 11, 14, 34],
         "28": 7,
         "renegotiation_info": 7,
         "65281": 7,
         "server_nam": [7, 11, 14, 28],
+        "session_ticket": 7,
+        "35": 7,
         "signature_algorithm": 7,
         "signature_algorithms_cert": 7,
         "12": [7, 11, 41],
         "supported_group": [7, 14],
         "supported_vers": 7,
         "supports_npn": [7, 28],
         "13172": [7, 11],
@@ -963,28 +970,29 @@
         "handshaketyp": [7, 28],
         "certificate_request": 7,
         "certificate_statu": 7,
         "certificate_verifi": 7,
         "client_hello": [7, 13],
         "client_key_exchang": 7,
         "encrypted_extens": 7,
+        "end_of_early_data": 7,
         "hello_request": 7,
         "hello_retry_request": 7,
         "key_upd": 7,
         "message_hash": 7,
         "254": 7,
         "new_session_ticket": 7,
         "next_protocol": 7,
         "67": [7, 45],
         "server_hello": [7, 28],
         "server_hello_don": 7,
         "server_key_exchang": 7,
         "hashalgorithm": 7,
         "hash": [7, 12, 13, 14, 26, 27, 28, 31, 45, 50, 71],
-        "tlsv1": [7, 26, 28, 30],
+        "tlsv1": [7, 26, 28, 30, 31],
         "intrins": 7,
         "md5": [7, 14, 45, 73],
         "sha1": [7, 14, 45, 50, 71],
         "sha224": [7, 14],
         "sha512": [7, 14],
         "heartbeatmessagetyp": 7,
         "rfc": [7, 11, 14, 27, 28, 29, 33, 34, 39, 40, 58],
@@ -1057,32 +1065,31 @@
         "rsa_pss_sha512": 7,
         "differ": [7, 10, 11, 27, 29, 43],
         "enum": [7, 11],
         "found": [7, 10, 57],
         "tostr": 7,
         "human": [7, 11, 14, 28, 52],
         "readabl": [7, 11, 14, 16, 22, 28, 34, 52],
-        "possibl": [7, 11, 28, 29, 70],
+        "possibl": [7, 11, 28, 29, 31, 70],
         "helper": [8, 11, 13, 17, 26, 27, 34, 42, 52],
         "handl": [8, 9, 10, 11, 12, 17, 18, 19, 20, 21, 24, 25, 26, 28, 29, 30, 34, 42, 48, 51, 52, 73, 75],
         "fragment": [8, 29, 30, 34],
         "demultiplex": 8,
         "sinc": [8, 11, 28],
         "interleav": 8,
         "each": [8, 11, 33, 42, 57],
-        "cach": [8, 28, 32, 33],
+        "cach": [8, 28, 31, 32, 33],
         "ones": [8, 13, 14, 32],
         "order": [8, 11, 13, 14, 27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "urgenc": 8,
         "length": [8, 11, 14, 27, 28, 33, 34, 38, 42, 43, 45, 51, 55, 62, 70, 71, 76],
         "header": [8, 11, 28, 30, 34],
         "place": [8, 11, 22],
         "prioriti": 8,
         "decod": [8, 38, 42, 49, 57, 75],
-        "up": [8, 14, 28, 30, 34, 45],
         "empti": [8, 11, 14, 29, 30, 44, 52, 71, 77],
         "defregment": 8,
         "add_data": 8,
         "msg_type": [8, 28],
         "add": [8, 11, 12, 14, 22, 23, 28, 30, 34, 42, 71, 76],
         "add_dynamic_s": 8,
         "size_offset": 8,
@@ -1092,21 +1099,22 @@
         "add_static_s": 8,
         "same": [8, 11, 12, 13, 28, 29, 33, 34, 42],
         "clear_buff": 8,
         "remov": [8, 22, 43],
         "get_messag": 8,
         "extract": 8,
         "highest": [8, 14, 28],
+        "is_empti": 8,
         "file": [9, 11, 26, 34, 68],
         "pars": [9, 10, 11, 22, 23, 28, 38, 42, 50, 51, 55, 68, 71, 77, 78],
         "binari": [9, 11, 14, 42, 50],
         "either": [9, 11, 17, 18, 19, 20, 21, 25, 27, 28, 30, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "byte": [9, 11, 13, 14, 22, 26, 27, 28, 30, 31, 33, 34, 38, 41, 42, 43, 44, 45, 49, 50, 51, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 67, 68, 70, 71, 75, 76, 77, 78],
         "tupl": [9, 11, 14, 26, 27, 28, 29, 30, 34, 42, 44, 76],
-        "int": [9, 10, 11, 14, 18, 19, 20, 26, 27, 28, 29, 30, 32, 33, 34, 38, 42, 44, 45, 50, 51, 55, 62, 70, 71, 76, 78],
+        "int": [9, 10, 11, 14, 18, 19, 20, 26, 27, 28, 29, 30, 31, 32, 33, 34, 38, 42, 44, 45, 50, 51, 55, 62, 70, 71, 76, 78],
         "gener": [9, 11, 14, 16, 26, 28, 29, 30, 33, 34, 39, 40, 45, 50, 51, 55, 62, 68, 71, 73, 75],
         "prime": [9, 26, 27, 28, 45],
         "parsebinari": [9, 77],
         "asn": [9, 38, 42, 77],
         "except": [10, 17, 18, 19, 20, 21, 22, 23, 25, 33, 34, 42, 43],
         "basetlsexcept": 10,
         "metaclass": [10, 47],
@@ -1152,25 +1160,25 @@
         "tlsbadrecordmac": [10, 30],
         "tlsprotocolexcept": 10,
         "case": [10, 11, 14, 17, 22, 29, 30, 34, 42, 51, 71],
         "tlsclosedconnectionerror": 10,
         "oserror": 10,
         "attempt": [10, 33, 34, 37],
         "made": [10, 17],
-        "after": [10, 17, 18, 19, 20, 21, 25, 30, 34, 57],
+        "after": [10, 14, 17, 18, 19, 20, 21, 25, 30, 34, 57],
         "tlsdecodeerror": 10,
         "doe": [10, 11, 14, 17, 18, 25, 26, 33, 37, 47, 68, 70],
         "tlsdecryptionfail": [10, 30],
         "unsuccess": [10, 30],
         "__str__": [10, 28],
         "At": 10,
         "least": [10, 13, 14, 22, 34],
         "print": [10, 23],
         "out": [10, 14, 34],
-        "time": [10, 11, 14, 28, 43, 44, 70],
+        "time": [10, 11, 14, 28, 31, 43, 44, 70],
         "tlsfaulterror": 10,
         "respond": [10, 11],
         "incorrectli": 10,
         "induc": 10,
         "test": [10, 11, 44, 70],
         "faulti": 10,
         "behavior": [10, 33],
@@ -1222,15 +1230,14 @@
         "applic": [11, 14, 22, 26, 30, 31, 33, 38, 42, 71],
         "negoti": [11, 14, 17, 27, 28, 30, 31, 33, 34],
         "7301": 11,
         "protocol_nam": 11,
         "bytearrai": [11, 12, 13, 14, 27, 28, 30, 31, 33, 34, 38, 41, 42, 43, 44, 45, 48, 50, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 75, 76, 77, 78],
         "peer": [11, 14, 29],
         "exttyp": [11, 28],
-        "i": [11, 16, 27, 32, 33, 45, 51, 71, 77],
         "extdata": 11,
         "raw": [11, 28, 29, 38, 42],
         "__repr__": [11, 28],
         "programm": 11,
         "properti": [11, 28, 30, 34, 53],
         "parser": [11, 28, 29, 38, 42],
         "wire": [11, 28, 30],
@@ -1266,26 +1273,26 @@
         "deal": [11, 49],
         "opaqu": 11,
         "arrai": [11, 27, 28, 31, 33, 34, 41, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "store": [11, 12, 14, 17, 18, 25, 28, 33, 45, 51, 76],
         "ext_typ": 11,
         "save": 11,
         "ecpointformatsextens": 11,
-        "side": [11, 14, 26, 27, 30, 37, 70],
+        "side": [11, 14, 26, 27, 30, 31, 37, 70],
         "hrrkeyshareextens": 11,
         "retri": 11,
         "ext": [11, 28],
         "notifi": 11,
         "selected_group": 11,
         "heartbeatextens": 11,
         "intextens": 11,
         "allow": [11, 14, 28, 30, 32, 33],
         "nor": 11,
         "handler": 11,
-        "integ": [11, 27, 28, 31, 33, 34, 39, 42, 43, 44, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
+        "integ": [11, 14, 27, 28, 31, 33, 34, 39, 42, 43, 44, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "elem_length": 11,
         "ext_tyo": 11,
         "item_enum": 11,
         "keyshareentri": 11,
         "item": [11, 33, 42, 52],
         "initialis": [11, 14, 28, 30, 42, 44, 68, 70],
         "key_exchang": 11,
@@ -1367,30 +1374,37 @@
         "shorter": 11,
         "than": [11, 14, 29, 30, 34, 42, 45, 71, 76],
         "lenght": 11,
         "longer": [11, 14, 30],
         "servercerttypeextens": 11,
         "serverkeyshareextens": 11,
         "server_shar": 11,
+        "sessionticketextens": 11,
+        "ticket": [11, 13, 14, 28, 31, 34],
+        "5077": 11,
+        "legaci": 11,
+        "method": [11, 18, 23, 25, 26, 27, 28, 42, 47, 49, 50, 55, 71],
+        "child": [11, 28, 38],
+        "overrid": 11,
+        "so": [11, 13, 14, 22, 30, 33, 34, 47, 51, 71],
         "signaturealgorithmscertextens": 11,
         "_siglistext": 11,
         "signaturealgorithmsextens": 11,
-        "method": [11, 18, 23, 25, 26, 27, 28, 42, 47, 49, 50, 55, 71],
         "In": [11, 14, 22, 28, 30, 42, 51],
         "practic": 11,
         "latter": 11,
         "rfc5246": 11,
         "srvpresharedkeyextens": 11,
         "srvsupportedversionsextens": 11,
         "supportedvers": 11,
         "sh": 11,
         "hrr": 11,
         "tls13": [11, 28],
         "ll": 11,
-        "actual": [11, 34, 42],
+        "actual": [11, 31, 34, 42],
         "usabl": 11,
         "encext": 11,
         "encryptedextens": [11, 28],
         "statusrequestextens": 11,
         "6066": [11, 28],
         "responder_id_list": 11,
         "trust": [11, 14],
@@ -1414,15 +1428,15 @@
         "programmm": 11,
         "public_kei": [11, 50],
         "min_gener": 11,
         "expir": [11, 32],
         "target_hash": 11,
         "py": [11, 22, 24, 57],
         "meth": 11,
-        "inform": [11, 41, 43, 47],
+        "inform": [11, 31, 41, 43, 47],
         "both": [11, 31, 33, 51],
         "http": [11, 22, 23, 24, 25, 33],
         "tool": [11, 51],
         "org": 11,
         "html": [11, 22],
         "rfc4366": 11,
         "more": [11, 31, 34, 50, 76],
@@ -1445,29 +1459,25 @@
         "would": [11, 30],
         "limit": [11, 29, 30, 32, 34],
         "servertyp": 11,
         "univers": [11, 38, 55, 62, 68, 71],
         "encexttyp": 11,
         "dict": [11, 47],
         "concret": 11,
-        "where": [11, 22],
+        "where": [11, 22, 31],
         "those": [11, 27, 28, 29, 34],
         "special": 11,
         "_certificateextens": 11,
         "_hrrextens": 11,
         "effect": 11,
         "Will": [11, 29, 42, 45, 52],
-        "them": [11, 22, 29],
-        "child": [11, 28, 38],
-        "overrid": 11,
+        "them": [11, 22, 29, 31],
         "render": 11,
         "arg": [11, 16, 24, 28, 30, 73],
         "kwarg": [11, 24, 28, 73],
-        "legaci": 11,
-        "so": [11, 13, 14, 22, 30, 33, 34, 47, 51, 71],
         "word": [11, 14],
         "overal": [11, 42],
         "exact": [11, 28],
         "revers": 11,
         "extension_typ": 11,
         "assertionerror": 11,
         "length_length": [11, 42],
@@ -1495,23 +1505,22 @@
         "encapsul": [13, 14],
         "alignclienthellopad": 13,
         "align": 13,
         "512": 13,
         "calc_res_binder_psk": 13,
         "iden": 13,
         "res_master_secret": 13,
-        "ticket": [13, 14, 28, 31, 34],
         "update_bind": 13,
         "handshake_hash": [13, 27, 45],
         "psk_config": 13,
         "extra": 13,
         "ok": [13, 30, 44],
         "far": 13,
         "verify_bind": 13,
-        "posit": [13, 42],
+        "posit": [13, 14, 42],
         "extern": 13,
         "minkeys": 14,
         "minimum": [14, 34],
         "asymmetr": [14, 51],
         "tri": [14, 29],
         "smaller": [14, 29, 45],
         "1023": 14,
@@ -1567,15 +1576,15 @@
         "callback": [14, 30, 51],
         "comput": 14,
         "cb_func": 14,
         "msg_size": 14,
         "content_typ": 14,
         "max_siz": 14,
         "pskconfig": 14,
-        "earlier": 14,
+        "earlier": [14, 31],
         "second": [14, 26, 28, 32, 46],
         "third": 14,
         "ticketkei": 14,
         "subsequ": [14, 78],
         "fallback": 14,
         "rollov": 14,
         "ticketciph": 14,
@@ -1585,16 +1594,19 @@
         "24h": 14,
         "life": 14,
         "48h": 14,
         "leav": [14, 22],
         "disabl": 14,
         "altern": [14, 33],
         "ticketlifetim": 14,
-        "lifetim": 14,
+        "lifetim": [14, 31],
         "dai": [14, 46],
+        "ticket_count": 14,
+        "establish": [14, 26, 34],
+        "resumpt": [14, 28, 31, 32, 33, 34],
         "psk_mode": 14,
         "max_early_data": [14, 30],
         "rtt": 14,
         "process": [14, 26, 30, 33, 42, 44, 70],
         "mani": 14,
         "ignor": [14, 17, 18, 25, 28, 30, 33, 41, 50],
         "use_heartbeat_extens": 14,
@@ -1682,15 +1694,14 @@
         "smtplib": [17, 21],
         "etc": [17, 27, 28, 30, 47],
         "reli": [17, 18, 19, 20, 21, 25],
         "mutual": [17, 18, 19, 20, 21, 25, 33],
         "perform": [17, 18, 19, 20, 21, 25, 26, 27, 28, 30, 33, 39, 50, 55, 62, 70, 71, 75],
         "itself": [17, 18, 25, 33, 38],
         "simpli": [17, 18, 25, 32],
-        "later": [17, 18, 25, 26, 28],
         "prepar": [17, 18, 19, 20, 21, 25, 26],
         "detail": [17, 18, 19, 20, 21, 25, 28, 33, 34],
         "might": [17, 18, 19, 20, 21, 22, 25],
         "callabl": [17, 18, 19, 20, 21, 25, 30, 51],
         "evalu": [17, 18, 19, 20, 21, 25],
         "control": [17, 18, 19, 20, 21, 25, 33],
         "exclus": 17,
@@ -1802,15 +1813,14 @@
         "dhparam": 26,
         "dhgroup": 26,
         "serverkeyexchang": [26, 28],
         "makeclientkeyexchang": 26,
         "makeserverkeyexchang": 26,
         "processclientkeyexchang": 26,
         "clientkeyexchang": [26, 28],
-        "establish": [26, 34],
         "processserverkeyexchang": 26,
         "srvpublickei": 26,
         "aecdhkeyexchang": 26,
         "acceptedcurv": 26,
         "elipt": 26,
         "sighash": 26,
         "aecdh": 26,
@@ -1921,15 +1931,15 @@
         "complement": [27, 28, 31, 33, 34, 42, 43, 45, 51, 53, 54, 55, 56, 57, 59, 60, 61, 62, 63, 67, 68, 71, 76, 77, 78],
         "calcextendedmastersecret": 27,
         "deriv": [27, 31, 45, 70],
         "calcfinish": 27,
         "isclient": 27,
         "calcmastersecret": 27,
         "calc_kei": 27,
-        "cipher_suit": [27, 28],
+        "cipher_suit": [27, 28, 31],
         "client_random": 27,
         "server_random": 27,
         "output_length": 27,
         "depend": [27, 33],
         "expans": 27,
         "ex": 27,
         "createhmac": 27,
@@ -1950,15 +1960,15 @@
         "levelnam": 28,
         "applicationdata": [28, 30],
         "splitfirstbyt": 28,
         "handshakemsg": 28,
         "getter": 28,
         "context": [28, 30, 34, 38],
         "certificateentri": 28,
-        "togeth": 28,
+        "togeth": [28, 31],
         "hellomessag": 28,
         "certificate_typ": 28,
         "certificate_author": 28,
         "sig_alg": 28,
         "instead": [28, 33, 47, 50, 71],
         "three": [28, 42],
         "consid": 28,
@@ -1977,15 +1987,14 @@
         "verify_data": 28,
         "srp_usernam": 28,
         "npn": [28, 33],
         "present": [28, 31, 50, 51],
         "inspect": [28, 31, 34],
         "session_id": 28,
         "challeng": 28,
-        "resumpt": [28, 31, 32, 33, 34],
         "whatev": [28, 41],
         "psk_truncat": 28,
         "srp_a": 28,
         "answer": 28,
         "dh_yc": 28,
         "ecdh_yc": 28,
         "coordin": [28, 75],
@@ -2009,17 +2018,18 @@
         "create_respons": 28,
         "leftov": 28,
         "code": [28, 33, 34, 42, 45],
         "addextens": 28,
         "getextens": 28,
         "hellorequest": 28,
         "newsessionticket": 28,
-        "ticket_lifetim": 28,
+        "ticket_lifetim": [28, 31],
         "ticket_age_add": 28,
         "ticket_nonc": 28,
+        "newsessionticket1_0": 28,
         "nextprotocol": 28,
         "next_proto": 28,
         "trial": 28,
         "recordhead": 28,
         "recordheader2": 28,
         "securityescap": 28,
         "escap": 28,
@@ -2055,15 +2065,15 @@
         "explicit": 28,
         "ecdh_i": 28,
         "hashalg": [28, 50, 71],
         "signalg": 28,
         "writeparam": 28,
         "sessionticketpayload": 28,
         "meant": 28,
-        "master_secret": 28,
+        "master_secret": [28, 31],
         "nonc": [28, 37, 39, 40],
         "kdf": 28,
         "creation_tim": 28,
         "unix": 28,
         "client_cert_chain": 28,
         "becaus": [29, 34],
         "hard": 29,
@@ -2163,20 +2173,24 @@
         "structur": [31, 42],
         "tackinhelloext": 31,
         "via": 31,
         "appproto": 31,
         "protect": 31,
         "exportermastersecret": 31,
         "resumptionmastersecret": 31,
+        "tls_1_0_ticket": 31,
         "sessionid": [31, 32],
         "extendedmastersecret": 31,
         "getbreaksig": 31,
         "getmacnam": 31,
         "algo": 31,
         "gettackid": 31,
+        "reciev": 31,
+        "sessionticket": 31,
+        "time_reciev": 31,
         "maxentri": 32,
         "10000": 32,
         "maxag": 32,
         "14400": 32,
         "expens": 32,
         "reach": 32,
         "oldest": [32, 34],
@@ -3156,30 +3170,33 @@
             [7, 3, 1, "", "dheDsaSuites"],
             [7, 3, 1, "", "ecdhAllSuites"],
             [7, 3, 1, "", "ecdhAnonSuites"],
             [7, 3, 1, "", "ecdheCertSuites"],
             [7, 3, 1, "", "ecdheEcdsaSuites"],
             [7, 2, 1, "", "filterForVersion"],
             [7, 2, 1, "", "filter_for_certificate"],
+            [7, 2, 1, "", "filter_for_prfs"],
             [7, 2, 1, "", "getAnonSuites"],
             [7, 2, 1, "", "getCertSuites"],
             [7, 2, 1, "", "getDheCertSuites"],
             [7, 2, 1, "", "getDheDsaSuites"],
             [7, 2, 1, "", "getEcdhAnonSuites"],
             [7, 2, 1, "", "getEcdheCertSuites"],
             [7, 2, 1, "", "getEcdsaSuites"],
             [7, 2, 1, "", "getSrpAllSuites"],
             [7, 2, 1, "", "getSrpCertSuites"],
             [7, 2, 1, "", "getSrpDsaSuites"],
             [7, 2, 1, "", "getSrpSuites"],
             [7, 2, 1, "", "getTLS13Suites"],
+            [7, 3, 1, "", "i"],
             [7, 3, 1, "", "ietfNames"],
             [7, 3, 1, "", "md5Suites"],
             [7, 3, 1, "", "nullSuites"],
             [7, 3, 1, "", "rc4Suites"],
+            [7, 3, 1, "", "sha256PrfSuites"],
             [7, 3, 1, "", "sha256Suites"],
             [7, 3, 1, "", "sha384PrfSuites"],
             [7, 3, 1, "", "sha384Suites"],
             [7, 3, 1, "", "shaSuites"],
             [7, 3, 1, "", "srpAllSuites"],
             [7, 3, 1, "", "srpCertSuites"],
             [7, 3, 1, "", "srpDsaSuites"],
@@ -3244,14 +3261,15 @@
             [7, 3, 1, "", "max_fragment_length"],
             [7, 3, 1, "", "post_handshake_auth"],
             [7, 3, 1, "", "pre_shared_key"],
             [7, 3, 1, "", "psk_key_exchange_modes"],
             [7, 3, 1, "", "record_size_limit"],
             [7, 3, 1, "", "renegotiation_info"],
             [7, 3, 1, "", "server_name"],
+            [7, 3, 1, "", "session_ticket"],
             [7, 3, 1, "", "signature_algorithms"],
             [7, 3, 1, "", "signature_algorithms_cert"],
             [7, 3, 1, "", "srp"],
             [7, 3, 1, "", "status_request"],
             [7, 3, 1, "", "supported_groups"],
             [7, 3, 1, "", "supported_versions"],
             [7, 3, 1, "", "supports_npn"],
@@ -3321,14 +3339,15 @@
             [7, 3, 1, "", "certificate"],
             [7, 3, 1, "", "certificate_request"],
             [7, 3, 1, "", "certificate_status"],
             [7, 3, 1, "", "certificate_verify"],
             [7, 3, 1, "", "client_hello"],
             [7, 3, 1, "", "client_key_exchange"],
             [7, 3, 1, "", "encrypted_extensions"],
+            [7, 3, 1, "", "end_of_early_data"],
             [7, 3, 1, "", "finished"],
             [7, 3, 1, "", "hello_request"],
             [7, 3, 1, "", "hello_retry_request"],
             [7, 3, 1, "", "key_update"],
             [7, 3, 1, "", "message_hash"],
             [7, 3, 1, "", "new_session_ticket"],
             [7, 3, 1, "", "next_protocol"],
@@ -3431,15 +3450,16 @@
         ],
         "tlslite.defragmenter.Defragmenter": [
             [8, 2, 1, "", "__init__"],
             [8, 2, 1, "", "add_data"],
             [8, 2, 1, "", "add_dynamic_size"],
             [8, 2, 1, "", "add_static_size"],
             [8, 2, 1, "", "clear_buffers"],
-            [8, 2, 1, "", "get_message"]
+            [8, 2, 1, "", "get_message"],
+            [8, 2, 1, "", "is_empty"]
         ],
         "tlslite.dh": [
             [9, 4, 1, "", "parse"],
             [9, 4, 1, "", "parseBinary"]
         ],
         "tlslite.errors": [
             [10, 5, 1, "", "BaseTLSException"],
@@ -3509,14 +3529,15 @@
             [11, 1, 1, "", "PskKeyExchangeModesExtension"],
             [11, 1, 1, "", "RecordSizeLimitExtension"],
             [11, 1, 1, "", "RenegotiationInfoExtension"],
             [11, 1, 1, "", "SNIExtension"],
             [11, 1, 1, "", "SRPExtension"],
             [11, 1, 1, "", "ServerCertTypeExtension"],
             [11, 1, 1, "", "ServerKeyShareExtension"],
+            [11, 1, 1, "", "SessionTicketExtension"],
             [11, 1, 1, "", "SignatureAlgorithmsCertExtension"],
             [11, 1, 1, "", "SignatureAlgorithmsExtension"],
             [11, 1, 1, "", "SrvPreSharedKeyExtension"],
             [11, 1, 1, "", "SrvSupportedVersionsExtension"],
             [11, 1, 1, "", "StatusRequestExtension"],
             [11, 1, 1, "", "SupportedGroupsExtension"],
             [11, 1, 1, "", "SupportedVersionsExtension"],
@@ -3650,14 +3671,21 @@
         ],
         "tlslite.extensions.ServerKeyShareExtension": [
             [11, 2, 1, "", "__init__"],
             [11, 2, 1, "", "create"],
             [11, 6, 1, "", "extData"],
             [11, 2, 1, "", "parse"]
         ],
+        "tlslite.extensions.SessionTicketExtension": [
+            [11, 2, 1, "", "__init__"],
+            [11, 2, 1, "", "__repr__"],
+            [11, 2, 1, "", "create"],
+            [11, 6, 1, "", "extData"],
+            [11, 2, 1, "", "parse"]
+        ],
         "tlslite.extensions.SignatureAlgorithmsCertExtension": [
             [11, 2, 1, "", "__init__"]
         ],
         "tlslite.extensions.SignatureAlgorithmsExtension": [
             [11, 2, 1, "", "__init__"]
         ],
         "tlslite.extensions.SrvPreSharedKeyExtension": [
@@ -3999,14 +4027,15 @@
             [28, 1, 1, "", "HandshakeMsg"],
             [28, 1, 1, "", "Heartbeat"],
             [28, 1, 1, "", "HelloMessage"],
             [28, 1, 1, "", "HelloRequest"],
             [28, 1, 1, "", "KeyUpdate"],
             [28, 1, 1, "", "Message"],
             [28, 1, 1, "", "NewSessionTicket"],
+            [28, 1, 1, "", "NewSessionTicket1_0"],
             [28, 1, 1, "", "NextProtocol"],
             [28, 1, 1, "", "RecordHeader"],
             [28, 1, 1, "", "RecordHeader2"],
             [28, 1, 1, "", "RecordHeader3"],
             [28, 1, 1, "", "SSL2Finished"],
             [28, 1, 1, "", "ServerFinished"],
             [28, 1, 1, "", "ServerHello"],
@@ -4152,14 +4181,20 @@
         ],
         "tlslite.messages.NewSessionTicket": [
             [28, 2, 1, "", "__init__"],
             [28, 2, 1, "", "create"],
             [28, 2, 1, "", "parse"],
             [28, 2, 1, "", "write"]
         ],
+        "tlslite.messages.NewSessionTicket1_0": [
+            [28, 2, 1, "", "__init__"],
+            [28, 2, 1, "", "create"],
+            [28, 2, 1, "", "parse"],
+            [28, 2, 1, "", "write"]
+        ],
         "tlslite.messages.NextProtocol": [
             [28, 2, 1, "", "__init__"],
             [28, 2, 1, "", "create"],
             [28, 2, 1, "", "parse"],
             [28, 2, 1, "", "write"]
         ],
         "tlslite.messages.RecordHeader": [
@@ -4282,25 +4317,30 @@
         "tlslite.recordlayer.RecordSocket": [
             [30, 2, 1, "", "__init__"],
             [30, 2, 1, "", "recv"],
             [30, 2, 1, "", "send"]
         ],
         "tlslite.session": [
             [31, 1, 1, "", "Session"],
+            [31, 1, 1, "", "Ticket"],
             [31, 4, 1, "", "bytes_to_int"]
         ],
         "tlslite.session.Session": [
             [31, 2, 1, "", "__init__"],
             [31, 2, 1, "", "create"],
             [31, 2, 1, "", "getBreakSigs"],
             [31, 2, 1, "", "getCipherName"],
             [31, 2, 1, "", "getMacName"],
             [31, 2, 1, "", "getTackId"],
             [31, 2, 1, "", "valid"]
         ],
+        "tlslite.session.Ticket": [
+            [31, 2, 1, "", "__init__"],
+            [31, 2, 1, "", "valid"]
+        ],
         "tlslite.sessioncache": [
             [32, 1, 1, "", "SessionCache"]
         ],
         "tlslite.sessioncache.SessionCache": [
             [32, 2, 1, "", "__getitem__"],
             [32, 2, 1, "", "__init__"],
             [32, 2, 1, "", "__setitem__"]
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.api.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.api module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.api module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.basedb.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.basedb.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.basedb module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.basedb module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.bufferedsocket.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.bufferedsocket.html`

 * *Files identical despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.bufferedsocket module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.bufferedsocket module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.checker.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.checker.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.checker module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.checker module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.constants.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.constants.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.constants module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.constants module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -1164,14 +1164,21 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.filter_for_certificate">
 <em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">filter_for_certificate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">suites</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cert_chain</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.constants.CipherSuite.filter_for_certificate" title="Permalink to this definition"></a></dt>
 <dd><p>Return a copy of suites without ciphers incompatible with the cert.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="tlslite.constants.CipherSuite.filter_for_prfs">
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">filter_for_prfs</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">suites</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prfs</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.constants.CipherSuite.filter_for_prfs" title="Permalink to this definition"></a></dt>
+<dd><p>Return a copy of suites without ciphers incompatible with the
+specified prfs (sha256 or sha384)</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.getAnonSuites">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">getAnonSuites</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">settings</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">version</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.constants.CipherSuite.getAnonSuites" title="Permalink to this definition"></a></dt>
 <dd><p>Provide anonymous DH ciphersuites matching settings</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.getCertSuites">
@@ -1236,14 +1243,19 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.getTLS13Suites">
 <em class="property"><span class="pre">classmethod</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">getTLS13Suites</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">settings</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">version</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.constants.CipherSuite.getTLS13Suites" title="Permalink to this definition"></a></dt>
 <dd><p>Return cipher suites that are TLS 1.3 specific.</p>
 </dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="tlslite.constants.CipherSuite.i">
+<span class="sig-name descname"><span class="pre">i</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">165</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.i" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.ietfNames">
 <span class="sig-name descname"><span class="pre">ietfNames</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">{1:</span> <span class="pre">'TLS_RSA_WITH_NULL_MD5',</span> <span class="pre">2:</span> <span class="pre">'TLS_RSA_WITH_NULL_SHA',</span> <span class="pre">4:</span> <span class="pre">'TLS_RSA_WITH_RC4_128_MD5',</span> <span class="pre">5:</span> <span class="pre">'TLS_RSA_WITH_RC4_128_SHA',</span> <span class="pre">10:</span> <span class="pre">'TLS_RSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">13:</span> <span class="pre">'TLS_DH_DSS_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">19:</span> <span class="pre">'TLS_DHE_DSS_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">22:</span> <span class="pre">'TLS_DHE_RSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">24:</span> <span class="pre">'TLS_DH_ANON_WITH_RC4_128_MD5',</span> <span class="pre">27:</span> <span class="pre">'TLS_DH_ANON_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">47:</span> <span class="pre">'TLS_RSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">48:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_128_CBC_SHA',</span> <span class="pre">50:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_128_CBC_SHA',</span> <span class="pre">51:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">52:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_128_CBC_SHA',</span> <span class="pre">53:</span> <span class="pre">'TLS_RSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">54:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_256_CBC_SHA',</span> <span class="pre">56:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_256_CBC_SHA',</span> <span class="pre">57:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">58:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_256_CBC_SHA',</span> <span class="pre">59:</span> <span class="pre">'TLS_RSA_WITH_NULL_SHA256',</span> <span class="pre">60:</span> <span class="pre">'TLS_RSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">61:</span> <span class="pre">'TLS_RSA_WITH_AES_256_CBC_SHA256',</span> <span class="pre">62:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_128_CBC_SHA256',</span> <span class="pre">64:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_128_CBC_SHA256',</span> <span class="pre">103:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">104:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_256_CBC_SHA256',</span> <span class="pre">106:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_256_CBC_SHA256',</span> <span class="pre">107:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_256_CBC_SHA256',</span> <span class="pre">108:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_128_CBC_SHA256',</span> <span class="pre">109:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_256_CBC_SHA256',</span> <span class="pre">156:</span> <span class="pre">'TLS_RSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">157:</span> <span class="pre">'TLS_RSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">158:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">159:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">162:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_128_GCM_SHA256',</span> <span class="pre">163:</span> <span class="pre">'TLS_DHE_DSS_WITH_AES_256_GCM_SHA384',</span> <span class="pre">164:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_128_GCM_SHA256',</span> <span class="pre">165:</span> <span class="pre">'TLS_DH_DSS_WITH_AES_256_GCM_SHA384',</span> <span class="pre">166:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_128_GCM_SHA256',</span> <span class="pre">167:</span> <span class="pre">'TLS_DH_ANON_WITH_AES_256_GCM_SHA384',</span> <span class="pre">255:</span> <span class="pre">'TLS_EMPTY_RENEGOTIATION_INFO_SCSV',</span> <span class="pre">4865:</span> <span class="pre">'TLS_AES_128_GCM_SHA256',</span> <span class="pre">4866:</span> <span class="pre">'TLS_AES_256_GCM_SHA384',</span> <span class="pre">4867:</span> <span class="pre">'TLS_CHACHA20_POLY1305_SHA256',</span> <span class="pre">4868:</span> <span class="pre">'TLS_AES_128_CCM_SHA256',</span> <span class="pre">4869:</span> <span class="pre">'TLS_AES_128_CCM_8_SHA256',</span> <span class="pre">22016:</span> <span class="pre">'TLS_FALLBACK_SCSV',</span> <span class="pre">49153:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_NULL_SHA',</span> <span class="pre">49154:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_RC4_128_SHA',</span> <span class="pre">49155:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49156:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49157:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49158:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_NULL_SHA',</span> <span class="pre">49159:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_RC4_128_SHA',</span> <span class="pre">49160:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49161:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49162:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49163:</span> <span class="pre">'TLS_ECDH_RSA_WITH_NULL_SHA',</span> <span class="pre">49164:</span> <span class="pre">'TLS_ECDH_RSA_WITH_RC4_128_SHA',</span> <span class="pre">49165:</span> <span class="pre">'TLS_ECDH_RSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49166:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49167:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49168:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_NULL_SHA',</span> <span class="pre">49169:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_RC4_128_SHA',</span> <span class="pre">49170:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49171:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49172:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49173:</span> <span class="pre">'TLS_ECDH_ANON_WITH_NULL_SHA',</span> <span class="pre">49174:</span> <span class="pre">'TLS_ECDH_ANON_WITH_RC4_128_SHA',</span> <span class="pre">49175:</span> <span class="pre">'TLS_ECDH_ANON_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49176:</span> <span class="pre">'TLS_ECDH_ANON_WITH_AES_128_CBC_SHA',</span> <span class="pre">49177:</span> <span class="pre">'TLS_ECDH_ANON_WITH_AES_256_CBC_SHA',</span> <span class="pre">49178:</span> <span class="pre">'TLS_SRP_SHA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49179:</span> <span class="pre">'TLS_SRP_SHA_RSA_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49180:</span> <span class="pre">'TLS_SRP_SHA_DSS_WITH_3DES_EDE_CBC_SHA',</span> <span class="pre">49181:</span> <span class="pre">'TLS_SRP_SHA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49182:</span> <span class="pre">'TLS_SRP_SHA_RSA_WITH_AES_128_CBC_SHA',</span> <span class="pre">49183:</span> <span class="pre">'TLS_SRP_SHA_DSS_WITH_AES_128_CBC_SHA',</span> <span class="pre">49184:</span> <span class="pre">'TLS_SRP_SHA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49185:</span> <span class="pre">'TLS_SRP_SHA_RSA_WITH_AES_256_CBC_SHA',</span> <span class="pre">49186:</span> <span class="pre">'TLS_SRP_SHA_DSS_WITH_AES_256_CBC_SHA',</span> <span class="pre">49187:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">49188:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA384',</span> <span class="pre">49189:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">49190:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA384',</span> <span class="pre">49191:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">49192:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384',</span> <span class="pre">49193:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_128_CBC_SHA256',</span> <span class="pre">49194:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_256_CBC_SHA384',</span> <span class="pre">49195:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">49196:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">49197:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">49198:</span> <span class="pre">'TLS_ECDH_ECDSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">49199:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">49200:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">49201:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_128_GCM_SHA256',</span> <span class="pre">49202:</span> <span class="pre">'TLS_ECDH_RSA_WITH_AES_256_GCM_SHA384',</span> <span class="pre">49308:</span> <span class="pre">'TLS_RSA_WITH_AES_128_CCM',</span> <span class="pre">49309:</span> <span class="pre">'TLS_RSA_WITH_AES_256_CCM',</span> <span class="pre">49310:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_128_CCM',</span> <span class="pre">49311:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_256_CCM',</span> <span class="pre">49312:</span> <span class="pre">'TLS_RSA_WITH_AES_128_CCM_8',</span> <span class="pre">49313:</span> <span class="pre">'TLS_RSA_WITH_AES_256_CCM_8',</span> <span class="pre">49314:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_128_CCM_8',</span> <span class="pre">49315:</span> <span class="pre">'TLS_DHE_RSA_WITH_AES_256_CCM_8',</span> <span class="pre">49324:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_128_CCM',</span> <span class="pre">49325:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_256_CCM',</span> <span class="pre">49326:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_128_CCM_8',</span> <span class="pre">49327:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_AES_256_CCM_8',</span> <span class="pre">52385:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_draft_00',</span> <span class="pre">52386:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_draft_00',</span> <span class="pre">52387:</span> <span class="pre">'TLS_DHE_RSA_WITH_CHACHA20_POLY1305_draft_00',</span> <span class="pre">52392:</span> <span class="pre">'TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256',</span> <span class="pre">52393:</span> <span class="pre">'TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256',</span> <span class="pre">52394:</span> <span class="pre">'TLS_DHE_RSA_WITH_CHACHA20_POLY1305_SHA256',</span> <span class="pre">65664:</span> <span class="pre">'SSL_CK_RC4_128_WITH_MD5',</span> <span class="pre">131200:</span> <span class="pre">'SSL_CK_RC4_128_EXPORT40_WITH_MD5',</span> <span class="pre">196736:</span> <span class="pre">'SSL_CK_RC2_128_CBC_WITH_MD5',</span> <span class="pre">262272:</span> <span class="pre">'SSL_CK_RC2_128_CBC_EXPORT40_WITH_MD5',</span> <span class="pre">327808:</span> <span class="pre">'SSL_CK_IDEA_128_CBC_WITH_MD5',</span> <span class="pre">393280:</span> <span class="pre">'SSL_CK_DES_64_CBC_WITH_MD5',</span> <span class="pre">458944:</span> <span class="pre">'SSL_CK_DES_192_EDE3_CBC_WITH_MD5'}</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.ietfNames" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.md5Suites">
 <span class="sig-name descname"><span class="pre">md5Suites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[24,</span> <span class="pre">4,</span> <span class="pre">1]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.md5Suites" title="Permalink to this definition"></a></dt>
@@ -1259,23 +1271,29 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.rc4Suites">
 <span class="sig-name descname"><span class="pre">rc4Suites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[49169,</span> <span class="pre">49159,</span> <span class="pre">49154,</span> <span class="pre">49164,</span> <span class="pre">24,</span> <span class="pre">5,</span> <span class="pre">4,</span> <span class="pre">49174]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.rc4Suites" title="Permalink to this definition"></a></dt>
 <dd><p>RC4 128 stream cipher</p>
 </dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="tlslite.constants.CipherSuite.sha256PrfSuites">
+<span class="sig-name descname"><span class="pre">sha256PrfSuites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[60,</span> <span class="pre">61,</span> <span class="pre">103,</span> <span class="pre">107,</span> <span class="pre">59,</span> <span class="pre">108,</span> <span class="pre">109,</span> <span class="pre">49187,</span> <span class="pre">49189,</span> <span class="pre">49193,</span> <span class="pre">49191,</span> <span class="pre">156,</span> <span class="pre">158,</span> <span class="pre">166,</span> <span class="pre">49195,</span> <span class="pre">49197,</span> <span class="pre">49201,</span> <span class="pre">49199,</span> <span class="pre">4865,</span> <span class="pre">162,</span> <span class="pre">164,</span> <span class="pre">49308,</span> <span class="pre">49310,</span> <span class="pre">49324,</span> <span class="pre">4868,</span> <span class="pre">49312,</span> <span class="pre">49314,</span> <span class="pre">49326,</span> <span class="pre">4869,</span> <span class="pre">49309,</span> <span class="pre">49311,</span> <span class="pre">49325,</span> <span class="pre">49313,</span> <span class="pre">49315,</span> <span class="pre">49327,</span> <span class="pre">52392,</span> <span class="pre">52393,</span> <span class="pre">52394,</span> <span class="pre">4867,</span> <span class="pre">52385,</span> <span class="pre">52386,</span> <span class="pre">52387]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.sha256PrfSuites" title="Permalink to this definition"></a></dt>
+<dd><p>any that will end up using SHA256 PRF in TLS 1.2 or later</p>
+</dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.sha256Suites">
 <span class="sig-name descname"><span class="pre">sha256Suites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[60,</span> <span class="pre">61,</span> <span class="pre">103,</span> <span class="pre">107,</span> <span class="pre">59,</span> <span class="pre">108,</span> <span class="pre">109,</span> <span class="pre">49187,</span> <span class="pre">49189,</span> <span class="pre">49193,</span> <span class="pre">49191]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.sha256Suites" title="Permalink to this definition"></a></dt>
 <dd><p>SHA-256 HMAC, SHA-256 PRF</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.sha384PrfSuites">
 <span class="sig-name descname"><span class="pre">sha384PrfSuites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[49188,</span> <span class="pre">49190,</span> <span class="pre">49194,</span> <span class="pre">49192,</span> <span class="pre">163,</span> <span class="pre">165,</span> <span class="pre">157,</span> <span class="pre">159,</span> <span class="pre">167,</span> <span class="pre">49196,</span> <span class="pre">49198,</span> <span class="pre">49202,</span> <span class="pre">49200,</span> <span class="pre">4866,</span> <span class="pre">163,</span> <span class="pre">165]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.sha384PrfSuites" title="Permalink to this definition"></a></dt>
-<dd><p>TLS1.2 with SHA384 PRF</p>
+<dd><p>any with SHA384 PRF</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.CipherSuite.sha384Suites">
 <span class="sig-name descname"><span class="pre">sha384Suites</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[49188,</span> <span class="pre">49190,</span> <span class="pre">49194,</span> <span class="pre">49192,</span> <span class="pre">163,</span> <span class="pre">165]</span></em><a class="headerlink" href="#tlslite.constants.CipherSuite.sha384Suites" title="Permalink to this definition"></a></dt>
 <dd><p>SHA-384 HMAC, SHA-384 PRF</p>
 </dd></dl>
@@ -1627,14 +1645,19 @@
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.ExtensionType.server_name">
 <span class="sig-name descname"><span class="pre">server_name</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">0</span></em><a class="headerlink" href="#tlslite.constants.ExtensionType.server_name" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="tlslite.constants.ExtensionType.session_ticket">
+<span class="sig-name descname"><span class="pre">session_ticket</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">35</span></em><a class="headerlink" href="#tlslite.constants.ExtensionType.session_ticket" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.ExtensionType.signature_algorithms">
 <span class="sig-name descname"><span class="pre">signature_algorithms</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">13</span></em><a class="headerlink" href="#tlslite.constants.ExtensionType.signature_algorithms" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.ExtensionType.signature_algorithms_cert">
 <span class="sig-name descname"><span class="pre">signature_algorithms_cert</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">50</span></em><a class="headerlink" href="#tlslite.constants.ExtensionType.signature_algorithms_cert" title="Permalink to this definition"></a></dt>
@@ -2003,14 +2026,19 @@
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.HandshakeType.encrypted_extensions">
 <span class="sig-name descname"><span class="pre">encrypted_extensions</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">8</span></em><a class="headerlink" href="#tlslite.constants.HandshakeType.encrypted_extensions" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="tlslite.constants.HandshakeType.end_of_early_data">
+<span class="sig-name descname"><span class="pre">end_of_early_data</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">5</span></em><a class="headerlink" href="#tlslite.constants.HandshakeType.end_of_early_data" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.HandshakeType.finished">
 <span class="sig-name descname"><span class="pre">finished</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">20</span></em><a class="headerlink" href="#tlslite.constants.HandshakeType.finished" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="tlslite.constants.HandshakeType.hello_request">
 <span class="sig-name descname"><span class="pre">hello_request</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">0</span></em><a class="headerlink" href="#tlslite.constants.HandshakeType.hello_request" title="Permalink to this definition"></a></dt>
```

#### html2text {}

```diff
@@ -341,14 +341,17 @@
         ecdheEcdsaSuites= [52393, 52386, 49196, 49195, 49325, 49324, 49188,
         49187, 49162, 49161, 49160, 49327, 49326, 49159, 49158]ï
             ECDHE key exchange, ECDSA authentication
         staticfilterForVersion(suites, minVersion, maxVersion)ï
             Return a copy of suites without ciphers incompatible with version
         staticfilter_for_certificate(suites, cert_chain)ï
             Return a copy of suites without ciphers incompatible with the cert.
+        staticfilter_for_prfs(suites, prfs)ï
+            Return a copy of suites without ciphers incompatible with the
+            specified prfs (sha256 or sha384)
         classmethodgetAnonSuites(settings, version=None)ï
             Provide anonymous DH ciphersuites matching settings
         classmethodgetCertSuites(settings, version=None)ï
             Return ciphers with RSA authentication matching settings
         classmethodgetDheCertSuites(settings, version=None)ï
             Provide authenticated DHE ciphersuites matching settings
         classmethodgetDheDsaSuites(settings, version=None)ï
@@ -365,14 +368,15 @@
             Return SRP cipher suites that use server certificates
         classmethodgetSrpDsaSuites(settings, version=None)ï
             Return SRP DSA cipher suites that use server certificates
         classmethodgetSrpSuites(settings, version=None)ï
             Return SRP cipher suites matching settings
         classmethodgetTLS13Suites(settings, version=None)ï
             Return cipher suites that are TLS 1.3 specific.
+        i= 165ï
         ietfNames= {1: 'TLS_RSA_WITH_NULL_MD5', 2: 'TLS_RSA_WITH_NULL_SHA', 4:
         'TLS_RSA_WITH_RC4_128_MD5', 5: 'TLS_RSA_WITH_RC4_128_SHA', 10:
         'TLS_RSA_WITH_3DES_EDE_CBC_SHA', 13:
         'TLS_DH_DSS_WITH_3DES_EDE_CBC_SHA', 19:
         'TLS_DHE_DSS_WITH_3DES_EDE_CBC_SHA', 22:
         'TLS_DHE_RSA_WITH_3DES_EDE_CBC_SHA', 24:
         'TLS_DH_ANON_WITH_RC4_128_MD5', 27:
@@ -477,20 +481,26 @@
         458944: 'SSL_CK_DES_192_EDE3_CBC_WITH_MD5'}ï
         md5Suites= [24, 4, 1]ï
             MD-5 HMAC, protocol default PRF
         nullSuites= [1, 2, 59, 49158, 49153, 49163, 49168, 49173]ï
             no encryption
         rc4Suites= [49169, 49159, 49154, 49164, 24, 5, 4, 49174]ï
             RC4 128 stream cipher
+        sha256PrfSuites= [60, 61, 103, 107, 59, 108, 109, 49187, 49189, 49193,
+        49191, 156, 158, 166, 49195, 49197, 49201, 49199, 4865, 162, 164,
+        49308, 49310, 49324, 4868, 49312, 49314, 49326, 4869, 49309, 49311,
+        49325, 49313, 49315, 49327, 52392, 52393, 52394, 4867, 52385, 52386,
+        52387]ï
+            any that will end up using SHA256 PRF in TLS 1.2 or later
         sha256Suites= [60, 61, 103, 107, 59, 108, 109, 49187, 49189, 49193,
         49191]ï
             SHA-256 HMAC, SHA-256 PRF
         sha384PrfSuites= [49188, 49190, 49194, 49192, 163, 165, 157, 159, 167,
         49196, 49198, 49202, 49200, 4866, 163, 165]ï
-            TLS1.2 with SHA384 PRF
+            any with SHA384 PRF
         sha384Suites= [49188, 49190, 49194, 49192, 163, 165]ï
             SHA-384 HMAC, SHA-384 PRF
         shaSuites= [49178, 49181, 49184, 49179, 49182, 49185, 49180, 49183,
         49186, 10, 47, 53, 5, 22, 51, 57, 19, 50, 56, 52, 58, 27, 13, 48, 54,
         2, 49162, 49161, 49160, 49159, 49158, 49157, 49156, 49155, 49154,
         49153, 49167, 49166, 49165, 49164, 49163, 49171, 49172, 49170, 49169,
         49168, 49177, 49176, 49175, 49174, 49173]ï
@@ -594,14 +604,15 @@
         max_fragment_length= 1ï
         post_handshake_auth= 49ï
         pre_shared_key= 41ï
         psk_key_exchange_modes= 45ï
         record_size_limit= 28ï
         renegotiation_info= 65281ï
         server_name= 0ï
+        session_ticket= 35ï
         signature_algorithms= 13ï
         signature_algorithms_cert= 50ï
         srp= 12ï
         status_request= 5ï
         supported_groups= 10ï
         supported_versions= 43ï
         supports_npn= 13172ï
@@ -681,14 +692,15 @@
         certificate= 11ï
         certificate_request= 13ï
         certificate_status= 22ï
         certificate_verify= 15ï
         client_hello= 1ï
         client_key_exchange= 16ï
         encrypted_extensions= 8ï
+        end_of_early_data= 5ï
         finished= 20ï
         hello_request= 0ï
         hello_retry_request= 6ï
         key_update= 24ï
         message_hash= 254ï
         new_session_ticket= 4ï
         next_protocol= 67ï
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.defragmenter.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.defragmenter.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.defragmenter module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.defragmenter module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -156,14 +156,20 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.defragmenter.Defragmenter.get_message">
 <span class="sig-name descname"><span class="pre">get_message</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.defragmenter.Defragmenter.get_message" title="Permalink to this definition"></a></dt>
 <dd><p>Extract the highest priority complete message from buffer</p>
 </dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.defragmenter.Defragmenter.is_empty">
+<span class="sig-name descname"><span class="pre">is_empty</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.defragmenter.Defragmenter.is_empty" title="Permalink to this definition"></a></dt>
+<dd><p>Return True if all buffers are empty.</p>
+</dd></dl>
+
 </dd></dl>
 
 </section>
 
 
            </div>
           </div>
```

#### html2text {}

```diff
@@ -65,11 +65,13 @@
             Add a message type which has a dynamic size set in a header
         add_static_size(msg_type, size)ï
             Add a message type which all messages are of same length
         clear_buffers()ï
             Remove all data from buffers
         get_message()ï
             Extract the highest priority complete message from buffer
+        is_empty()ï
+            Return True if all buffers are empty.
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.dh.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.dh.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.dh module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.dh module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.errors.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.errors.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.errors module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.errors module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.extensions.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.extensions.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.extensions module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.extensions module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -1161,14 +1161,79 @@
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.extensions.</span></span><span class="sig-name descname"><span class="pre">SessionTicketExtension</span></span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference internal" href="#tlslite.extensions.TLSExtension" title="tlslite.extensions.TLSExtension"><code class="xref py py-class docutils literal notranslate"><span class="pre">TLSExtension</span></code></a></p>
+<p>Client and server session ticket extension from RFC 5077</p>
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension.__init__" title="Permalink to this definition"></a></dt>
+<dd><p>Create instance of the object.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension.__repr__">
+<span class="sig-name descname"><span class="pre">__repr__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension.__repr__" title="Permalink to this definition"></a></dt>
+<dd><p>Return human readable representation of the extension.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension.create">
+<span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ticket</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension.create" title="Permalink to this definition"></a></dt>
+<dd><p>Initializes a generic TLS extension.</p>
+<p>The extension can carry arbitrary data and have arbitrary payload, can
+be used in client hello or server hello messages.</p>
+<p>The legacy calling method uses two arguments - the <cite>extType</cite> and
+<cite>data</cite>.
+If the new calling method is used, only one argument is passed in -
+<cite>data</cite>.</p>
+<p>Child classes need to override this method so that it is possible
+to set values for all fields used by the extension.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>extType</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – if int: type of the extension encoded as an integer
+between <cite>0</cite> and <cite>2^16-1</cite></p></li>
+<li><p><strong>data</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – raw data representing extension on the wire</p></li>
+</ul>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference internal" href="#tlslite.extensions.TLSExtension" title="tlslite.extensions.TLSExtension">TLSExtension</a></p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py property">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension.extData">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">extData</span></span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension.extData" title="Permalink to this definition"></a></dt>
+<dd><p>Serialise the payload of the extension.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.SessionTicketExtension.parse">
+<span class="sig-name descname"><span class="pre">parse</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parser</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.SessionTicketExtension.parse" title="Permalink to this definition"></a></dt>
+<dd><p>Parse the extension from on the wire format.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><strong>parser</strong> (<a class="reference internal" href="tlslite.utils.codec.html#tlslite.utils.codec.Parser" title="tlslite.utils.codec.Parser"><em>Parser</em></a>) – data to be parsed</p>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference internal" href="#tlslite.extensions.SessionTicketExtension" title="tlslite.extensions.SessionTicketExtension">SessionTicketExtension</a></p>
+</dd>
+</dl>
+</dd></dl>
+
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="tlslite.extensions.SignatureAlgorithmsCertExtension">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.extensions.</span></span><span class="sig-name descname"><span class="pre">SignatureAlgorithmsCertExtension</span></span><a class="headerlink" href="#tlslite.extensions.SignatureAlgorithmsCertExtension" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">_SigListExt</span></code></p>
 <p>Client side list of supported signatures in certificates.</p>
 <p>Should be used when the signatures supported in certificates and in TLS
 messages differ.</p>
 <p>See TLS1.3 RFC</p>
```

#### html2text {}

```diff
@@ -501,14 +501,45 @@
             Serialise the payload of the extension
         parse(parser)ï
             Parse the extension from on the wire format.
               Parameters:
                   parser (Parser) â data to be parsed
               Return type:
                   ServerKeyShareExtension
+  classtlslite.extensions.SessionTicketExtensionï
+      Bases: TLSExtension
+      Client and server session ticket extension from RFC 5077
+        __init__()ï
+            Create instance of the object.
+        __repr__()ï
+            Return human readable representation of the extension.
+        create(ticket)ï
+            Initializes a generic TLS extension.
+            The extension can carry arbitrary data and have arbitrary payload,
+            can be used in client hello or server hello messages.
+            The legacy calling method uses two arguments - theextTypeanddata.
+            If the new calling method is used, only one argument is passed in -
+            data.
+            Child classes need to override this method so that it is possible
+            to set values for all fields used by the extension.
+              Parameters:
+                      * extType (int) â if int: type of the extension encoded
+                        as an integer between0and2^16-1
+                      * data (bytearray) â raw data representing extension on
+                        the wire
+              Return type:
+                  TLSExtension
+        propertyextDataï
+            Serialise the payload of the extension.
+        parse(parser)ï
+            Parse the extension from on the wire format.
+              Parameters:
+                  parser (Parser) â data to be parsed
+              Return type:
+                  SessionTicketExtension
   classtlslite.extensions.SignatureAlgorithmsCertExtensionï
       Bases: _SigListExt
       Client side list of supported signatures in certificates.
       Should be used when the signatures supported in certificates and in TLS
       messages differ.
       See TLS1.3 RFC
         __init__()ï
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehashes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakehashes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakehashes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.handshakehashes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehelpers.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakehelpers.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakehelpers module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.handshakehelpers module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakesettings.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.handshakesettings.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakesettings module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.handshakesettings module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -227,15 +227,15 @@
 <li><p><strong>padding_cb</strong> (<em>func</em>) – Callback to function computing number of padding bytes
 for TLS 1.3. Signature is cb_func(msg_size, content_type, max_size).</p></li>
 <li><p><strong>pskConfigs</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><em>list</em></a><em>(</em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#tuple" title="(in Python v3.11)"><em>tuple</em></a><em>(</em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a><em>, </em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a><em>, </em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a><em>)</em><em>)</em>) – list of tuples, first element of the tuple is the
 human readable, UTF-8 encoded, “identity” of the associated secret
 (bytearray, can be empty for TLS 1.2 and earlier), second element is
 the binary secret (bytearray), third is an optional parameter
 specifying the PRF hash to be used in TLS 1.3 (<code class="docutils literal notranslate"><span class="pre">sha256</span></code> or
-<code class="docutils literal notranslate"><span class="pre">sha384</span></code>)</p></li>
+<code class="docutils literal notranslate"><span class="pre">sha384</span></code>, with <code class="docutils literal notranslate"><span class="pre">sha256</span></code> being the default)</p></li>
 <li><p><strong>ticketKeys</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><em>list</em></a><em>(</em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a><em>)</em>) – keys to be used for encrypting and decrypting session
 tickets. First entry is the encryption key for new tickets and the
 default decryption key, subsequent entries are the fallback keys
 allowing for key rollover. The keys need to be of size appropriate
 for a selected cipher in ticketCipher, 32 bytes for ‘aes256gcm’ and
 ‘chacha20-poly1305’, 16 bytes for ‘aes128-gcm’.
 New keys should be generated regularly and replace old ones. Key use
@@ -243,14 +243,17 @@
 not be longer than 48h.
 Leave empty to disable session ticket support on server side.</p></li>
 <li><p><strong>ticketCipher</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – name of the cipher used for encrypting the session
 tickets. ‘aes256gcm’ by default, ‘aes128gcm’ or ‘chacha20-poly1305’
 alternatively.</p></li>
 <li><p><strong>ticketLifetime</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – maximum allowed lifetime of ticket encryption key,
 in seconds. 1 day by default</p></li>
+<li><p><strong>ticket_count</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – number of tickets the server will send to the client
+after establishing the connection in TLS 1.3. If a positive integer,
+it enabled support for ticket based resumption in TLS 1.2 and earlier.</p></li>
 <li><p><strong>psk_modes</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><em>list</em></a><em>(</em><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a><em>)</em>) – acceptable modes for the PSK key exchange in TLS 1.3</p></li>
 <li><p><strong>max_early_data</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – maximum number of bytes acceptable for 0-RTT
 early_data processing. In other words, how many bytes will the server
 try to process, but ignore, in case the Client Hello includes
 early_data extension.</p></li>
 <li><p><strong>use_heartbeat_extension</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – whether to support heartbeat extension from
 RFC 6520. True by default.</p></li>
```

#### html2text {}

```diff
@@ -76,15 +76,15 @@
                   content_type, max_size).
                 * pskConfigs (list(tuple(bytearray,bytearray,bytearray))) â
                   list of tuples, first element of the tuple is the human
                   readable, UTF-8 encoded, âidentityâ of the associated
                   secret (bytearray, can be empty for TLS 1.2 and earlier),
                   second element is the binary secret (bytearray), third is an
                   optional parameter specifying the PRF hash to be used in TLS
-                  1.3 (sha256 or sha384)
+                  1.3 (sha256 or sha384, with sha256 being the default)
                 * ticketKeys (list(bytearray)) â keys to be used for
                   encrypting and decrypting session tickets. First entry is the
                   encryption key for new tickets and the default decryption
                   key, subsequent entries are the fallback keys allowing for
                   key rollover. The keys need to be of size appropriate for a
                   selected cipher in ticketCipher, 32 bytes for âaes256gcmâ
                   and âchacha20-poly1305â, 16 bytes for âaes128-gcmâ.
@@ -93,14 +93,18 @@
                   life-time should not be longer than 48h. Leave empty to
                   disable session ticket support on server side.
                 * ticketCipher (str) â name of the cipher used for encrypting
                   the session tickets. âaes256gcmâ by default,
                   âaes128gcmâ or âchacha20-poly1305â alternatively.
                 * ticketLifetime (int) â maximum allowed lifetime of ticket
                   encryption key, in seconds. 1 day by default
+                * ticket_count (int) â number of tickets the server will send
+                  to the client after establishing the connection in TLS 1.3.
+                  If a positive integer, it enabled support for ticket based
+                  resumption in TLS 1.2 and earlier.
                 * psk_modes (list(str)) â acceptable modes for the PSK key
                   exchange in TLS 1.3
                 * max_early_data (int) â maximum number of bytes acceptable
                   for 0-RTT early_data processing. In other words, how many
                   bytes will the server try to process, but ignore, in case the
                   Client Hello includes early_data extension.
                 * use_heartbeat_extension (bool) â whether to support
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite package &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.asyncstatemachine.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.asyncstatemachine.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.asyncstatemachine module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.asyncstatemachine module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.clienthelper.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.clienthelper.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.clienthelper module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.clienthelper module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration package &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.httptlsconnection.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.httptlsconnection.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.httptlsconnection module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.httptlsconnection module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.imap4_tls.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.imap4_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.imap4_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.imap4_tls module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.pop3_tls.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.pop3_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.pop3_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.pop3_tls module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.smtp_tls.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.smtp_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.smtp_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.smtp_tls module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.tlsasyncdispatchermixin module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.tlsasyncdispatchermixin module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlssocketservermixin.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.tlssocketservermixin.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.tlssocketservermixin module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.tlssocketservermixin module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpcserver.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.xmlrpcserver.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.xmlrpcserver module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.xmlrpcserver module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpctransport.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.integration.xmlrpctransport.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.xmlrpctransport module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.integration.xmlrpctransport module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.keyexchange.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.keyexchange.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.keyexchange module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.keyexchange module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.mathtls.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.mathtls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.mathtls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.mathtls module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messages.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.messages.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.messages module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.messages module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -1051,14 +1051,50 @@
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="tlslite.messages.NewSessionTicket1_0">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.messages.</span></span><span class="sig-name descname"><span class="pre">NewSessionTicket1_0</span></span><a class="headerlink" href="#tlslite.messages.NewSessionTicket1_0" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference internal" href="#tlslite.messages.HelloMessage" title="tlslite.messages.HelloMessage"><code class="xref py py-class docutils literal notranslate"><span class="pre">HelloMessage</span></code></a></p>
+<p>Handling of the TLS1.0-TLS1.2 NewSessionTicket message.</p>
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.messages.NewSessionTicket1_0.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.NewSessionTicket1_0.__init__" title="Permalink to this definition"></a></dt>
+<dd><p>Create New Session Ticket object.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.messages.NewSessionTicket1_0.create">
+<span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ticket_lifetime</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ticket</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.NewSessionTicket1_0.create" title="Permalink to this definition"></a></dt>
+<dd><p>Initialise a New Session Ticket.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.messages.NewSessionTicket1_0.parse">
+<span class="sig-name descname"><span class="pre">parse</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parser</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.NewSessionTicket1_0.parse" title="Permalink to this definition"></a></dt>
+<dd><p>Parse the object from on the wire data.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.messages.NewSessionTicket1_0.write">
+<span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.NewSessionTicket1_0.write" title="Permalink to this definition"></a></dt>
+<dd><p>Serialise the message to on the wire data.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)">bytearray</a></p>
+</dd>
+</dl>
+</dd></dl>
+
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="tlslite.messages.NextProtocol">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.messages.</span></span><span class="sig-name descname"><span class="pre">NextProtocol</span></span><a class="headerlink" href="#tlslite.messages.NextProtocol" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference internal" href="#tlslite.messages.HandshakeMsg" title="tlslite.messages.HandshakeMsg"><code class="xref py py-class docutils literal notranslate"><span class="pre">HandshakeMsg</span></code></a></p>
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.messages.NextProtocol.__init__">
 <span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.NextProtocol.__init__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
@@ -1514,28 +1550,32 @@
 
 <dl class="py class">
 <dt class="sig sig-object py" id="tlslite.messages.SessionTicketPayload">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.messages.</span></span><span class="sig-name descname"><span class="pre">SessionTicketPayload</span></span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <p>Serialisation and deserialisation of server state for resumption.</p>
 <p>This is the internal (meant to be encrypted) representation of server
-state that is set to client in the NewSessionTicket message.</p>
+state that is sent to the client in the NewSessionTicket message.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Variables<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>~.version</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – implementation detail for forward compatibility</p></li>
 <li><p><strong>master_secret</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – master secret for TLS 1.2-, resumption
 master secret for TLS 1.3</p></li>
 <li><p><strong>protocol_version</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#tuple" title="(in Python v3.11)"><em>tuple</em></a>) – version of protocol that was previously
 negotiated in this session</p></li>
 <li><p><strong>cipher_suite</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – numerical ID of ciphersuite that was negotiated
 previously</p></li>
 <li><p><strong>nonce</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – nonce for TLS 1.3 KDF</p></li>
 <li><p><strong>creation_time</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – Unix time in seconds when was the ticket created</p></li>
 <li><p><strong>client_cert_chain</strong> (<a class="reference internal" href="tlslite.x509certchain.html#tlslite.x509certchain.X509CertChain" title="tlslite.x509certchain.X509CertChain"><em>X509CertChain</em></a>) – Client X509 Certificate Chain</p></li>
+<li><p><strong>encrypt_then_mac</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – The session used the encrypt_then_mac
+extension</p></li>
+<li><p><strong>extended_master_secret</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – The session used the
+extended_master_secret extension</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.messages.SessionTicketPayload.__init__">
 <span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload.__init__" title="Permalink to this definition"></a></dt>
 <dd><p>Create instance of the object.</p>
@@ -1545,15 +1585,15 @@
 <dt class="sig sig-object py" id="tlslite.messages.SessionTicketPayload.client_cert_chain">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">client_cert_chain</span></span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload.client_cert_chain" title="Permalink to this definition"></a></dt>
 <dd><p>Getter for the client_cert_chain property.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.messages.SessionTicketPayload.create">
-<span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">master_secret</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">protocol_version</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cipher_suite</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creation_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">nonce</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">client_cert_chain</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload.create" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">master_secret</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">protocol_version</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cipher_suite</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creation_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">nonce</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">client_cert_chain</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">encrypt_then_mac</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">extended_master_secret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">server_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload.create" title="Permalink to this definition"></a></dt>
 <dd><p>Initialise the object with cryptographic data.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.messages.SessionTicketPayload.parse">
 <span class="sig-name descname"><span class="pre">parse</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parser</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.messages.SessionTicketPayload.parse" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
```

#### html2text {}

```diff
@@ -421,14 +421,27 @@
             Initialise a New Session Ticket.
         parse(parser)ï
             Parse the object from on the wire data.
         write()ï
             Serialise the message to on the wire data.
               Return type:
                   bytearray
+  classtlslite.messages.NewSessionTicket1_0ï
+      Bases: HelloMessage
+      Handling of the TLS1.0-TLS1.2 NewSessionTicket message.
+        __init__()ï
+            Create New Session Ticket object.
+        create(ticket_lifetime, ticket)ï
+            Initialise a New Session Ticket.
+        parse(parser)ï
+            Parse the object from on the wire data.
+        write()ï
+            Serialise the message to on the wire data.
+              Return type:
+                  bytearray
   classtlslite.messages.NextProtocolï
       Bases: HandshakeMsg
         __init__()ï
         create(next_proto)ï
         parse(p)ï
         write(trial=False)ï
   classtlslite.messages.RecordHeader(ssl2)ï
@@ -616,35 +629,40 @@
             Serialise the key exchange parameters.
               Return type:
                   bytearray
   classtlslite.messages.SessionTicketPayloadï
       Bases: object
       Serialisation and deserialisation of server state for resumption.
       This is the internal (meant to be encrypted) representation of server
-      state that is set to client in the NewSessionTicket message.
+      state that is sent to the client in the NewSessionTicket message.
         Variables:
                 * ~.version (int) â implementation detail for forward
                   compatibility
                 * master_secret (bytearray) â master secret for TLS 1.2-,
                   resumption master secret for TLS 1.3
                 * protocol_version (tuple) â version of protocol that was
                   previously negotiated in this session
                 * cipher_suite (int) â numerical ID of ciphersuite that was
                   negotiated previously
                 * nonce (bytearray) â nonce for TLS 1.3 KDF
                 * creation_time (int) â Unix time in seconds when was the
                   ticket created
                 * client_cert_chain (X509CertChain) â Client X509 Certificate
                   Chain
+                * encrypt_then_mac (bool) â The session used the
+                  encrypt_then_mac extension
+                * extended_master_secret (bool) â The session used the
+                  extended_master_secret extension
         __init__()ï
             Create instance of the object.
         propertyclient_cert_chainï
             Getter for the client_cert_chain property.
         create(master_secret, protocol_version, cipher_suite, creation_time,
-        nonce=bytearray(b''), client_cert_chain=None)ï
+        nonce=bytearray(b''), client_cert_chain=None, encrypt_then_mac=False,
+        extended_master_secret=False, server_name=bytearray(b''))ï
             Initialise the object with cryptographic data.
         parse(parser)ï
         write()ï
   tlslite.messages.bytes_to_int(bytes, byteorder='big', *, signed=False)ï
       Return the integer represented by the given array of bytes.
         bytes
             Holds the array of bytes to convert. The argument must either
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messagesocket.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.messagesocket.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.messagesocket module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.messagesocket module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.recordlayer.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.recordlayer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.recordlayer module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.recordlayer module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.session.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.constanttime.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.session module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.constanttime module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.sessioncache module" href="tlslite.sessioncache.html" />
-    <link rel="prev" title="tlslite.recordlayer module" href="tlslite.recordlayer.html" /> 
+    <link rel="next" title="tlslite.utils.cryptomath module" href="tlslite.utils.cryptomath.html" />
+    <link rel="prev" title="tlslite.utils.compat module" href="tlslite.utils.compat.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -37,42 +37,20 @@
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul class="current">
 <li class="toctree-l1 current"><a class="reference internal" href="modules.html">tlslite</a><ul class="current">
 <li class="toctree-l2 current"><a class="reference internal" href="tlslite.html">tlslite package</a><ul class="current">
-<li class="toctree-l3"><a class="reference internal" href="tlslite.html#subpackages">Subpackages</a></li>
-<li class="toctree-l3 current"><a class="reference internal" href="tlslite.html#submodules">Submodules</a><ul class="current">
-<li class="toctree-l4"><a class="reference internal" href="tlslite.api.html">tlslite.api module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.basedb.html">tlslite.basedb module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.bufferedsocket.html">tlslite.bufferedsocket module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.checker.html">tlslite.checker module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.constants.html">tlslite.constants module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.defragmenter.html">tlslite.defragmenter module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.dh.html">tlslite.dh module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.errors.html">tlslite.errors module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.extensions.html">tlslite.extensions module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.handshakehashes.html">tlslite.handshakehashes module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.handshakehelpers.html">tlslite.handshakehelpers module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.handshakesettings.html">tlslite.handshakesettings module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.keyexchange.html">tlslite.keyexchange module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.mathtls.html">tlslite.mathtls module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.messages.html">tlslite.messages module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.messagesocket.html">tlslite.messagesocket module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.recordlayer.html">tlslite.recordlayer module</a></li>
-<li class="toctree-l4 current"><a class="current reference internal" href="#">tlslite.session module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.sessioncache.html">tlslite.sessioncache module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.tlsconnection.html">tlslite.tlsconnection module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.tlsrecordlayer.html">tlslite.tlsrecordlayer module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.verifierdb.html">tlslite.verifierdb module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.x509.html">tlslite.x509 module</a></li>
-<li class="toctree-l4"><a class="reference internal" href="tlslite.x509certchain.html">tlslite.x509certchain module</a></li>
+<li class="toctree-l3 current"><a class="reference internal" href="tlslite.html#subpackages">Subpackages</a><ul class="current">
+<li class="toctree-l4"><a class="reference internal" href="tlslite.integration.html">tlslite.integration package</a></li>
+<li class="toctree-l4 current"><a class="reference internal" href="tlslite.utils.html">tlslite.utils package</a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="tlslite.html#submodules">Submodules</a></li>
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 
         </div>
@@ -87,159 +65,171 @@
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
-      <li>tlslite.session module</li>
+          <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
+      <li>tlslite.utils.constanttime module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.session.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.constanttime.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.session">
-<span id="tlslite-session-module"></span><h1>tlslite.session module<a class="headerlink" href="#module-tlslite.session" title="Permalink to this heading"></a></h1>
-<p>Class representing a TLS session.</p>
-<dl class="py class">
-<dt class="sig sig-object py" id="tlslite.session.Session">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.session.</span></span><span class="sig-name descname"><span class="pre">Session</span></span><a class="headerlink" href="#tlslite.session.Session" title="Permalink to this definition"></a></dt>
-<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
-<p>This class represents a TLS session.</p>
-<p>TLS distinguishes between connections and sessions.  A new
-handshake creates both a connection and a session.  Data is
-transmitted over the connection.</p>
-<p>The session contains a more permanent record of the handshake.  The
-session can be inspected to determine handshake results.  The
-session can also be used to create a new connection through
-“session resumption”. If the client and server both support this,
-they can create a new connection based on an old session without
-the overhead of a full handshake.</p>
-<p>The session for a <a class="reference internal" href="tlslite.tlsconnection.html#tlslite.tlsconnection.TLSConnection" title="tlslite.tlsconnection.TLSConnection"><code class="xref py py-class docutils literal notranslate"><span class="pre">TLSConnection</span></code></a> can be
-retrieved from the connection’s ‘session’ attribute.</p>
+  <section id="module-tlslite.utils.constanttime">
+<span id="tlslite-utils-constanttime-module"></span><h1>tlslite.utils.constanttime module<a class="headerlink" href="#module-tlslite.utils.constanttime" title="Permalink to this heading"></a></h1>
+<p>Various constant time functions for processing sensitive data</p>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_check_cbc_mac_and_pad">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_check_cbc_mac_and_pad</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mac</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">seqnumBytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">contentType</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">version</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">block_size</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">16</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_check_cbc_mac_and_pad" title="Permalink to this definition"></a></dt>
+<dd><p>Check CBC cipher HMAC and padding. Close to constant time.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Variables<span class="colon">:</span></dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>srpUsername</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – The client’s SRP username (or None).</p></li>
-<li><p><strong>clientCertChain</strong> (<a class="reference internal" href="tlslite.x509certchain.html#tlslite.x509certchain.X509CertChain" title="tlslite.x509certchain.X509CertChain"><em>X509CertChain</em></a>) – The client’s certificate chain (or None).</p></li>
-<li><p><strong>serverCertChain</strong> (<a class="reference internal" href="tlslite.x509certchain.html#tlslite.x509certchain.X509CertChain" title="tlslite.x509certchain.X509CertChain"><em>X509CertChain</em></a>) – The server’s certificate chain (or None).</p></li>
-<li><p><strong>tackExt</strong> (<em>tack.structures.TackExtension.TackExtension</em>) – The server’s TackExtension (or None).</p></li>
-<li><p><strong>tackInHelloExt</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – True if a TACK was presented via TLS Extension.</p></li>
-<li><p><strong>~.encryptThenMAC</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – True if connection uses CBC cipher in
-encrypt-then-MAC mode</p></li>
-<li><p><strong>appProto</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – name of the negotiated application level protocol, None
-if not negotiated</p></li>
-<li><p><strong>cl_app_secret</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – key used for deriving keys used by client to encrypt
-and protect data in TLS 1.3</p></li>
-<li><p><strong>sr_app_secret</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – key used for deriving keys used by server to encrypt
-and protect data in TLS 1.3</p></li>
-<li><p><strong>exporterMasterSecret</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – master secret used for TLS Exporter in TLS1.3</p></li>
-<li><p><strong>resumptionMasterSecret</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – master secret used for session resumption in
-TLS 1.3</p></li>
-<li><p><strong>tickets</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><em>list</em></a>) – list of tickets received from the server</p></li>
+<li><p><strong>data</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – data with HMAC value to test and padding</p></li>
+<li><p><strong>mac</strong> (<em>hashlib mac</em>) – empty HMAC, initialised with a key</p></li>
+<li><p><strong>seqnumBytes</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – TLS sequence number, used as input to HMAC</p></li>
+<li><p><strong>contentType</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – a single byte, used as input to HMAC</p></li>
+<li><p><strong>version</strong> (<em>tuple of int</em>) – a tuple of two ints, used as input to HMAC and to guide
+checking of padding</p></li>
 </ul>
 </dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p>boolean</p>
+</dd>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>True if MAC and pad is ok, False otherwise</p>
+</dd>
 </dl>
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.__init__" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.create">
-<span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">masterSecret</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sessionID</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cipherSuite</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">srpUsername</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">clientCertChain</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">serverCertChain</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tackExt</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tackInHelloExt</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">serverName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">resumable</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">encryptThenMAC</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">extendedMasterSecret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">appProto</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cl_app_secret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sr_app_secret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exporterMasterSecret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">resumptionMasterSecret</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">bytearray(b'')</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tickets</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.create" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.getBreakSigs">
-<span class="sig-name descname"><span class="pre">getBreakSigs</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.getBreakSigs" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
+</dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.getCipherName">
-<span class="sig-name descname"><span class="pre">getCipherName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.getCipherName" title="Permalink to this definition"></a></dt>
-<dd><p>Get the name of the cipher used with this connection.</p>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_eq_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_eq_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_eq_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Return 1 if val_a == val_b, 0 otherwise. Constant time.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+</ul>
 </dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>The name of the cipher used with this connection.</p>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.getMacName">
-<span class="sig-name descname"><span class="pre">getMacName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.getMacName" title="Permalink to this definition"></a></dt>
-<dd><p>Get the name of the HMAC hash algo used with this connection.</p>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_gt_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_gt_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_gt_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Return 1 if val_a &gt; val_b, 0 otherwise. Constant time.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+</ul>
 </dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>The name of the HMAC hash algo used with this connection.</p>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.getTackId">
-<span class="sig-name descname"><span class="pre">getTackId</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.getTackId" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_isnonzero_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_isnonzero_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_isnonzero_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Returns 1 if val is != 0, 0 otherwise. Constant time.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><strong>val</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+</dd>
+</dl>
+</dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.session.Session.valid">
-<span class="sig-name descname"><span class="pre">valid</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.Session.valid" title="Permalink to this definition"></a></dt>
-<dd><p>If this session can be used for session resumption.</p>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_le_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_le_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_le_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Return 1 if val_a &lt;= val_b, 0 otherwise. Constant time.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+</ul>
 </dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>If this session can be used for session resumption.</p>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lsb_prop_u16">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lsb_prop_u16</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lsb_prop_u16" title="Permalink to this definition"></a></dt>
+<dd><p>Propagate LSB to all 16 bits of the returned int. Constant time.</p>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.session.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.session.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.session.bytes_to_int" title="Permalink to this definition"></a></dt>
-<dd><p>Return the integer represented by the given array of bytes.</p>
-<dl class="simple">
-<dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
-support the buffer protocol or be an iterable object producing bytes.
-Bytes and bytearray are examples of built-in objects that support the
-buffer protocol.</p>
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lsb_prop_u8">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lsb_prop_u8</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lsb_prop_u8" title="Permalink to this definition"></a></dt>
+<dd><p>Propagate LSB to all 8 bits of the returned int. Constant time.</p>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lt_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lt_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lt_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Returns 1 if val_a &lt; val_b, 0 otherwise. Constant time.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+</ul>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
-<dt>byteorder</dt><dd><p>The byte order used to represent the integer.  If byteorder is ‘big’,
-the most significant byte is at the beginning of the byte array.  If
-byteorder is ‘little’, the most significant byte is at the end of the
-byte array.  To request the native byte order of the host system, use
-<a href="#id1"><span class="problematic" id="id2">`</span></a>sys.byteorder’ as the byte order value.  Default is to use ‘big’.</p>
+</dl>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_neq_u32">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_neq_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_neq_u32" title="Permalink to this definition"></a></dt>
+<dd><p>Return 1 if val_a != val_b, 0 otherwise. Constant time.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+</ul>
 </dd>
-<dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.recordlayer.html" class="btn btn-neutral float-left" title="tlslite.recordlayer module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.sessioncache.html" class="btn btn-neutral float-right" title="tlslite.sessioncache module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.compat.html" class="btn btn-neutral float-left" title="tlslite.utils.compat module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.cryptomath.html" class="btn btn-neutral float-right" title="tlslite.utils.cryptomath module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -6,126 +6,94 @@
 
 tlslite-ng
 0.8
 [q                   ]
     * tlslite
           o tlslite_package
                 # Subpackages
+                      # tlslite.integration_package
+                      # tlslite.utils_package
                 # Submodules
-                      # tlslite.api_module
-                      # tlslite.basedb_module
-                      # tlslite.bufferedsocket_module
-                      # tlslite.checker_module
-                      # tlslite.constants_module
-                      # tlslite.defragmenter_module
-                      # tlslite.dh_module
-                      # tlslite.errors_module
-                      # tlslite.extensions_module
-                      # tlslite.handshakehashes_module
-                      # tlslite.handshakehelpers_module
-                      # tlslite.handshakesettings_module
-                      # tlslite.keyexchange_module
-                      # tlslite.mathtls_module
-                      # tlslite.messages_module
-                      # tlslite.messagesocket_module
-                      # tlslite.recordlayer_module
-                      # tlslite.session_module
-                      # tlslite.sessioncache_module
-                      # tlslite.tlsconnection_module
-                      # tlslite.tlsrecordlayer_module
-                      # tlslite.verifierdb_module
-                      # tlslite.x509_module
-                      # tlslite.x509certchain_module
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
-    * tlslite.session module
+    * tlslite.utils_package »
+    * tlslite.utils.constanttime module
     * View_page_source
 ===============================================================================
-****** tlslite.session moduleï ******
-Class representing a TLS session.
-  classtlslite.session.Sessionï
-      Bases: object
-      This class represents a TLS session.
-      TLS distinguishes between connections and sessions. A new handshake
-      creates both a connection and a session. Data is transmitted over the
-      connection.
-      The session contains a more permanent record of the handshake. The
-      session can be inspected to determine handshake results. The session can
-      also be used to create a new connection through âsession resumptionâ.
-      If the client and server both support this, they can create a new
-      connection based on an old session without the overhead of a full
-      handshake.
-      The session for a TLSConnection can be retrieved from the connectionâs
-      âsessionâ attribute.
-        Variables:
-                * srpUsername (str) â The clientâs SRP username (or None).
-                * clientCertChain (X509CertChain) â The clientâs
-                  certificate chain (or None).
-                * serverCertChain (X509CertChain) â The serverâs
-                  certificate chain (or None).
-                * tackExt (tack.structures.TackExtension.TackExtension) â The
-                  serverâs TackExtension (or None).
-                * tackInHelloExt (bool) â True if a TACK was presented via
-                  TLS Extension.
-                * ~.encryptThenMAC (bool) â True if connection uses CBC
-                  cipher in encrypt-then-MAC mode
-                * appProto (bytearray) â name of the negotiated application
-                  level protocol, None if not negotiated
-                * cl_app_secret (bytearray) â key used for deriving keys used
-                  by client to encrypt and protect data in TLS 1.3
-                * sr_app_secret (bytearray) â key used for deriving keys used
-                  by server to encrypt and protect data in TLS 1.3
-                * exporterMasterSecret (bytearray) â master secret used for
-                  TLS Exporter in TLS1.3
-                * resumptionMasterSecret (bytearray) â master secret used for
-                  session resumption in TLS 1.3
-                * tickets (list) â list of tickets received from the server
-        __init__()ï
-        create(masterSecret, sessionID, cipherSuite, srpUsername,
-        clientCertChain, serverCertChain, tackExt, tackInHelloExt, serverName,
-        resumable=True, encryptThenMAC=False, extendedMasterSecret=False,
-        appProto=bytearray(b''), cl_app_secret=bytearray(b''),
-        sr_app_secret=bytearray(b''), exporterMasterSecret=bytearray(b''),
-        resumptionMasterSecret=bytearray(b''), tickets=None)ï
-        getBreakSigs()ï
-        getCipherName()ï
-            Get the name of the cipher used with this connection.
-              Return type:
-                  str
-              Returns:
-                  The name of the cipher used with this connection.
-        getMacName()ï
-            Get the name of the HMAC hash algo used with this connection.
-              Return type:
-                  str
-              Returns:
-                  The name of the HMAC hash algo used with this connection.
-        getTackId()ï
-        valid()ï
-            If this session can be used for session resumption.
-              Return type:
-                  bool
-              Returns:
-                  If this session can be used for session resumption.
-  tlslite.session.bytes_to_int(bytes, byteorder='big', *, signed=False)ï
-      Return the integer represented by the given array of bytes.
-        bytes
-            Holds the array of bytes to convert. The argument must either
-            support the buffer protocol or be an iterable object producing
-            bytes. Bytes and bytearray are examples of built-in objects that
-            support the buffer protocol.
-        byteorder
-            The byte order used to represent the integer. If byteorder is
-            âbigâ, the most significant byte is at the beginning of the
-            byte array. If byteorder is âlittleâ, the most significant byte
-            is at the end of the byte array. To request the native byte order
-            of the host system, use `sys.byteorderâ as the byte order value.
-            Default is to use âbigâ.
-        signed
-            Indicates whether twoâs complement is used to represent the
-            integer.
+****** tlslite.utils.constanttime moduleï ******
+Various constant time functions for processing sensitive data
+  tlslite.utils.constanttime.ct_check_cbc_mac_and_pad(data, mac, seqnumBytes,
+  contentType, version, block_size=16)ï
+      Check CBC cipher HMAC and padding. Close to constant time.
+        Parameters:
+                * data (bytearray) â data with HMAC value to test and padding
+                * mac (hashlib mac) â empty HMAC, initialised with a key
+                * seqnumBytes (bytearray) â TLS sequence number, used as
+                  input to HMAC
+                * contentType (int) â a single byte, used as input to HMAC
+                * version (tuple of int) â a tuple of two ints, used as input
+                  to HMAC and to guide checking of padding
+        Return type:
+            boolean
+        Returns:
+            True if MAC and pad is ok, False otherwise
+  tlslite.utils.constanttime.ct_eq_u32(val_a, val_b)ï
+      Return 1 if val_a == val_b, 0 otherwise. Constant time.
+        Parameters:
+                * val_a (int) â an unsigned integer representable as a 32 bit
+                  value
+                * val_b (int) â an unsigned integer representable as a 32 bit
+                  value
+        Return type:
+            int
+  tlslite.utils.constanttime.ct_gt_u32(val_a, val_b)ï
+      Return 1 if val_a > val_b, 0 otherwise. Constant time.
+        Parameters:
+                * val_a (int) â an unsigned integer representable as a 32 bit
+                  value
+                * val_b (int) â an unsigned integer representable as a 32 bit
+                  value
+        Return type:
+            int
+  tlslite.utils.constanttime.ct_isnonzero_u32(val)ï
+      Returns 1 if val is != 0, 0 otherwise. Constant time.
+        Parameters:
+            val (int) â an unsigned integer representable as a 32 bit value
+        Return type:
+            int
+  tlslite.utils.constanttime.ct_le_u32(val_a, val_b)ï
+      Return 1 if val_a <= val_b, 0 otherwise. Constant time.
+        Parameters:
+                * val_a (int) â an unsigned integer representable as a 32 bit
+                  value
+                * val_b (int) â an unsigned integer representable as a 32 bit
+                  value
+        Return type:
+            int
+  tlslite.utils.constanttime.ct_lsb_prop_u16(val)ï
+      Propagate LSB to all 16 bits of the returned int. Constant time.
+  tlslite.utils.constanttime.ct_lsb_prop_u8(val)ï
+      Propagate LSB to all 8 bits of the returned int. Constant time.
+  tlslite.utils.constanttime.ct_lt_u32(val_a, val_b)ï
+      Returns 1 if val_a < val_b, 0 otherwise. Constant time.
+        Parameters:
+                * val_a (int) â an unsigned integer representable as a 32 bit
+                  value
+                * val_b (int) â an unsigned integer representable as a 32 bit
+                  value
+        Return type:
+            int
+  tlslite.utils.constanttime.ct_neq_u32(val_a, val_b)ï
+      Return 1 if val_a != val_b, 0 otherwise. Constant time.
+        Parameters:
+                * val_a (int) â an unsigned integer representable as a 32 bit
+                  value
+                * val_b (int) â an unsigned integer representable as a 32 bit
+                  value
+        Return type:
+            int
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.sessioncache.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.sessioncache.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.sessioncache module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.sessioncache module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsconnection.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.tlsconnection.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.tlsconnection module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.tlsconnection module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsrecordlayer.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.tlsrecordlayer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.tlsrecordlayer module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.tlsrecordlayer module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.aes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.aes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aesgcm.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.aesgcm module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.asn1parser.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.asn1parser.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.asn1parser module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.asn1parser module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.chacha.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.chacha module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.chacha module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha20_poly1305.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.chacha20_poly1305.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cipherfactory.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.cipherfactory.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.cipherfactory module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.cipherfactory module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.codec.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.codec.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.codec module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.codec module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.compat.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.compat.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.compat module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.compat module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.constanttime.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.keyfactory.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.constanttime module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.keyfactory module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.cryptomath module" href="tlslite.utils.cryptomath.html" />
-    <link rel="prev" title="tlslite.utils.compat module" href="tlslite.utils.compat.html" /> 
+    <link rel="next" title="tlslite.utils.lists module" href="tlslite.utils.lists.html" />
+    <link rel="prev" title="tlslite.utils.ecdsakey module" href="tlslite.utils.ecdsakey.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,170 +66,173 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.constanttime module</li>
+      <li>tlslite.utils.keyfactory module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.constanttime.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.keyfactory.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.constanttime">
-<span id="tlslite-utils-constanttime-module"></span><h1>tlslite.utils.constanttime module<a class="headerlink" href="#module-tlslite.utils.constanttime" title="Permalink to this heading"></a></h1>
-<p>Various constant time functions for processing sensitive data</p>
+  <section id="module-tlslite.utils.keyfactory">
+<span id="tlslite-utils-keyfactory-module"></span><h1>tlslite.utils.keyfactory module<a class="headerlink" href="#module-tlslite.utils.keyfactory" title="Permalink to this heading"></a></h1>
+<p>Factory functions for asymmetric cryptography.</p>
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_check_cbc_mac_and_pad">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_check_cbc_mac_and_pad</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mac</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">seqnumBytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">contentType</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">version</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">block_size</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">16</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_check_cbc_mac_and_pad" title="Permalink to this definition"></a></dt>
-<dd><p>Check CBC cipher HMAC and padding. Close to constant time.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>data</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – data with HMAC value to test and padding</p></li>
-<li><p><strong>mac</strong> (<em>hashlib mac</em>) – empty HMAC, initialised with a key</p></li>
-<li><p><strong>seqnumBytes</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – TLS sequence number, used as input to HMAC</p></li>
-<li><p><strong>contentType</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – a single byte, used as input to HMAC</p></li>
-<li><p><strong>version</strong> (<em>tuple of int</em>) – a tuple of two ints, used as input to HMAC and to guide
-checking of padding</p></li>
-</ul>
+<dt class="sig sig-object py" id="tlslite.utils.keyfactory.bytes_to_int">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.bytes_to_int" title="Permalink to this definition"></a></dt>
+<dd><p>Return the integer represented by the given array of bytes.</p>
+<dl class="simple">
+<dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
+support the buffer protocol or be an iterable object producing bytes.
+Bytes and bytearray are examples of built-in objects that support the
+buffer protocol.</p>
 </dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p>boolean</p>
+<dt>byteorder</dt><dd><p>The byte order used to represent the integer.  If byteorder is ‘big’,
+the most significant byte is at the beginning of the byte array.  If
+byteorder is ‘little’, the most significant byte is at the end of the
+byte array.  To request the native byte order of the host system, use
+<a href="#id1"><span class="problematic" id="id2">`</span></a>sys.byteorder’ as the byte order value.  Default is to use ‘big’.</p>
 </dd>
-<dt class="field-odd">Returns<span class="colon">:</span></dt>
-<dd class="field-odd"><p>True if MAC and pad is ok, False otherwise</p>
+<dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_eq_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_eq_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_eq_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Return 1 if val_a == val_b, 0 otherwise. Constant time.</p>
+<dt class="sig sig-object py" id="tlslite.utils.keyfactory.generateRSAKey">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">generateRSAKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bits</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">implementations</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['openssl',</span> <span class="pre">'python']</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.generateRSAKey" title="Permalink to this definition"></a></dt>
+<dd><p>Generate an RSA key with the specified bit length.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-</ul>
+<dd class="field-odd"><p><strong>bits</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – Desired bit length of the new key’s modulus.</p>
 </dd>
 <dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
+</dd>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>A new RSA private key.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_gt_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_gt_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_gt_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Return 1 if val_a &gt; val_b, 0 otherwise. Constant time.</p>
+<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parseAsPublicKey">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parseAsPublicKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parseAsPublicKey" title="Permalink to this definition"></a></dt>
+<dd><p>Parse a PEM-formatted public key.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-</ul>
+<dd class="field-odd"><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded public or private key.</p>
 </dd>
 <dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
 </dd>
-</dl>
-</dd></dl>
-
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_isnonzero_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_isnonzero_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_isnonzero_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Returns 1 if val is != 0, 0 otherwise. Constant time.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>val</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>An RSA public key.</p>
 </dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dt class="field-even">Raises<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_le_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_le_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_le_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Return 1 if val_a &lt;= val_b, 0 otherwise. Constant time.</p>
+<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parsePEMKey">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parsePEMKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">private</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">public</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">passwordCallback</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">implementations</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['openssl',</span> <span class="pre">'python']</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parsePEMKey" title="Permalink to this definition"></a></dt>
+<dd><p>Parse a PEM-format key.</p>
+<p>The PEM format is used by OpenSSL and other tools.  The
+format is typically used to store both the public and private
+components of a key.  For example:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">-----</span><span class="n">BEGIN</span> <span class="n">RSA</span> <span class="n">PRIVATE</span> <span class="n">KEY</span><span class="o">-----</span>
+ <span class="n">MIICXQIBAAKBgQDYscuoMzsGmW0pAYsmyHltxB2TdwHS0dImfjCMfaSDkfLdZY5</span><span class="o">+</span>
+ <span class="n">dOWORVns9etWnr194mSGA1F0Pls</span><span class="o">/</span><span class="n">VJW8</span><span class="o">+</span><span class="n">cX9</span><span class="o">+</span><span class="mi">3</span><span class="n">vtJV8zSdANPYUoQf0TP7VlJxkH</span>
+ <span class="n">dSRkUbEoz5bAAs</span><span class="o">/+</span><span class="mi">970</span><span class="n">uos7n7iXQIni</span><span class="o">+</span><span class="mi">3</span><span class="n">erUTdYEk2iWnMBjTljfgbK</span><span class="o">/</span><span class="n">dQIDAQAB</span>
+ <span class="n">AoGAJHoJZk75aKr7DSQNYIHuruOMdv5ZeDuJvKERWxTrVJqE32</span><span class="o">/</span><span class="n">xBKh42</span><span class="o">/</span><span class="n">IgqRrc</span>
+ <span class="n">esBN9ZregRCd7YtxoL</span><span class="o">+</span><span class="n">EVUNWaJNVx2mNmezEznrc9zhcYUrgeaVdFO2yBF1889zO</span>
+ <span class="n">gCOVwrO8uDgeyj6IKa25H6c1N13ih</span><span class="o">/</span><span class="n">o7ZzEgWbGG</span><span class="o">+</span><span class="n">ylU1yECQQDv4ZSJ4EjSh</span><span class="o">/</span><span class="n">Fl</span>
+ <span class="n">aHdz3wbBa</span><span class="o">/</span><span class="n">HKGTjC8iRy476Cyg2Fm8MZUe9Yy3udOrb5ZnS2MTpIXt5AF3h2TfYV</span>
+ <span class="n">VoFXIorjAkEA50FcJmzT8sNMrPaV8vn</span><span class="o">+</span><span class="mi">9</span><span class="n">W2Lu4U7C</span><span class="o">+</span><span class="n">K</span><span class="o">/</span><span class="n">O2g1iXMaZms5PC5zV5aV</span>
+ <span class="n">CKXZWUX1fq2RaOzlbQrpgiolhXpeh8FjxwJBAOFHzSQfSsTNfttp3KUpU0LbiVvv</span>
+ <span class="n">i</span><span class="o">+</span><span class="n">spVSnA0O4rq79KpVNmK44Mq67hsW1P11QzrzTAQ6GVaUBRv0YS061td1kCQHnP</span>
+ <span class="n">wtN2tboFR6lABkJDjxoGRvlSt4SOPr7zKGgrWjeiuTZLHXSAnCY</span><span class="o">+/</span><span class="n">hr5L9Q3ZwXG</span>
+ <span class="mi">6</span><span class="n">x6iBdgLjVIe4BZQNtcCQQDXGv</span><span class="o">/</span><span class="n">gWinCNTN3MPWfTW</span><span class="o">/</span><span class="n">RGzuMYVmyBFais0</span><span class="o">/</span><span class="n">VrgdH</span>
+ <span class="n">h1dLpztmpQqfyH</span><span class="o">/</span><span class="n">zrBXQ9qL</span><span class="o">/</span><span class="n">zR4ojS6XYneO</span><span class="o">/</span><span class="n">U18WpEe</span>
+ <span class="o">-----</span><span class="n">END</span> <span class="n">RSA</span> <span class="n">PRIVATE</span> <span class="n">KEY</span><span class="o">-----</span>
+</pre></div>
+</div>
+<p>To generate a key like this with OpenSSL, run:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">openssl</span> <span class="n">genrsa</span> <span class="mi">2048</span> <span class="o">&gt;</span> <span class="n">key</span><span class="o">.</span><span class="n">pem</span>
+</pre></div>
+</div>
+<p>This format also supports password-encrypted private keys.  TLS
+Lite can only handle password-encrypted private keys when OpenSSL
+and M2Crypto are installed.  In this case, passwordCallback will be
+invoked to query the user for the password.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
+<li><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded public or private key.</p></li>
+<li><p><strong>private</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – If True, a <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">SyntaxError</span></code></a> will be raised if the
+private key component is not present.</p></li>
+<li><p><strong>public</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – If True, the private key component (if present) will
+be discarded, so this function will always return a public key.</p></li>
+<li><p><strong>passwordCallback</strong> (<em>callable</em>) – This function will be called, with no
+arguments, if the PEM-encoded private key is password-encrypted.
+The callback should return the password string.  If the password is
+incorrect, SyntaxError will be raised.  If no callback is passed
+and the key is password-encrypted, a prompt will be displayed at
+the console.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
 </dd>
-</dl>
-</dd></dl>
-
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lsb_prop_u16">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lsb_prop_u16</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lsb_prop_u16" title="Permalink to this definition"></a></dt>
-<dd><p>Propagate LSB to all 16 bits of the returned int. Constant time.</p>
-</dd></dl>
-
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lsb_prop_u8">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lsb_prop_u8</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lsb_prop_u8" title="Permalink to this definition"></a></dt>
-<dd><p>Propagate LSB to all 8 bits of the returned int. Constant time.</p>
-</dd></dl>
-
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_lt_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_lt_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_lt_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Returns 1 if val_a &lt; val_b, 0 otherwise. Constant time.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-</ul>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>An RSA key.</p>
 </dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dt class="field-even">Raises<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.constanttime.ct_neq_u32">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.constanttime.</span></span><span class="sig-name descname"><span class="pre">ct_neq_u32</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">val_b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.constanttime.ct_neq_u32" title="Permalink to this definition"></a></dt>
-<dd><p>Return 1 if val_a != val_b, 0 otherwise. Constant time.</p>
+<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parsePrivateKey">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parsePrivateKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parsePrivateKey" title="Permalink to this definition"></a></dt>
+<dd><p>Parse a PEM-formatted private key.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>val_a</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-<li><p><strong>val_b</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – an unsigned integer representable as a 32 bit value</p></li>
-</ul>
+<dd class="field-odd"><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded private key.</p>
 </dd>
 <dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)">int</a></p>
+<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
+</dd>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
+<dd class="field-odd"><p>An RSA private key.</p>
+</dd>
+<dt class="field-even">Raises<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.compat.html" class="btn btn-neutral float-left" title="tlslite.utils.compat module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.cryptomath.html" class="btn btn-neutral float-right" title="tlslite.utils.cryptomath module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.ecdsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.ecdsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.lists.html" class="btn btn-neutral float-right" title="tlslite.utils.lists module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,86 +14,111 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.constanttime module
+    * tlslite.utils.keyfactory module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.constanttime moduleï ******
-Various constant time functions for processing sensitive data
-  tlslite.utils.constanttime.ct_check_cbc_mac_and_pad(data, mac, seqnumBytes,
-  contentType, version, block_size=16)ï
-      Check CBC cipher HMAC and padding. Close to constant time.
+****** tlslite.utils.keyfactory moduleï ******
+Factory functions for asymmetric cryptography.
+  tlslite.utils.keyfactory.bytes_to_int(bytes, byteorder='big', *,
+  signed=False)ï
+      Return the integer represented by the given array of bytes.
+        bytes
+            Holds the array of bytes to convert. The argument must either
+            support the buffer protocol or be an iterable object producing
+            bytes. Bytes and bytearray are examples of built-in objects that
+            support the buffer protocol.
+        byteorder
+            The byte order used to represent the integer. If byteorder is
+            âbigâ, the most significant byte is at the beginning of the
+            byte array. If byteorder is âlittleâ, the most significant byte
+            is at the end of the byte array. To request the native byte order
+            of the host system, use `sys.byteorderâ as the byte order value.
+            Default is to use âbigâ.
+        signed
+            Indicates whether twoâs complement is used to represent the
+            integer.
+  tlslite.utils.keyfactory.generateRSAKey(bits, implementations=['openssl',
+  'python'])ï
+      Generate an RSA key with the specified bit length.
         Parameters:
-                * data (bytearray) â data with HMAC value to test and padding
-                * mac (hashlib mac) â empty HMAC, initialised with a key
-                * seqnumBytes (bytearray) â TLS sequence number, used as
-                  input to HMAC
-                * contentType (int) â a single byte, used as input to HMAC
-                * version (tuple of int) â a tuple of two ints, used as input
-                  to HMAC and to guide checking of padding
+            bits (int) â Desired bit length of the new keyâs modulus.
         Return type:
-            boolean
+            RSAKey
         Returns:
-            True if MAC and pad is ok, False otherwise
-  tlslite.utils.constanttime.ct_eq_u32(val_a, val_b)ï
-      Return 1 if val_a == val_b, 0 otherwise. Constant time.
+            A new RSA private key.
+  tlslite.utils.keyfactory.parseAsPublicKey(s)ï
+      Parse a PEM-formatted public key.
         Parameters:
-                * val_a (int) â an unsigned integer representable as a 32 bit
-                  value
-                * val_b (int) â an unsigned integer representable as a 32 bit
-                  value
+            s (str) â A string containing a PEM-encoded public or private
+            key.
         Return type:
-            int
-  tlslite.utils.constanttime.ct_gt_u32(val_a, val_b)ï
-      Return 1 if val_a > val_b, 0 otherwise. Constant time.
-        Parameters:
-                * val_a (int) â an unsigned integer representable as a 32 bit
-                  value
-                * val_b (int) â an unsigned integer representable as a 32 bit
-                  value
-        Return type:
-            int
-  tlslite.utils.constanttime.ct_isnonzero_u32(val)ï
-      Returns 1 if val is != 0, 0 otherwise. Constant time.
-        Parameters:
-            val (int) â an unsigned integer representable as a 32 bit value
-        Return type:
-            int
-  tlslite.utils.constanttime.ct_le_u32(val_a, val_b)ï
-      Return 1 if val_a <= val_b, 0 otherwise. Constant time.
-        Parameters:
-                * val_a (int) â an unsigned integer representable as a 32 bit
-                  value
-                * val_b (int) â an unsigned integer representable as a 32 bit
-                  value
-        Return type:
-            int
-  tlslite.utils.constanttime.ct_lsb_prop_u16(val)ï
-      Propagate LSB to all 16 bits of the returned int. Constant time.
-  tlslite.utils.constanttime.ct_lsb_prop_u8(val)ï
-      Propagate LSB to all 8 bits of the returned int. Constant time.
-  tlslite.utils.constanttime.ct_lt_u32(val_a, val_b)ï
-      Returns 1 if val_a < val_b, 0 otherwise. Constant time.
-        Parameters:
-                * val_a (int) â an unsigned integer representable as a 32 bit
-                  value
-                * val_b (int) â an unsigned integer representable as a 32 bit
-                  value
+            RSAKey
+        Returns:
+            An RSA public key.
+        Raises:
+            SyntaxError â If the key is not properly formatted.
+  tlslite.utils.keyfactory.parsePEMKey(s, private=False, public=False,
+  passwordCallback=None, implementations=['openssl', 'python'])ï
+      Parse a PEM-format key.
+      The PEM format is used by OpenSSL and other tools. The format is
+      typically used to store both the public and private components of a key.
+      For example:
+      -----BEGIN RSA PRIVATE KEY-----
+       MIICXQIBAAKBgQDYscuoMzsGmW0pAYsmyHltxB2TdwHS0dImfjCMfaSDkfLdZY5+
+       dOWORVns9etWnr194mSGA1F0Pls/VJW8+cX9+3vtJV8zSdANPYUoQf0TP7VlJxkH
+       dSRkUbEoz5bAAs/+970uos7n7iXQIni+3erUTdYEk2iWnMBjTljfgbK/dQIDAQAB
+       AoGAJHoJZk75aKr7DSQNYIHuruOMdv5ZeDuJvKERWxTrVJqE32/xBKh42/IgqRrc
+       esBN9ZregRCd7YtxoL+EVUNWaJNVx2mNmezEznrc9zhcYUrgeaVdFO2yBF1889zO
+       gCOVwrO8uDgeyj6IKa25H6c1N13ih/o7ZzEgWbGG+ylU1yECQQDv4ZSJ4EjSh/Fl
+       aHdz3wbBa/HKGTjC8iRy476Cyg2Fm8MZUe9Yy3udOrb5ZnS2MTpIXt5AF3h2TfYV
+       VoFXIorjAkEA50FcJmzT8sNMrPaV8vn+9W2Lu4U7C+K/O2g1iXMaZms5PC5zV5aV
+       CKXZWUX1fq2RaOzlbQrpgiolhXpeh8FjxwJBAOFHzSQfSsTNfttp3KUpU0LbiVvv
+       i+spVSnA0O4rq79KpVNmK44Mq67hsW1P11QzrzTAQ6GVaUBRv0YS061td1kCQHnP
+       wtN2tboFR6lABkJDjxoGRvlSt4SOPr7zKGgrWjeiuTZLHXSAnCY+/hr5L9Q3ZwXG
+       6x6iBdgLjVIe4BZQNtcCQQDXGv/gWinCNTN3MPWfTW/RGzuMYVmyBFais0/VrgdH
+       h1dLpztmpQqfyH/zrBXQ9qL/zR4ojS6XYneO/U18WpEe
+       -----END RSA PRIVATE KEY-----
+      To generate a key like this with OpenSSL, run:
+      openssl genrsa 2048 > key.pem
+      This format also supports password-encrypted private keys. TLS Lite can
+      only handle password-encrypted private keys when OpenSSL and M2Crypto are
+      installed. In this case, passwordCallback will be invoked to query the
+      user for the password.
+        Parameters:
+                * s (str) â A string containing a PEM-encoded public or
+                  private key.
+                * private (bool) â If True, a SyntaxError will be raised if
+                  the private key component is not present.
+                * public (bool) â If True, the private key component (if
+                  present) will be discarded, so this function will always
+                  return a public key.
+                * passwordCallback (callable) â This function will be called,
+                  with no arguments, if the PEM-encoded private key is
+                  password-encrypted. The callback should return the password
+                  string. If the password is incorrect, SyntaxError will be
+                  raised. If no callback is passed and the key is password-
+                  encrypted, a prompt will be displayed at the console.
         Return type:
-            int
-  tlslite.utils.constanttime.ct_neq_u32(val_a, val_b)ï
-      Return 1 if val_a != val_b, 0 otherwise. Constant time.
+            RSAKey
+        Returns:
+            An RSA key.
+        Raises:
+            SyntaxError â If the key is not properly formatted.
+  tlslite.utils.keyfactory.parsePrivateKey(s)ï
+      Parse a PEM-formatted private key.
         Parameters:
-                * val_a (int) â an unsigned integer representable as a 32 bit
-                  value
-                * val_b (int) â an unsigned integer representable as a 32 bit
-                  value
+            s (str) â A string containing a PEM-encoded private key.
         Return type:
-            int
+            RSAKey
+        Returns:
+            An RSA private key.
+        Raises:
+            SyntaxError â If the key is not properly formatted.
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cryptomath.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.cryptomath.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.cryptomath module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.cryptomath module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.datefuncs.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.datefuncs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.datefuncs module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.datefuncs module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.deprecations.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.deprecations.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.deprecations module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.deprecations module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.dns_utils.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.dns_utils.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.dns_utils module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.dns_utils module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecc.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.ecc.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.ecc module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.ecc module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecdsakey.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.ecdsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.ecdsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.ecdsakey module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils package &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.keyfactory.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_rsakey.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.keyfactory module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.openssl_rsakey module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.lists module" href="tlslite.utils.lists.html" />
-    <link rel="prev" title="tlslite.utils.ecdsakey module" href="tlslite.utils.ecdsakey.html" /> 
+    <link rel="next" title="tlslite.utils.openssl_tripledes module" href="tlslite.utils.openssl_tripledes.html" />
+    <link rel="prev" title="tlslite.utils.openssl_rc4 module" href="tlslite.utils.openssl_rc4.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,173 +66,155 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.keyfactory module</li>
+      <li>tlslite.utils.openssl_rsakey module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.keyfactory.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.openssl_rsakey.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.keyfactory">
-<span id="tlslite-utils-keyfactory-module"></span><h1>tlslite.utils.keyfactory module<a class="headerlink" href="#module-tlslite.utils.keyfactory" title="Permalink to this heading"></a></h1>
-<p>Factory functions for asymmetric cryptography.</p>
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.keyfactory.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.bytes_to_int" title="Permalink to this definition"></a></dt>
-<dd><p>Return the integer represented by the given array of bytes.</p>
-<dl class="simple">
-<dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
-support the buffer protocol or be an iterable object producing bytes.
-Bytes and bytearray are examples of built-in objects that support the
-buffer protocol.</p>
-</dd>
-<dt>byteorder</dt><dd><p>The byte order used to represent the integer.  If byteorder is ‘big’,
-the most significant byte is at the beginning of the byte array.  If
-byteorder is ‘little’, the most significant byte is at the end of the
-byte array.  To request the native byte order of the host system, use
-<a href="#id1"><span class="problematic" id="id2">`</span></a>sys.byteorder’ as the byte order value.  Default is to use ‘big’.</p>
-</dd>
-<dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
+  <section id="module-tlslite.utils.openssl_rsakey">
+<span id="tlslite-utils-openssl-rsakey-module"></span><h1>tlslite.utils.openssl_rsakey module<a class="headerlink" href="#module-tlslite.utils.openssl_rsakey" title="Permalink to this heading"></a></h1>
+<p>OpenSSL/M2Crypto RSA implementation.</p>
+<dl class="py class">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">OpenSSL_RSAKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">e</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><code class="xref py py-class docutils literal notranslate"><span class="pre">RSAKey</span></code></a></p>
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__del__">
+<span class="sig-name descname"><span class="pre">__del__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__del__" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__getattr__">
+<span class="sig-name descname"><span class="pre">__getattr__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__getattr__" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">e</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__init__" title="Permalink to this definition"></a></dt>
+<dd><p>Create a new RSA key.</p>
+<p>If n and e are passed in, the new key will be initialized.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>n</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – RSA modulus.</p></li>
+<li><p><strong>e</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – RSA public exponent.</p></li>
+<li><p><strong>key_type</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – type of the RSA key, “rsa” for rsaEncryption
+(universal, able to perform all operations) or “rsa-pss” for a
+RSASSA-PSS key (able to perform only RSA-PSS signature verification
+and creation)</p></li>
+</ul>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.keyfactory.generateRSAKey">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">generateRSAKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bits</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">implementations</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['openssl',</span> <span class="pre">'python']</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.generateRSAKey" title="Permalink to this definition"></a></dt>
-<dd><p>Generate an RSA key with the specified bit length.</p>
+<dl class="py attribute">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__module__">
+<span class="sig-name descname"><span class="pre">__module__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'tlslite.utils.openssl_rsakey'</span></em><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__module__" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.acceptsPassword">
+<span class="sig-name descname"><span class="pre">acceptsPassword</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.acceptsPassword" title="Permalink to this definition"></a></dt>
+<dd><p>Return True if the write() method accepts a password for use
+in encrypting the private key.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>bits</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – Desired bit length of the new key’s modulus.</p>
-</dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
-</dd>
-<dt class="field-odd">Returns<span class="colon">:</span></dt>
-<dd class="field-odd"><p>A new RSA private key.</p>
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parseAsPublicKey">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parseAsPublicKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parseAsPublicKey" title="Permalink to this definition"></a></dt>
-<dd><p>Parse a PEM-formatted public key.</p>
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.generate">
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">generate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bits</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.generate" title="Permalink to this definition"></a></dt>
+<dd><p>Generate a new key with the specified bit length.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded public or private key.</p>
-</dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
-</dd>
-<dt class="field-odd">Returns<span class="colon">:</span></dt>
-<dd class="field-odd"><p>An RSA public key.</p>
-</dd>
-<dt class="field-even">Raises<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><em>RSAKey</em></p>
 </dd>
 </dl>
 </dd></dl>
 
-<dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parsePEMKey">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parsePEMKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">private</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">public</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">passwordCallback</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">implementations</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['openssl',</span> <span class="pre">'python']</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parsePEMKey" title="Permalink to this definition"></a></dt>
-<dd><p>Parse a PEM-format key.</p>
-<p>The PEM format is used by OpenSSL and other tools.  The
-format is typically used to store both the public and private
-components of a key.  For example:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">-----</span><span class="n">BEGIN</span> <span class="n">RSA</span> <span class="n">PRIVATE</span> <span class="n">KEY</span><span class="o">-----</span>
- <span class="n">MIICXQIBAAKBgQDYscuoMzsGmW0pAYsmyHltxB2TdwHS0dImfjCMfaSDkfLdZY5</span><span class="o">+</span>
- <span class="n">dOWORVns9etWnr194mSGA1F0Pls</span><span class="o">/</span><span class="n">VJW8</span><span class="o">+</span><span class="n">cX9</span><span class="o">+</span><span class="mi">3</span><span class="n">vtJV8zSdANPYUoQf0TP7VlJxkH</span>
- <span class="n">dSRkUbEoz5bAAs</span><span class="o">/+</span><span class="mi">970</span><span class="n">uos7n7iXQIni</span><span class="o">+</span><span class="mi">3</span><span class="n">erUTdYEk2iWnMBjTljfgbK</span><span class="o">/</span><span class="n">dQIDAQAB</span>
- <span class="n">AoGAJHoJZk75aKr7DSQNYIHuruOMdv5ZeDuJvKERWxTrVJqE32</span><span class="o">/</span><span class="n">xBKh42</span><span class="o">/</span><span class="n">IgqRrc</span>
- <span class="n">esBN9ZregRCd7YtxoL</span><span class="o">+</span><span class="n">EVUNWaJNVx2mNmezEznrc9zhcYUrgeaVdFO2yBF1889zO</span>
- <span class="n">gCOVwrO8uDgeyj6IKa25H6c1N13ih</span><span class="o">/</span><span class="n">o7ZzEgWbGG</span><span class="o">+</span><span class="n">ylU1yECQQDv4ZSJ4EjSh</span><span class="o">/</span><span class="n">Fl</span>
- <span class="n">aHdz3wbBa</span><span class="o">/</span><span class="n">HKGTjC8iRy476Cyg2Fm8MZUe9Yy3udOrb5ZnS2MTpIXt5AF3h2TfYV</span>
- <span class="n">VoFXIorjAkEA50FcJmzT8sNMrPaV8vn</span><span class="o">+</span><span class="mi">9</span><span class="n">W2Lu4U7C</span><span class="o">+</span><span class="n">K</span><span class="o">/</span><span class="n">O2g1iXMaZms5PC5zV5aV</span>
- <span class="n">CKXZWUX1fq2RaOzlbQrpgiolhXpeh8FjxwJBAOFHzSQfSsTNfttp3KUpU0LbiVvv</span>
- <span class="n">i</span><span class="o">+</span><span class="n">spVSnA0O4rq79KpVNmK44Mq67hsW1P11QzrzTAQ6GVaUBRv0YS061td1kCQHnP</span>
- <span class="n">wtN2tboFR6lABkJDjxoGRvlSt4SOPr7zKGgrWjeiuTZLHXSAnCY</span><span class="o">+/</span><span class="n">hr5L9Q3ZwXG</span>
- <span class="mi">6</span><span class="n">x6iBdgLjVIe4BZQNtcCQQDXGv</span><span class="o">/</span><span class="n">gWinCNTN3MPWfTW</span><span class="o">/</span><span class="n">RGzuMYVmyBFais0</span><span class="o">/</span><span class="n">VrgdH</span>
- <span class="n">h1dLpztmpQqfyH</span><span class="o">/</span><span class="n">zrBXQ9qL</span><span class="o">/</span><span class="n">zR4ojS6XYneO</span><span class="o">/</span><span class="n">U18WpEe</span>
- <span class="o">-----</span><span class="n">END</span> <span class="n">RSA</span> <span class="n">PRIVATE</span> <span class="n">KEY</span><span class="o">-----</span>
-</pre></div>
-</div>
-<p>To generate a key like this with OpenSSL, run:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">openssl</span> <span class="n">genrsa</span> <span class="mi">2048</span> <span class="o">&gt;</span> <span class="n">key</span><span class="o">.</span><span class="n">pem</span>
-</pre></div>
-</div>
-<p>This format also supports password-encrypted private keys.  TLS
-Lite can only handle password-encrypted private keys when OpenSSL
-and M2Crypto are installed.  In this case, passwordCallback will be
-invoked to query the user for the password.</p>
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.hasPrivateKey">
+<span class="sig-name descname"><span class="pre">hasPrivateKey</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.hasPrivateKey" title="Permalink to this definition"></a></dt>
+<dd><p>Return whether or not this key has a private component.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded public or private key.</p></li>
-<li><p><strong>private</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – If True, a <a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">SyntaxError</span></code></a> will be raised if the
-private key component is not present.</p></li>
-<li><p><strong>public</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><em>bool</em></a>) – If True, the private key component (if present) will
-be discarded, so this function will always return a public key.</p></li>
-<li><p><strong>passwordCallback</strong> (<em>callable</em>) – This function will be called, with no
-arguments, if the PEM-encoded private key is password-encrypted.
-The callback should return the password string.  If the password is
-incorrect, SyntaxError will be raised.  If no callback is passed
-and the key is password-encrypted, a prompt will be displayed at
-the console.</p></li>
-</ul>
-</dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
 </dd>
-<dt class="field-odd">Returns<span class="colon">:</span></dt>
-<dd class="field-odd"><p>An RSA key.</p>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.parse">
+<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">parse</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">passwordCallback</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.parse" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.write">
+<span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">password</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.write" title="Permalink to this definition"></a></dt>
+<dd><p>Return a string containing the key.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
 </dd>
-<dt class="field-even">Raises<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A string describing the key, in whichever format (PEM)
+is native to the implementation.</p>
 </dd>
 </dl>
 </dd></dl>
 
+</dd></dl>
+
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.keyfactory.parsePrivateKey">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.keyfactory.</span></span><span class="sig-name descname"><span class="pre">parsePrivateKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.keyfactory.parsePrivateKey" title="Permalink to this definition"></a></dt>
-<dd><p>Parse a PEM-formatted private key.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><p><strong>s</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – A string containing a PEM-encoded private key.</p>
-</dd>
-<dt class="field-even">Return type<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><em>RSAKey</em></a></p>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.bytes_to_int">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.bytes_to_int" title="Permalink to this definition"></a></dt>
+<dd><p>Return the integer represented by the given array of bytes.</p>
+<dl class="simple">
+<dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
+support the buffer protocol or be an iterable object producing bytes.
+Bytes and bytearray are examples of built-in objects that support the
+buffer protocol.</p>
 </dd>
-<dt class="field-odd">Returns<span class="colon">:</span></dt>
-<dd class="field-odd"><p>An RSA private key.</p>
+<dt>byteorder</dt><dd><p>The byte order used to represent the integer.  If byteorder is ‘big’,
+the most significant byte is at the beginning of the byte array.  If
+byteorder is ‘little’, the most significant byte is at the end of the
+byte array.  To request the native byte order of the host system, use
+<a href="#id1"><span class="problematic" id="id2">`</span></a>sys.byteorder’ as the byte order value.  Default is to use ‘big’.</p>
 </dd>
-<dt class="field-even">Raises<span class="colon">:</span></dt>
-<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/exceptions.html#SyntaxError" title="(in Python v3.11)"><strong>SyntaxError</strong></a> – If the key is not properly formatted.</p>
+<dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.password_callback">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">password_callback</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">v</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prompt1</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'Enter</span> <span class="pre">private</span> <span class="pre">key</span> <span class="pre">passphrase:'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prompt2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'Verify</span> <span class="pre">passphrase:'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.password_callback" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.ecdsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.ecdsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.lists.html" class="btn btn-neutral float-right" title="tlslite.utils.lists module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.openssl_rc4.html" class="btn btn-neutral float-left" title="tlslite.utils.openssl_rc4 module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.openssl_tripledes.html" class="btn btn-neutral float-right" title="tlslite.utils.openssl_tripledes module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,20 +14,57 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.keyfactory module
+    * tlslite.utils.openssl_rsakey module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.keyfactory moduleï ******
-Factory functions for asymmetric cryptography.
-  tlslite.utils.keyfactory.bytes_to_int(bytes, byteorder='big', *,
+****** tlslite.utils.openssl_rsakey moduleï ******
+OpenSSL/M2Crypto RSA implementation.
+  classtlslite.utils.openssl_rsakey.OpenSSL_RSAKey(n=0, e=0, key_type='rsa')ï
+      Bases: RSAKey
+        __del__()ï
+        __getattr__(name)ï
+        __init__(n=0, e=0, key_type='rsa')ï
+            Create a new RSA key.
+            If n and e are passed in, the new key will be initialized.
+              Parameters:
+                      * n (int) â RSA modulus.
+                      * e (int) â RSA public exponent.
+                      * key_type (str) â type of the RSA key, ârsaâ for
+                        rsaEncryption (universal, able to perform all
+                        operations) or ârsa-pssâ for a RSASSA-PSS key (able
+                        to perform only RSA-PSS signature verification and
+                        creation)
+        __module__= 'tlslite.utils.openssl_rsakey'ï
+        acceptsPassword()ï
+            Return True if the write() method accepts a password for use in
+            encrypting the private key.
+              Return type:
+                  bool
+        staticgenerate(bits, key_type='rsa')ï
+            Generate a new key with the specified bit length.
+              Return type:
+                  RSAKey
+        hasPrivateKey()ï
+            Return whether or not this key has a private component.
+              Return type:
+                  bool
+        staticparse(s, passwordCallback=None)ï
+        write(password=None)ï
+            Return a string containing the key.
+              Return type:
+                  str
+              Returns:
+                  A string describing the key, in whichever format (PEM) is
+                  native to the implementation.
+  tlslite.utils.openssl_rsakey.bytes_to_int(bytes, byteorder='big', *,
   signed=False)ï
       Return the integer represented by the given array of bytes.
         bytes
             Holds the array of bytes to convert. The argument must either
             support the buffer protocol or be an iterable object producing
             bytes. Bytes and bytearray are examples of built-in objects that
             support the buffer protocol.
@@ -37,88 +74,13 @@
             byte array. If byteorder is âlittleâ, the most significant byte
             is at the end of the byte array. To request the native byte order
             of the host system, use `sys.byteorderâ as the byte order value.
             Default is to use âbigâ.
         signed
             Indicates whether twoâs complement is used to represent the
             integer.
-  tlslite.utils.keyfactory.generateRSAKey(bits, implementations=['openssl',
-  'python'])ï
-      Generate an RSA key with the specified bit length.
-        Parameters:
-            bits (int) â Desired bit length of the new keyâs modulus.
-        Return type:
-            RSAKey
-        Returns:
-            A new RSA private key.
-  tlslite.utils.keyfactory.parseAsPublicKey(s)ï
-      Parse a PEM-formatted public key.
-        Parameters:
-            s (str) â A string containing a PEM-encoded public or private
-            key.
-        Return type:
-            RSAKey
-        Returns:
-            An RSA public key.
-        Raises:
-            SyntaxError â If the key is not properly formatted.
-  tlslite.utils.keyfactory.parsePEMKey(s, private=False, public=False,
-  passwordCallback=None, implementations=['openssl', 'python'])ï
-      Parse a PEM-format key.
-      The PEM format is used by OpenSSL and other tools. The format is
-      typically used to store both the public and private components of a key.
-      For example:
-      -----BEGIN RSA PRIVATE KEY-----
-       MIICXQIBAAKBgQDYscuoMzsGmW0pAYsmyHltxB2TdwHS0dImfjCMfaSDkfLdZY5+
-       dOWORVns9etWnr194mSGA1F0Pls/VJW8+cX9+3vtJV8zSdANPYUoQf0TP7VlJxkH
-       dSRkUbEoz5bAAs/+970uos7n7iXQIni+3erUTdYEk2iWnMBjTljfgbK/dQIDAQAB
-       AoGAJHoJZk75aKr7DSQNYIHuruOMdv5ZeDuJvKERWxTrVJqE32/xBKh42/IgqRrc
-       esBN9ZregRCd7YtxoL+EVUNWaJNVx2mNmezEznrc9zhcYUrgeaVdFO2yBF1889zO
-       gCOVwrO8uDgeyj6IKa25H6c1N13ih/o7ZzEgWbGG+ylU1yECQQDv4ZSJ4EjSh/Fl
-       aHdz3wbBa/HKGTjC8iRy476Cyg2Fm8MZUe9Yy3udOrb5ZnS2MTpIXt5AF3h2TfYV
-       VoFXIorjAkEA50FcJmzT8sNMrPaV8vn+9W2Lu4U7C+K/O2g1iXMaZms5PC5zV5aV
-       CKXZWUX1fq2RaOzlbQrpgiolhXpeh8FjxwJBAOFHzSQfSsTNfttp3KUpU0LbiVvv
-       i+spVSnA0O4rq79KpVNmK44Mq67hsW1P11QzrzTAQ6GVaUBRv0YS061td1kCQHnP
-       wtN2tboFR6lABkJDjxoGRvlSt4SOPr7zKGgrWjeiuTZLHXSAnCY+/hr5L9Q3ZwXG
-       6x6iBdgLjVIe4BZQNtcCQQDXGv/gWinCNTN3MPWfTW/RGzuMYVmyBFais0/VrgdH
-       h1dLpztmpQqfyH/zrBXQ9qL/zR4ojS6XYneO/U18WpEe
-       -----END RSA PRIVATE KEY-----
-      To generate a key like this with OpenSSL, run:
-      openssl genrsa 2048 > key.pem
-      This format also supports password-encrypted private keys. TLS Lite can
-      only handle password-encrypted private keys when OpenSSL and M2Crypto are
-      installed. In this case, passwordCallback will be invoked to query the
-      user for the password.
-        Parameters:
-                * s (str) â A string containing a PEM-encoded public or
-                  private key.
-                * private (bool) â If True, a SyntaxError will be raised if
-                  the private key component is not present.
-                * public (bool) â If True, the private key component (if
-                  present) will be discarded, so this function will always
-                  return a public key.
-                * passwordCallback (callable) â This function will be called,
-                  with no arguments, if the PEM-encoded private key is
-                  password-encrypted. The callback should return the password
-                  string. If the password is incorrect, SyntaxError will be
-                  raised. If no callback is passed and the key is password-
-                  encrypted, a prompt will be displayed at the console.
-        Return type:
-            RSAKey
-        Returns:
-            An RSA key.
-        Raises:
-            SyntaxError â If the key is not properly formatted.
-  tlslite.utils.keyfactory.parsePrivateKey(s)ï
-      Parse a PEM-formatted private key.
-        Parameters:
-            s (str) â A string containing a PEM-encoded private key.
-        Return type:
-            RSAKey
-        Returns:
-            An RSA private key.
-        Raises:
-            SyntaxError â If the key is not properly formatted.
+  tlslite.utils.openssl_rsakey.password_callback(v, prompt1='Enter private key
+  passphrase:', prompt2='Verify passphrase:')ï
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.lists.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.lists.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.lists module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.lists module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_aes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_aes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.openssl_aes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rc4.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.openssl_rc4 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rsakey.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.openssl_tripledes.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.openssl_tripledes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.openssl_tripledes module" href="tlslite.utils.openssl_tripledes.html" />
-    <link rel="prev" title="tlslite.utils.openssl_rc4 module" href="tlslite.utils.openssl_rc4.html" /> 
+    <link rel="next" title="tlslite.utils.pem module" href="tlslite.utils.pem.html" />
+    <link rel="prev" title="tlslite.utils.openssl_rsakey module" href="tlslite.utils.openssl_rsakey.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,124 +66,61 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.openssl_rsakey module</li>
+      <li>tlslite.utils.openssl_tripledes module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.openssl_rsakey.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.openssl_tripledes.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.openssl_rsakey">
-<span id="tlslite-utils-openssl-rsakey-module"></span><h1>tlslite.utils.openssl_rsakey module<a class="headerlink" href="#module-tlslite.utils.openssl_rsakey" title="Permalink to this heading"></a></h1>
-<p>OpenSSL/M2Crypto RSA implementation.</p>
+  <section id="module-tlslite.utils.openssl_tripledes">
+<span id="tlslite-utils-openssl-tripledes-module"></span><h1>tlslite.utils.openssl_tripledes module<a class="headerlink" href="#module-tlslite.utils.openssl_tripledes" title="Permalink to this heading"></a></h1>
+<p>OpenSSL/M2Crypto 3DES implementation.</p>
 <dl class="py class">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">OpenSSL_RSAKey</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">e</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey" title="Permalink to this definition"></a></dt>
-<dd><p>Bases: <a class="reference internal" href="tlslite.utils.rsakey.html#tlslite.utils.rsakey.RSAKey" title="tlslite.utils.rsakey.RSAKey"><code class="xref py py-class docutils literal notranslate"><span class="pre">RSAKey</span></code></a></p>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">OpenSSL_TripleDES</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference internal" href="tlslite.utils.tripledes.html#tlslite.utils.tripledes.TripleDES" title="tlslite.utils.tripledes.TripleDES"><code class="xref py py-class docutils literal notranslate"><span class="pre">TripleDES</span></code></a></p>
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__del__">
-<span class="sig-name descname"><span class="pre">__del__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__del__" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__del__">
+<span class="sig-name descname"><span class="pre">__del__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__del__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__getattr__">
-<span class="sig-name descname"><span class="pre">__getattr__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__getattr__" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__init__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">e</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__init__" title="Permalink to this definition"></a></dt>
-<dd><p>Create a new RSA key.</p>
-<p>If n and e are passed in, the new key will be initialized.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>n</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – RSA modulus.</p></li>
-<li><p><strong>e</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – RSA public exponent.</p></li>
-<li><p><strong>key_type</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><em>str</em></a>) – type of the RSA key, “rsa” for rsaEncryption
-(universal, able to perform all operations) or “rsa-pss” for a
-RSASSA-PSS key (able to perform only RSA-PSS signature verification
-and creation)</p></li>
-</ul>
-</dd>
-</dl>
-</dd></dl>
-
 <dl class="py attribute">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__module__">
-<span class="sig-name descname"><span class="pre">__module__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'tlslite.utils.openssl_rsakey'</span></em><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.__module__" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__module__">
+<span class="sig-name descname"><span class="pre">__module__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'tlslite.utils.openssl_tripledes'</span></em><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__module__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.acceptsPassword">
-<span class="sig-name descname"><span class="pre">acceptsPassword</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.acceptsPassword" title="Permalink to this definition"></a></dt>
-<dd><p>Return True if the write() method accepts a password for use
-in encrypting the private key.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
-</dd>
-</dl>
-</dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.generate">
-<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">generate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bits</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rsa'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.generate" title="Permalink to this definition"></a></dt>
-<dd><p>Generate a new key with the specified bit length.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><em>RSAKey</em></p>
-</dd>
-</dl>
-</dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.hasPrivateKey">
-<span class="sig-name descname"><span class="pre">hasPrivateKey</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.hasPrivateKey" title="Permalink to this definition"></a></dt>
-<dd><p>Return whether or not this key has a private component.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)">bool</a></p>
-</dd>
-</dl>
-</dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.parse">
-<em class="property"><span class="pre">static</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">parse</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">passwordCallback</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.parse" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.decrypt">
+<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.decrypt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.write">
-<span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">password</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.OpenSSL_RSAKey.write" title="Permalink to this definition"></a></dt>
-<dd><p>Return a string containing the key.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Return type<span class="colon">:</span></dt>
-<dd class="field-odd"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)">str</a></p>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>A string describing the key, in whichever format (PEM)
-is native to the implementation.</p>
-</dd>
-</dl>
-</dd></dl>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.encrypt">
+<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.encrypt" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.bytes_to_int" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.bytes_to_int">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.bytes_to_int" title="Permalink to this definition"></a></dt>
 <dd><p>Return the integer represented by the given array of bytes.</p>
 <dl class="simple">
 <dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
 support the buffer protocol or be an iterable object producing bytes.
 Bytes and bytearray are examples of built-in objects that support the
 buffer protocol.</p>
 </dd>
@@ -195,26 +132,26 @@
 </dd>
 <dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_rsakey.password_callback">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_rsakey.</span></span><span class="sig-name descname"><span class="pre">password_callback</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">v</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prompt1</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'Enter</span> <span class="pre">private</span> <span class="pre">key</span> <span class="pre">passphrase:'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">prompt2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'Verify</span> <span class="pre">passphrase:'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_rsakey.password_callback" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.new">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.new" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.openssl_rc4.html" class="btn btn-neutral float-left" title="tlslite.utils.openssl_rc4 module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.openssl_tripledes.html" class="btn btn-neutral float-right" title="tlslite.utils.openssl_tripledes module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.openssl_rsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.openssl_rsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.pem.html" class="btn btn-neutral float-right" title="tlslite.utils.pem module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,57 +14,27 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.openssl_rsakey module
+    * tlslite.utils.openssl_tripledes module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.openssl_rsakey moduleï ******
-OpenSSL/M2Crypto RSA implementation.
-  classtlslite.utils.openssl_rsakey.OpenSSL_RSAKey(n=0, e=0, key_type='rsa')ï
-      Bases: RSAKey
+****** tlslite.utils.openssl_tripledes moduleï ******
+OpenSSL/M2Crypto 3DES implementation.
+  classtlslite.utils.openssl_tripledes.OpenSSL_TripleDES(key, mode, IV)ï
+      Bases: TripleDES
         __del__()ï
-        __getattr__(name)ï
-        __init__(n=0, e=0, key_type='rsa')ï
-            Create a new RSA key.
-            If n and e are passed in, the new key will be initialized.
-              Parameters:
-                      * n (int) â RSA modulus.
-                      * e (int) â RSA public exponent.
-                      * key_type (str) â type of the RSA key, ârsaâ for
-                        rsaEncryption (universal, able to perform all
-                        operations) or ârsa-pssâ for a RSASSA-PSS key (able
-                        to perform only RSA-PSS signature verification and
-                        creation)
-        __module__= 'tlslite.utils.openssl_rsakey'ï
-        acceptsPassword()ï
-            Return True if the write() method accepts a password for use in
-            encrypting the private key.
-              Return type:
-                  bool
-        staticgenerate(bits, key_type='rsa')ï
-            Generate a new key with the specified bit length.
-              Return type:
-                  RSAKey
-        hasPrivateKey()ï
-            Return whether or not this key has a private component.
-              Return type:
-                  bool
-        staticparse(s, passwordCallback=None)ï
-        write(password=None)ï
-            Return a string containing the key.
-              Return type:
-                  str
-              Returns:
-                  A string describing the key, in whichever format (PEM) is
-                  native to the implementation.
-  tlslite.utils.openssl_rsakey.bytes_to_int(bytes, byteorder='big', *,
+        __init__(key, mode, IV)ï
+        __module__= 'tlslite.utils.openssl_tripledes'ï
+        decrypt(ciphertext)ï
+        encrypt(plaintext)ï
+  tlslite.utils.openssl_tripledes.bytes_to_int(bytes, byteorder='big', *,
   signed=False)ï
       Return the integer represented by the given array of bytes.
         bytes
             Holds the array of bytes to convert. The argument must either
             support the buffer protocol or be an iterable object producing
             bytes. Bytes and bytearray are examples of built-in objects that
             support the buffer protocol.
@@ -74,13 +44,12 @@
             byte array. If byteorder is âlittleâ, the most significant byte
             is at the end of the byte array. To request the native byte order
             of the host system, use `sys.byteorderâ as the byte order value.
             Default is to use âbigâ.
         signed
             Indicates whether twoâs complement is used to represent the
             integer.
-  tlslite.utils.openssl_rsakey.password_callback(v, prompt1='Enter private key
-  passphrase:', prompt2='Verify passphrase:')ï
+  tlslite.utils.openssl_tripledes.new(key, mode, IV)ï
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_tripledes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_tripledes.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pycrypto_tripledes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.pem module" href="tlslite.utils.pem.html" />
-    <link rel="prev" title="tlslite.utils.openssl_rsakey module" href="tlslite.utils.openssl_rsakey.html" /> 
+    <link rel="next" title="tlslite.utils.python_aes module" href="tlslite.utils.python_aes.html" />
+    <link rel="prev" title="tlslite.utils.pycrypto_rsakey module" href="tlslite.utils.pycrypto_rsakey.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,61 +66,51 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.openssl_tripledes module</li>
+      <li>tlslite.utils.pycrypto_tripledes module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.openssl_tripledes.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.pycrypto_tripledes.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.openssl_tripledes">
-<span id="tlslite-utils-openssl-tripledes-module"></span><h1>tlslite.utils.openssl_tripledes module<a class="headerlink" href="#module-tlslite.utils.openssl_tripledes" title="Permalink to this heading"></a></h1>
-<p>OpenSSL/M2Crypto 3DES implementation.</p>
+  <section id="module-tlslite.utils.pycrypto_tripledes">
+<span id="tlslite-utils-pycrypto-tripledes-module"></span><h1>tlslite.utils.pycrypto_tripledes module<a class="headerlink" href="#module-tlslite.utils.pycrypto_tripledes" title="Permalink to this heading"></a></h1>
+<p>PyCrypto 3DES implementation.</p>
 <dl class="py class">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">OpenSSL_TripleDES</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">PyCrypto_TripleDES</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference internal" href="tlslite.utils.tripledes.html#tlslite.utils.tripledes.TripleDES" title="tlslite.utils.tripledes.TripleDES"><code class="xref py py-class docutils literal notranslate"><span class="pre">TripleDES</span></code></a></p>
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__del__">
-<span class="sig-name descname"><span class="pre">__del__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__del__" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.__init__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__init__" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py attribute">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__module__">
-<span class="sig-name descname"><span class="pre">__module__</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'tlslite.utils.openssl_tripledes'</span></em><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__module__" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.decrypt">
-<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.decrypt" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.decrypt">
+<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.decrypt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.encrypt">
-<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.encrypt" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.encrypt">
+<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.encrypt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.bytes_to_int" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.bytes_to_int">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.bytes_to_int" title="Permalink to this definition"></a></dt>
 <dd><p>Return the integer represented by the given array of bytes.</p>
 <dl class="simple">
 <dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
 support the buffer protocol or be an iterable object producing bytes.
 Bytes and bytearray are examples of built-in objects that support the
 buffer protocol.</p>
 </dd>
@@ -132,26 +122,26 @@
 </dd>
 <dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.openssl_tripledes.new">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.openssl_tripledes.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.openssl_tripledes.new" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.new">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.new" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.openssl_rsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.openssl_rsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.pem.html" class="btn btn-neutral float-right" title="tlslite.utils.pem module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.pycrypto_rsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.pycrypto_rsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.python_aes.html" class="btn btn-neutral float-right" title="tlslite.utils.python_aes module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,27 +14,25 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.openssl_tripledes module
+    * tlslite.utils.pycrypto_tripledes module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.openssl_tripledes moduleï ******
-OpenSSL/M2Crypto 3DES implementation.
-  classtlslite.utils.openssl_tripledes.OpenSSL_TripleDES(key, mode, IV)ï
+****** tlslite.utils.pycrypto_tripledes moduleï ******
+PyCrypto 3DES implementation.
+  classtlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES(key, mode, IV)ï
       Bases: TripleDES
-        __del__()ï
         __init__(key, mode, IV)ï
-        __module__= 'tlslite.utils.openssl_tripledes'ï
         decrypt(ciphertext)ï
         encrypt(plaintext)ï
-  tlslite.utils.openssl_tripledes.bytes_to_int(bytes, byteorder='big', *,
+  tlslite.utils.pycrypto_tripledes.bytes_to_int(bytes, byteorder='big', *,
   signed=False)ï
       Return the integer represented by the given array of bytes.
         bytes
             Holds the array of bytes to convert. The argument must either
             support the buffer protocol or be an iterable object producing
             bytes. Bytes and bytearray are examples of built-in objects that
             support the buffer protocol.
@@ -44,12 +42,12 @@
             byte array. If byteorder is âlittleâ, the most significant byte
             is at the end of the byte array. To request the native byte order
             of the host system, use `sys.byteorderâ as the byte order value.
             Default is to use âbigâ.
         signed
             Indicates whether twoâs complement is used to represent the
             integer.
-  tlslite.utils.openssl_tripledes.new(key, mode, IV)ï
+  tlslite.utils.pycrypto_tripledes.new(key, mode, IV)ï
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pem.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pem.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pem module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pem module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.poly1305.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.poly1305.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.poly1305 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_aes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pycrypto_aes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pycrypto_aesgcm module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rc4.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pycrypto_rc4 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rsakey.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.pycrypto_rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.pycrypto_rsakey module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_tripledes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_rc4.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.python_rc4 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.python_aes module" href="tlslite.utils.python_aes.html" />
-    <link rel="prev" title="tlslite.utils.pycrypto_rsakey module" href="tlslite.utils.pycrypto_rsakey.html" /> 
+    <link rel="next" title="tlslite.utils.python_rsakey module" href="tlslite.utils.python_rsakey.html" />
+    <link rel="prev" title="tlslite.utils.python_chacha20_poly1305 module" href="tlslite.utils.python_chacha20_poly1305.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,51 +66,51 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.pycrypto_tripledes module</li>
+      <li>tlslite.utils.python_rc4 module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.pycrypto_tripledes.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.python_rc4.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.pycrypto_tripledes">
-<span id="tlslite-utils-pycrypto-tripledes-module"></span><h1>tlslite.utils.pycrypto_tripledes module<a class="headerlink" href="#module-tlslite.utils.pycrypto_tripledes" title="Permalink to this heading"></a></h1>
-<p>PyCrypto 3DES implementation.</p>
+  <section id="module-tlslite.utils.python_rc4">
+<span id="tlslite-utils-python-rc4-module"></span><h1>tlslite.utils.python_rc4 module<a class="headerlink" href="#module-tlslite.utils.python_rc4" title="Permalink to this heading"></a></h1>
+<p>Pure-Python RC4 implementation.</p>
 <dl class="py class">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">PyCrypto_TripleDES</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES" title="Permalink to this definition"></a></dt>
-<dd><p>Bases: <a class="reference internal" href="tlslite.utils.tripledes.html#tlslite.utils.tripledes.TripleDES" title="tlslite.utils.tripledes.TripleDES"><code class="xref py py-class docutils literal notranslate"><span class="pre">TripleDES</span></code></a></p>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">Python_RC4</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keyBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference internal" href="tlslite.utils.rc4.html#tlslite.utils.rc4.RC4" title="tlslite.utils.rc4.RC4"><code class="xref py py-class docutils literal notranslate"><span class="pre">RC4</span></code></a></p>
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.__init__" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.__init__">
+<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keyBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.__init__" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.decrypt">
-<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.decrypt" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.decrypt">
+<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.decrypt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.encrypt">
-<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES.encrypt" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.encrypt">
+<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintextBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.encrypt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.bytes_to_int" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.bytes_to_int">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.bytes_to_int" title="Permalink to this definition"></a></dt>
 <dd><p>Return the integer represented by the given array of bytes.</p>
 <dl class="simple">
 <dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
 support the buffer protocol or be an iterable object producing bytes.
 Bytes and bytearray are examples of built-in objects that support the
 buffer protocol.</p>
 </dd>
@@ -122,26 +122,26 @@
 </dd>
 <dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.pycrypto_tripledes.new">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.pycrypto_tripledes.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mode</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">IV</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.pycrypto_tripledes.new" title="Permalink to this definition"></a></dt>
+<dt class="sig sig-object py" id="tlslite.utils.python_rc4.new">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.new" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.pycrypto_rsakey.html" class="btn btn-neutral float-left" title="tlslite.utils.pycrypto_rsakey module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.python_aes.html" class="btn btn-neutral float-right" title="tlslite.utils.python_aes module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.python_chacha20_poly1305.html" class="btn btn-neutral float-left" title="tlslite.utils.python_chacha20_poly1305 module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.utils.python_rsakey.html" class="btn btn-neutral float-right" title="tlslite.utils.python_rsakey module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,25 +14,25 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.pycrypto_tripledes module
+    * tlslite.utils.python_rc4 module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.pycrypto_tripledes moduleï ******
-PyCrypto 3DES implementation.
-  classtlslite.utils.pycrypto_tripledes.PyCrypto_TripleDES(key, mode, IV)ï
-      Bases: TripleDES
-        __init__(key, mode, IV)ï
+****** tlslite.utils.python_rc4 moduleï ******
+Pure-Python RC4 implementation.
+  classtlslite.utils.python_rc4.Python_RC4(keyBytes)ï
+      Bases: RC4
+        __init__(keyBytes)ï
         decrypt(ciphertext)ï
-        encrypt(plaintext)ï
-  tlslite.utils.pycrypto_tripledes.bytes_to_int(bytes, byteorder='big', *,
+        encrypt(plaintextBytes)ï
+  tlslite.utils.python_rc4.bytes_to_int(bytes, byteorder='big', *,
   signed=False)ï
       Return the integer represented by the given array of bytes.
         bytes
             Holds the array of bytes to convert. The argument must either
             support the buffer protocol or be an iterable object producing
             bytes. Bytes and bytearray are examples of built-in objects that
             support the buffer protocol.
@@ -42,12 +42,12 @@
             byte array. If byteorder is âlittleâ, the most significant byte
             is at the end of the byte array. To request the native byte order
             of the host system, use `sys.byteorderâ as the byte order value.
             Default is to use âbigâ.
         signed
             Indicates whether twoâs complement is used to represent the
             integer.
-  tlslite.utils.pycrypto_tripledes.new(key, mode, IV)ï
+  tlslite.utils.python_rc4.new(key)ï
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_aes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.python_aes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aesgcm.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.python_aesgcm module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.python_chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rc4.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.x25519.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.x25519 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="tlslite.utils.python_rsakey module" href="tlslite.utils.python_rsakey.html" />
-    <link rel="prev" title="tlslite.utils.python_chacha20_poly1305 module" href="tlslite.utils.python_chacha20_poly1305.html" /> 
+    <link rel="next" title="tlslite.api module" href="tlslite.api.html" />
+    <link rel="prev" title="tlslite.utils.tripledes module" href="tlslite.utils.tripledes.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -66,82 +66,93 @@
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home"></a> &raquo;</li>
           <li><a href="modules.html">tlslite</a> &raquo;</li>
           <li><a href="tlslite.html">tlslite package</a> &raquo;</li>
           <li><a href="tlslite.utils.html">tlslite.utils package</a> &raquo;</li>
-      <li>tlslite.utils.python_rc4 module</li>
+      <li>tlslite.utils.x25519 module</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/tlslite.utils.python_rc4.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/tlslite.utils.x25519.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="module-tlslite.utils.python_rc4">
-<span id="tlslite-utils-python-rc4-module"></span><h1>tlslite.utils.python_rc4 module<a class="headerlink" href="#module-tlslite.utils.python_rc4" title="Permalink to this heading"></a></h1>
-<p>Pure-Python RC4 implementation.</p>
-<dl class="py class">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">Python_RC4</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keyBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4" title="Permalink to this definition"></a></dt>
-<dd><p>Bases: <a class="reference internal" href="tlslite.utils.rc4.html#tlslite.utils.rc4.RC4" title="tlslite.utils.rc4.RC4"><code class="xref py py-class docutils literal notranslate"><span class="pre">RC4</span></code></a></p>
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.__init__">
-<span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keyBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.__init__" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.decrypt">
-<span class="sig-name descname"><span class="pre">decrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ciphertext</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.decrypt" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
-
-<dl class="py method">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.Python_RC4.encrypt">
-<span class="sig-name descname"><span class="pre">encrypt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">plaintextBytes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.Python_RC4.encrypt" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
+  <section id="module-tlslite.utils.x25519">
+<span id="tlslite-utils-x25519-module"></span><h1>tlslite.utils.x25519 module<a class="headerlink" href="#module-tlslite.utils.x25519" title="Permalink to this heading"></a></h1>
+<p>Handling X25519 and X448 curve based key agreement protocol.</p>
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.x25519.cswap">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">cswap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">swap</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">x_2</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">x_3</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.cswap" title="Permalink to this definition"></a></dt>
+<dd><p>Conditional swap function.</p>
+</dd></dl>
 
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.x25519.decodeScalar22519">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">decodeScalar22519</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">k</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.decodeScalar22519" title="Permalink to this definition"></a></dt>
+<dd><p>Function to decode the private K parameter of the x25519 function.</p>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.bytes_to_int">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">bytes_to_int</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bytes</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">byteorder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'big'</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.bytes_to_int" title="Permalink to this definition"></a></dt>
-<dd><p>Return the integer represented by the given array of bytes.</p>
-<dl class="simple">
-<dt>bytes</dt><dd><p>Holds the array of bytes to convert.  The argument must either
-support the buffer protocol or be an iterable object producing bytes.
-Bytes and bytearray are examples of built-in objects that support the
-buffer protocol.</p>
-</dd>
-<dt>byteorder</dt><dd><p>The byte order used to represent the integer.  If byteorder is ‘big’,
-the most significant byte is at the beginning of the byte array.  If
-byteorder is ‘little’, the most significant byte is at the end of the
-byte array.  To request the native byte order of the host system, use
-<a href="#id1"><span class="problematic" id="id2">`</span></a>sys.byteorder’ as the byte order value.  Default is to use ‘big’.</p>
+<dt class="sig sig-object py" id="tlslite.utils.x25519.decodeScalar448">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">decodeScalar448</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">k</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.decodeScalar448" title="Permalink to this definition"></a></dt>
+<dd><p>Function to decode the private K parameter of the X448 function.</p>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.x25519.decodeUCoordinate">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">decodeUCoordinate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">u</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">bits</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.decodeUCoordinate" title="Permalink to this definition"></a></dt>
+<dd><p>Function to decode the public U coordinate of X25519-family curves.</p>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="tlslite.utils.x25519.x25519">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">x25519</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">k</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">u</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.x25519" title="Permalink to this definition"></a></dt>
+<dd><p>Perform point multiplication on X25519 curve.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>k</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – random secret value (multiplier), should be 32 byte long</p></li>
+<li><p><strong>u</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – curve generator or the other party key share</p></li>
+</ul>
 </dd>
-<dt>signed</dt><dd><p>Indicates whether two’s complement is used to represent the integer.</p>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)">bytearray</a></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="tlslite.utils.python_rc4.new">
-<span class="sig-prename descclassname"><span class="pre">tlslite.utils.python_rc4.</span></span><span class="sig-name descname"><span class="pre">new</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.python_rc4.new" title="Permalink to this definition"></a></dt>
-<dd></dd></dl>
+<dt class="sig sig-object py" id="tlslite.utils.x25519.x448">
+<span class="sig-prename descclassname"><span class="pre">tlslite.utils.x25519.</span></span><span class="sig-name descname"><span class="pre">x448</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">k</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">u</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.utils.x25519.x448" title="Permalink to this definition"></a></dt>
+<dd><p>Perform point multiplication on X448 curve.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>k</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – random secret value (multiplier), should be 56 bytes long</p></li>
+<li><p><strong>u</strong> (<a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)"><em>bytearray</em></a>) – curve generator or the other party key share</p></li>
+</ul>
+</dd>
+<dt class="field-even">Return type<span class="colon">:</span></dt>
+<dd class="field-even"><p><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytearray" title="(in Python v3.11)">bytearray</a></p>
+</dd>
+</dl>
+</dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="tlslite.utils.python_chacha20_poly1305.html" class="btn btn-neutral float-left" title="tlslite.utils.python_chacha20_poly1305 module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="tlslite.utils.python_rsakey.html" class="btn btn-neutral float-right" title="tlslite.utils.python_rsakey module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="tlslite.utils.tripledes.html" class="btn btn-neutral float-left" title="tlslite.utils.tripledes module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="tlslite.api.html" class="btn btn-neutral float-right" title="tlslite.api module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Hubert Kario.</p>
   </div>
```

#### html2text {}

```diff
@@ -14,40 +14,42 @@
                       # tlslite.utils_package
                 # Submodules
    tlslite-ng
     *  »
     * tlslite »
     * tlslite_package »
     * tlslite.utils_package »
-    * tlslite.utils.python_rc4 module
+    * tlslite.utils.x25519 module
     * View_page_source
 ===============================================================================
-****** tlslite.utils.python_rc4 moduleï ******
-Pure-Python RC4 implementation.
-  classtlslite.utils.python_rc4.Python_RC4(keyBytes)ï
-      Bases: RC4
-        __init__(keyBytes)ï
-        decrypt(ciphertext)ï
-        encrypt(plaintextBytes)ï
-  tlslite.utils.python_rc4.bytes_to_int(bytes, byteorder='big', *,
-  signed=False)ï
-      Return the integer represented by the given array of bytes.
-        bytes
-            Holds the array of bytes to convert. The argument must either
-            support the buffer protocol or be an iterable object producing
-            bytes. Bytes and bytearray are examples of built-in objects that
-            support the buffer protocol.
-        byteorder
-            The byte order used to represent the integer. If byteorder is
-            âbigâ, the most significant byte is at the beginning of the
-            byte array. If byteorder is âlittleâ, the most significant byte
-            is at the end of the byte array. To request the native byte order
-            of the host system, use `sys.byteorderâ as the byte order value.
-            Default is to use âbigâ.
-        signed
-            Indicates whether twoâs complement is used to represent the
-            integer.
-  tlslite.utils.python_rc4.new(key)ï
+****** tlslite.utils.x25519 moduleï ******
+Handling X25519 and X448 curve based key agreement protocol.
+  tlslite.utils.x25519.cswap(swap, x_2, x_3)ï
+      Conditional swap function.
+  tlslite.utils.x25519.decodeScalar22519(k)ï
+      Function to decode the private K parameter of the x25519 function.
+  tlslite.utils.x25519.decodeScalar448(k)ï
+      Function to decode the private K parameter of the X448 function.
+  tlslite.utils.x25519.decodeUCoordinate(u, bits)ï
+      Function to decode the public U coordinate of X25519-family curves.
+  tlslite.utils.x25519.x25519(k, u)ï
+      Perform point multiplication on X25519 curve.
+        Parameters:
+                * k (bytearray) â random secret value (multiplier), should be
+                  32 byte long
+                * u (bytearray) â curve generator or the other party key
+                  share
+        Return type:
+            bytearray
+  tlslite.utils.x25519.x448(k, u)ï
+      Perform point multiplication on X448 curve.
+        Parameters:
+                * k (bytearray) â random secret value (multiplier), should be
+                  56 bytes long
+                * u (bytearray) â curve generator or the other party key
+                  share
+        Return type:
+            bytearray
 Previous Next
 ===============================================================================
 © Copyright 2023, Hubert Kario.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rsakey.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.python_rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.python_rsakey module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rc4.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.rc4 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rijndael.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rijndael.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rijndael module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.rijndael module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rsakey.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.rsakey module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tackwrapper.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tackwrapper.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tackwrapper module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.tackwrapper module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tlshashlib.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tlshashlib.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tlshashlib module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.tlshashlib module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tripledes.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.utils.tripledes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.utils.tripledes module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.verifierdb.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.verifierdb.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.verifierdb module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.verifierdb module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.x509.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.x509 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.x509 module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509certchain.html` & `tlslite-ng-0.8.0a46/docs/_build/html/tlslite.x509certchain.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.x509certchain module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
+  <title>tlslite.x509certchain module &mdash; tlslite-ng 0.8.0-alpha46 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a45/docs/conf.py` & `tlslite-ng-0.8.0a46/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = u'0.8'
 # The full version, including alpha/beta/rc tags.
-release = u'0.8.0-alpha45'
+release = u'0.8.0-alpha46'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `tlslite-ng-0.8.0a45/docs/make.bat` & `tlslite-ng-0.8.0a46/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/tlslite.integration.rst` & `tlslite-ng-0.8.0a46/docs/tlslite.integration.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/tlslite.rst` & `tlslite-ng-0.8.0a46/docs/tlslite.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/docs/tlslite.utils.rst` & `tlslite-ng-0.8.0a46/docs/tlslite.utils.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/pylintrc` & `tlslite-ng-0.8.0a46/pylintrc`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/scripts/speed.py` & `tlslite-ng-0.8.0a46/scripts/speed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/scripts/tls.py` & `tlslite-ng-0.8.0a46/scripts/tls.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,27 +320,27 @@
         retList.append(echo)
     return retList
 
 
 def printGoodConnection(connection, seconds):
     print("  Handshake time: %.3f seconds" % seconds)
     print("  Version: %s" % connection.getVersionName())
-    print("  Cipher: %s %s" % (connection.getCipherName(), 
+    print("  Cipher: %s %s" % (connection.getCipherName(),
         connection.getCipherImplementation()))
     print("  Ciphersuite: {0}".\
             format(CipherSuite.ietfNames[connection.session.cipherSuite]))
     if connection.session.srpUsername:
         print("  Client SRP username: %s" % connection.session.srpUsername)
     if connection.session.clientCertChain:
-        print("  Client X.509 SHA1 fingerprint: %s" % 
+        print("  Client X.509 SHA1 fingerprint: %s" %
             connection.session.clientCertChain.getFingerprint())
     else:
         print("  No client certificate provided by peer")
     if connection.session.serverCertChain:
-        print("  Server X.509 SHA1 fingerprint: %s" % 
+        print("  Server X.509 SHA1 fingerprint: %s" %
             connection.session.serverCertChain.getFingerprint())
     if connection.version >= (3, 3) and connection.serverSigAlg is not None:
         scheme = SignatureScheme.toRepr(connection.serverSigAlg)
         if scheme is None:
             scheme = "{1}+{0}".format(
                 HashAlgorithm.toStr(connection.serverSigAlg[0]),
                 SignatureAlgorithm.toStr(connection.serverSigAlg[1]))
@@ -348,28 +348,29 @@
     if connection.ecdhCurve is not None:
         print("  Group used for key exchange: {0}".format(\
                 GroupName.toStr(connection.ecdhCurve)))
     if connection.dhGroupSize is not None:
         print("  DH group size: {0} bits".format(connection.dhGroupSize))
     if connection.session.serverName:
         print("  SNI: %s" % connection.session.serverName)
-    if connection.session.tackExt:   
+    if connection.session.tackExt:
         if connection.session.tackInHelloExt:
             emptyStr = "\n  (via TLS Extension)"
         else:
-            emptyStr = "\n  (via TACK Certificate)" 
+            emptyStr = "\n  (via TACK Certificate)"
         print("  TACK: %s" % emptyStr)
         print(str(connection.session.tackExt))
     if connection.session.appProto:
         print("  Application Layer Protocol negotiated: {0}".format(
             connection.session.appProto.decode('utf-8')))
-    print("  Next-Protocol Negotiated: %s" % connection.next_proto) 
+    print("  Next-Protocol Negotiated: %s" % connection.next_proto)
     print("  Encrypt-then-MAC: {0}".format(connection.encryptThenMAC))
     print("  Extended Master Secret: {0}".format(
                                                connection.extendedMasterSecret))
+    print("  Session Resumed: {0}".format(connection.resumed))
 
 def printExporter(connection, expLabel, expLength):
     if expLabel is None:
         return
     expLabel = bytearray(expLabel, "utf-8")
     exp = connection.keyingMaterialExporter(expLabel, expLength)
     exp = b2a_hex(exp).upper()
@@ -460,35 +461,31 @@
         except TLSAbruptCloseError:
             break
     connection.close()
     # we're expecting an abrupt close error which marks the session as
     # unreasumable, override it
     session.resumable = True
 
-    print("Received {0} ticket[s]".format(len(connection.tickets)))
+    print("Received {0} ticket[s]".format(len(connection.tickets) + len(connection.tls_1_0_tickets)))
     assert connection.tickets is session.tickets
 
-    if not session.tickets:
-        return
-
     if not resumption:
         return
 
     print("Trying resumption handshake")
 
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.settimeout(5)
     sock.connect(address)
     sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
     connection = TLSConnection(sock)
-
     try:
         start = time_stamp()
         connection.handshakeClientCert(serverName=address[0], alpn=alpn,
-            session=session)
+            session=session, settings=settings)
         stop = time_stamp()
         print("Handshake success")
     except TLSLocalAlert as a:
         if a.description == AlertDescription.user_canceled:
             print(str(a))
         else:
             raise
```

### Comparing `tlslite-ng-0.8.0a45/scripts/tlsdb.py` & `tlslite-ng-0.8.0a46/scripts/tlsdb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/setup.py` & `tlslite-ng-0.8.0a46/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README")) as f:
     README = f.read()
 
 setup(name="tlslite-ng",
-      version="0.8.0-alpha45",
+      version="0.8.0-alpha46",
       author="Hubert Kario",
       author_email="hkario@redhat.com",
       url="https://github.com/tlsfuzzer/tlslite-ng",
       description="Pure python implementation of SSL and TLS.",
       long_description=README,
       license="LGPLv2",
       scripts=["scripts/tls.py", "scripts/tlsdb.py"],
@@ -36,13 +36,16 @@
             'Programming Language :: Python :: 2.7',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.5',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
             'Topic :: Security :: Cryptography',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: System :: Networking'
           ],
       keywords="ssl, tls, pure-python"
       )
```

### Comparing `tlslite-ng-0.8.0a45/tests/TACKs.pem` & `tlslite-ng-0.8.0a46/tests/TACKs.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/clientECCert.pem` & `tlslite-ng-0.8.0a46/tests/clientECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/clientX509Cert.pem` & `tlslite-ng-0.8.0a46/tests/clientX509Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/clientX509Key.pem` & `tlslite-ng-0.8.0a46/tests/clientX509Key.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverBrainpoolP256r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverBrainpoolP384r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverBrainpoolP512r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverDSACert.pem` & `tlslite-ng-0.8.0a46/tests/serverDSACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverDSAKey.pem` & `tlslite-ng-0.8.0a46/tests/serverDSAKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverECDSANonCACert.pem` & `tlslite-ng-0.8.0a46/tests/serverECDSANonCACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverEd448Cert.pem` & `tlslite-ng-0.8.0a46/tests/serverEd448Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverP384ECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverP384ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverP521ECCert.pem` & `tlslite-ng-0.8.0a46/tests/serverP521ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSANonCACert.pem` & `tlslite-ng-0.8.0a46/tests/serverRSANonCACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSANonCAKey.pem` & `tlslite-ng-0.8.0a46/tests/serverRSANonCAKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSAPSSCert.pem` & `tlslite-ng-0.8.0a46/tests/serverRSAPSSCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSAPSSKey.pem` & `tlslite-ng-0.8.0a46/tests/serverRSAPSSKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSAPSSSigCert.pem` & `tlslite-ng-0.8.0a46/tests/serverRSAPSSSigCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverRSAPSSSigKey.pem` & `tlslite-ng-0.8.0a46/tests/serverRSAPSSSigKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverX509Cert.pem` & `tlslite-ng-0.8.0a46/tests/serverX509Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/serverX509Key.pem` & `tlslite-ng-0.8.0a46/tests/serverX509Key.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tests/tlstest.py` & `tlslite-ng-0.8.0a46/tests/tlstest.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,14 +724,46 @@
     synchro.recv(1)
     connection = connect()
     settings = HandshakeSettings()
     settings.pskConfigs = [(b'test', b'\x00secret', 'sha384')]
     connection.handshakeClientCert(settings=settings)
     assert connection.session.serverCertChain is None
     assert connection.ecdhCurve is not None
+    assert connection.session.cipherSuite in \
+            constants.CipherSuite.sha384PrfSuites
+    testConnClient(connection)
+    connection.close()
+
+    test_no += 1
+
+    print("Test {0} - good PSK SHA-256 PRF".format(test_no))
+    synchro.recv(1)
+    connection = connect()
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'test', b'\x00secret', 'sha256')]
+    connection.handshakeClientCert(settings=settings)
+    assert connection.session.serverCertChain is None
+    assert connection.ecdhCurve is not None
+    assert connection.session.cipherSuite in \
+            constants.CipherSuite.sha256PrfSuites
+    testConnClient(connection)
+    connection.close()
+
+    test_no += 1
+
+    print("Test {0} - good PSK default PRF".format(test_no))
+    synchro.recv(1)
+    connection = connect()
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'test', b'\x00secret', 'sha256')]
+    connection.handshakeClientCert(settings=settings)
+    assert connection.session.serverCertChain is None
+    assert connection.ecdhCurve is not None
+    assert connection.session.cipherSuite in \
+            constants.CipherSuite.sha256PrfSuites
     testConnClient(connection)
     connection.close()
 
     test_no += 1
 
     print("Test {0} - good PSK, no DH".format(test_no))
     synchro.recv(1)
@@ -757,14 +789,29 @@
     assert connection.session.serverCertChain is None
     assert connection.ecdhCurve is None
     testConnClient(connection)
     connection.close()
 
     test_no += 1
 
+    print("Test {0} - bad PSK X.509 fallback".format(test_no))
+    synchro.recv(1)
+    connection = connect()
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'bad identity', b'\x00secret', 'sha256')]
+    connection.handshakeClientCert(settings=settings)
+    assert connection.session.serverCertChain
+    assert connection.ecdhCurve is not None
+    assert connection.session.cipherSuite in \
+            constants.CipherSuite.sha384PrfSuites
+    testConnClient(connection)
+    connection.close()
+
+    test_no += 1
+
     print("Test {0} - good SRP (db)".format(test_no))
     print("client {0} - waiting for synchro".format(time.time()))
     try:
         synchro.recv(1)
     except Exception:
         print("client {0} - wait abort".format(time.time()))
         raise
@@ -1442,30 +1489,34 @@
     settings = HandshakeSettings()
     settings.macNames.remove("aead")
     settings.maxVersion = (3, 3)
     connection.handshakeClientCert(serverName=address[0], settings=settings)
     testConnClient(connection)
     assert(isinstance(connection.session.serverCertChain, X509CertChain))
     assert(connection.session.serverName == address[0])
+    assert(connection.version == (3, 3))
     assert(not connection.resumed)
     assert(connection.encryptThenMAC)
+    assert(connection.session.tls_1_0_tickets)
     connection.close()
     session = connection.session
 
     # resume
     synchro.recv(1)
     connection = connect()
     settings = HandshakeSettings()
+    settings.macNames.remove("aead")
     settings.maxVersion = (3, 3)
     connection.handshakeClientCert(serverName=address[0], session=session,
                                    settings=settings)
     testConnClient(connection)
     assert(isinstance(connection.session.serverCertChain, X509CertChain))
     assert(connection.session.serverName == address[0])
     assert(connection.resumed)
+    assert(connection.session.encryptThenMAC)
     assert(connection.encryptThenMAC)
     connection.close()
 
     test_no += 1
 
     print("Test {0} - resumption with no EtM in 2nd handshake".format(test_no))
     synchro.recv(1)
@@ -1497,14 +1548,61 @@
         assert(str(e) == "illegal_parameter")
     else:
         raise AssertionError("No exception raised")
     connection.close()
 
     test_no += 1
 
+    print("Test {0} - session_ticket resumption in TLSv1.2".format(test_no))
+    synchro.recv(1)
+    connection = connect()
+    settings = HandshakeSettings()
+    connection.handshakeClientCert(serverName=address[0], settings=settings)
+    testConnClient(connection)
+    assert isinstance(connection.session.serverCertChain, X509CertChain)
+    assert connection.session.serverName == address[0]
+    assert not connection.resumed
+    session = connection.session
+    connection.close()
+
+    # resume
+    synchro.recv(1)
+    settings = HandshakeSettings()
+    connection = connect()
+    connection.handshakeClientCert(serverName=address[0], settings=settings, session=session)
+    testConnClient(connection)
+    assert connection.resumed
+    connection.close()
+
+    test_no += 1
+
+    print("Test {0} - session_ticket resumption in TLSv1.2 "
+          "with expired ticket".format(test_no))
+    synchro.recv(1)
+    connection = connect()
+    settings = HandshakeSettings()
+    connection.handshakeClientCert(serverName=address[0], settings=settings)
+    testConnClient(connection)
+    assert isinstance(connection.session.serverCertChain, X509CertChain)
+    assert connection.session.serverName == address[0]
+    assert not connection.resumed
+    session = connection.session
+    connection.close()
+
+    # resume
+    synchro.recv(1)
+    settings = HandshakeSettings()
+    connection = connect()
+    connection.handshakeClientCert(serverName=address[0], settings=settings, session=session)
+    testConnClient(connection)
+    assert not connection.resumed
+    connection.close()
+
+    test_no += 1
+
     print("Test {0} - resumption in TLSv1.3".format(test_no))
     synchro.recv(1)
     connection = connect()
     settings = HandshakeSettings()
     # force HRR
     settings.keyShares = []
     connection.handshakeClientCert(serverName=address[0], settings=settings)
@@ -2349,14 +2447,38 @@
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
                                settings=settings)
     testConnServer(connection)
     connection.close()
 
     test_no += 1
 
+    print("Test {0} - good PSK SHA-256 PRF".format(test_no))
+    synchro.send(b'R')
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'test', b'\x00secret', 'sha256')]
+    connection = connect()
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    test_no += 1
+
+    print("Test {0} - good PSK default PRF".format(test_no))
+    synchro.send(b'R')
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'test', b'\x00secret')]
+    connection = connect()
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    test_no += 1
+
     print("Test {0} - good PSK, no DH".format(test_no))
     synchro.send(b'R')
     settings = HandshakeSettings()
     settings.psk_modes = ["psk_ke"]
     settings.pskConfigs = [(b'test', b'\x00secret', 'sha384')]
     connection = connect()
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
@@ -2374,14 +2496,26 @@
     connection = connect()
     connection.handshakeServer(settings=settings)
     testConnServer(connection)
     connection.close()
 
     test_no += 1
 
+    print("Test {0} - bad PSK X.509 fallback".format(test_no))
+    synchro.send(b'R')
+    settings = HandshakeSettings()
+    settings.pskConfigs = [(b'test', b'\x00secret', 'sha256')]
+    connection = connect()
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    test_no += 1
+
     print("Test {0} - good SRP (db)".format(test_no))
     try:
         import logging
         logging.basicConfig(level=logging.DEBUG)
         (db_file, db_name) = mkstemp()
         print("server {0} - tmp file created".format(time.time()))
         os.close(db_file)
@@ -2982,41 +3116,46 @@
     synchro.send(b'R')
     connection = connect()
     settings = HandshakeSettings()
     settings.useEncryptThenMAC = False
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
                                settings=settings)
     testConnServer(connection)
+    assert(not connection.encryptThenMAC)
     connection.close()
 
     test_no += 1
 
     print("Test {0} - no EtM client side".format(test_no))
     synchro.send(b'R')
     connection = connect()
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key)
     testConnServer(connection)
+    assert(not connection.encryptThenMAC)
     connection.close()
 
     test_no += 1
 
     print("Test {0} - resumption with EtM".format(test_no))
     synchro.send(b'R')
     sessionCache = SessionCache()
+    settings = HandshakeSettings()
+    settings.ticketKeys = [getRandomBytes(32)]
     connection = connect()
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
-                               sessionCache=sessionCache)
+                               sessionCache=sessionCache, settings=settings)
     testConnServer(connection)
+    assert(connection.encryptThenMAC)
     connection.close()
 
     # resume
     synchro.send(b'R')
     connection = connect()
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
-                               sessionCache=sessionCache)
+                               sessionCache=sessionCache, settings=settings)
     testConnServer(connection)
     connection.close()
 
     test_no += 1
 
     print("Test {0} - resumption with no EtM in 2nd handshake".format(test_no))
     synchro.send(b'R')
@@ -3038,14 +3177,60 @@
         assert(str(e) == "illegal_parameter")
     else:
         raise AssertionError("no exception raised")
     connection.close()
 
     test_no += 1
 
+    print("Test {0} - session_ticket resumption in TLSv1.2".format(test_no))
+    synchro.send(b'R')
+    connection = connect()
+    settings = HandshakeSettings()
+    settings.maxVersion = (3, 3)
+    settings.ticketKeys = [getRandomBytes(32)]
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    # resume
+    synchro.send(b'R')
+    connection = connect()
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    test_no += 1
+
+    print("Test {0} - session_ticket resumption in TLSv1.2 "
+          "with expired ticket".format(test_no))
+    synchro.send(b'R')
+    connection = connect()
+    settings = HandshakeSettings()
+    settings.ticketLifetime = 1
+    settings.maxVersion = (3, 3)
+    settings.ticketKeys = [getRandomBytes(32)]
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    time.sleep(2)
+
+    # resume
+    synchro.send(b'R')
+    connection = connect()
+    connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
+                               settings=settings)
+    testConnServer(connection)
+    connection.close()
+
+    test_no += 1
+
     print("Test {0} - resumption in TLSv1.3".format(test_no))
     synchro.send(b'R')
     connection = connect()
     settings = HandshakeSettings()
     settings.minVersion = (3,4)
     settings.ticketKeys = [getRandomBytes(32)]
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
@@ -3068,14 +3253,15 @@
     connection = connect()
     settings = HandshakeSettings()
     settings.minVersion = (3,4)
     settings.ticketKeys = [getRandomBytes(32)]
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
                                reqCert=True, settings=settings)
     testConnServer(connection)
+    assert connection.session.clientCertChain
     connection.close()
 
     # resume
     synchro.send(b'R')
     connection = connect()
     connection.handshakeServer(certChain=x509Chain, privateKey=x509Key,
                                reqCert=True, settings=settings)
```

### Comparing `tlslite-ng-0.8.0a45/tests/verifierDB` & `tlslite-ng-0.8.0a46/tests/verifierDB`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/__init__.py` & `tlslite-ng-0.8.0a46/tlslite/__init__.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/api.py` & `tlslite-ng-0.8.0a46/tlslite/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # Author: Trevor Perrin
 # See the LICENSE file for legal information regarding use of this file.
 
-__version__ = "0.8.0-alpha45"
+__version__ = "0.8.0-alpha46"
+# the whole module is about importing most commonly used methods, for use
+# by other applications
+# pylint: disable=unused-import
 from .constants import AlertLevel, AlertDescription, Fault
 from .errors import *
 from .checker import Checker
 from .handshakesettings import HandshakeSettings
 from .session import Session
 from .sessioncache import SessionCache
 from .tlsconnection import TLSConnection
 from .verifierdb import VerifierDB
 from .x509 import X509
 from .x509certchain import X509CertChain
 
 from .integration.httptlsconnection import HTTPTLSConnection
 from .integration.tlssocketservermixin import TLSSocketServerMixIn
-from .integration.tlsasyncdispatchermixin import TLSAsyncDispatcherMixIn
+try:
+    from .integration.tlsasyncdispatchermixin import TLSAsyncDispatcherMixIn
+except ModuleNotFoundError:
+    # asyncore was removed in 3.12, I don't use use it, so don't know how
+    # to fix it
+    pass
 from .integration.pop3_tls import POP3_TLS
 from .integration.imap4_tls import IMAP4_TLS
 from .integration.smtp_tls import SMTP_TLS
 from .integration.xmlrpctransport import XMLRPCTransport
 from .integration.xmlrpcserver import TLSXMLRPCRequestHandler, \
                                       TLSXMLRPCServer, \
                                       MultiPathTLSXMLRPCServer
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/basedb.py` & `tlslite-ng-0.8.0a46/tlslite/basedb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/bufferedsocket.py` & `tlslite-ng-0.8.0a46/tlslite/bufferedsocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/checker.py` & `tlslite-ng-0.8.0a46/tlslite/checker.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/constants.py` & `tlslite-ng-0.8.0a46/tlslite/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,17 @@
 class HandshakeType(TLSEnum):
     """Message types in TLS Handshake protocol"""
 
     hello_request = 0
     client_hello = 1
     server_hello = 2
     new_session_ticket = 4
-    hello_retry_request = 6  # draft version of TLS 1.3
-    encrypted_extensions = 8
+    end_of_early_data = 5  # TLS 1.3
+    hello_retry_request = 6  # TLS 1.3
+    encrypted_extensions = 8  # TLS 1.3
     certificate = 11
     server_key_exchange = 12
     certificate_request = 13
     server_hello_done = 14
     certificate_verify = 15
     client_key_exchange = 16
     finished = 20
@@ -164,14 +165,15 @@
     signature_algorithms = 13  # RFC 5246
     heartbeat = 15  # RFC 6520
     alpn = 16  # RFC 7301
     client_hello_padding = 21  # RFC 7685
     encrypt_then_mac = 22  # RFC 7366
     extended_master_secret = 23  # RFC 7627
     record_size_limit = 28  # RFC 8449
+    session_ticket = 35 # RFC 5077
     extended_random = 40  # draft-rescorla-tls-extended-random-02
     pre_shared_key = 41  # TLS 1.3
     early_data = 42  # TLS 1.3
     supported_versions = 43  # TLS 1.3
     cookie = 44  # TLS 1.3
     psk_key_exchange_modes = 45  # TLS 1.3
     post_handshake_auth = 49  # TLS 1.3
@@ -1200,15 +1202,15 @@
     aeadSuites.extend(aes128CcmSuites)
     aeadSuites.extend(aes128Ccm_8Suites)
     aeadSuites.extend(aes256CcmSuites)
     aeadSuites.extend(aes256Ccm_8Suites)
     aeadSuites.extend(chacha20Suites)
     aeadSuites.extend(chacha20draft00Suites)
 
-    #: TLS1.2 with SHA384 PRF
+    #: any with SHA384 PRF
     sha384PrfSuites = []
     sha384PrfSuites.extend(sha384Suites)
     sha384PrfSuites.extend(aes256GcmSuites)
 
     #: MD-5 HMAC, protocol default PRF
     md5Suites = []
     md5Suites.append(TLS_DH_ANON_WITH_RC4_128_MD5)
@@ -1222,14 +1224,20 @@
 
     #: TLS1.2 specific ciphersuites
     tls12Suites = []
     tls12Suites.extend(sha256Suites)
     tls12Suites.extend(sha384Suites)
     tls12Suites.extend(aeadSuites)
 
+    #: any that will end up using SHA256 PRF in TLS 1.2 or later
+    sha256PrfSuites = []
+    sha256PrfSuites.extend(tls12Suites)
+    for i in sha384PrfSuites:
+        sha256PrfSuites.remove(i)
+
     #: TLS1.3 specific ciphersuites
     tls13Suites = []
 
     # TLS 1.3 suites are not a superset of TLS 1.2 suites, but they
     # use the same mechanism (AEAD), so we need to remove TLS 1.3 items
     # from the TLS 1.2 list
     tls13Suites.append(TLS_AES_256_GCM_SHA384)
@@ -1276,14 +1284,31 @@
         else:
             includeSuites.update(CipherSuite.srpSuites)
             includeSuites.update(CipherSuite.anonSuites)
             includeSuites.update(CipherSuite.ecdhAnonSuites)
         return [s for s in suites if s in includeSuites]
 
     @staticmethod
+    def filter_for_prfs(suites, prfs):
+        """Return a copy of suites without ciphers incompatible with the
+        specified prfs (sha256 or sha384)"""
+        includeSuites = set()
+        prfs = set(prfs)
+        if None in prfs:
+            prfs.update(["sha256"])
+            prfs.remove(None)
+        assert len(prfs) <= 2, prfs
+
+        if "sha256" in prfs:
+            includeSuites.update(CipherSuite.sha256PrfSuites)
+        if "sha384" in prfs:
+            includeSuites.update(CipherSuite.sha384PrfSuites)
+        return [s for s in suites if s in includeSuites]
+
+    @staticmethod
     def _filterSuites(suites, settings, version=None):
         if version is None:
             version = settings.maxVersion
         macNames = settings.macNames
         cipherNames = settings.cipherNames
         keyExchangeNames = settings.keyExchangeNames
         macSuites = []
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/defragmenter.py` & `tlslite-ng-0.8.0a46/tlslite/defragmenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,7 +122,11 @@
             return (msg_type, data)
         return None
 
     def clear_buffers(self):
         """Remove all data from buffers"""
         for key in self.buffers.keys():
             self.buffers[key] = bytearray(0)
+
+    def is_empty(self):
+        """Return True if all buffers are empty."""
+        return all(not i for i in self.buffers.values())
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/dh.py` & `tlslite-ng-0.8.0a46/tlslite/dh.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/errors.py` & `tlslite-ng-0.8.0a46/tlslite/errors.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/extensions.py` & `tlslite-ng-0.8.0a46/tlslite/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2107,14 +2107,61 @@
 
     def __init__(self):
         """Create instance."""
         super(RecordSizeLimitExtension, self).__init__(
             2, 'record_size_limit', ExtensionType.record_size_limit)
 
 
+class SessionTicketExtension(TLSExtension):
+    """
+    Client and server session ticket extension from RFC 5077
+    """
+    def __init__(self):
+        """Create instance of the object."""
+        super(SessionTicketExtension, self).__init__(extType=ExtensionType.
+                                                     session_ticket)
+        self.ticket = None
+
+    def create(self, ticket):
+
+        self.ticket = ticket
+        return self
+
+    @property
+    def extData(self):
+        """Serialise the payload of the extension."""
+        if not self.ticket:
+            return bytearray(0)
+
+        w = Writer()
+        w.bytes += self.ticket
+        return w.bytes
+
+    def parse(self, parser):
+        """
+        Parse the extension from on the wire format.
+
+        :param Parser parser: data to be parsed
+
+        :rtype: SessionTicketExtension
+        """
+        if not parser.getRemainingLength():
+            self.ticket = bytearray(0)
+            return self
+        self.ticket = parser.getFixBytes(parser.getRemainingLength())
+
+        return self
+
+    def __repr__(self):
+        """Return human readable representation of the extension."""
+        return "{0}({1}={2!r})".format(self.__class__.__name__,
+                                       "ticket",
+                                       self.ticket)
+
+
 TLSExtension._universalExtensions = \
     {
         ExtensionType.server_name: SNIExtension,
         ExtensionType.status_request: StatusRequestExtension,
         ExtensionType.cert_type: ClientCertTypeExtension,
         ExtensionType.supported_groups: SupportedGroupsExtension,
         ExtensionType.ec_point_formats: ECPointFormatsExtension,
@@ -2128,15 +2175,16 @@
         ExtensionType.supported_versions: SupportedVersionsExtension,
         ExtensionType.key_share: ClientKeyShareExtension,
         ExtensionType.signature_algorithms_cert:
             SignatureAlgorithmsCertExtension,
         ExtensionType.pre_shared_key: PreSharedKeyExtension,
         ExtensionType.psk_key_exchange_modes: PskKeyExchangeModesExtension,
         ExtensionType.cookie: CookieExtension,
-        ExtensionType.record_size_limit: RecordSizeLimitExtension}
+        ExtensionType.record_size_limit: RecordSizeLimitExtension,
+        ExtensionType.session_ticket: SessionTicketExtension}
 
 TLSExtension._serverExtensions = \
     {
         ExtensionType.cert_type: ServerCertTypeExtension,
         ExtensionType.tack: TACKExtension,
         ExtensionType.key_share: ServerKeyShareExtension,
         ExtensionType.supported_versions: SrvSupportedVersionsExtension,
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/handshakehashes.py` & `tlslite-ng-0.8.0a46/tlslite/handshakehashes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/handshakehelpers.py` & `tlslite-ng-0.8.0a46/tlslite/handshakehelpers.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/handshakesettings.py` & `tlslite-ng-0.8.0a46/tlslite/handshakesettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
     :vartype pskConfigs: list(tuple(bytearray, bytearray, bytearray))
     :ivar pskConfigs: list of tuples, first element of the tuple is the
         human readable, UTF-8 encoded, "identity" of the associated secret
         (bytearray, can be empty for TLS 1.2 and earlier), second element is
         the binary secret (bytearray), third is an optional parameter
         specifying the PRF hash to be used in TLS 1.3 (``sha256`` or
-        ``sha384``)
+        ``sha384``, with ``sha256`` being the default)
 
     :vartype ticketKeys: list(bytearray)
     :ivar ticketKeys: keys to be used for encrypting and decrypting session
         tickets. First entry is the encryption key for new tickets and the
         default decryption key, subsequent entries are the fallback keys
         allowing for key rollover. The keys need to be of size appropriate
         for a selected cipher in ticketCipher, 32 bytes for 'aes256gcm' and
@@ -317,14 +317,19 @@
         tickets. 'aes256gcm' by default, 'aes128gcm' or 'chacha20-poly1305'
         alternatively.
 
     :vartype ticketLifetime: int
     :ivar ticketLifetime: maximum allowed lifetime of ticket encryption key,
         in seconds. 1 day by default
 
+    :vartype ticket_count: int
+    :ivar ticket_count: number of tickets the server will send to the client
+        after establishing the connection in TLS 1.3. If a positive integer,
+        it enabled support for ticket based resumption in TLS 1.2 and earlier.
+
     :vartype psk_modes: list(str)
     :ivar psk_modes: acceptable modes for the PSK key exchange in TLS 1.3
 
     :ivar int max_early_data: maximum number of bytes acceptable for 0-RTT
         early_data processing. In other words, how many bytes will the server
         try to process, but ignore, in case the Client Hello includes
         early_data extension.
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/asyncstatemachine.py` & `tlslite-ng-0.8.0a46/tlslite/integration/asyncstatemachine.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/clienthelper.py` & `tlslite-ng-0.8.0a46/tlslite/integration/clienthelper.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/httptlsconnection.py` & `tlslite-ng-0.8.0a46/tlslite/integration/httptlsconnection.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/imap4_tls.py` & `tlslite-ng-0.8.0a46/tlslite/integration/imap4_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/pop3_tls.py` & `tlslite-ng-0.8.0a46/tlslite/integration/pop3_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/smtp_tls.py` & `tlslite-ng-0.8.0a46/tlslite/integration/smtp_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/tlsasyncdispatchermixin.py` & `tlslite-ng-0.8.0a46/tlslite/integration/tlsasyncdispatchermixin.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/tlssocketservermixin.py` & `tlslite-ng-0.8.0a46/tlslite/integration/tlssocketservermixin.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/xmlrpcserver.py` & `tlslite-ng-0.8.0a46/tlslite/integration/xmlrpcserver.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/integration/xmlrpctransport.py` & `tlslite-ng-0.8.0a46/tlslite/integration/xmlrpctransport.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/keyexchange.py` & `tlslite-ng-0.8.0a46/tlslite/keyexchange.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/mathtls.py` & `tlslite-ng-0.8.0a46/tlslite/mathtls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/messages.py` & `tlslite-ng-0.8.0a46/tlslite/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -618,14 +618,16 @@
             self.compression_methods = [0]  # Fake this value
             p.stopLengthCheck()
         else:
             p.startLengthCheck(3)
             self.client_version = (p.get(1), p.get(1))
             self.random = p.getFixBytes(32)
             self.session_id = p.getVarBytes(1)
+            if len(self.session_id) > 32:
+                raise DecodeError("session_id too long")
             self.cipher_suites = p.getVarList(2, 2)
             self.compression_methods = p.getVarList(1, 1)
             if not p.atLengthCheck():
                 self.extensions = []
                 totalExtLength = p.get(2)
                 p2 = Parser(p.getFixBytes(totalExtLength))
                 while p2.getRemainingLength() > 0:
@@ -2064,19 +2066,59 @@
         while ext_parser.getRemainingLength():
             self.extensions.append(TLSExtension().parse(ext_parser))
 
         parser.stopLengthCheck()
         return self
 
 
+class NewSessionTicket1_0(HelloMessage):
+    """Handling of the TLS1.0-TLS1.2 NewSessionTicket message."""
+
+    def __init__(self):
+        """Create New Session Ticket object."""
+        super(NewSessionTicket1_0, self).__init__(HandshakeType
+                                                  .new_session_ticket)
+        self.ticket_lifetime = 0
+        self.ticket = bytearray(0)
+
+    def create(self, ticket_lifetime, ticket):
+        """Initialise a New Session Ticket."""
+        self.ticket_lifetime = ticket_lifetime
+        self.ticket = ticket
+        return self
+
+    def write(self):
+        """
+        Serialise the message to on the wire data.
+
+        :rtype: bytearray
+        """
+        w = Writer()
+        w.add(self.ticket_lifetime, 4)
+        w.addVarSeq(self.ticket, 1, 2)
+        w2 = Writer()
+        w.bytes += w2.bytes
+
+        return self.postWrite(w)
+
+    def parse(self, parser):
+        """Parse the object from on the wire data."""
+        parser.startLengthCheck(3)
+        self.ticket_lifetime = parser.get(4)
+        self.ticket = parser.getVarBytes(2)
+        parser.stopLengthCheck()
+
+        return self
+
+
 class SessionTicketPayload(object):
     """Serialisation and deserialisation of server state for resumption.
 
     This is the internal (meant to be encrypted) representation of server
-    state that is set to client in the NewSessionTicket message.
+    state that is sent to the client in the NewSessionTicket message.
 
     :ivar int ~.version: implementation detail for forward compatibility
     :ivar bytearray master_secret: master secret for TLS 1.2-, resumption
         master secret for TLS 1.3
 
     :ivar tuple protocol_version: version of protocol that was previously
         negotiated in this session
@@ -2084,25 +2126,32 @@
     :ivar int cipher_suite: numerical ID of ciphersuite that was negotiated
         previously
 
     :ivar bytearray nonce: nonce for TLS 1.3 KDF
 
     :ivar int creation_time: Unix time in seconds when was the ticket created
     :ivar X509CertChain client_cert_chain: Client X509 Certificate Chain
+    :ivar bool encrypt_then_mac: The session used the encrypt_then_mac
+        extension
+    :ivar bool extended_master_secret: The session used the
+        extended_master_secret extension
     """
 
     def __init__(self):
         """Create instance of the object."""
         self.version = 0
         self.master_secret = bytearray()
         self.protocol_version = bytearray()
         self.cipher_suite = 0
         self.creation_time = 0
         self.nonce = bytearray()
         self._cert_chain = None
+        self.encrypt_then_mac = False
+        self.extended_master_secret = False
+        self.server_name = bytearray()
 
     @property
     def client_cert_chain(self):
         """Getter for the client_cert_chain property."""
         if self._cert_chain:
             return X509CertChain([i.certificate
                                   for i in self._cert_chain])
@@ -2111,43 +2160,59 @@
     @client_cert_chain.setter
     def client_cert_chain(self, client_cert_chain):
         """Setter for the cert_chain property."""
         self._cert_chain = [CertificateEntry(CertificateType.x509)
                             .create(i, []) for i in client_cert_chain.x509List]
 
     def create(self, master_secret, protocol_version, cipher_suite,
-               creation_time, nonce=bytearray(), client_cert_chain=None):
+               creation_time, nonce=bytearray(), client_cert_chain=None,
+               encrypt_then_mac=False, extended_master_secret=False,
+               server_name=bytearray()):
         """Initialise the object with cryptographic data."""
         self.master_secret = master_secret
         self.protocol_version = protocol_version
         self.cipher_suite = cipher_suite
         self.creation_time = creation_time
         self.nonce = nonce
         if client_cert_chain:
             self.version = 1
             self.client_cert_chain = client_cert_chain
+        if encrypt_then_mac or extended_master_secret or server_name:
+            if self.client_cert_chain is None:
+                self._cert_chain = []
+            self.version = 2
+            self.encrypt_then_mac = encrypt_then_mac
+            self.extended_master_secret = extended_master_secret
+            if server_name is None:
+                self.server_name = bytearray()
+            else:
+                self.server_name = server_name
         return self
 
     def _parse_cert_chain(self, parser):
         self._cert_chain = []
         while parser.getRemainingLength():
             entry = CertificateEntry(CertificateType.x509)
             self._cert_chain.append(entry.parse(parser))
 
     def parse(self, parser):
         self.version = parser.get(2)
-        if self.version > 1:
+        if self.version > 2:
             raise ValueError("Unrecognised version number")
         self.master_secret = parser.getVarBytes(2)
         self.protocol_version = (parser.get(1), parser.get(1))
         self.cipher_suite = parser.get(2)
         self.nonce = parser.getVarBytes(1)
         self.creation_time = parser.get(8)
-        if self.version == 1:
+        if self.version >= 1:
             self._parse_cert_chain(Parser(parser.getVarBytes(3)))
+        if self.version >= 2:
+            self.encrypt_then_mac = bool(parser.get(1))
+            self.extended_master_secret = bool(parser.get(1))
+            self.server_name = parser.getVarBytes(2)
         if parser.getRemainingLength():
             raise ValueError("Malformed ticket")
         return self
 
     def write(self):
         writer = Writer()
         writer.addTwo(self.version)
@@ -2155,19 +2220,24 @@
         writer.bytes += self.master_secret
         writer.addOne(self.protocol_version[0])
         writer.addOne(self.protocol_version[1])
         writer.addTwo(self.cipher_suite)
         writer.addOne(len(self.nonce))
         writer.bytes += self.nonce
         writer.add(self.creation_time, 8)
-        if self.version == 1:
+        if self.version >= 1:
             wcert = Writer()
             for entry in self._cert_chain:
                 wcert.bytes += entry.write()
             writer.addVarSeq(wcert.bytes, 1, 3)
+        if self.version >= 2:
+            writer.addOne(int(self.encrypt_then_mac))
+            writer.addOne(int(self.extended_master_secret))
+            writer.addTwo(len(self.server_name))
+            writer.bytes += self.server_name
         return writer.bytes
 
 
 class SSL2Finished(HandshakeMsg):
     """Handling of the SSL2 FINISHED messages."""
 
     def __init__(self, msg_type):
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/messagesocket.py` & `tlslite-ng-0.8.0a46/tlslite/messagesocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/ocsp.py` & `tlslite-ng-0.8.0a46/tlslite/ocsp.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/recordlayer.py` & `tlslite-ng-0.8.0a46/tlslite/recordlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,21 @@
         return self._writeState.encryptThenMAC
 
     @encryptThenMAC.setter
     def encryptThenMAC(self, value):
         self._pendingWriteState.encryptThenMAC = value
         self._pendingReadState.encryptThenMAC = value
 
+    def _get_pending_state_etm(self):
+        """
+        Return the state of encrypt then MAC for the connection after
+        CCS will be exchanged
+        """
+        return self._pendingWriteState.encryptThenMAC
+
     @property
     def blockSize(self):
         """Return the size of block used by current symmetric cipher (R/O)"""
         return self._writeState.encContext.block_size
 
     @property
     def tls13record(self):
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/session.py` & `tlslite-ng-0.8.0a46/tlslite/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,15 +63,19 @@
     :ivar exporterMasterSecret: master secret used for TLS Exporter in TLS1.3
 
     :vartype resumptionMasterSecret: bytearray
     :ivar resumptionMasterSecret: master secret used for session resumption in
         TLS 1.3
 
     :vartype tickets: list
-    :ivar tickets: list of tickets received from the server
+    :ivar tickets: list of TLS 1.3 session tickets received from the server
+
+    :vartype tls_1_0_tickets: list
+    :ivar tls_1_0_tickets: list of TLS 1.2 and earlier session tickets received
+        from the server
     """
 
     def __init__(self):
         self.masterSecret = bytearray(0)
         self.sessionID = bytearray(0)
         self.cipherSuite = 0
         self.srpUsername = ""
@@ -85,22 +89,24 @@
         self.extendedMasterSecret = False
         self.appProto = bytearray(0)
         self.cl_app_secret = bytearray(0)
         self.sr_app_secret = bytearray(0)
         self.exporterMasterSecret = bytearray(0)
         self.resumptionMasterSecret = bytearray(0)
         self.tickets = None
+        self.tls_1_0_tickets = None
 
     def create(self, masterSecret, sessionID, cipherSuite,
                srpUsername, clientCertChain, serverCertChain,
                tackExt, tackInHelloExt, serverName, resumable=True,
                encryptThenMAC=False, extendedMasterSecret=False,
                appProto=bytearray(0), cl_app_secret=bytearray(0),
                sr_app_secret=bytearray(0), exporterMasterSecret=bytearray(0),
-               resumptionMasterSecret=bytearray(0), tickets=None):
+               resumptionMasterSecret=bytearray(0), tickets=None,
+               tls_1_0_tickets=None):
         self.masterSecret = masterSecret
         self.sessionID = sessionID
         self.cipherSuite = cipherSuite
         self.srpUsername = srpUsername
         self.clientCertChain = clientCertChain
         self.serverCertChain = serverCertChain
         self.tackExt = tackExt
@@ -112,14 +118,15 @@
         self.appProto = appProto
         self.cl_app_secret = cl_app_secret
         self.sr_app_secret = sr_app_secret
         self.exporterMasterSecret = exporterMasterSecret
         self.resumptionMasterSecret = resumptionMasterSecret
         # NOTE we need a reference copy not a copy of object here!
         self.tickets = tickets
+        self.tls_1_0_tickets = tls_1_0_tickets
 
     def _clone(self):
         other = Session()
         other.masterSecret = self.masterSecret
         other.sessionID = self.sessionID
         other.cipherSuite = self.cipherSuite
         other.srpUsername = self.srpUsername
@@ -133,24 +140,26 @@
         other.extendedMasterSecret = self.extendedMasterSecret
         other.appProto = self.appProto
         other.cl_app_secret = self.cl_app_secret
         other.sr_app_secret = self.sr_app_secret
         other.exporterMasterSecret = self.exporterMasterSecret
         other.resumptionMasterSecret = self.resumptionMasterSecret
         other.tickets = self.tickets
+        other.tls_1_0_tickets = self.tls_1_0_tickets
         return other
 
     def valid(self):
         """If this session can be used for session resumption.
 
         :rtype: bool
         :returns: If this session can be used for session resumption.
         """
         # TODO add checks for tickets received from server (freshness etc.)
-        return self.resumable and (self.sessionID or self.tickets)
+        return self.resumable and (self.sessionID or self.tickets or
+                                   self.tls_1_0_tickets)
 
     def _setResumable(self, boolean):
         #Only let it be set to True if the sessionID is non-null
         if (not boolean) or (boolean and self.sessionID):
             self.resumable = boolean
 
     def getTackId(self):
@@ -176,7 +185,42 @@
     def getMacName(self):
         """Get the name of the HMAC hash algo used with this connection.
 
         :rtype: str
         :returns: The name of the HMAC hash algo used with this connection.
         """
         return CipherSuite.canonicalMacName(self.cipherSuite)
+
+
+class Ticket(object):
+    """
+    This class holds the ticket and ticket lifetime which are recieved from
+    the server, together with the session object, it's all the information
+    needed to resume a session using SessionTickets in TLSv1.2.
+    Currently objects of this class are only used in client side session cache
+    where we can iterate over them and use them for resumption when possible.
+
+    :vartype ticket: bytearray
+    :ivar ticket: the actual ticket recieved from the server
+
+    :vartype ticket_lifetime: int
+    :ivar ticket_lifetime: lifetime of the ticket defined by the server
+
+    :vartype master_secret: bytearray
+    :ivar master_secret: master secret used to resume the session
+
+    :vartype cipher_suite: int
+    :ivar cipher_suite: ciphersuite used to resume the session
+
+    :vartype time_recieved: int
+    :ivar time_recieved: the actual time when we recieved the ticket
+    """
+
+    def __init__(self, ticket, ticket_lifetime, master_secret, cipher_suite):
+        self.ticket = ticket
+        self.ticket_lifetime = ticket_lifetime
+        self.master_secret = master_secret
+        self.cipher_suite = cipher_suite
+        self.time_received = time.time()
+
+    def valid(self):
+        return time.time() < self.time_received + self.ticket_lifetime
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/sessioncache.py` & `tlslite-ng-0.8.0a46/tlslite/sessioncache.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/signed.py` & `tlslite-ng-0.8.0a46/tlslite/signed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/tlsconnection.py` & `tlslite-ng-0.8.0a46/tlslite/tlsconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from __future__ import division
 import time
 import socket
 from itertools import chain
 from .utils.compat import formatExceptionTrace
 from .tlsrecordlayer import TLSRecordLayer
-from .session import Session
+from .session import Session, Ticket
 from .constants import *
 from .utils.cryptomath import derive_secret, getRandomBytes, HKDF_expand_label
 from .utils.dns_utils import is_valid_hostname
 from .utils.lists import getFirstMatching
 from .errors import *
 from .messages import *
 from .mathtls import *
@@ -571,18 +571,18 @@
 
         if serverHello.getExtension(ExtensionType.extended_master_secret):
             self.extendedMasterSecret = True
 
         #If the server elected to resume the session, it is handled here.
         for result in self._clientResume(session, serverHello,
                         clientHello.random,
-                        settings.cipherImplementations,
                         nextProto, settings):
             if result in (0,1): yield result
             else: break
+
         if result == "resumed_and_finished":
             self._handshakeDone(resumed=True)
             self._serverRandom = serverHello.random
             self._clientRandom = clientHello.random
             # alpn protocol is independent of resumption and renegotiation
             # and needs to be negotiated every time
             alpnExt = serverHello.getExtension(ExtensionType.alpn)
@@ -662,15 +662,16 @@
                             srpUsername, clientCertChain, serverCertChain,
                             tackExt, (serverHello.tackExt is not None),
                             serverName,
                             encryptThenMAC=self._recordLayer.encryptThenMAC,
                             extendedMasterSecret=self.extendedMasterSecret,
                             appProto=alpnProto,
                             # NOTE it must be a reference not a copy
-                            tickets=self.tickets)
+                            tickets=self.tickets,
+                            tls_1_0_tickets=self.tls_1_0_tickets)
         self._handshakeDone(resumed=False)
         self._serverRandom = serverHello.random
         self._clientRandom = clientHello.random
 
 
     def _clientSendClientHello(self, settings, session, srpUsername,
                                 srpParams, certParams, anonParams,
@@ -782,14 +783,35 @@
                 HeartbeatMode.PEER_ALLOWED_TO_SEND))
             self.heartbeat_can_receive = True
 
         if settings.record_size_limit:
             extensions.append(RecordSizeLimitExtension().create(
                 settings.record_size_limit))
 
+        # If SessionTicket support is enabled and we have a valid ticket, we
+        # send it in an attempt to resume the session, if SessionTicket support
+        # is enabled but we don't have a valid ticket, we send an empty ext
+        # to indicate support for the feaure
+        if session and session.tls_1_0_tickets:
+            # first get rid of expired tickets
+            session.tls_1_0_tickets[:] = [
+                i for i in session.tls_1_0_tickets if i.valid()]
+            # then send first ticket
+            for cached_ticket in session.tls_1_0_tickets:
+                extensions.append(SessionTicketExtension().create(
+                    cached_ticket.ticket))
+                break
+            else:
+                # or just advertise that we support session resumption
+                extensions.append(SessionTicketExtension().create(
+                    bytearray(0)))
+        else:
+            extensions.append(SessionTicketExtension().create(
+                bytearray(0)))
+
         # don't send empty list of extensions or extensions in SSLv3
         if not extensions or settings.maxVersion == (3, 0):
             extensions = None
 
         sent_version = min(settings.maxVersion, (3, 3))
 
         #Either send ClientHello (with a resumable session)...
@@ -1592,31 +1614,32 @@
             else:
                 # If the client doesn't support any of server's protocols,
                 # or the server doesn't advertise any (next_protos == [])
                 # the client SHOULD select the first protocol it supports.
                 return bytearray(nextProtos[0])
         return None
  
-    def _clientResume(self, session, serverHello, clientRandom, 
-                      cipherImplementations, nextProto, settings):
-        #If the server agrees to resume
-        if session and session.sessionID and \
-            serverHello.session_id == session.sessionID:
+    def _clientResume(self, session, serverHello, clientRandom,
+                      nextProto, settings):
+
+        if session and ((session.sessionID and \
+            serverHello.session_id == session.sessionID) or
+            session.tls_1_0_tickets):
 
             if serverHello.cipher_suite != session.cipherSuite:
                 for result in self._sendError(\
                     AlertDescription.illegal_parameter,\
                     "Server's ciphersuite doesn't match session"):
                     yield result
 
             #Calculate pending connection states
             self._calcPendingStates(session.cipherSuite,
                                     session.masterSecret,
                                     clientRandom, serverHello.random,
-                                    cipherImplementations)
+                                    settings.cipherImplementations)
 
             #Exchange ChangeCipherSpec and Finished messages
             for result in self._getFinished(session.masterSecret,
                                             session.cipherSuite):
                 yield result
             # buffer writes so that CCS and Finished go out in one TCP packet
             self.sock.buffer_writes = True
@@ -1824,30 +1847,19 @@
                 yield result
 
         yield (premasterSecret, serverCertChain, clientCertChain, tackExt)
 
     def _clientFinished(self, premasterSecret, clientRandom, serverRandom,
                         cipherSuite, cipherImplementations, nextProto,
                         settings):
-        if self.extendedMasterSecret:
-            cvhh = self._certificate_verify_handshake_hash
-            # in case of session resumption, or when the handshake doesn't
-            # use the certificate authentication, the hashes are the same
-            if not cvhh:
-                cvhh = self._handshake_hash
-            masterSecret = calc_key(self.version, premasterSecret,
-                                    cipherSuite, b"extended master secret",
-                                    handshake_hashes=cvhh,
-                                    output_length=48)
-        else:
-            masterSecret = calc_key(self.version, premasterSecret,
-                                    cipherSuite, b"master secret",
-                                    client_random=clientRandom,
-                                    server_random=serverRandom,
-                                    output_length=48)
+
+        masterSecret = self._calculate_master_secret(premasterSecret,
+                                                     cipherSuite,
+                                                     clientRandom,
+                                                     serverRandom)
         self._calcPendingStates(cipherSuite, masterSecret, 
                                 clientRandom, serverRandom, 
                                 cipherImplementations)
 
         #Exchange ChangeCipherSpec and Finished messages
         for result in self._sendFinished(masterSecret, cipherSuite, nextProto,
                 settings=settings):
@@ -2271,14 +2283,24 @@
 
         if clientHello.getExtension(ExtensionType.record_size_limit) and \
                 settings.record_size_limit:
             # in TLS 1.2 and earlier we can select at most 2^14B records
             extensions.append(RecordSizeLimitExtension().create(
                 min(2**14, settings.record_size_limit)))
 
+        # If the client indicates that it supports resumption using
+        # session_ticket extension, we send a zero len extension to indicate
+        # that we are going to
+        # send a new ticket in a NewSessionTicket message
+        send_session_ticket = False
+        session_ticket = clientHello.getExtension(ExtensionType.session_ticket)
+        if session_ticket and len(session_ticket.ticket) == 0:
+            send_session_ticket = True
+            extensions.append(SessionTicketExtension().create(
+                bytearray(0)))
 
         # don't send empty list of extensions
         if not extensions:
             extensions = None
 
         serverHello = ServerHello()
         # RFC 8446, section 4.1.3
@@ -2373,47 +2395,51 @@
                                                       cipherSuite):
                 if result in (0,1): yield result
                 else: break
             premasterSecret = result
 
         else:
             assert(False)
-                        
-        # Exchange Finished messages      
-        for result in self._serverFinished(premasterSecret, 
-                                clientHello.random, serverHello.random,
-                                cipherSuite, settings.cipherImplementations,
-                                nextProtos, settings):
-                if result in (0,1): yield result
-                else: break
-        masterSecret = result
 
-        #Create the session object
+        # Create the session object
         self.session = Session()
         if cipherSuite in CipherSuite.certAllSuites or \
                 cipherSuite in CipherSuite.ecdheEcdsaSuites:
             serverCertChain = cert_chain
         else:
             serverCertChain = None
         srpUsername = None
         serverName = None
         if clientHello.srp_username:
             srpUsername = clientHello.srp_username.decode("utf-8")
         if clientHello.server_name:
             serverName = clientHello.server_name.decode("utf-8")
-        self.session.create(masterSecret, serverHello.session_id, cipherSuite,
+
+        # We'll update the session master secret once it is calculated
+        # in _serverFinished
+        self.session.create(b"", serverHello.session_id, cipherSuite,
                             srpUsername, clientCertChain, serverCertChain,
                             tackExt, (serverHello.tackExt is not None),
                             serverName,
-                            encryptThenMAC=self._recordLayer.encryptThenMAC,
+                            encryptThenMAC=
+                            self._recordLayer._get_pending_state_etm(),
                             extendedMasterSecret=self.extendedMasterSecret,
                             appProto=selectedALPN,
                             # NOTE it must be a reference, not a copy!
                             tickets=self.tickets)
 
+        # Exchange Finished messages
+        for result in self._serverFinished(premasterSecret,
+                                clientHello.random, serverHello.random,
+                                cipherSuite, settings.cipherImplementations,
+                                nextProtos, settings, send_session_ticket,
+                                clientCertChain):
+                if result in (0,1): yield result
+                else: break
+
         #Add the session object to the session cache
         if sessionCache and sessionID:
             sessionCache[sessionID] = self.session
 
         self._handshakeDone(resumed=False)
         self._serverRandom = serverHello.random
         self._clientRandom = clientHello.random
@@ -2479,23 +2505,35 @@
         return key, iv
 
     def _serverSendTickets(self, settings):
         """Send session tickets to client."""
         if not settings.ticketKeys:
             return
 
-        for _ in range(settings.ticket_count):
+        if self.version < (3, 4):
+            secret = self.session.masterSecret
+        else:
+            secret = self.session.resumptionMasterSecret
+
+        # make sure we send at most one ticket in TLS 1.2 and earlier
+        for _ in range(settings.ticket_count if self.version > (3, 3) else
+                       int(bool(settings.ticket_count))):
             # prepare the ticket
             ticket = SessionTicketPayload()
-            ticket.create(self.session.resumptionMasterSecret,
+            ticket.create(secret,
                           self.version,
                           self.session.cipherSuite,
                           int(time.time()),
                           getRandomBytes(len(settings.ticketKeys[0])),
-                          client_cert_chain=self.session.clientCertChain)
+                          client_cert_chain=self.session.clientCertChain,
+                          encrypt_then_mac=
+                          self._recordLayer._get_pending_state_etm(),
+                          extended_master_secret=self.extendedMasterSecret,
+                          server_name=self.session.serverName.encode("utf-8")
+                          if self.session.serverName else bytearray())
 
             # encrypt the ticket
 
             # generate keys for the encryption
             nonce = getRandomBytes(32)
             key, iv = self._derive_key_iv(nonce, settings.ticketKeys[0],
                                           settings)
@@ -2511,36 +2549,47 @@
                 assert settings.ticketCipher == "chacha20-poly1305"
                 cipher = createCHACHA20(key,
                                         settings.cipherImplementations)
 
             encrypted_ticket = cipher.seal(iv, ticket.write(), b'')
 
             # encapsulate the ticket and send to client
-            new_ticket = NewSessionTicket()
-            new_ticket.create(settings.ticketLifetime,
-                              getRandomNumber(1, 8**4),
-                              ticket.nonce,
-                              nonce + encrypted_ticket,
-                              [])
+            if self.version < (3, 4):
+                new_ticket = NewSessionTicket1_0()
+                new_ticket.create(settings.ticketLifetime,
+                                  nonce + encrypted_ticket)
+                self.tls_1_0_tickets.append(encrypted_ticket)
+            else:
+                new_ticket = NewSessionTicket()
+                new_ticket.create(settings.ticketLifetime,
+                                  getRandomNumber(1, 8**4),
+                                  ticket.nonce,
+                                  nonce + encrypted_ticket,
+                                  [])
             self._queue_message(new_ticket)
 
         # send tickets to client
         if settings.ticket_count:
             for result in self._queue_flush():
                 yield result
 
-    def _tryDecrypt(self, settings, identity):
+    def _tryDecrypt(self, settings, identity=None, ticket=None):
         if not settings.ticketKeys:
             return None, None
 
-        if len(identity.identity) < 33:
-            # too small for an encrypted ticket
-            return None, None
+        if self.version < (3, 4):
+            assert ticket
+            nonce, encrypted_ticket = ticket[:32], ticket[32:]
+        else:
+            assert identity
+            if len(identity.identity) < 33:
+                # too small for an encrypted ticket
+                return None, None
+            nonce, encrypted_ticket = identity.identity[:32], identity.identity[32:]
 
-        nonce, encrypted_ticket = identity.identity[:32], identity.identity[32:]
         for user_key in settings.ticketKeys:
             key, iv = self._derive_key_iv(nonce, user_key, settings)
             if settings.ticketCipher in ("aes128gcm", "aes256gcm"):
                 cipher = createAESGCM(key, settings.cipherImplementations)
             elif settings.ticketCipher in ("aes128ccm", "aes256ccm"):
                 cipher = createAESCCM(key, settings.cipherImplementations)
             elif settings.ticketCipher in ("aes128ccm_8", "aes256ccm_8"):
@@ -2555,28 +2604,31 @@
 
             parser = Parser(ticket)
             try:
                 ticket = SessionTicketPayload().parse(parser)
             except ValueError:
                 continue
 
+            if self.version < (3, 4):
+                return None, ticket
+
             prf = 'sha384' if ticket.cipher_suite \
                 in CipherSuite.sha384PrfSuites else 'sha256'
 
             new_sess_ticket = NewSessionTicket()
             new_sess_ticket.ticket_nonce = ticket.nonce
             new_sess_ticket.ticket = identity.identity
 
             psk = HandshakeHelpers.calc_res_binder_psk(identity,
                                                        ticket.master_secret,
                                                        [new_sess_ticket])
 
             return ((identity.identity, psk, prf), ticket)
 
-        # no keys
+        # no working keys
         return None, None
 
     def _serverTLS13Handshake(self, settings, clientHello, cipherSuite,
                               privateKey, serverCertChain, version, scheme,
                               srv_alpns, reqCert):
         """Perform a TLS 1.3 handshake"""
         prf_name, prf_size = self._getPRFParams(cipherSuite)
@@ -2615,14 +2667,19 @@
                 if not match:
                     (match, ticket) = self._tryDecrypt(settings, ident)
                     external = False
                     if not match:
                         continue
                     match = [match]
 
+                # check if the ticket version matches
+                # but with PSK we don't have a ticket, but we still can have a
+                # binder value, so `match` will be non-null
+                if ticket and self.version != ticket.protocol_version:
+                    continue
                 # check if PSK can be used with selected cipher suite
                 psk_hash = match[0][2] if len(match[0]) > 2 else 'sha256'
                 if psk_hash != prf_name:
                     continue
 
                 psk = match[0][1]
                 selected_psk = i
@@ -3009,14 +3066,39 @@
         self._changeReadState()
 
         for result in self._serverSendTickets(settings):
             yield result
 
         yield "finished"
 
+    def _ticket_to_session(self, settings, ticket_ext):
+        if not ticket_ext.ticket:
+            return None
+        _, ticket = self._tryDecrypt(settings, ticket=ticket_ext.ticket)
+        if not ticket:
+            return None
+
+        if ticket.creation_time + settings.ticketLifetime < time.time():
+            return None
+
+        session = Session()
+        session.create(ticket.master_secret,
+                       b'',  # no session_id
+                       ticket.cipher_suite,
+                       '',  # not SRP
+                       ticket.client_cert_chain,
+                       None,  # no server cert chain
+                       None,  # no TACK
+                       False,  # no TACK
+                       serverName=ticket.server_name.decode("utf-8") if
+                       ticket.server_name else "",
+                       encryptThenMAC=ticket.encrypt_then_mac,
+                       extendedMasterSecret=ticket.extended_master_secret)
+        return session
+
     def _serverGetClientHello(self, settings, private_key, cert_chain,
                               verifierDB,
                               sessionCache, anon, alpn, sni):
         # Tentatively set version to most-desirable version, so if an error
         # occurs parsing the ClientHello, this will be the version we'll use
         # for the error alert
         # If TLS 1.3 is enabled, use the "compatible" TLS 1.2 version
@@ -3452,22 +3534,39 @@
                                                        version)
         else:
             assert False
         cipherSuites = CipherSuite.filterForVersion(cipherSuites,
                                                     minVersion=version,
                                                     maxVersion=version)
 
-        #If resumption was requested and we have a session cache...
-        if clientHello.session_id and sessionCache:
+        ticket_ext = clientHello.getExtension(ExtensionType.session_ticket)
+
+        # If resumption was requested and we have a session cache...
+        if (clientHello.session_id and sessionCache) or (
+                ticket_ext and ticket_ext.ticket):
             session = None
 
             # Check if the session there is good enough and consistent with
             # new Client Hello
             try:
-                session = sessionCache[clientHello.session_id]
+                if ticket_ext:
+                    session = self._ticket_to_session(settings, ticket_ext)
+                    # client MAY send a random session_id to easily tell
+                    # if the session is resumed, for that server has to
+                    # echo the session_ID back
+                    if session and clientHello.session_id:
+                        session.sessionID = clientHello.session_id
+                if not session and \
+                        (not ticket_ext or ticket_ext and not ticket_ext.ticket)\
+                        and sessionCache and clientHello.session_id:
+                    # Session ID resumption is allowed only if the client
+                    # didn't send a ticket
+                    session = sessionCache[clientHello.session_id]
+                if not session:
+                    raise KeyError()
                 if not session.resumable:
                     raise AssertionError()
                 # Check if we are willing to use that old cipher still
                 if session.cipherSuite not in cipherSuites:
                     session = None
                     raise KeyError()
                 # Check for consistency with ClientHello
@@ -3517,17 +3616,17 @@
 
             #If a session is found..
             if session:
                 #Send ServerHello
                 extensions = []
                 if session.encryptThenMAC:
                     self._recordLayer.encryptThenMAC = True
-                    mte = TLSExtension().create(ExtensionType.encrypt_then_mac,
+                    etm = TLSExtension().create(ExtensionType.encrypt_then_mac,
                                                 bytearray(0))
-                    extensions.append(mte)
+                    extensions.append(etm)
                 if session.extendedMasterSecret:
                     ems = TLSExtension().create(ExtensionType.
                                                 extended_master_secret,
                                                 bytearray(0))
                     extensions.append(ems)
                 secureRenego = False
                 renegoExt = clientHello.\
@@ -3956,35 +4055,49 @@
                 client_sigalgs = \
                         client_hello. \
                         getExtension(ExtensionType.signature_algorithms). \
                         sigalgs
             else:
                 client_sigalgs = []
 
+        client_psks = client_hello.getExtension(ExtensionType.pre_shared_key)
+
         # Get all the certificates we can offer
         alt_certs = ((X509CertChain(i.certificates), i.key) for vh in
                      settings.virtual_hosts for i in vh.keys)
         certs = [(cert, key)
                  for cert, key in chain([(cert_chain, private_key)], alt_certs)]
 
         for cert, key in certs:
-
             # Check if this is the last (cert, key) pair we have to check
             if (cert, key) == certs[-1]:
                 last_cert = True
 
             # Mandatory checks. If any one of these checks fail, the certificate
             # is not usuable.
             try:
                 # Find a suitable ciphersuite based on the certificate
                 ciphers = CipherSuite.filter_for_certificate(cipher_suites, cert)
+                # but if we have matching PSKs, prefer those
+                if settings.pskConfigs and client_psks:
+                    client_identities = [
+                        i.identity for i in client_psks.identities]
+                    psks_prfs = [i[2] if len(i) == 3 else None for i in
+                                 settings.pskConfigs if
+                                 i[0] in client_identities]
+                    if psks_prfs:
+                        ciphers = CipherSuite.filter_for_prfs(ciphers,
+                                                              psks_prfs)
                 for cipher in ciphers:
+                    # select first mutually supported
                     if cipher in client_hello.cipher_suites:
                         break
                 else:
+                    # abort with context-specific alert if client indicated
+                    # support for FFDHE groups
                     if client_groups and \
                         any(i in range(256, 512) for i in client_groups) and \
                         any(i in CipherSuite.dhAllSuites
                             for i in client_hello.cipher_suites):
                             raise TLSInsufficientSecurity(
                                     "FFDHE groups not acceptable and no other common "
                                     "ciphers")
@@ -4282,60 +4395,52 @@
             for result in self._sendError(AlertDescription.decode_error,
                                           str(alert)):
                 yield result
 
         yield premasterSecret
 
 
-    def _serverFinished(self,  premasterSecret, clientRandom, serverRandom,
+    def _serverFinished(self, premasterSecret, clientRandom, serverRandom,
                         cipherSuite, cipherImplementations, nextProtos,
-                        settings):
-        if self.extendedMasterSecret:
-            cvhh = self._certificate_verify_handshake_hash
-            # in case of resumption or lack of certificate authentication,
-            # the CVHH won't be initialised, but then it would also be equal
-            # to regular handshake hash
-            if not cvhh:
-                cvhh = self._handshake_hash
-            masterSecret = calc_key(self.version, premasterSecret,
-                                    cipherSuite, b"extended master secret",
-                                    handshake_hashes=cvhh,
-                                    output_length=48)
-        else:
-            masterSecret = calc_key(self.version, premasterSecret,
-                                    cipherSuite, b"master secret",
-                                    client_random=clientRandom,
-                                    server_random=serverRandom,
-                                    output_length=48)
+                        settings, send_session_ticket=False,
+                        client_cert_chain=None):
+
+        masterSecret = self._calculate_master_secret(premasterSecret,
+                                                     cipherSuite,
+                                                     clientRandom,
+                                                     serverRandom)
+        self.session.masterSecret = masterSecret
 
         #Calculate pending connection states
         self._calcPendingStates(cipherSuite, masterSecret, 
                                 clientRandom, serverRandom,
                                 cipherImplementations)
 
         #Exchange ChangeCipherSpec and Finished messages
         for result in self._getFinished(masterSecret,
                                         cipherSuite,
                                    expect_next_protocol=nextProtos is not None):
             yield result
 
         for result in self._sendFinished(masterSecret, cipherSuite,
-                settings=settings):
+                                         settings=settings,
+                                         send_session_ticket=send_session_ticket,
+                                         client_cert_chain=client_cert_chain):
             yield result
-        
-        yield masterSecret        
-
 
     #*********************************************************
     # Shared Handshake Functions
     #*********************************************************
 
-
     def _sendFinished(self, masterSecret, cipherSuite=None, nextProto=None,
-            settings=None):
+            settings=None, send_session_ticket=False, client_cert_chain=None):
+        if send_session_ticket:
+            for result in self._serverSendTickets(settings):
+                yield result
+
         # send the CCS and Finished in single TCP packet
         self.sock.buffer_writes = True
         #Send ChangeCipherSpec
         for result in self._sendMsg(ChangeCipherSpec()):
             yield result
 
         #Switch to pending write state
@@ -4370,24 +4475,54 @@
         for result in self._sendMsg(finished):
             yield result
         self.sock.flush()
         self.sock.buffer_writes = False
 
     def _getFinished(self, masterSecret, cipherSuite=None,
                      expect_next_protocol=False, nextProto=None):
-        #Get and check ChangeCipherSpec
-        for result in self._getMsg(ContentType.change_cipher_spec):
+
+        expect_ccs_message = True
+        # If we use SessionTicket resumption on client side, there are multiple
+        # situations where the server has the option to send new ticket
+        for result in self._getMsg(
+                (ContentType.handshake, ContentType.change_cipher_spec),
+                HandshakeType.new_session_ticket):
             if result in (0,1):
                 yield result
-        changeCipherSpec = result
+            else: break
 
-        if changeCipherSpec.type != 1:
-            for result in self._sendError(AlertDescription.illegal_parameter,
-                                         "ChangeCipherSpec type incorrect"):
-                yield result
+        if isinstance(result, NewSessionTicket1_0):
+            session_ticket = result
+            # If we receive new ticket we clear the old ones
+            del self.tls_1_0_tickets[:]
+            self.tls_1_0_tickets.append(Ticket(session_ticket.ticket,
+                                        session_ticket.ticket_lifetime,
+                                        masterSecret, cipherSuite))
+
+        else:
+            assert isinstance(result, ChangeCipherSpec)
+            expect_ccs_message = False
+
+            changeCipherSpec = result
+            if changeCipherSpec.type != 1:
+                for result in self._sendError(
+                        AlertDescription.illegal_parameter,
+                        "ChangeCipherSpec type incorrect"):
+                    yield result
+
+        if expect_ccs_message:
+            for result in self._getMsg(ContentType.change_cipher_spec):
+                if result in (0,1):
+                    yield result
+            changeCipherSpec = result
+
+            if changeCipherSpec.type != 1:
+                for result in self._sendError(AlertDescription.illegal_parameter,
+                                             "ChangeCipherSpec type incorrect"):
+                    yield result
 
         #Switch to pending read state
         self._changeReadState()
 
         #Server Finish - Are we waiting for a next protocol echo? 
         if expect_next_protocol:
             for result in self._getMsg(ContentType.handshake, HandshakeType.next_protocol):
@@ -4451,14 +4586,35 @@
                 raise TLSFaultError(str(alert))
             else:
                 pass
         except:
             self._shutdown(False)
             raise
 
+    def _calculate_master_secret(self, premaster_secret, cipher_suite,
+                                 client_random, server_random):
+        if self.extendedMasterSecret:
+            cvhh = self._certificate_verify_handshake_hash
+            # in case of resumption or lack of certificate authentication,
+            # the CVHH won't be initialised, but then it would also be equal
+            # to regular handshake hash
+            if not cvhh:
+                cvhh = self._handshake_hash
+            secret = calc_key(self.version, premaster_secret,
+                              cipher_suite, b"extended master secret",
+                              handshake_hashes=cvhh,
+                              output_length=48)
+        else:
+            secret = calc_key(self.version, premaster_secret,
+                              cipher_suite, b"master secret",
+                              client_random=client_random,
+                              server_random=server_random,
+                              output_length=48)
+        return secret
+
     @staticmethod
     def _pickServerKeyExchangeSig(settings, clientHello, certList=None,
                                   private_key=None,
                                   version=(3, 3), check_alt=True):
         """Pick a hash that matches most closely the supported ones"""
         hashAndAlgsExt = clientHello.getExtension(
             ExtensionType.signature_algorithms)
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/tlsrecordlayer.py` & `tlslite-ng-0.8.0a46/tlslite/tlsrecordlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,16 @@
         self.fault = None
 
         # Temporarily limit the size of outgoing records to following size
         self._user_record_limit = 16384  # 2**14
 
         # NewSessionTickets received from server
         self.tickets = []
+        # TLS 1.2 and earlier tickets received from server
+        self.tls_1_0_tickets = []
 
         # Indicator for heartbeat extension mode, if we can receive
         # heartbeat requests
         self.heartbeat_can_receive = False
 
         # Indicator for heartbeat extension mode, if we can send
         # heartbeat requests
@@ -1035,14 +1037,25 @@
                         for result in self._sendError(
                                 AlertDescription.unexpected_message,
                                 "Invalid CCS message received"):
                             yield result
                     # ignore the message
                     continue
 
+                # TLS 1.3 Handshake messages MUST NOT be interleaved with
+                # other messages, Section 5.1 RFC 8446
+                if self.version > (3, 3) and \
+                        recordHeader.type != ContentType.handshake and \
+                        self._defragmenter.buffers[ContentType.handshake]:
+                    for result in self._sendError(
+                            AlertDescription.unexpected_message,
+                            "Interleaved Handshake and "
+                            "non-handshake messages"):
+                        yield result
+
                 #If we received an unexpected record type...
                 if recordHeader.type not in expectedType:
 
                     #If we received an alert...
                     if recordHeader.type == ContentType.alert:
                         alert = Alert().parse(p)
 
@@ -1184,14 +1197,28 @@
                         rec = HandshakeType.toStr(subType)
                         for result in self._sendError(AlertDescription
                                                       .unexpected_message,
                                                       "Expecting {0}, got {1}"
                                                       .format(exp, rec)):
                             yield result
 
+                # in TLS 1.3 some Handshake messages MUST NOT span key changes
+                if self.version > (3, 3) and \
+                        subType in (HandshakeType.client_hello,
+                                    HandshakeType.end_of_early_data,
+                                    HandshakeType.server_hello,
+                                    HandshakeType.finished,
+                                    HandshakeType.key_update) and \
+                        not self._defragmenter.is_empty():
+                    for result in self._sendError(
+                            AlertDescription.unexpected_message,
+                            "CH, EOED, SH, Finished, or KU not aligned with "
+                            "record boundary"):
+                        yield result
+
                 #Update handshake hashes
                 self._handshake_hash.update(p.bytes)
 
                 #Parse based on handshake type
                 if subType == HandshakeType.client_hello:
                     yield ClientHello(recordHeader.ssl2).parse(p)
                 elif subType == HandshakeType.server_hello:
@@ -1213,15 +1240,18 @@
                 elif subType == HandshakeType.finished:
                     yield Finished(self.version, constructorType).parse(p)
                 elif subType == HandshakeType.next_protocol:
                     yield NextProtocol().parse(p)
                 elif subType == HandshakeType.encrypted_extensions:
                     yield EncryptedExtensions().parse(p)
                 elif subType == HandshakeType.new_session_ticket:
-                    yield NewSessionTicket().parse(p)
+                    if self.version < (3, 4):
+                        yield NewSessionTicket1_0().parse(p)
+                    else:
+                        yield NewSessionTicket().parse(p)
                 elif subType == HandshakeType.key_update:
                     yield KeyUpdate().parse(p)
                 else:
                     raise AssertionError()
 
         #If an exception was raised by a Parser or Message instance:
         except BadCertificateError as e:
```

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/__init__.py` & `tlslite-ng-0.8.0a46/tlslite/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/aes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/aesccm.py` & `tlslite-ng-0.8.0a46/tlslite/utils/aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/aesgcm.py` & `tlslite-ng-0.8.0a46/tlslite/utils/aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/asn1parser.py` & `tlslite-ng-0.8.0a46/tlslite/utils/asn1parser.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/chacha.py` & `tlslite-ng-0.8.0a46/tlslite/utils/chacha.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/chacha20_poly1305.py` & `tlslite-ng-0.8.0a46/tlslite/utils/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/cipherfactory.py` & `tlslite-ng-0.8.0a46/tlslite/utils/cipherfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/codec.py` & `tlslite-ng-0.8.0a46/tlslite/utils/codec.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/compat.py` & `tlslite-ng-0.8.0a46/tlslite/utils/compat.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/constanttime.py` & `tlslite-ng-0.8.0a46/tlslite/utils/constanttime.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/cryptomath.py` & `tlslite-ng-0.8.0a46/tlslite/utils/cryptomath.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/datefuncs.py` & `tlslite-ng-0.8.0a46/tlslite/utils/datefuncs.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/deprecations.py` & `tlslite-ng-0.8.0a46/tlslite/utils/deprecations.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/dns_utils.py` & `tlslite-ng-0.8.0a46/tlslite/utils/dns_utils.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/dsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/ecc.py` & `tlslite-ng-0.8.0a46/tlslite/utils/ecc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/ecdsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/eddsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/eddsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/keyfactory.py` & `tlslite-ng-0.8.0a46/tlslite/utils/keyfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/lists.py` & `tlslite-ng-0.8.0a46/tlslite/utils/lists.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesccm.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesgcm.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_rc4.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_rsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/openssl_tripledes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/openssl_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/pem.py` & `tlslite-ng-0.8.0a46/tlslite/utils/pem.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/poly1305.py` & `tlslite-ng-0.8.0a46/tlslite/utils/poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rc4.py` & `tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_tripledes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/pycrypto_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_aes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_dsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_ecdsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_eddsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_eddsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_key.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_key.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_rc4.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_rsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/python_tripledes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/python_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/rc4.py` & `tlslite-ng-0.8.0a46/tlslite/utils/rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/rijndael.py` & `tlslite-ng-0.8.0a46/tlslite/utils/rijndael.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/rsakey.py` & `tlslite-ng-0.8.0a46/tlslite/utils/rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/tlshashlib.py` & `tlslite-ng-0.8.0a46/tlslite/utils/tlshashlib.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/tlshmac.py` & `tlslite-ng-0.8.0a46/tlslite/utils/tlshmac.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/tripledes.py` & `tlslite-ng-0.8.0a46/tlslite/utils/tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/utils/x25519.py` & `tlslite-ng-0.8.0a46/tlslite/utils/x25519.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/verifierdb.py` & `tlslite-ng-0.8.0a46/tlslite/verifierdb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/x509.py` & `tlslite-ng-0.8.0a46/tlslite/x509.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite/x509certchain.py` & `tlslite-ng-0.8.0a46/tlslite/x509certchain.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/tlslite_ng.egg-info/PKG-INFO` & `tlslite-ng-0.8.0a46/tlslite_ng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlslite-ng
-Version: 0.8.0a45
+Version: 0.8.0a46
 Summary: Pure python implementation of SSL and TLS.
 Home-page: https://github.com/tlsfuzzer/tlslite-ng
 Author: Hubert Kario
 Author-email: hkario@redhat.com
 License: LGPLv2
 Keywords: ssl,tls,pure-python
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Obsoletes: tlslite
 Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
 
@@ -50,16 +53,16 @@
  - secp256r1, secp384r1, secp521r1, secp256k1, secp224r1 and secp192r1 curves
    for ECDHE key exchange (support for last two depends on the version of ecdsa
    library used)
  - x25519 and x448 curves for ECDHE key exchage (RFC 7748. RFC 4492bis)
  - anonymous DHE key exchange
  - anonymous ECDH key exchange
  - PSK and PSK-DH key exchange in TLS 1.3
- - session ticket based resumption in TLS 1.3
- - post-handshake key authentication in TLS 1.3
+ - session ticket based resumption (RFC 5077) and in TLS 1.3
+ - post-handshake client authentication in TLS 1.3
  - NULL encryption ciphersuites
  - FALLBACK_SCSV (RFC 7507)
  - encrypt-then-MAC mode of operation for CBC ciphersuites (RFC 7366)
  - TACK certificate pinning
  - SRP_SHA_RSA and SRP_SHA ciphersuites (RFC 5054)
  - Extended Master Secret calculation for TLS connections (RFC 7627)
  - padding extension (RFC 7685)
```

### Comparing `tlslite-ng-0.8.0a45/tlslite_ng.egg-info/SOURCES.txt` & `tlslite-ng-0.8.0a46/tlslite_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/mocksock.py` & `tlslite-ng-0.8.0a46/unit_tests/mocksock.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tls1_3_vectors.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tls1_3_vectors.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_bufferedsocket.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_bufferedsocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_constants.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_constants.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_defragmenter.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_defragmenter.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_dh.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_dh.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_extensions.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         RenegotiationInfoExtension, ALPNExtension, StatusRequestExtension, \
         SupportedVersionsExtension, VarSeqListExtension, ListExtension, \
         ClientKeyShareExtension, KeyShareEntry, ServerKeyShareExtension, \
         CertificateStatusExtension, HRRKeyShareExtension, \
         SrvSupportedVersionsExtension, SignatureAlgorithmsCertExtension, \
         PreSharedKeyExtension, PskIdentity, SrvPreSharedKeyExtension, \
         PskKeyExchangeModesExtension, CookieExtension, VarBytesExtension, \
-        HeartbeatExtension, IntExtension, RecordSizeLimitExtension
+        HeartbeatExtension, IntExtension, RecordSizeLimitExtension, \
+        SessionTicketExtension
 from tlslite.utils.codec import Parser, Writer
 from tlslite.constants import NameType, ExtensionType, GroupName,\
         ECPointFormat, HashAlgorithm, SignatureAlgorithm, \
         CertificateStatusType, SignatureScheme, HeartbeatMode, CertificateType
 from tlslite.errors import TLSInternalError
 
 class TestTLSExtension(unittest.TestCase):
@@ -2815,9 +2816,97 @@
             "CookieExtension(len(cookie)=4)")
 
     def test___repr___with_none(self):
         ext = CookieExtension()
         self.assertEqual(repr(ext), "CookieExtension(cookie=None)")
 
 
+class TestSessionTicketExtension(unittest.TestCase):
+    def test___init__(self):
+        ext = SessionTicketExtension()
+
+        self.assertIsNotNone(ext)
+        self.assertIsNone(ext.ticket)
+
+        self.assertEqual(ext.extType, 35)
+
+    def test_create(self):
+        ticket = mock.Mock()
+        ext = SessionTicketExtension().create(ticket)
+
+        self.assertIsInstance(ext, SessionTicketExtension)
+        self.assertIs(ext.ticket, ticket)
+
+    def test_write(self):
+        ticket = b"\x7b\x16\xa8\xd3\xac\xa8\xb9\x4f\x4f\x3e\xd1\x24\x21\xd0\x9c\xa7" \
+                 b"\x68\x20\xd3\x49\xbc\x53\x85\xfa\x84\x94\x44\x2a\x13\x9f\x36\xbd" \
+                 b"\x27\xda\x74\xad\x90\xb1\xf9\x4d\x51\x2c\x90\x83\x32\x57\xc7\x7d" \
+                 b"\x79\xcb\xba\x5e\xff\x12\x31\x7f\xf7\x20\x6d\x95\xac\xd3\x00\x15" \
+                 b"\x00\x40\xfc\x8a\x7b\x99\x02\x53\xa1\xdd\x2a\x46\x2a\xcc\x34\x23" \
+                 b"\x10\x48\xb8\x31\xed\xc5\x96\x83\xb8\x7a\xef\x8b\x1b\x60\x55\x4b" \
+                 b"\x0b\x42\x70\x69\x2f\x80\x84\xb5\x9f\x00\xfe\x91\x67\x4a\x58\xee" \
+                 b"\xc6\xf6\xe5\x87\x39\x6e\xd4\x40\x1a\x82\xc7\x62\x35\xa1\x2d\x5a" \
+                 b"\x15\x98"
+
+        ext = SessionTicketExtension().create(ticket)
+
+        self.assertEqual(bytearray(
+            b"\x00\x23" +         # ext type
+            b"\x00\x82" +         # ext length
+            ticket), ext.write()) # ticket
+
+    def test_parse(self):
+        ext = TLSExtension()
+
+        ticket = b"\x7b\x16\xa8\xd3\xac\xa8\xb9\x4f\x4f\x3e\xd1\x24\x21\xd0\x9c\xa7" \
+                 b"\x68\x20\xd3\x49\xbc\x53\x85\xfa\x84\x94\x44\x2a\x13\x9f\x36\xbd" \
+                 b"\x27\xda\x74\xad\x90\xb1\xf9\x4d\x51\x2c\x90\x83\x32\x57\xc7\x7d" \
+                 b"\x79\xcb\xba\x5e\xff\x12\x31\x7f\xf7\x20\x6d\x95\xac\xd3\x00\x15" \
+                 b"\x00\x40\xfc\x8a\x7b\x99\x02\x53\xa1\xdd\x2a\x46\x2a\xcc\x34\x23" \
+                 b"\x10\x48\xb8\x31\xed\xc5\x96\x83\xb8\x7a\xef\x8b\x1b\x60\x55\x4b" \
+                 b"\x0b\x42\x70\x69\x2f\x80\x84\xb5\x9f\x00\xfe\x91\x67\x4a\x58\xee" \
+                 b"\xc6\xf6\xe5\x87\x39\x6e\xd4\x40\x1a\x82\xc7\x62\x35\xa1\x2d\x5a" \
+                 b"\x15\x98"
+
+        parser = Parser(bytearray(
+            b"\x00\x23" + # ext type
+            b"\x00\x82" + # ext length
+            ticket))      # ticket
+
+        ext = ext.parse(parser)
+        self.assertIsInstance(ext, SessionTicketExtension)
+        self.assertEqual(ext.ticket, ticket)
+
+    def test_write_empty(self):
+        ticket = bytearray(0)
+
+        ext = SessionTicketExtension().create(ticket)
+
+        self.assertEqual(bytearray(
+            b"\x00\x23" +         # ext type
+            b"\x00\x00" +         # ext length
+            ticket), ext.write()) # ticket
+
+    def test_parse_empty(self):
+        ext = TLSExtension()
+
+        ticket = bytearray(0)
+
+        parser = Parser(bytearray(
+            b"\x00\x23" + # ext type
+            b"\x00\x00" + # ext length
+            ticket))      # ticket
+
+        ext = ext.parse(parser)
+        self.assertIsInstance(ext, SessionTicketExtension)
+        self.assertEqual(ext.ticket, ticket)
+
+    def test___repr__(self):
+        ext = SessionTicketExtension().create(bytearray(b'\xab\xcd'))
+
+        self.assertEqual(
+            str(ext),
+            "SessionTicketExtension(ticket=bytearray(b'\\xab\\xcd'))")
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehashes.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakehashes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehelpers.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakehelpers.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakesettings.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_handshakesettings.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_keyexchange.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_keyexchange.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_mathtls.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_mathtls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messages.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from tlslite.messages import ClientHello, ServerHello, RecordHeader3, Alert, \
         RecordHeader2, Message, ClientKeyExchange, ServerKeyExchange, \
         CertificateRequest, CertificateVerify, ServerHelloDone, ServerHello2, \
         ClientMasterKey, ClientFinished, ServerFinished, CertificateStatus, \
         Certificate, Finished, HelloMessage, ChangeCipherSpec, NextProtocol, \
         ApplicationData, EncryptedExtensions, CertificateEntry, \
         NewSessionTicket, SessionTicketPayload, Heartbeat, HelloRequest, \
-        KeyUpdate
-from tlslite.utils.codec import Parser
+        KeyUpdate, NewSessionTicket1_0
+from tlslite.utils.codec import Parser, DecodeError
 from tlslite.constants import CipherSuite, CertificateType, ContentType, \
         AlertLevel, AlertDescription, ExtensionType, ClientCertificateType, \
         HashAlgorithm, SignatureAlgorithm, ECCurveType, GroupName, \
         SSL2HandshakeType, CertificateStatusType, HandshakeType, \
         SignatureScheme, TLS_1_3_HRR, HeartbeatMessageType, \
         KeyUpdateMessageType
 from tlslite.extensions import SNIExtension, ClientCertTypeExtension, \
@@ -203,14 +203,34 @@
         self.assertEqual((1,1), client_hello.client_version)
         self.assertEqual(bytearray(32), client_hello.random)
         self.assertEqual(bytearray(0), client_hello.session_id)
         self.assertEqual([], client_hello.cipher_suites)
         self.assertEqual([], client_hello.compression_methods)
         self.assertEqual([], client_hello.extensions)
 
+    def test_parse_with_too_long_session_id(self):
+        p = Parser(bytearray(
+            # we don't include the type of message as it is handled by the
+            # hello protocol parser
+            #b'x01' +             # type of message - client_hello
+            b'\x00'*2 + b'\x48' + # length - 38 bytes
+            b'\x01\x01' +         # protocol version - arbitrary (invalid)
+            b'\x00'*32 +          # client random
+            b'\x21' +             # session ID length
+            b'\x00' * 33 +        # session ID
+            b'\x00'*2 +           # cipher suites length
+            b'\x00' +             # compression methods length
+            b'\x00\x00'           # extensions length
+            ))
+        client_hello = ClientHello()
+        with self.assertRaises(DecodeError) as e:
+            client_hello = client_hello.parse(p)
+
+        self.assertIn("session_id", str(e.exception))
+
     def test_parse_with_SNI_extension(self):
         p = Parser(bytearray(
             # we don't include the type of message as it is handled by the
             # hello protocol parser
             #b'x01' +             # type of message - client_hello
             b'\x00'*2 + b'\x3c' + # length - 60 bytes
             b'\x01\x01' +         # protocol version - arbitrary (invalid)
@@ -3510,14 +3530,37 @@
                       b'\x11' * 16 +  # nonce
                       b'\x00\x00\x00\x00\x00\xbc\x61\x4e' +  # creation time
                       b'\x00\x01\xff' +  # length of array of certificates
                       b'\x00\x01\xfa' +  # length of certificate
                       self.der_cert + # certificate payload
                       b'\x00\x00'))
 
+    def test_write_v2(self):
+        ticket = SessionTicketPayload()
+        ticket.create(bytearray(b'\x11' * 32),
+                      (3, 3),
+                      0x00af,
+                      12345678,
+                      encrypt_then_mac=True,
+                      server_name=None)
+
+        self.assertEqual(
+            ticket.write(),
+            bytearray(b'\x00\x02' +  # version
+                      b'\x00\x20' +  # master secret length
+                      b'\x11' * 32 +  # master secret
+                      b'\x03\x03' +  # protocol version
+                      b'\x00\xaf' +  # cipher suite
+                      b'\x00' +  # nonce length
+                      b'\x00\x00\x00\x00\x00\xbc\x61\x4e' +  # creation time
+                      b'\x00\x00\x00' +  # length of certificate
+                      b'\x01' +  # encrypt then mac
+                      b'\x00' +  # extended master secret
+                      b'\x00\x00'))  # server name length
+
     def test_parse(self):
         parser = Parser(
             bytearray(b'\x00\x00' +  # version (internal)
                       b'\x00\x20' +  # master secret length
                       b'\x22' * 32 +  # master secret
                       b'\x03\x04' +  # protocol version
                       b'\x13\x02' +  # cipher suite
@@ -3556,14 +3599,39 @@
         self.assertEqual(ticket.nonce, bytearray(b'\x11' * 16))
         self.assertIsNotNone(ticket.client_cert_chain)
         self.assertIsInstance(ticket.client_cert_chain, X509CertChain)
         self.assertEqual(len(ticket.client_cert_chain.x509List), 1)
         self.assertEqual(ticket.client_cert_chain.x509List[0].writeBytes(),
                          self.der_cert)
 
+    def test_parse_v2(self):
+        parser = Parser(
+            bytearray(b'\x00\x02' +  # version
+                      b'\x00\x20' +  # master secret length
+                      b'\x11' * 32 +  # master secret
+                      b'\x03\x03' +  # protocol version
+                      b'\x00\xaf' +  # cipher suite
+                      b'\x00' +  # nonce length
+                      b'\x00\x00\x00\x00\x00\xbc\x61\x4e' +  # creation time
+                      b'\x00\x00\x00' +  # length of certificate
+                      b'\x01' +  # encrypt then mac
+                      b'\x00' +  # extended master secret
+                      b'\x00\x00'))  # server name length
+
+        ticket = SessionTicketPayload().parse(parser)
+
+        self.assertEqual(ticket.master_secret, bytearray(b'\x11' * 32))
+        self.assertEqual(ticket.protocol_version, (3, 3))
+        self.assertEqual(ticket.cipher_suite, 0x00af)
+        self.assertEqual(ticket.creation_time, 12345678)
+        self.assertEqual(ticket.nonce, bytearray())
+        self.assertEqual(ticket.client_cert_chain, None)
+        self.assertEqual(ticket.encrypt_then_mac, True)
+        self.assertEqual(ticket.extended_master_secret, False)
+        self.assertEqual(ticket.server_name, bytearray())
 
     def test_parse_with_wrong_version(self):
         parser = Parser(
             bytearray(b'\x00\xff' +  # version (internal)
                       b'\x00\x20' +  # master secret length
                       b'\x22' * 32 +  # master secret
                       b'\x03\x04' +  # protocol version
@@ -3692,14 +3760,61 @@
             b'\x00'  # trailing byte
             ))
 
         with self.assertRaises(SyntaxError):
             ticket.parse(parser)
 
 
+class TestNewSessionTicket1_0(unittest.TestCase):
+    def test___init__(self):
+        ticket = NewSessionTicket1_0()
+
+        self.assertEqual(ticket.ticket_lifetime, 0)
+        self.assertEqual(ticket.ticket, bytearray(0))
+
+    def test_create(self):
+        ticket = NewSessionTicket1_0()
+        lifetime = mock.Mock()
+        ticket_proper = mock.Mock()
+
+        ticket = ticket.create(lifetime, ticket_proper)
+
+        self.assertIs(ticket.ticket_lifetime, lifetime)
+        self.assertIs(ticket.ticket, ticket_proper)
+
+    def test_write(self):
+        ticket = NewSessionTicket1_0()
+        ticket = ticket.create(1, bytearray(b'ticket'))
+
+
+        self.assertEqual(ticket.write(), bytearray(
+            b'\x04'  # handshake type - new session ticket
+            b'\x00\x00\x0c'  # overall length
+            b'\x00\x00\x00\x01'  # ticket_lifetime
+            b'\x00\x06'  # ticket length
+            b'ticket'  # ticket
+            ))
+
+    def test_parse(self):
+        ticket = NewSessionTicket1_0()
+
+        parser = Parser(bytearray(
+            b'\x00\x00\x0c'  # overall length
+            b'\x00\x00\x00\x01'  # ticket_lifetime
+            b'\x00\x06'  # ticket length
+            b'ticket'  # ticket
+            ))
+
+        ticket = ticket.parse(parser)
+
+        self.assertIsInstance(ticket, NewSessionTicket1_0)
+        self.assertEqual(ticket.ticket_lifetime, 1)
+        self.assertEqual(ticket.ticket, bytearray(b'ticket'))
+
+
 class TestHeartbeat(unittest.TestCase):
     def test___init__(self):
         heartbeat_msg = Heartbeat()
 
         self.assertEqual(heartbeat_msg.message_type, 0)
         self.assertEqual(heartbeat_msg.payload, bytearray(0))
```

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messagesocket.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_messagesocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_ocsp.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_ocsp.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_recordlayer.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_recordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_session.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_session.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_sessioncache.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_sessioncache.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_signed.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_signed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsconnection.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_tlsconnection.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsrecordlayer.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_tlsrecordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aes_split.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aes_split.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aescbc.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aescbc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesccm.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesctr.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesctr.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesgcm.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_asn1.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_asn1.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_chacha.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha20_poly1305.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_codec.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_codec.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_compat.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_compat.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_constanttime.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_constanttime.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_cryptomath.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_deprecations.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_deprecations.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_dns_utils.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_dns_utils.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecc.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_ecc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecdsakey.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_keyfactory.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_keyfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_lists.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_lists.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_poly1305.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_dsakey.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_ecdsakey.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_key.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_python_key.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rijndael.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_rijndael.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rsakey.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tlshashlib.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tlshashlib.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes_split.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_tripledes_split.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_x25519.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_utils_x25519.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_x509.py` & `tlslite-ng-0.8.0a46/unit_tests/test_tlslite_x509.py`

 * *Files identical despite different names*

