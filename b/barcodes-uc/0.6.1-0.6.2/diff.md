# Comparing `tmp/barcodes_uc-0.6.1.tar.gz` & `tmp/barcodes_uc-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcodes_uc-0.6.1.tar", max compression
+gzip compressed data, was "barcodes_uc-0.6.2.tar", max compression
```

## Comparing `barcodes_uc-0.6.1.tar` & `barcodes_uc-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       81 2023-07-27 08:53:47.149695 barcodes_uc-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.6.1/barcodes_uc/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.6.1/barcodes_uc/barcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.6.1/barcodes_uc/barcodes/__main__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.6.1/barcodes_uc/qrcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:23.049740 barcodes_uc-0.6.1/barcodes_uc/qrcodes/__main__.py
--rw-r--r--   0        0        0    13170 2023-07-30 17:06:37.851607 barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrgenerator.py
--rw-r--r--   0        0        0    40363 2023-07-30 07:58:05.620515 barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrutils.py
--rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.6.1/data/GF256.csv
--rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.6.1/data/alignment_locations.csv
--rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.6.1/data/capabilities.csv
--rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.6.1/data/error_correction_table.csv
--rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.6.1/data/format_table.csv
--rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.6.1/data/version_table.csv
--rw-r--r--   0        0        0      442 2023-07-31 21:52:02.948955 barcodes_uc-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10174 2023-07-30 21:54:01.391050 barcodes_uc-0.6.1/requirements.txt
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 barcodes_uc-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1154 2023-08-02 07:23:12.167972 barcodes_uc-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.6.2/barcodes_uc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.6.2/barcodes_uc/barcodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.6.2/barcodes_uc/barcodes/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.6.2/barcodes_uc/qrcodes/__init__.py
+-rw-r--r--   0        0        0     1983 2023-08-03 10:12:15.529960 barcodes_uc-0.6.2/barcodes_uc/qrcodes/__main__.py
+-rw-r--r--   0        0        0    15074 2023-08-03 10:45:48.988272 barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrgenerator.py
+-rw-r--r--   0        0        0    51328 2023-08-03 10:06:59.755532 barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrutils.py
+-rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.6.2/data/GF256.csv
+-rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.6.2/data/alignment_locations.csv
+-rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.6.2/data/capabilities.csv
+-rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.6.2/data/error_correction_table.csv
+-rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.6.2/data/format_table.csv
+-rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.6.2/data/version_table.csv
+-rw-r--r--   0        0        0      647 2023-08-03 10:49:18.185011 barcodes_uc-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    10174 2023-07-30 21:54:01.391050 barcodes_uc-0.6.2/requirements.txt
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 barcodes_uc-0.6.2/PKG-INFO
```

### Comparing `barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrgenerator.py` & `barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrgenerator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 #imports
 from . import qrutils
 from PIL import Image
 import numpy as np
 from enum import Enum
+# from aenum import extend_enum, Enum
 
 finderPattern = [
     [1,1,1,1,1,1,1],
     [1,0,0,0,0,0,1],
     [1,0,1,1,1,0,1],
     [1,0,1,1,1,0,1],
     [1,0,1,1,1,0,1],
@@ -25,29 +26,53 @@
 
 #White and black background colors
 class ModuleColors:
     WHITE = '\x1b[0;37;47m'
     BLACK = '\x1b[0;30;40m'
     RESET = '\x1b[0m'
 
+class NewColour:
+    def __init__(self, name, rgb: list[float]) -> None:
+        if len(rgb) != 3:
+            raise ValueError("RGB list must have 3 values")
+        for i in rgb:
+            if i < 0 or i > 1:
+                raise ValueError("RGB values must be in range [0-1]")
+        
+        self.value = rgb
+        self.name = name
+
 #Colour class to save qr code as an image with colour
 class QRColour(Enum):
     black = [0, 0, 0]
     red = [1, 0, 0]
     green = [0, 1, 0]
     blue = [0, 0, 1]
     yellow = [1, 1, 0]
     cyan = [0, 1, 1]
     magenta = [1, 0, 1]
     white = [1, 1, 1]
 
+    @classmethod
+    def new_colour(cls, name, rgb: list[float]):
+        if len(rgb) != 3:
+            raise ValueError("RGB list must have 3 values")
+        for i in rgb:
+            if i < 0 or i > 1:
+                raise ValueError("RGB values must be in range [0-1]")
+        
+        return NewColour(name, rgb)
+
 class QR:
-    def __init__(self, version: qrutils.QRVersion = qrutils.QRVersion.v1) -> None:
+    def __init__(self, encoding: qrutils.QREncoding, message: str, error_correction: qrutils.QRErrorCorrectionLevels, version: qrutils.QRVersion = qrutils.QRVersion.v1) -> None:
         self.size = qrutils.qr_size(version)
         self.version = version
+        self.encoding = encoding
+        self.message = message
+        self.error_correction = error_correction
         self.matrix = [['X' for i in range(self.size)] for j in range(self.size)]
         self.reserved_positions = [[0 for i in range(self.size)] for j in range(self.size)]
 
     # def set_size(self, size: int):
     #     self.size = size
     #     self.matrix = [[0 for i in range(size)] for j in range(size)]
 
@@ -169,15 +194,15 @@
 
         #interleave data blocks and error correction blocks if necessary
         interleavedData = qrutils.interleave_blocks(rawData['dataBytes'], rawData['ErrorCorrection'], self.version)
         #Join the interleaved data blocks into one string
         interleavedData = ''.join(interleavedData)
 
         #Place the modules and function patterns in the matrix
-        qr = QR(version=self.version)
+        qr = QR(version=self.version, encoding=self.encoding, message=self.msg, error_correction=self.error_correction)
         # print(qr)
 
         #1 - Place the finder patterns, at (0,0), (0, qr.size - 7), (qr.size - 7, 0)
         #(0,0)
         for posx,row in enumerate(finderPattern):
             for posy,col in enumerate(row):
                 qr.matrix[posx][posy] = col
@@ -335,19 +360,45 @@
         #     qr.show()
 
         # print(qr)
         # print(dataPos, len(interleavedData), (len(interleavedData)-dataPos))
 
         return qr
 
+#Function to get the correct encoding for the message
+def get_encoding(msg: str):
+    #Check if message is numeric
+    if msg.isnumeric():
+        return qrutils.QREncoding.numeric
+    #Check if message is alphanumeric
+    elif msg.isalnum():
+        return qrutils.QREncoding.alphanumeric
+    #Check if message is kanji
+    elif qrutils.is_byte(msg):
+        return qrutils.QREncoding.byte
+    elif qrutils.is_kanji(msg):
+        return qrutils.QREncoding.kanji
+
+
 #Function that returns the minimum QR version needed to encode the message
 def get_min_version(msg: str, encoding: qrutils.QREncoding = qrutils.QREncoding.byte, error_correction: qrutils.QRErrorCorrectionLevels = qrutils.QRErrorCorrectionLevels.Q):
     min_version = None
     #assign max value to minlength
     minlength = 9999999
     for version in qrutils.QRVersion:
         if len(msg) < qrutils.MAX_CHARACTERS[qrutils.QREncoding(encoding).name][error_correction][version.value] and qrutils.MAX_CHARACTERS[qrutils.QREncoding(encoding).name][error_correction][version.value] < minlength:
             min_version = version
             minlength = qrutils.MAX_CHARACTERS[qrutils.QREncoding(encoding).name][error_correction][version.value]
 
     return min_version, error_correction
+
+def smallest_qr(msg: str, error_correction: qrutils.QRErrorCorrectionLevels = qrutils.QRErrorCorrectionLevels.Q):
+    #Get the encoding
+    encoding = get_encoding(msg)
+    #Get the minimum version
+    version, err = get_min_version(msg, encoding, error_correction)
+    #Generate QR code
+    generator = QRGenerator(msg=msg, encoding=encoding, version=version, error_correction=err)
+    qr = generator.generate()
+    #Return QR code
+    return qr
```

### Comparing `barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrutils.py` & `barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -527,50 +527,201 @@
             for i in range(0, len(exponentsGenerator)):
                 exponentsGenerator[i] -= 1
 
         divisions.append(XORResult)
 
     return divisions
     
-def qr_encode_data_numeric(version: QRVersion, data: str) -> dict: #TODO: Finish the numeric encoding
+def qr_encode_data_numeric(version: QRVersion, correction: QRErrorCorrectionLevels, data: str) -> dict: #TODO: Finish the numeric encoding
     blocks = {
         'Mode': '',
         'CharacterCount': '',
-        'Data': []
+        'Data': [],
+        'ExtraPadding': {
+            'TerminatorZeros': '',
+            'MultipleOf8': '',
+            'PadBytes': [],
+        },
+        'TotalLength': 0,
+        'dataBytes': [],
+        'ErrorCorrection': [],
     }
+    totalLength = 0
+    totalBits = ''
+
     count_indicator = qr_count_indicator(version, QREncoding.numeric, data)
 
     blocks['Mode'] = QREncoding.numeric
     blocks['CharacterCount'] = count_indicator
+    totalLength += len(count_indicator)
+    totalLength += len(QREncoding.alphanumeric.value)
+    totalBits += QREncoding.numeric.value
+    totalBits += count_indicator
 
     # print(len(data))
     for i in range(0, len(data), 3):
         if i + 3 <= len(data):
             number = int(data[i:i+3])
-            # print(number)
+            
             if number > 99:
                 formatted = '{0:010b}'.format(number)
             elif number > 9:
                 formatted = '{0:07b}'.format(number)
             else:
                 formatted = '{0:04b}'.format(number)
 
+            # print(number, formatted)
+
             blocks['Data'].append(formatted)
         else:
             number = int(data[i:])
-            # print(number)
+
             if number > 99:
                 formatted = '{0:010b}'.format(number)
             elif number > 9:
                 formatted = '{0:07b}'.format(number)
             else:
                 formatted = '{0:04b}'.format(number)
 
+            # print(number, formatted)
+
             blocks['Data'].append(formatted)
 
+        totalLength += len(formatted)
+        totalBits += formatted
+
+    dataBits = DATA_CODEWORDS[version.value][correction]*8
+    remainderLength = dataBits - totalLength
+    # print(remainderLength)
+    # print(dataBits)
+
+    #Extra padding
+
+    #Terminator zeros (4 bits max)
+    if remainderLength >= 4:
+        blocks['ExtraPadding']['TerminatorZeros'] = '0'*4
+        remainderLength -= 4
+        totalLength += 4
+        totalBits += '0'*4
+    else:
+        blocks['ExtraPadding']['TerminatorZeros'] = '0'*remainderLength
+        remainderLength = 0
+        totalLength += remainderLength
+        totalBits += '0'*remainderLength
+
+    #Add 0 until the length is a multiple of 8
+    if remainderLength != 0 and remainderLength%8 != 0:
+        blocks['ExtraPadding']['MultipleOf8'] = '0'*(remainderLength%8)
+        totalBits += '0'*(remainderLength%8)
+
+        totalLength += remainderLength%8
+        remainderLength -= remainderLength%8
+
+    #Padding bytes (8 bits per byte)
+    if remainderLength != 8:
+        padBytePos = 0
+        while remainderLength >= 8:
+            blocks['ExtraPadding']['PadBytes'].append(PAD_BYTES[padBytePos%2])
+            remainderLength -= 8
+            totalLength += 8
+            totalBits += PAD_BYTES[padBytePos%2]
+            
+            padBytePos += 1
+
+    blocks['TotalLength'] = totalLength
+    # print(totalLength)
+
+    blockInfo = GROUPS[version.value][correction]
+    g1Blocks = blockInfo['GroupOne']['Blocks']
+    g1CodewordsPerBlock = blockInfo['GroupOne']['CodewordsPerBlock']
+    g2Blocks = blockInfo['GroupTwo']['Blocks']
+    g2CodewordsPerBlock = blockInfo['GroupTwo']['CodewordsPerBlock']
+
+    #Split the data in bytes
+    pos = 0
+    for i in range(0, g1Blocks):
+        codewords = []
+        for j in range(pos, pos+g1CodewordsPerBlock*8, 8):
+            codewords.append(totalBits[j:j+8])
+
+        blocks['dataBytes'].append(codewords)
+        pos += g1CodewordsPerBlock*8
+
+    if g2Blocks:
+        for i in range(0, g2Blocks):
+            codewords = []
+            for j in range(pos, pos+g2CodewordsPerBlock*8, 8):
+                codewords.append(totalBits[j:j+8])
+            
+            blocks['dataBytes'].append(codewords)
+            pos += g2CodewordsPerBlock*8
+
+    #Error correction using Reed-Solomon algorithm
+    # print(blockInfo)
+
+    singleListBytes = []
+    for i in range(0, len(totalBits), 8):
+        singleListBytes.append(totalBits[i:i+8])
+
+    #Message polynomial
+    messagePolynomial = []
+    codewordIdx = 0
+    for _ in range(0, blockInfo['GroupOne']['Blocks']):
+        blockPolynomial = []
+        for _ in range(0, blockInfo['GroupOne']['CodewordsPerBlock']):
+            codeword = singleListBytes[codewordIdx]
+            blockPolynomial.append(int(codeword, 2))
+
+            codewordIdx += 1
+
+        #Flip the block polynomial and append it to the message polynomial
+        blockPolynomial.reverse()
+        messagePolynomial.append(blockPolynomial)
+
+    # blocks['ErrorCorrection']['GroupOne'] = messagePolynomial
+    # messagePolynomial = []
+
+    if blockInfo['GroupTwo']['Blocks']:
+        for _ in range(0, blockInfo['GroupTwo']['Blocks']):
+            blockPolynomial = []
+            for _ in range(0, blockInfo['GroupTwo']['CodewordsPerBlock']):
+                codeword = singleListBytes[codewordIdx]
+                blockPolynomial.append(int(codeword, 2))
+
+                codewordIdx += 1
+
+            #Flip the block polynomial and append it to the message polynomial
+            blockPolynomial.reverse()
+            messagePolynomial.append(blockPolynomial)
+
+    # blocks['ErrorCorrection']['GroupTwo'] = messagePolynomial
+
+    # print(messagePolynomial)
+
+    #Generator polynomial
+    generatorPolynomial = generator_polynomial(version, correction)
+    # print(generatorPolynomial)
+
+    #Divide the message polynomial by the generator polynomial
+    remainder = divide_polynomials(messagePolynomial, generatorPolynomial, version, correction)
+    # print(errorCorrectionPolynomial)
+
+    #Turn remainder to list of 8 bit strings
+    for i in range(0, len(remainder)):
+        # print(len(remainder[i]))
+        for j in range(0, len(remainder[i])):
+            remainder[i][j] = '{0:08b}'.format(remainder[i][j])
+
+        #Flip the remainder
+        remainder[i].reverse()
+
+    blocks['ErrorCorrection'] = remainder
+
+    # print(blocks)
+
     return blocks
 
 def qr_encode_data_alphanumeric(version: QRVersion, correction: QRErrorCorrectionLevels, data: str) -> dict:
     blocks = {
         'Mode': '',
         'CharacterCount': '',
         'Data': [],
@@ -777,15 +928,16 @@
     blocks['CharacterCount'] = count_indicator
     totalLength += len(count_indicator)
     totalLength += len(QREncoding.byte.value)
     totalBits += QREncoding.byte.value
     totalBits += count_indicator
     
     for i in range(0, len(data)):
-        byte = ord(data[i])
+        # print(data[i])
+        byte = ord(data[i].encode('ISO-8859-1'))
         # print(byte)
         formatted = '{0:08b}'.format(byte)
 
         blocks['Data'].append(formatted)
         totalLength += len(formatted)
         totalBits += formatted
 
@@ -908,30 +1060,205 @@
 
         #Flip the remainder
         remainder[i].reverse()
 
     blocks['ErrorCorrection'] = remainder
 
     return blocks
+
+def qr_encode_data_kanji(version: QRVersion, correction: QRErrorCorrectionLevels, data: str) -> list:
+    blocks = {
+        'Mode': '',
+        'CharacterCount': '',
+        'Data': [],
+        'ExtraPadding': {
+            'TerminatorZeros': '',
+            'MultipleOf8': '',
+            'PadBytes': [],
+        },
+        'TotalLength': 0,
+        'dataBytes': [],
+        'ErrorCorrection': [],
+    }
+    totalLength = 0
+    totalBits = ''
+
+    count_indicator = qr_count_indicator(version, QREncoding.kanji, data)
+
+    blocks['Mode'] = QREncoding.kanji.value
+    blocks['CharacterCount'] = count_indicator
+    totalLength += len(count_indicator)
+    totalLength += len(QREncoding.kanji.value)
+    totalBits += QREncoding.kanji.value
+    totalBits += count_indicator
+
+    for i in range(0, len(data)):
+        bs = data[i].encode('shift-jis')
+        # print(bs, hex(bs[0]), hex(bs[1]))
+
+        #check if shift JIS is in range 8140 - 9FFC or E040 - EBBF
+        number = [0, 0]
+        if bs[0] >= 0x81 and bs[0] <= 0x9F and bs[1] >= 0x40 and bs[1] <= 0xFC:
+            number[0] = bs[0] - 0x81
+            number[1] = bs[1] - 0x40
+        elif bs[0] >= 0xE0 and bs[0] <= 0xEB and bs[1] >= 0x40 and bs[1] <= 0xBF:
+            number[0] = bs[0] - 0xC1 
+            number[1] = bs[1] - 0x40
+        # print(bs, number)
+
+        number = number[0]*0xC0 + number[1]
+        # print(hex(number))
+
+        formatted = '{0:013b}'.format(number)
+        # print(formatted)
+
+        blocks['Data'].append(formatted)
+        totalLength += len(formatted)
+        totalBits += formatted
+
+    dataBits = DATA_CODEWORDS[version.value][correction]*8
+    remainderLength = dataBits - totalLength
+    # print(remainderLength)
+    # print(dataBits)
+
+    #Extra padding
+
+    #Terminator zeros (4 bits max)
+    if remainderLength >= 4:
+        blocks['ExtraPadding']['TerminatorZeros'] = '0'*4
+        remainderLength -= 4
+        totalLength += 4
+        totalBits += '0'*4
+    else:
+        blocks['ExtraPadding']['TerminatorZeros'] = '0'*remainderLength
+        remainderLength = 0
+        totalLength += remainderLength
+        totalBits += '0'*remainderLength
+
+    #Add 0 until the length is a multiple of 8
+    if remainderLength != 0 and remainderLength%8 != 0:
+        blocks['ExtraPadding']['MultipleOf8'] = '0'*(remainderLength%8)
+        totalBits += '0'*(remainderLength%8)
+
+        totalLength += remainderLength%8
+        remainderLength -= remainderLength%8
+
+    #Padding bytes (8 bits per byte)
+    if remainderLength != 8:
+        padBytePos = 0
+        while remainderLength >= 8:
+            blocks['ExtraPadding']['PadBytes'].append(PAD_BYTES[padBytePos%2])
+            remainderLength -= 8
+            totalLength += 8
+            totalBits += PAD_BYTES[padBytePos%2]
+            
+            padBytePos += 1
+
+    blocks['TotalLength'] = totalLength
+
+    blockInfo = GROUPS[version.value][correction]
+    g1Blocks = blockInfo['GroupOne']['Blocks']
+    g1CodewordsPerBlock = blockInfo['GroupOne']['CodewordsPerBlock']
+    g2Blocks = blockInfo['GroupTwo']['Blocks']
+    g2CodewordsPerBlock = blockInfo['GroupTwo']['CodewordsPerBlock']
+
+    #Split the data in bytes
+    pos = 0
+    for i in range(0, g1Blocks):
+        codewords = []
+        for j in range(pos, pos+g1CodewordsPerBlock*8, 8):
+            codewords.append(totalBits[j:j+8])
+
+        blocks['dataBytes'].append(codewords)
+        pos += g1CodewordsPerBlock*8
+
+    if g2Blocks:
+        for i in range(0, g2Blocks):
+            codewords = []
+            for j in range(pos, pos+g2CodewordsPerBlock*8, 8):
+                codewords.append(totalBits[j:j+8])
+            
+            blocks['dataBytes'].append(codewords)
+            pos += g2CodewordsPerBlock*8
+
+    #Error correction using Reed-Solomon algorithm
+    # print(blockInfo)
+
+    singleListBytes = []
+    for i in range(0, len(totalBits), 8):
+        singleListBytes.append(totalBits[i:i+8])
+
+    #Message polynomial
+    messagePolynomial = []
+    codewordIdx = 0
+    for _ in range(0, blockInfo['GroupOne']['Blocks']):
+        blockPolynomial = []
+        for _ in range(0, blockInfo['GroupOne']['CodewordsPerBlock']):
+            codeword = singleListBytes[codewordIdx]
+            blockPolynomial.append(int(codeword, 2))
+
+            codewordIdx += 1
+
+        #Flip the block polynomial and append it to the message polynomial
+        blockPolynomial.reverse()
+        messagePolynomial.append(blockPolynomial)
+
+    # blocks['ErrorCorrection']['GroupOne'] = messagePolynomial
+    # messagePolynomial = []
+
+    if blockInfo['GroupTwo']['Blocks']:
+        for _ in range(0, blockInfo['GroupTwo']['Blocks']):
+            blockPolynomial = []
+            for _ in range(0, blockInfo['GroupTwo']['CodewordsPerBlock']):
+                codeword = singleListBytes[codewordIdx]
+                blockPolynomial.append(int(codeword, 2))
+
+                codewordIdx += 1
+
+            #Flip the block polynomial and append it to the message polynomial
+            blockPolynomial.reverse()
+            messagePolynomial.append(blockPolynomial)
+
+    # blocks['ErrorCorrection']['GroupTwo'] = messagePolynomial
+
+    #Generator polynomial
+    generatorPolynomial = generator_polynomial(version, correction)
+
+    #Divide the message polynomial by the generator polynomial
+    remainder = divide_polynomials(messagePolynomial, generatorPolynomial, version, correction)
+
+    #Turn remainder to list of 8 bit strings
+    for i in range(0, len(remainder)):
+        # print(len(remainder[i]))
+        for j in range(0, len(remainder[i])):
+            remainder[i][j] = '{0:08b}'.format(remainder[i][j])
+
+        #Flip the remainder
+        remainder[i].reverse()
+
+    blocks['ErrorCorrection'] = remainder
+
+    return blocks
+        
     
 #Function that encodes the data in the qr code and returns every block of data
 def qr_encode_data(version: QRVersion, encoding: QREncoding, correction: QRErrorCorrectionLevels, data: str) -> list:
     max_character_count = MAX_CHARACTERS[QREncoding(encoding).name][correction][version.value]
 
     if len(data) >= max_character_count:
         raise Exception('The data is too long for the version and error correction level chosen.')
 
     if encoding == QREncoding.numeric:
-        return qr_encode_data_numeric(version, data)
+        return qr_encode_data_numeric(version, correction, data)
     elif encoding == QREncoding.alphanumeric:
         return qr_encode_data_alphanumeric(version, correction, data)
     elif encoding == QREncoding.byte:
         return qr_encode_data_byte(version, correction, data)
     elif encoding == QREncoding.kanji:
-        return None
+        return qr_encode_data_kanji(version, correction, data)
 
 def alignment_pattern_locations(version: QRVersion) -> list:
     if version.value != 1:
         positions = ALIGNMENT_PATTERNS[version.value]
     else:
         positions = []
 
@@ -1206,7 +1533,21 @@
     # for row in maskedPatterns:
     #         for col in row:
     #             print(col, end='')
     #         print()
     # print()
     
     return maskedPatterns#, maskNum
+
+def is_kanji(data: str) -> bool:
+    try:
+        data.encode('shift-jis')
+        return True
+    except:
+        return False
+    
+def is_byte(data: str) -> bool:
+    try:
+        data.encode('ISO-8859-1')
+        return True
+    except:
+        return False
```

### Comparing `barcodes_uc-0.6.1/data/GF256.csv` & `barcodes_uc-0.6.2/data/GF256.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/data/alignment_locations.csv` & `barcodes_uc-0.6.2/data/alignment_locations.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/data/capabilities.csv` & `barcodes_uc-0.6.2/data/capabilities.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/data/error_correction_table.csv` & `barcodes_uc-0.6.2/data/error_correction_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/data/format_table.csv` & `barcodes_uc-0.6.2/data/format_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/data/version_table.csv` & `barcodes_uc-0.6.2/data/version_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.1/requirements.txt` & `barcodes_uc-0.6.2/requirements.txt`

 * *Files identical despite different names*

