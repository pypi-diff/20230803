# Comparing `tmp/bitcoin-utils-0.6.1.tar.gz` & `tmp/bitcoin-utils-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin-utils-0.6.1.tar", last modified: Fri Jun  2 10:28:25 2023, max compression
+gzip compressed data, was "bitcoin-utils-0.6.2.tar", last modified: Thu Aug  3 11:08:22 2023, max compression
```

## Comparing `bitcoin-utils-0.6.1.tar` & `bitcoin-utils-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/LICENSE
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5737 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5421 2023-06-02 10:26:34.000000 bitcoin-utils-0.6.1/README.rst
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5737 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)      535 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/not-zip-safe
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       98 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/requires.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/top_level.txt
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/bitcoinutils/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       23 2023-05-18 16:07:35.000000 bitcoin-utils-0.6.1/bitcoinutils/__init__.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5023 2023-01-16 19:50:58.000000 bitcoin-utils-0.6.1/bitcoinutils/bech32.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     2138 2023-05-18 16:04:30.000000 bitcoin-utils-0.6.1/bitcoinutils/constants.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1944 2023-06-02 10:16:41.000000 bitcoin-utils-0.6.1/bitcoinutils/hdwallet.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    41391 2023-05-31 19:26:29.000000 bitcoin-utils-0.6.1/bitcoinutils/keys.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1834 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/bitcoinutils/proxy.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5345 2023-05-30 16:59:52.000000 bitcoin-utils-0.6.1/bitcoinutils/ripemd160.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     6259 2023-05-19 14:21:51.000000 bitcoin-utils-0.6.1/bitcoinutils/schnorr.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    16142 2023-05-23 13:35:16.000000 bitcoin-utils-0.6.1/bitcoinutils/script.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)      966 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/bitcoinutils/setup.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    36448 2023-06-01 14:58:58.000000 bitcoin-utils-0.6.1/bitcoinutils/transactions.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     8345 2023-05-31 19:25:36.000000 bitcoin-utils-0.6.1/bitcoinutils/utils.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/setup.cfg
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1074 2023-06-01 15:38:14.000000 bitcoin-utils-0.6.1/setup.py
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-08-03 11:08:22.447291 bitcoin-utils-0.6.2/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.2/LICENSE
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     7735 2023-08-03 11:08:22.447291 bitcoin-utils-0.6.2/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     7419 2023-08-03 11:05:37.000000 bitcoin-utils-0.6.2/README.rst
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-08-03 11:08:22.443291 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     7735 2023-08-03 11:08:22.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)      535 2023-08-03 11:08:22.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-08-03 11:08:22.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       98 2023-08-03 11:08:22.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2023-08-03 11:08:22.000000 bitcoin-utils-0.6.2/bitcoin_utils.egg-info/top_level.txt
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-08-03 11:08:22.447291 bitcoin-utils-0.6.2/bitcoinutils/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       23 2023-07-14 13:46:57.000000 bitcoin-utils-0.6.2/bitcoinutils/__init__.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5023 2023-01-16 19:50:58.000000 bitcoin-utils-0.6.2/bitcoinutils/bech32.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2168 2023-07-14 13:46:57.000000 bitcoin-utils-0.6.2/bitcoinutils/constants.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2069 2023-07-18 12:29:01.000000 bitcoin-utils-0.6.2/bitcoinutils/hdwallet.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    46633 2023-07-18 08:02:52.000000 bitcoin-utils-0.6.2/bitcoinutils/keys.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1834 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.2/bitcoinutils/proxy.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5345 2023-05-30 16:59:52.000000 bitcoin-utils-0.6.2/bitcoinutils/ripemd160.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     6259 2023-05-19 14:21:51.000000 bitcoin-utils-0.6.2/bitcoinutils/schnorr.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    16126 2023-07-18 08:01:51.000000 bitcoin-utils-0.6.2/bitcoinutils/script.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)      966 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.2/bitcoinutils/setup.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    37553 2023-07-18 08:02:24.000000 bitcoin-utils-0.6.2/bitcoinutils/transactions.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    13325 2023-07-18 08:03:23.000000 bitcoin-utils-0.6.2/bitcoinutils/utils.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2023-08-03 11:08:22.447291 bitcoin-utils-0.6.2/setup.cfg
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1074 2023-06-01 15:38:14.000000 bitcoin-utils-0.6.2/setup.py
```

### Comparing `bitcoin-utils-0.6.1/LICENSE` & `bitcoin-utils-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoin_utils.egg-info/SOURCES.txt` & `bitcoin-utils-0.6.2/bitcoin_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/bech32.py` & `bitcoin-utils-0.6.2/bitcoinutils/bech32.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/constants.py` & `bitcoin-utils-0.6.2/bitcoinutils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 EMPTY_TX_SEQUENCE = b'\x00\x00\x00\x00'
 DEFAULT_TX_SEQUENCE = b'\xff\xff\xff\xff'
 ABSOLUTE_TIMELOCK_SEQUENCE = b'\xfe\xff\xff\xff'
 
 REPLACE_BY_FEE_SEQUENCE = b'\x01\x00\x00\x00'
 
+LEAF_VERSION_TAPSCRIPT = 0xc0
 
 # TX version 2 was introduced in BIP-68 with relative locktime -- tx v1
 # does not support relative locktime
 DEFAULT_TX_VERSION  = b'\x02\x00\x00\x00'
 
 SATOSHIS_PER_BITCOIN = 100000000
 NEGATIVE_SATOSHI = -1
```

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/hdwallet.py` & `bitcoin-utils-0.6.2/bitcoinutils/hdwallet.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,36 +24,37 @@
     hdw : object
         a hdwallet object
     """
 
     def __init__(self, xprivate_key=None, path=None, mnemonic=None):
         """Instantiate a hdwallet object using the corresponding library with BTC"""
 
-        symbo = None
+        symbol = None
         if is_mainnet():
             symbol = BTC
         else:
             symbol = BTCTEST
 
         self.hdw = ext_HDWallet(symbol)
         
         if mnemonic:
             self.from_mnemonic(mnemonic)
 
         if xprivate_key:
             self.from_xprivate_key(xprivate_key, path)
 
 
-
+    # TODO make this a class method, return cls(mnemonic=)
     def from_mnemonic(self, mnemonic: str):
         """Set a mnemonic code for the HD Wallet"""
 
-        self.hdw.from_xprivate_key(mnemonic=mnemonic)
+        self.hdw.from_mnemonic(mnemonic=mnemonic)
 
 
+    # TODO make this a class method, return cls(xprivate_key=, path=)
     def from_xprivate_key(self, xprivate_key: str, path: str):
         """Set an extended private key and optionally the path for the HD Wallet"""
 
         self.hdw.from_xprivate_key(xprivate_key=xprivate_key)
         if path:
             self.hdw.from_path(path=path)
```

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/keys.py` & `bitcoin-utils-0.6.2/bitcoinutils/keys.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,21 +21,18 @@
 from sympy.ntheory import sqrt_mod
 
 from bitcoinutils.constants import NETWORK_WIF_PREFIXES, \
         NETWORK_P2PKH_PREFIXES, NETWORK_P2SH_PREFIXES, SIGHASH_ALL, \
         P2PKH_ADDRESS, P2SH_ADDRESS, P2WPKH_ADDRESS_V0, P2WSH_ADDRESS_V0, \
         P2TR_ADDRESS_V1, NETWORK_SEGWIT_PREFIXES, TAPROOT_SIGHASH_ALL
 from bitcoinutils.setup import get_network
-from bitcoinutils.utils import bytes32_from_int, encode_varint, add_magic_prefix, \
-                               hex_str_to_int, \
-                               tweak_taproot_pubkey, \
-                               tweak_taproot_privkey
 from bitcoinutils.ripemd160 import ripemd160
 from bitcoinutils.schnorr import schnorr_sign
-from bitcoinutils.utils import EcdsaParams
+from bitcoinutils.utils import EcdsaParams, calculate_tweak, bytes32_from_int, add_magic_prefix, \
+                               hex_str_to_int, tweak_taproot_pubkey, tweak_taproot_privkey
 import bitcoinutils.script
 import bitcoinutils.bech32
 
 
 class PrivateKey:
     """Represents an ECDSA private key.
 
@@ -44,46 +41,58 @@
     key : bytes
         the raw key of 32 bytes
 
     Methods
     -------
     from_wif(wif)
         creates an object from a WIF of WIFC format (string)
+    from_bytes()
+        creates an object from raw 32 bytes
     to_wif(compressed=True)
         returns as WIFC (compressed) or WIF format (string)
     to_bytes()
         returns the key's raw bytes
     sign_message(message, compressed=True)
         signs the message's digest and returns the signature
     sign_input(tx, txin_index, script, sighash=SIGHASH_ALL)
-        signs the transaction's digest for a particular index and returns the
-        signature.
+        creates the transaction's digest and signs it for a particular index
+        and returns the signature.
     sign_segwit_input(tx, txin_index, script, amount, sighash=SIGHASH_ALL)
-        signs the transaction's digest for a particular index and amount and 
-        returns the signature.
+        creates the transaction's digest and signs it for a particular index
+        and amount and returns the signature.
+    sign_taproot_input(tx, txin_index, utxo_scripts, amounts, script_path=False, script=None, sighash=TAPROOT_SIGHASH_ALL, tweak=True)
+        creates the transaction's digest and signs it for a particular index
+        input script_pub_keys and amounts and returns the signature. By default
+        it tweaks the keys but it can be disabled for tapleaf scripts.
+    get_taproot_tweak()
+        returns the tweaked private key as a hexadecimal string (classmethod)
     get_public_key()
         returns the corresponding PublicKey object
     """
 
-    def __init__(self, wif=None, secret_exponent=None):
+    def __init__(self, wif=None, secret_exponent=None, b=None):
         """With no parameters a random key is created
 
         Parameters
         ----------
         wif : str, optional
             the key in WIF of WIFC format (default None)
         secret_exponent : int, optional
             used to create a specific key deterministically (default None)
+        b : bytes, optional
+            used to create a key from raw bytes
         """
 
-        if not secret_exponent and not wif:
+        if not secret_exponent and not wif and not b:
             self.key = SigningKey.generate(curve=SECP256k1)
         else:
             if wif:
                 self._from_wif(wif)
+            elif b:
+                self._from_bytes(b)
             elif secret_exponent:
                 self.key = SigningKey.from_secret_exponent(secret_exponent,
                                                            curve=SECP256k1)
 
     def to_bytes(self):
         """Returns key's bytes"""
 
@@ -93,14 +102,28 @@
     @classmethod
     def from_wif(cls, wif):
         """Creates key from WIFC or WIF format key"""
 
         return cls(wif=wif)
 
 
+    @classmethod
+    def from_bytes(cls, b):
+        """Creates key from WIFC or WIF format key"""
+
+        return cls(b=b)
+
+
+    def _from_bytes(self, b):
+        """Creates a key directly from 32 raw bytes"""
+        
+        # TODO check if b is len 32 and raise error
+        self.key = SigningKey.from_string(b, curve=SECP256k1)
+
+
     # expects wif in hex string
     def _from_wif(self, wif):
         """Creates key from WIFC or WIF format key
 
         Check to_wif for the detailed process. From WIF is the reverse.
 
         Raises
@@ -213,32 +236,36 @@
                 if PublicKey.verify_message(address, sig, message):
                     return sig
             except:
                 continue
 
 
     def sign_input(self, tx, txin_index, script, sighash=SIGHASH_ALL):
-        # the tx knows how to calculate the digest for the corresponding
-        # sighash)
+        # get the digest from the transaction object and sign
         tx_digest = tx.get_transaction_digest(txin_index, script, sighash)
         return self._sign_input(tx_digest, sighash)
 
 
     def sign_segwit_input(self, tx, txin_index, script, amount, sighash=SIGHASH_ALL):
-        # the tx knows how to calculate the digest for the corresponding
-        # sighash)
+        # get the digest from the transaction object and sign
         tx_digest = tx.get_transaction_segwit_digest(txin_index, script, amount, sighash)
         return self._sign_input(tx_digest, sighash)
 
 
-    def sign_taproot_input(self, tx, txin_index, utxo_scripts, amounts, sighash=TAPROOT_SIGHASH_ALL):
-        # the tx knows how to calculate the digest for the corresponding
-        # sighash)
-        tx_digest = tx.get_transaction_taproot_digest(txin_index, utxo_scripts, amounts, 0, sighash)
-        return self._sign_taproot_input(tx_digest, sighash)
+    def sign_taproot_input(self, tx, txin_index, utxo_scripts, amounts, script_path=False, tapleaf_script=None,  tapleaf_scripts=None, sighash=TAPROOT_SIGHASH_ALL, tweak=True):
+        # get the digest from the transaction object and sign
+        # note that when signing a tapleaf we typically won't use tweaked 
+        # keys - so tweak should be set to False
+        if script_path:
+            tx_digest = tx.get_transaction_taproot_digest(txin_index, utxo_scripts, 
+                    amounts, 1, script=tapleaf_script, sighash=sighash)
+        else:
+            tx_digest = tx.get_transaction_taproot_digest(txin_index, utxo_scripts, 
+                    amounts, 0, sighash=sighash)
+        return self._sign_taproot_input(tx_digest, sighash, tapleaf_scripts, tweak)
 
 
     def _sign_input(self, tx_digest, sighash=SIGHASH_ALL):
         """Signs a transaction input with the private key
 
         Bitcoin uses the normal DER format for transactions. Each input is
         signed separately (thus txin_index is required). The script of the
@@ -258,15 +285,15 @@
         # nonces (RFC6979 - deterministic nonce generation).
         #
         # https://bitcoin.stackexchange.com/questions/88702/why-is-a-librarys-
         # signature-of-a-segwit-tx-different-from-bitcoin-core-signatur
         #
         # For this reason we test if we get a Low R value (should be <0x80 and
         # thus not have the 0x00 prefix that specifies a negative signed
-        # number) we need to change the entropy by using extra_entropy and resign
+        # number) we need to change the entropy by using extra_entropy and re-sign
         # until we get a Low R value.
 
         # sign - note that deterministic signing is used
         signature = self.key.sign_digest_deterministic(tx_digest,
                                                        sigencode=sigencode_der,
                                                        hashfunc=hashlib.sha256)
 
@@ -339,49 +366,98 @@
 
         # note that this is the final sig that needs to be added in the
         # script_sig (i.e. the DER signature plus the sighash)
         return hexlify(signature).decode('utf-8')
 
 
 
-    def _sign_taproot_input(self, tx_digest, sighash=SIGHASH_ALL):
+    # TODO add all_scripts to proper tweaking
+    def _sign_taproot_input(self, tx_digest, sighash=SIGHASH_ALL, scripts=None, tweak=True):
         """Signs a taproot transaction input with the private key
 
         Taproot uses Schnorr signatures. The format is just R and S so only
         64 bytes. If SIGHASH_ALL then nothing is included (i.e. default).
         If another sighash then it is included in the end (65 bytes).
 
+        Note that when signing for script path (tapleafs) we typically won't 
+        use tweaking so tweak should be set to False
+
         Returns a signature for that input
         """
 
-        # tweak private key before signing (tweaking code takes care of
-        # negating the private key if it is necessary (i.e. if
-        # the corresponding public key's y is odd).
-        tagged_key = tweak_taproot_privkey(self.key.to_string(), 'TapTweak')
+        byte_key = None
 
-        byte_key = unhexlify(tagged_key)
+        if tweak:
+            tweak_int = calculate_tweak(self.get_public_key(), scripts)
+            byte_key = tweak_taproot_privkey(self.key.to_string(), tweak_int)
+        else:
+            # negating the private key is not necessary since the schnorr lib
+            # is handling it
+            #negated_key = self.get_negated_key()
+            #byte_key = bytes.fromhex(negated_key)
+            byte_key = self.key.to_string()
 
-        # deterministic signing nonce is random and based in RFC6979
+        # deterministic signing nonce is random and RFC6979-like
         # it is the hash of the tx_digest and private key
         # TODO not identical to Bitcoin Core's signature, rand_aux
-        # needs slight changes if we want identical signatures!
+        # needs to change if we want identical signatures!
         rand_aux = hashlib.sha256(tx_digest + byte_key).digest()
 
         # use BIP-340 python's reference implementation for signing
         sig = schnorr_sign(tx_digest, byte_key, rand_aux)
 
         # 65 bytes if sighash is not TAPROOT_SIGHASH_ALL
         if sighash != TAPROOT_SIGHASH_ALL:
             sig += sighash.to_bytes(1, 'big')
 
         sig_hex = hexlify(sig)
         
         return sig_hex 
 
 
+#    def get_negated_key(self):
+#        """Checks if corresponding public is has odd y and negates"""
+#
+#        key_secret_exponent = hex_str_to_int(self.key.to_string().hex())
+#
+#        pubkey = self.get_public_key()
+#
+#        if not pubkey.is_y_even():
+#            # negate private key
+#            key_secret_exponent = EcdsaParams._order - key_secret_exponent
+#
+#        return hex(key_secret_exponent)[2:]
+
+
+#    @classmethod
+#    def get_taproot_tweak(self, internal_key: str, negated_privkey: str, script: object) -> str:
+#        """Returns a tweaked private key as a hexadecimal string.
+#
+#        TODO cleanup: we pass internal_key because the pubkey_x_bytes used to tweak
+#        should be from the internal key!
+#
+#        Assumes that the key is already negated, if necessary. (privkey is the negated one)
+#        """
+#
+#        # could also use the PrivateKey object to get pubkey_x_bytes
+#        internal_pubkey_bytes = full_pubkey_gen(bytes.fromhex(internal_key))
+#        #pubkey_x_bytes = pubkey_bytes[:32]
+#        internal_pubkey = PublicKey( '04' + internal_pubkey_bytes.hex() )
+#
+#        tweak_int = calculate_tweak( internal_pubkey, script )
+#
+#        # privkey is already negated
+#        key_secret_exponent = hex_str_to_int(negated_privkey)
+#
+#        tweaked_privkey_int = (key_secret_exponent + tweak_int) % EcdsaParams._order
+#
+#        #print(f'Tweaked Private Key: {tweaked_privkey_int:064x}')
+#        return f'{tweaked_privkey_int:064x}'
+
+ 
 
     def get_public_key(self):
         """Returns the corresponding PublicKey"""
 
         verifying_key = hexlify(self.key.get_verifying_key().to_string())
         return PublicKey( '04' + verifying_key.decode('utf-8') )
 
@@ -394,36 +470,42 @@
     ----------
     key : bytes
         the raw public key of 64 bytes (x, y coordinates of the ECDSA curve)
 
     Methods
     -------
     from_hex(hex_str)
-        creates an object from a hex string in SEC format
+        creates an object from a hex string in SEC format (classmethod)
     from_message_signature(signature)
-        NO-OP!
-    verify_message(address, signature, message)
-        Class method that constructs the public key, confirms the address and
-        verifies the signature
+        NO-OP! (classmethod)
+    verify_message(address, signature, message) (classmethod)
+        constructs the public key, confirms the address and
+        verifies the signature (classmethod)
     verify(signature, message)
         returns true if the message was signed with this public key's
         corresponding private key.
     to_hex(compressed=True)
         returns the key as hex string (in SEC format - compressed by default)
-    to_taproot_hex()
-        returns the x coordinate only as hex string (needed for taproot)
+    to_x_only_hex(script)
+        returns the x coordinate only as hex string before tweaking (needed for taproot)
+    to_taproot_hex(script)
+        returns the x coordinate only as hex string after tweaking (needed for taproot)
+    is_y_even()
+        returns true if y coordinate is even
+    get_taproot_tweak()
+        returns the tweaked public key as a hexadecimal string (classmethod)
     to_bytes()
         returns the key's raw bytes
     to_hash160()
         returns the hash160 hex string of the public key
     get_address(compressed=True))
         returns the corresponding P2pkhAddress object
     get_segwit_address()
         returns the corresponding P2wpkhAddress object
-    get_taproot_address()
+    get_taproot_address(scripts)
         returns the corresponding P2trAddress object
     """
 
 
     def __init__(self, hex_str):
         """
         Parameters
@@ -433,14 +515,15 @@
 
         Raises
         ------
         TypeError
             If first byte of public key (corresponding to SEC format) is
             invalid.
         """
+        # TODO accepts hex str in any format and handle here!
 
         # expects key as hex string - SEC format
         first_byte_in_hex = hex_str[:2] # 2 since a byte is represented by 2 hex characters
         hex_bytes = unhexlify(hex_str)
         # TODO needed?? - see flag below
         taproot = False 
 
@@ -513,29 +596,91 @@
         else:
             # uncompressed starts with 04
             key_str = b'04' + key_hex
 
         return key_str.decode('utf-8')
 
 
-    # TODO probably remove tagged flag in the future to always tag the public key
-    # Note that we do not optionally tag the private key when signing!!!
-    def to_taproot_hex(self, tagged=True):
-        """Returns the x coordinate of the public key as a hex string.
+    def to_x_only_hex(self):
+        """Returns the x coordinate of the public key as hex string."""
+
+        key_hex = self.key.to_string().hex()
+        return key_hex[:64]
 
-        Tweaks and negates, if necessary, the key first.
+
+
+    def to_taproot_hex(self, scripts=None):
+        """Returns the tweaked x coordinate of the public key as a hex string.
+
+        Parameters
+        ==========
+        scripts : list[ list[Script] ]
+            a list of list of Scripts describing the merkle tree of scripts to commit
         """
-        if tagged:
-            # public key in x form only (TODO pass x-only for here rather than
-            # do it from tweak_taproot_pubkey!?)
-            pubkey = tweak_taproot_pubkey(self.key.to_string(), 'TapTweak')[:64]
-        else:
-            pubkey = self.to_hex(compressed=True)[2:]
 
-        return pubkey
+        # Tweak public key (BIP340)
+        # https://bitcoin.stackexchange.com/a/116391/31844
+        tweak_int = calculate_tweak(self, scripts)
+
+        # keep x-only coordinate
+        pubkey = tweak_taproot_pubkey(self.key.to_string(), tweak_int)[:32]
+        
+        return pubkey.hex()
+
+
+    def is_y_even(self):
+        """Returns True if the y coordinate of the public key is even and False otherwise."""
+        
+        key_hex = self.key.to_string().hex()
+
+        y = hex_str_to_int( key_hex[64:] )
+
+        return y % 2 == 0
+
+
+#    def get_negated_key(self):
+#        """Returns a negated hexadecimal string of the public key or just the key if already a key with even y (i.e. key that starts with 02 pre-taproot)."""
+#        
+#        key_hex = self.key.to_string().hex()
+#
+#        x = hex_str_to_int( key_hex[:64] )
+#        y = hex_str_to_int( key_hex[64:] )
+#
+#        # if y is odd then negate y (effectively P) to make it even and equivalent
+#        # to a 02 compressed pk
+#        if y % 2 != 0:
+#            y = EcdsaParams._field - y
+#
+#        #print(f'{x:064x}{y:064x}')
+#        return f'{x:064x}{y:064x}'
+
+
+#    @classmethod
+#    def get_taproot_tweak(self, internal_pubkey: str, negated_pubkey: str,
+#                          script: object) -> str:
+#        # TODO CLEAN
+#        """Returns a tweaked public key as a hexadecimal string.
+#
+#        Assumes that the key is already negated, if necessary.
+#        """
+#        
+#        pub_key = PublicKey( '04' + internal_pubkey )
+#
+#        # calculate tweak
+#        tweak_int = calculate_tweak( pub_key, script )
+#
+#        # convert public key bytes to tuple Point
+#        P = (hex_str_to_int(negated_pubkey[:64]), 
+#             hex_str_to_int(negated_pubkey[64:]))
+#
+#        # calculated tweaked public key Q = P + th*G
+#        Q = point_add(P, (point_mul(G, tweak_int)))
+#
+#        #print(f'Tweaked Public Key: {Q[0]:064x}{Q[1]:064x}')
+#        return f'{Q[0]:064x}{Q[1]:064x}'
 
 
     @classmethod
     def from_message_signature(self, signature):
         # TODO implement (add signature=None in __init__, etc.)
         # TODO plus does this apply to DER signatures as well?
         #return cls(signature=signature)
@@ -677,25 +822,25 @@
         address.
         """
         hash160 = self._to_hash160(True)
         addr_string_hex = hexlify(hash160).decode('utf-8')
         return P2wpkhAddress(witness_program=addr_string_hex)
 
 
-    def get_taproot_address(self):
+    def get_taproot_address(self, scripts=None):
         """Returns the corresponding P2TR address
 
         Only compressed is allowed. Taproot uses x-only public key with
         even y (02 compressed keys). By default tagged_hashes are used.
+
+        scripts contains the list of lists of Scripts describing the merkle
+        tree
         """
 
-        # Tweak public key (BIP340)
-        # https://bitcoin.stackexchange.com/a/116391/31844
-        # note that taproot's even y is checked/negated during tweaking
-        pubkey = tweak_taproot_pubkey(self.key.to_string(), 'TapTweak')[:64]
+        pubkey = self.to_taproot_hex(scripts)
 
         return P2trAddress(witness_program=pubkey)
 
 
 class Address(ABC):
     """Represents a Bitcoin address
 
@@ -1188,14 +1333,12 @@
 
 
     def get_type(self):
         """Returns the type of address"""
         return self.version
 
 
-
-
 def main():
     pass
 
 if __name__ == "__main__":
     main()
```

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/proxy.py` & `bitcoin-utils-0.6.2/bitcoinutils/proxy.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/ripemd160.py` & `bitcoin-utils-0.6.2/bitcoinutils/ripemd160.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/schnorr.py` & `bitcoin-utils-0.6.2/bitcoinutils/schnorr.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/script.py` & `bitcoin-utils-0.6.2/bitcoinutils/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
 # propagated, or distributed except according to the terms contained in the
 # LICENSE file.
 
 import struct
 import copy
 import hashlib
-from bitcoinutils.utils import prepend_varint, to_bytes, vi_to_int
+from bitcoinutils.utils import to_bytes, vi_to_int
 from binascii import unhexlify, hexlify
 
 import bitcoinutils.keys
 
 
 # Bitcoin's op codes. Complete list at: https://en.bitcoin.it/wiki/Script
 OP_CODES = {
```

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/setup.py` & `bitcoin-utils-0.6.2/bitcoinutils/setup.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/transactions.py` & `bitcoin-utils-0.6.2/bitcoinutils/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 import math
 import hashlib
 import struct
 from binascii import unhexlify, hexlify
 
 from bitcoinutils.constants import DEFAULT_TX_SEQUENCE, DEFAULT_TX_LOCKTIME, \
-                    DEFAULT_TX_VERSION, NEGATIVE_SATOSHI, \
+                    DEFAULT_TX_VERSION, NEGATIVE_SATOSHI, LEAF_VERSION_TAPSCRIPT, \
                     EMPTY_TX_SEQUENCE, SIGHASH_ALL, SIGHASH_NONE, \
                     SIGHASH_SINGLE, SIGHASH_ANYONECANPAY, TAPROOT_SIGHASH_ALL, \
                     ABSOLUTE_TIMELOCK_SEQUENCE, REPLACE_BY_FEE_SEQUENCE, \
                     TYPE_ABSOLUTE_TIMELOCK, TYPE_RELATIVE_TIMELOCK, \
-                    TYPE_REPLACE_BY_FEE, SATOSHIS_PER_BITCOIN
+                    TYPE_REPLACE_BY_FEE
 from bitcoinutils.script import Script
 from bitcoinutils.utils import to_bytes, vi_to_int, encode_varint, \
         tagged_hash, prepend_varint
 
 class TxInput:
     """Represents a transaction input.
 
@@ -763,41 +763,44 @@
 
         return hashlib.sha256(hashlib.sha256(tx_for_signing).digest()).digest()
 
 
 
     # TODO Update doc with TAPROOT_SIGHASH_ALL
     # clean prints after finishing other sighashes
-    def get_transaction_taproot_digest(self, txin_index, script_pubkeys, amounts, ext_flag=0, sighash=TAPROOT_SIGHASH_ALL):
+    def get_transaction_taproot_digest(self, txin_index, script_pubkeys, amounts, ext_flag=0, script=Script([]), leaf_ver=LEAF_VERSION_TAPSCRIPT, sighash=TAPROOT_SIGHASH_ALL):
         """Returns the segwit v1 (taproot) transaction's digest for signing.
            https://github.com/bitcoin/bips/blob/master/bip-0341.mediawiki
            Also consult Bitcoin Core code at: https://github.com/bitcoin/bitcoin/blob/29c36f070618ea5148cd4b2da3732ee4d37af66b/src/script/interpreter.cpp#L1478
-           And: https://github.com/bitcoinops/taproot-workshop/blob/1d90851b8301fa4ac7469b9027f5ab543a67f269/test_framework/script.py#L730   (note, fields' order is old/wrong in this one)
+           And: https://github.com/bitcoin/bitcoin/blob/b5f33ac1f82aea290b4653af36ac2ad1bf1cce7b/test/functional/test_framework/script.py
 
                 |  SIGHASH types (see constants.py):
-                |      SIGHASH_ALL - signs all inputs and outputs (default)
+                |      TAPROOT_SIGHASH_ALL - signs all inputs and outputs (default)
+                |      SIGHASH_ALL - signs all inputs and outputs
                 |      SIGHASH_NONE - signs all of the inputs
                 |      SIGHASH_SINGLE - signs all inputs but only txin_index output
                 |      SIGHASH_ANYONECANPAY (only combined with one of the above)
                 |      - with ALL - signs all outputs but only txin_index input
                 |      - with NONE - signs only the txin_index input
                 |      - with SINGLE - signs txin_index input and output
 
                 Attributes
                 ----------
                 txin_index : int
                     The index of the input that we wish to sign
-                script : list (string)
-                    The scriptCode (template) that corresponds to the segwit
-                    transaction output type that we want to spend
-                amount : int/float/Decimal
-                    The amount of the UTXO to spend is included in the
-                    signature for segwit (in satoshis)
+                script_pubkeys : list (string)
+                    The scriptPubkeys that correspond to all the inputs/UTXOs
+                amounts : int/float/Decimal
+                    The amounts that correspond to all the inputs/UTXOs
                 ext_flag : int
-                    Extension mechanism, default is 0; 1 is for BIP342
+                    Extension mechanism, default is 0; 1 is for script spending (BIP342)
+                script : Script object
+                    The script that we are spending (ext_flag=1)
+                leaf_ver : int
+                    The script version, LEAF_VERSION_TAPSCRIPT for the default tapscript
                 sighash : int
                     The type of the signature hash to be created
         """
 
         # clone transaction to modify without messing up the real transaction
         # tmp_tx is not really used for its to_bytes() here
         # TODO we could use self directly to access fields
@@ -869,15 +872,16 @@
                                 struct.pack('B', len(script_bytes)) + \
                                 script_bytes
             hash_outputs = hashlib.sha256(hash_outputs).digest()
             tx_for_signing += hash_outputs
 
 
         # Data about this input
-        spend_type = ext_flag * 2 + 0      # hard-coded annex_present
+        spend_type = ext_flag * 2 + 0      # 0 for hard-coded - no annex_present
+
         tx_for_signing += bytes([spend_type])
 
         if anyone_can_pay:
             #print('3')
             txin = tmp_tx.inputs[txin_index]
             # convert txid to big-endian first
             tx_for_signing += unhexlify(txin.txid)[::-1] + \
@@ -891,26 +895,41 @@
 
             tx_for_signing += txin.sequence
         else:
             #print('4')
             tx_for_signing += txin_index.to_bytes(4, 'little')
 
         # TODO if annex is present it should be added here
+        # length of annex should use prepend_varint (compact_size)
 
         # Data about this output
         if sighash_single:
             #print('5')
             txout = tmp_tx.outputs[txin_index]
             amount_bytes = struct.pack('<Q', txout.amount)
             script_bytes = txout.script_pubkey.to_bytes()
             hash_output = amount_bytes + struct.pack('B', len(script_bytes)) + \
                               script_bytes
             tx_for_signing += hashlib.sha256(hash_output).digest()
 
-        # tagged hash the digest and return
+        if ext_flag == 1:    # script spending path (Signature Message Extension BIP-342)
+            # committing the tapleaf hash - makes it safe to reuse keys for separate
+            # scripts in the same output
+            leaf_ver = LEAF_VERSION_TAPSCRIPT   # pass as a parameter if a new version comes
+            tx_for_signing += tagged_hash(bytes([leaf_ver]) + prepend_varint(script.to_bytes()),
+                                          "TapLeaf").digest()
+
+            # key version - type of public key used for this signature, currently only 0
+            tx_for_signing += bytes([0])
+
+            # code separator position - records position of when the last OP_CODESEPARATOR 
+            # was executed; not supported for now, we always use 0xffffffff
+            tx_for_signing += b'\xff\xff\xff\xff'
+
+        # tag hash the digest and return
         return tagged_hash(tx_for_signing, "TapSighash").digest()
 
 
 
     def to_bytes(self, has_segwit):
         """Serializes to bytes"""
```

### Comparing `bitcoin-utils-0.6.1/bitcoinutils/utils.py` & `bitcoin-utils-0.6.2/bitcoinutils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # directory of this distribution.
 #
 # No part of python-bitcoin-utils, including this file, may be copied, modified,
 # propagated, or distributed except according to the terms contained in the
 # LICENSE file.
 
 import hashlib
-from binascii import hexlify, unhexlify
+from binascii import hexlify
 from ecdsa import ellipticcurve
-from bitcoinutils.constants import SATOSHIS_PER_BITCOIN
+from bitcoinutils.constants import SATOSHIS_PER_BITCOIN, LEAF_VERSION_TAPSCRIPT
 from bitcoinutils.schnorr import full_pubkey_gen, point_add, point_mul, G
 
 
 # TODO rename to Secp256k1Params and clean whatever is not used!
 class EcdsaParams:
     # ECDSA curve using secp256k1 is defined by: y**2 = x**3 + 7
     # This is done modulo p which (secp256k1) is:
@@ -45,19 +45,116 @@
     # The generator base point is:
     # Note that we could get that from ecdsa lib, e.g.:
     # SECP256k1.__dict__['generator']
     _G = ellipticcurve.Point( _curve, _Gx, _Gy, _order )
 
 
 
+class ControlBlock:
+    '''Represents a control block for spending a taproot script path
+
+    Attributes
+    ----------
+    pubkey : PublicKey
+        the internal public key object
+    script_to_spend : Script
+        the tapscript leaf that we want to spend
+    scripts : list[ list[Script] ]
+        a list of list of Scripts describing the merkle tree of scripts to commit
+
+    Methods
+    -------
+    to_bytes()
+        returns the control block as bytes
+    to_hex()
+        returns the control block as a hexadecimal string
+    '''
+
+
+    # TODO TEMP scripts is just the top root th_branch manually calculated!
+    def __init__(self, pubkey, script_to_spend=None, scripts=None):
+        '''
+        Parameters
+        ----------
+        pubkey : PublicKey
+            the internal public key object
+        script_to_spend : Script (ignored for now)
+            the tapscript leaf that we want to spend
+        scripts : bytes
+            concatenated path (leafs/branches) hashes in bytes
+        '''
+        self.pubkey = pubkey
+        # script_to_spend is ignored for now - needed for automatically
+        # constructing the merkle path
+        self.script_to_spend = script_to_spend
+        self.scripts = scripts
+
+
+    def to_bytes(self):
+        leaf_version = bytes([LEAF_VERSION_TAPSCRIPT])
+
+        # x-only public key is required
+        pub_key = bytes.fromhex( self.pubkey.to_x_only_hex() )
+
+        merkle_path = b''
+
+        # get merkle path from scripts, if any
+        # TODO currently the manually constructed merkle path is passed
+        if self.scripts:
+            merkle_path = self.scripts # manually constructed path
+        
+        return leaf_version + pub_key + merkle_path
+
+
+    def to_hex(self):
+        """Converts object to hexadecimal string"""
+
+        return hexlify(self.to_bytes()).decode('utf-8')
+
+
+def get_tag_hashed_merkle_root(scripts):
+    '''Tag hashed merkle root of all scripts - tag hashes tapleafs and branches
+    as needed.
+
+    Scripts is a list of list of Scripts describing the merkle tree of scripts to commit
+    Example of scripts' list:  [ [A, B], C ] 
+    '''
+    # TODO raise errors
+
+    # empty scripts or empty list
+    if not scripts:
+        return b''
+    #print('1')
+    # if not list return tapleaf_hash of Script
+    if not isinstance(scripts, list):
+        #print('2')
+        return tapleaf_tagged_hash(scripts)
+    # list
+    else:
+        if len(scripts) == 0:
+            #print('3')
+            return b''
+        elif len(scripts) == 1:
+            #print('4')
+            return get_tag_hashed_merkle_root(scripts[0])
+        elif len(scripts) == 2:
+            #print('5')
+            left = get_tag_hashed_merkle_root(scripts[0])
+            right = get_tag_hashed_merkle_root(scripts[1])
+            return tapbranch_tagged_hash(left, right)
+        else:
+            # TODO throw exception
+            exit('List cannot have more than 2 branches.')
+
+
 def to_satoshis(num):
     '''
     Converts from any number type (int/float/Decimal) to satoshis (int)
     '''
-    # we need to round because of how floats are stored insternally:
+    # we need to round because of how floats are stored internally:
     # e.g. 0.29 * 100000000 = 28999999.999999996
     return int( round(num * SATOSHIS_PER_BITCOIN) )
 
 
 def prepend_varint(data):
     '''
     Counts bytes and returns them with their varint (or compact size) prepended.
@@ -180,73 +277,139 @@
     Returns hashlib object (can then use .digest() or hexdigest())
     '''
 
     tag_digest = hashlib.sha256(tag.encode()).digest()
     return hashlib.sha256( tag_digest + tag_digest + data )
 
 
-# TODO script also needs to be passed when spending with script
-# since it is part of the calculation
-def tweak_taproot_pubkey(pubkey: bytes, tweak: str) -> str:
+def calculate_tweak(pubkey: object, scripts: object) -> int:
     '''
-    Tweaks the public key with the specified tweak. Required to create the
-    taproot public key from the internal key.
+    Calculates the tweak to apply to the public and private key when required.
     '''
 
     # only the x coordinate is tagged_hash'ed
-    # TODO if also script spending this should include the script!)
-    th = tagged_hash(pubkey[:32], tweak)
+    key_x = pubkey.to_bytes()[:32]
+
+    if not scripts:
+        tweak = tagged_hash(key_x, 'TapTweak')
+    else:
+        # if also script spending this should include the tapleaf of the versioned script!
+        merkle_root = get_tag_hashed_merkle_root(scripts)
+        tweak = tagged_hash(key_x + merkle_root, 'TapTweak')
+
     # we convert to int for later elliptic curve  arithmetics
-    th_as_int = hex_str_to_int( th.hexdigest() )
+    tweak_int = hex_str_to_int( tweak.hexdigest() )
+
+    return tweak_int
+
+
+def tapleaf_tagged_hash(script: object) -> bytes:
+    '''Calculates the tagged hash for a tapleaf'''
+    script_part = bytes([LEAF_VERSION_TAPSCRIPT]) + prepend_varint(script.to_bytes())
+    return tagged_hash(script_part, 'TapLeaf').digest()
+
+
+def tapbranch_tagged_hash(thashed_a: bytes, thashed_b: bytes) -> bytes:
+    '''Calculates the tagged hash for a tapbranch'''
+    # order - smaller left side
+    if thashed_a < thashed_b:
+        return tagged_hash(thashed_a + thashed_b, 'TapBranch').digest()
+    else:
+        return tagged_hash(thashed_b + thashed_a, 'TapBranch').digest()
+
+
+def negate_privkey(key: bytes) -> str:
+    '''Negate private key, if necessary'''
+
+    # get the public key from BIP-340 schnorr ref impl.
+    internal_pubkey_bytes = full_pubkey_gen(key)
+    pubkey_hex = internal_pubkey_bytes.hex()
+
+    # negate private key if necessary
+    if int(pubkey_hex[64:], 16) % 2 == 0:
+        negated_key = hex_str_to_int(key.hex())
+    else:
+        key_secret_exponent = hex_str_to_int(key.hex())
+        # negate private key
+        negated_key = EcdsaParams._order - key_secret_exponent
+
+    return f'{negated_key:064x}'
+
+
+#def negate_pubkey(key: bytes) -> str:
+#    '''Negate public key, if necessary'''
+#
+#    # convert public key bytes to tuple Point
+#    x = hex_str_to_int( key[:32].hex() )
+#    y = hex_str_to_int( key[32:].hex() )
+#
+#    # negate public key if necessary
+#    if y % 2 != 0:
+#        y = EcdsaParams._field - y
+#
+#    return f'{x:064x}{y:064x}'
+
+
+def tweak_taproot_pubkey(internal_pubkey: bytes, tweak: int) -> bytes:
+    '''
+    Tweaks the public key with the specified tweak. Required to create the
+    taproot public key from the internal key.
+    '''
+
+    # calculate tweak
+    #tweak_int = calculate_tweak( internal_pubkey, script )
 
     # convert public key bytes to tuple Point
-    x = hex_str_to_int( pubkey[:32].hex() )
-    y = hex_str_to_int( pubkey[32:].hex() )
-    P = (x, y)
+    x = hex_str_to_int( internal_pubkey[:32].hex() )
+    y = hex_str_to_int( internal_pubkey[32:].hex() )
 
-    # if y is odd then negate y (effectively P) to make it even and equiv
+    # if y is odd then negate y (effectively P) to make it even and equivalent
     # to a 02 compressed pk
     if y % 2 != 0:
         y = EcdsaParams._field - y 
-
     P = (x, y)
 
-    # calculated tweaked public key Q = P + th*G
-    Q = point_add(P, (point_mul(G, th_as_int)))
+    # apply tweak to public key (Q = P + th*G)
+    Q = point_add(P, (point_mul(G, tweak)))
+    #Q = point_add(P, (point_mul(G, tweak_int)))
     
-    return f'{Q[0]:064x}{Q[1]:064x}'
+    # negate Q as well before returning ?!?
+    if Q[1] % 2 != 0:
+        Q = ( Q[0], EcdsaParams._field - Q[1] )
+
+    #print(f'Tweaked Public Key: {Q[0]:064x}{Q[1]:064x}')
+    return bytes.fromhex( f'{Q[0]:064x}{Q[1]:064x}' )
 
 
-def tweak_taproot_privkey(privkey: bytes, tweak: str) -> str:
+def tweak_taproot_privkey(privkey: bytes, tweak: int) -> bytes:
     '''
     Tweaks the private key before signing with it. Check if public key's y
     is even and negate the private key before tweaking if it is not.
     '''
-    key_secret_exponent = int(hexlify(privkey).decode('utf-8'), 16)
 
-    # get the private key from BIP-340 schnorr ref impl.
-    pubkey_bytes = full_pubkey_gen(privkey)
-    pubkey_x_bytes = pubkey_bytes[:32]
-    pubkey_y_int = int.from_bytes(pubkey_bytes[32:], byteorder="big")
+    # get the public key from BIP-340 schnorr ref impl.
+    internal_pubkey_bytes = full_pubkey_gen(privkey)
 
-    # if y coordinate is not even, negate private key
-    if pubkey_y_int % 2 != 0:
-        # negate private key
-        key_secret_exponent = EcdsaParams._order - key_secret_exponent
+    #tweak_int = calculate_tweak( internal_pubkey_bytes, script )
 
-    # tag hash the public key (bytes)
-    th = tagged_hash(pubkey_x_bytes, tweak)
-    th_as_int = hex_str_to_int( th.hexdigest() )
+    internal_pubkey_hex = internal_pubkey_bytes.hex()
+
+    # negate private key if necessary
+    if int(internal_pubkey_hex[64:], 16) % 2 == 0:
+        negated_key = privkey.hex()
+    else:
+        negated_key = negate_privkey(privkey)
 
     # The tweaked private key can be computed by d + hash(P || S)
     # where d is the normal private key, P is the normal public key
     # and S is the alt script, if any (empty script, if none?? TODO)
-    tweaked_privkey_int = (key_secret_exponent + th_as_int) % EcdsaParams._order
+    tweaked_privkey_int = (hex_str_to_int(negated_key) + tweak) % EcdsaParams._order
 
-    return hex(tweaked_privkey_int)[2:]
+    #print(f'Tweaked Private Key:', hex(tweaked_privkey_int)[2:])
+    return bytes.fromhex( f'{tweaked_privkey_int:064x}' )
 
 
 
 # TODO are these required - maybe bytestoint and inttobytes are only required?!?
 def hex_str_to_int(hex_str):
     '''
     Converts a string hexadecimal to a number
```

### Comparing `bitcoin-utils-0.6.1/setup.py` & `bitcoin-utils-0.6.2/setup.py`

 * *Files identical despite different names*

