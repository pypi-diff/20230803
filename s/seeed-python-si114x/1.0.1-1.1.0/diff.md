# Comparing `tmp/seeed_python_si114x-1.0.1-py2.py3-none-any.whl.zip` & `tmp/seeed_python_si114x-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 6932 bytes, number of entries: 7
--rw-r--r--  2.0 unx     9441 b- defN 20-Jun-01 09:07 seeed_si114x.py
--rw-r--r--  2.0 unx     1068 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4837 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      626 b- defN 20-Jun-01 09:10 seeed_python_si114x-1.0.1.dist-info/RECORD
-7 files, 16147 bytes uncompressed, 5806 bytes compressed:  64.0%
+Zip file size: 8735 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     8916 b- defN 23-Aug-03 01:39 seeed_si114x.py
+-rw-rw-rw-  2.0 fat     6476 b- defN 23-Aug-03 05:41 seeed_si115x.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       84 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      697 b- defN 23-Aug-03 06:11 seeed_python_si114x-1.1.0.dist-info/RECORD
+8 files, 22617 bytes uncompressed, 7503 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: seeed_si114x.py
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/LICENSE
+Filename: seeed_si115x.py
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/METADATA
+Filename: seeed_python_si114x-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/WHEEL
+Filename: seeed_python_si114x-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/entry_points.txt
+Filename: seeed_python_si114x-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/top_level.txt
+Filename: seeed_python_si114x-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: seeed_python_si114x-1.0.1.dist-info/RECORD
+Filename: seeed_python_si114x-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: seeed_python_si114x-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seeed_si114x.py

```diff
@@ -1,330 +1,299 @@
-#!/usr/bin/python3
-# -*- coding:utf-8 -*-
-from grove.i2c import Bus
-import logging
-import time
-import signal
-#Registers,Parameters and commands
-
-# commands
-
-SI114X_QUERY = 0x80
-SI114X_SET = 0xA0
-SI114X_NOP = 0x0
-SI114X_RESET    = 0x01
-SI114X_BUSADDR    = 0x02
-SI114X_PS_FORCE    = 0x05
-SI114X_GET_CAL    = 0x12
-SI114X_ALS_FORCE    = 0x06
-SI114X_PSALS_FORCE    = 0x07
-SI114X_PS_PAUSE    = 0x09
-SI114X_ALS_PAUSE    = 0x0A
-SI114X_PSALS_PAUSE    = 0xB
-SI114X_PS_AUTO    = 0x0D
-SI114X_ALS_AUTO   = 0x0E
-SI114X_PSALS_AUTO = 0x0F
-
-# IIC REGISTERS
-
-SI114X_PART_ID  = 0x00
-SI114X_REV_ID  = 0x01
-SI114X_SEQ_ID  = 0x02
-SI114X_INT_CFG  = 0x03
-SI114X_IRQ_ENABLE  = 0x04
-SI114X_IRQ_MODE1 = 0x05
-SI114X_IRQ_MODE2 = 0x06
-SI114X_HW_KEY  = 0x07
-SI114X_MEAS_RATE0 = 0x08
-SI114X_MEAS_RATE1  = 0x09
-SI114X_PS_RATE  = 0x0A
-SI114X_PS_LED21  = 0x0F
-SI114X_PS_LED3  = 0x10
-SI114X_UCOEFF0  = 0x13
-SI114X_UCOEFF1  = 0x14
-SI114X_UCOEFF2  = 0x15
-SI114X_UCOEFF3  = 0x16
-SI114X_WR  = 0x17
-SI114X_COMMAND  = 0x18
-SI114X_RESPONSE  = 0x20
-SI114X_IRQ_STATUS  = 0x21
-SI114X_ALS_VIS_DATA0 = 0x22
-SI114X_ALS_VIS_DATA1 = 0x23
-SI114X_ALS_IR_DATA0 = 0x24
-SI114X_ALS_IR_DATA1 = 0x25
-SI114X_PS1_DATA0 = 0x26
-SI114X_PS1_DATA1 = 0x27
-SI114X_PS2_DATA0 = 0x28
-SI114X_PS2_DATA1 = 0x29
-SI114X_PS3_DATA0 = 0x2A
-SI114X_PS3_DATA1 = 0x2B
-SI114X_AUX_DATA0_UVINDEX0 = 0x2C
-SI114X_AUX_DATA1_UVINDEX1 = 0x2D
-SI114X_RD = 0x2E
-SI114X_CHIP_STAT = 0x30
-
-#Parameters
-
-SI114X_I2C_ADDR = 0x00
-
-SI114X_CHLIST   = 0x01
-SI114X_CHLIST_ENUV = 0x80
-SI114X_CHLIST_ENAUX = 0x40
-SI114X_CHLIST_ENALSIR = 0x20
-SI114X_CHLIST_ENALSVIS = 0x10
-SI114X_CHLIST_ENPS1 = 0x01
-SI114X_CHLIST_ENPS2 = 0x02
-SI114X_CHLIST_ENPS3 = 0x04
-
-SI114X_PSLED12_SELECT   = 0x02
-SI114X_PSLED3_SELECT   = 0x03
-
-SI114X_PS_ENCODE   = 0x05
-SI114X_ALS_ENCODE  = 0x06
-
-SI114X_PS1_ADCMUX   = 0x07
-SI114X_PS2_ADCMUX   = 0x08
-SI114X_PS3_ADCMUX   = 0x09
-
-SI114X_PS_ADC_COUNTER   = 0x0A
-SI114X_PS_ADC_GAIN = 0x0B
-SI114X_PS_ADC_MISC = 0x0C
-
-SI114X_ALS_IR_ADC_MUX   = 0x0E
-SI114X_AUX_ADC_MUX   = 0x0F
-
-SI114X_ALS_VIS_ADC_COUNTER   = 0x10
-SI114X_ALS_VIS_ADC_GAIN = 0x11
-SI114X_ALS_VIS_ADC_MISC = 0x12
-
-SI114X_LED_REC = 0x1C
-
-SI114X_ALS_IR_ADC_COUNTER   = 0x1D
-SI114X_ALS_IR_ADC_GAIN = 0x1E
-SI114X_ALS_IR_ADC_MISC = 0x1F
-
-#USER SETTINGS DEFINE
-
-#ADCMUX
-
-SI114X_ADCMUX_SMALL_IR  = 0x00
-SI114X_ADCMUX_VISIABLE = 0x02
-SI114X_ADCMUX_LARGE_IR  = 0x03
-SI114X_ADCMUX_NO  = 0x06
-SI114X_ADCMUX_GND  = 0x25
-SI114X_ADCMUX_TEMPERATURE  = 0x65
-SI114X_ADCMUX_VDD  = 0x75
-
-#LED SEL
-
-SI114X_PSLED12_SELECT_PS1_NONE = 0x00
-SI114X_PSLED12_SELECT_PS1_LED1 = 0x01
-SI114X_PSLED12_SELECT_PS1_LED2 = 0x02
-SI114X_PSLED12_SELECT_PS1_LED3 = 0x04
-SI114X_PSLED12_SELECT_PS2_NONE = 0x00
-SI114X_PSLED12_SELECT_PS2_LED1 = 0x10
-SI114X_PSLED12_SELECT_PS2_LED2 = 0x20
-SI114X_PSLED12_SELECT_PS2_LED3 = 0x40
-SI114X_PSLED3_SELECT_PS2_NONE = 0x00
-SI114X_PSLED3_SELECT_PS2_LED1 = 0x10
-SI114X_PSLED3_SELECT_PS2_LED2 = 0x20
-SI114X_PSLED3_SELECT_PS2_LED3 = 0x40
-
-#ADC GAIN DIV
-
-SI114X_ADC_GAIN_DIV1 = 0x00
-SI114X_ADC_GAIN_DIV2 = 0x01
-SI114X_ADC_GAIN_DIV4 = 0x02
-SI114X_ADC_GAIN_DIV8 = 0x03
-SI114X_ADC_GAIN_DIV16 = 0x04
-SI114X_ADC_GAIN_DIV32 = 0x05
-
-#LED CURRENT
-
-SI114X_LED_CURRENT_5MA = 0x01
-SI114X_LED_CURRENT_11MA = 0x02
-SI114X_LED_CURRENT_22MA = 0x03
-SI114X_LED_CURRENT_45MA = 0x04
-
-#Recovery period the  ADC takes before making a PS measurement
-
-SI114X_ADC_COUNTER_1ADCCLK = 0x00
-SI114X_ADC_COUNTER_7ADCCLK = 0x01
-SI114X_ADC_COUNTER_15ADCCLK = 0x02
-SI114X_ADC_COUNTER_31ADCCLK = 0x03
-SI114X_ADC_COUNTER_63ADCCLK = 0x04
-SI114X_ADC_COUNTER_127ADCCLK = 0x05
-SI114X_ADC_COUNTER_255ADCCLK = 0x06
-SI114X_ADC_COUNTER_511ADCCLK = 0x07
-
-#ADC MISC
-
-SI114X_ADC_MISC_LOWRANGE = 0x00
-SI114X_ADC_MISC_HIGHRANGE = 0x20
-SI114X_ADC_MISC_ADC_NORMALPROXIMITY = 0x00
-SI114X_ADC_MISC_ADC_RAWADC = 0x04
-
-#INT OE
-
-SI114X_INT_CFG_INTOE = 0x01
-
-#IRQ ENABLE
-
-SI114X_IRQEN_ALS = 0x01
-SI114X_IRQEN_PS1 = 0x04
-SI114X_IRQEN_PS2 = 0x08
-SI114X_IRQEN_PS3 = 0x10
-
-SI114X_ADDR = 0x60
-
-class grove_si114x(object):
-    def __init__(self,address = SI114X_ADDR):
-        self.bus = Bus()
-        self.addr = address
-        self._logger = logging.getLogger('grove_si114x')
-        assert self.Begin() , "Please check if the I2C device insert in I2C of Base Hat"
-    def __del__(self):
-        self._WriteByte(SI114X_COMMAND, SI114X_RESET)
-        time.sleep(0.1)
-        self.bus.close()
-        # Calling __delete__ 
-    def __exit__(self):
-        self.bus.close()
-    #Init the si114x and begin to collect data
-    def Begin(self):
-        if self._ReadByte(SI114X_PART_ID) != 0X45:
-            return False
-        self.Reset()
-        #INIT
-        self.DeInit()
-        return True
-    #reset the si114x
-    #inclue IRQ reg, command regs...
-    def Reset(self):
-        self._WriteByte(SI114X_MEAS_RATE0, 0)
-        self._WriteByte(SI114X_MEAS_RATE1, 0)
-        self._WriteByte(SI114X_IRQ_ENABLE, 0)
-        self._WriteByte(SI114X_IRQ_MODE1, 0)
-        self._WriteByte(SI114X_IRQ_MODE2, 0)
-        self._WriteByte(SI114X_INT_CFG, 0)
-        self._WriteByte(SI114X_IRQ_STATUS, 0xFF)
-        self._WriteByte(SI114X_COMMAND, SI114X_RESET)
-        time.sleep(0.1)
-        self._WriteByte(SI114X_HW_KEY, 0x17)
-        time.sleep(0.1)  
-
-    #default init  
-    def DeInit(self):
-        #ENABLE UV reading
-        #these reg must be set to the fixed value
-        self._WriteByte(SI114X_UCOEFF0, 0x29)
-        self._WriteByte(SI114X_UCOEFF1, 0x89)
-        self._WriteByte(SI114X_UCOEFF2, 0x02)
-        self._WriteByte(SI114X_UCOEFF3, 0x00)
-        self.WriteParamData(SI114X_CHLIST, SI114X_CHLIST_ENUV | SI114X_CHLIST_ENALSIR | SI114X_CHLIST_ENALSVIS |
-                    SI114X_CHLIST_ENPS1)
-        #
-        #set LED1 CURRENT(22.4mA)(It is a normal value for many LED)
-        #
-        self.WriteParamData(SI114X_PS1_ADCMUX, SI114X_ADCMUX_LARGE_IR)
-        self._WriteByte(SI114X_PS_LED21, SI114X_LED_CURRENT_22MA)
-        self.WriteParamData(SI114X_PSLED12_SELECT, SI114X_PSLED12_SELECT_PS1_LED1) #
-        #
-        #PS ADC SETTING
-        #
-        self.WriteParamData(SI114X_PS_ADC_GAIN, SI114X_ADC_GAIN_DIV1)
-        self.WriteParamData(SI114X_PS_ADC_COUNTER, SI114X_ADC_COUNTER_511ADCCLK)
-        self.WriteParamData(SI114X_PS_ADC_MISC, SI114X_ADC_MISC_HIGHRANGE | SI114X_ADC_MISC_ADC_RAWADC)
-        #
-        #VIS ADC SETTING
-        #
-        self.WriteParamData(SI114X_ALS_VIS_ADC_GAIN, SI114X_ADC_GAIN_DIV1)
-        self.WriteParamData(SI114X_ALS_VIS_ADC_COUNTER, SI114X_ADC_COUNTER_511ADCCLK)
-        self.WriteParamData(SI114X_ALS_VIS_ADC_MISC, SI114X_ADC_MISC_HIGHRANGE)
-        #
-        #IR ADC SETTING
-        #
-        self.WriteParamData(SI114X_ALS_IR_ADC_GAIN, SI114X_ADC_GAIN_DIV1)
-        self.WriteParamData(SI114X_ALS_IR_ADC_COUNTER, SI114X_ADC_COUNTER_511ADCCLK)
-        self.WriteParamData(SI114X_ALS_IR_ADC_MISC, SI114X_ADC_MISC_HIGHRANGE)
-        #
-        #interrupt enable
-        #
-        self._WriteByte(SI114X_INT_CFG, SI114X_INT_CFG_INTOE)
-        self._WriteByte(SI114X_IRQ_ENABLE, SI114X_IRQEN_ALS)
-        #
-        #AUTO RUN
-        #
-        self._WriteByte(SI114X_MEAS_RATE0, 0xFF)
-        self._WriteByte(SI114X_COMMAND, SI114X_PSALS_AUTO)
-
-    #read param data
-    def ReadParamData(self,Reg):
-        self._WriteByte(SI114X_COMMAND,Reg|SI114X_QUERY)
-        return self._ReadByte(SI114X_RD)
-
-    #writ param data
-    def WriteParamData(self,Reg,Value):
-        #write Value into PARAMWR reg first
-        self._WriteByte(SI114X_WR, Value)
-        self._WriteByte(SI114X_COMMAND, Reg | SI114X_SET)
-        #SI114X writes value out to PARAM_RD,read and confirm its right
-        return self._ReadByte(SI114X_RD)
-
-    #Read Visible Value
-    @property
-    def ReadVisible(self):
-        return self._ReadHalfWord(SI114X_ALS_VIS_DATA0)
-
-    #Read IR Value    
-    @property
-    def ReadIR(self):
-        return self._ReadHalfWord(SI114X_ALS_IR_DATA0)
-
-    #Read UV Value
-    #this function is a int value ,but the real value must be div 100
-    @property
-    def ReadUV(self):
-        return self._ReadHalfWord(SI114X_AUX_DATA0_UVINDEX0)
-    
-    #Read Proximity Value
-    def ReadProximity(self,PSn):
-         return self._ReadHalfWord(PSn)
-
-    # read 8 bit data from Reg
-    def _ReadByte(self,Reg):
-        try:
-            read_data = self.bus.read_byte_data(self.addr,Reg)
-        except OSError:
-            raise  OSError("Please check if the I2C device insert in I2C of Base Hat")
-        return read_data
-
-    # Write 8 bit data to Reg
-    def _WriteByte(self,Reg,Value):
-        try:
-            self.bus.write_byte_data(self.addr,Reg,Value)
-        except OSError:
-            raise OSError("Please check if the I2C device insert in I2C of Base Hat")
-
-    # read 16 bit data from Reg
-    def _ReadHalfWord(self,Reg):
-        try:
-            block = self.bus.read_i2c_block_data(self.addr,Reg, 2)
-        except OSError:
-            raise OSError("Please check if the I2C device insert in I2C of Base Hat")
-        read_data = (block[0] & 0xff) | (block[1] << 8)
-        return read_data   
-def handler(signalnum, handler):
-    print("Please use Ctrl C to quit")
-def main():
-    signal.signal(signal.SIGTSTP, handler) # Ctrl-z
-    signal.signal(signal.SIGQUIT, handler) # Ctrl-\
-    SI1145 = grove_si114x()
-    print("Please use Ctrl C to quit")
-    while True:
-        print('Visible %03d UV %.2f IR %03d' % (SI1145.ReadVisible , SI1145.ReadUV/100 , SI1145.ReadIR),end=" ")
-        print('\r', end='')
-        time.sleep(0.5)
-
-if __name__ == "__main__":
-    main()     
+#!/usr/bin/python3
+# -*- coding:utf-8 -*-
+from grove.i2c import Bus
+from enum import IntEnum
+import logging
+import time
+import signal
+
+
+class I2C_ADDR(IntEnum):
+    SI114X = 0x60
+
+class SI114X_REG(IntEnum):
+    PART_ID = 0x00
+    REV_ID = 0x01
+    SEQ_ID = 0x02
+    INT_CFG = 0x03
+    IRQ_ENABLE = 0x04
+    IRQ_MODE1 = 0x05
+    IRQ_MODE2 = 0x06
+    HW_KEY = 0x07
+    MEAS_RATE0 = 0x08
+    MEAS_RATE1 = 0x09
+    PS_RATE = 0x0A
+    PS_LED21 = 0x0F
+    PS_LED3 = 0x10
+    UCOEFF0 = 0x13
+    UCOEFF1 = 0x14
+    UCOEFF2 = 0x15
+    UCOEFF3 = 0x16
+    WR = 0x17
+    COMMAND = 0x18
+    RESPONSE = 0x20
+    IRQ_STATUS = 0x21
+    ALS_VIS_DATA0 = 0x22
+    ALS_VIS_DATA1 = 0x23
+    ALS_IR_DATA0 = 0x24
+    ALS_IR_DATA1 = 0x25
+    PS1_DATA0 = 0x26
+    PS1_DATA1 = 0x27
+    PS2_DATA0 = 0x28
+    PS2_DATA1 = 0x29
+    PS3_DATA0 = 0x2A
+    PS3_DATA1 = 0x2B
+    AUX_DATA0_UVINDEX0 = 0x2C
+    AUX_DATA1_UVINDEX1 = 0x2D
+    RD = 0x2E
+    CHIP_STAT = 0x30
+
+
+class SI114X_CMD(IntEnum):
+    NOP = 0x00
+    RESET = 0x01
+    BUSADDR = 0x02
+    PS_FORCE = 0x05
+    ALS_FORCE = 0x06
+    PSALS_FORCE = 0x07
+    PS_PAUSE = 0x09
+    ALS_PAUSE = 0x0A
+    PSALS_PAUSE = 0x0B
+    PS_AUTO = 0x0D
+    ALS_AUTO = 0x0E
+    PSALS_AUTO = 0x0F
+    QUERY = 0x80
+    SET = 0xA0
+
+
+class SI114X_PARAM(IntEnum):
+    I2CADDR = 0x00
+    CHLIST = 0x01
+    PSLED12_SELECT = 0x02
+    PSLED3_SELECT = 0x03
+    PS_ENCODING = 0x05
+    ALS_ENCODING = 0x06
+    PS1_ADCMUX = 0x07
+    PS2_ADCMUX = 0x08
+    PS3_ADCMUX = 0x09
+    PS_ADC_COUNTER = 0x0A
+    PS_ADC_GAIN = 0x0B
+    PS_ADC_MISC = 0x0C
+    ALS_IR_ADCMUX = 0x0E
+    AUX_ADCMUX = 0x0F
+    ALS_VIS_ADC_COUNTER = 0x10
+    ALS_VIS_ADC_GAIN = 0x11
+    ALS_VIS_ADC_MISC = 0x12
+    LED_REC = 0x1C
+    ALS_IR_ADC_COUNTER = 0x1D
+    ALS_IR_ADC_GAIN = 0x1E
+    ALS_IR_ADC_MISC = 0x1F
+
+
+class SI114X_CHLIST(IntEnum):
+    ENPS1 = 0x01
+    ENPS2 = 0x02
+    ENPS3 = 0x04
+    ENALSVIS = 0x10
+    ENALSIR = 0x20
+    ENAUX = 0x40
+    ENUV = 0x80
+
+#USER SETTINGS DEFINE
+
+class SI114X_ADCMUX(IntEnum):
+    SMALL_IR = 0x00
+    VISIABLE = 0x02
+    LARGE_IR = 0x03
+    NO = 0x06
+    GND = 0x25
+    TEMPERATURE = 0x65
+    VDD = 0x75
+
+class SI114X_LED_SEL(IntEnum):
+    PS1_NONE = 0x00
+    PS1_LED1 = 0x01
+    PS1_LED2 = 0x02
+    PS1_LED3 = 0x04
+    PS2_NONE = 0x00
+    PS2_LED1 = 0x10
+    PS2_LED2 = 0x20
+    PS2_LED3 = 0x40
+
+class SI114X_ADC_GAIN(IntEnum):
+    DIV1 = 0x00
+    DIV2 = 0x01
+    DIV4 = 0x02
+    DIV8 = 0x03
+    DIV16 = 0x04
+    DIV32 = 0x05
+
+class SI114X_LED_CURRENT(IntEnum):
+    CUR5MA = 0x01
+    CUR11MA = 0x02
+    CUR22MA = 0x03
+    CUR45MA = 0x04
+
+#Recovery period the  ADC takes before making a PS measurement
+class SI114X_ADC_COUNTER(IntEnum):
+    ADCCLK1 = 0x00
+    ADCCLK7 = 0x01
+    ADCCLK15 = 0x02
+    ADCCLK31 = 0x03
+    ADCCLK63 = 0x04
+    ADCCLK127 = 0x05
+    ADCCLK255 = 0x06
+    ADCCLK511 = 0x07
+
+class SI114X_ADC_MISC(IntEnum):
+    LOWRANGE = 0x00
+    HIGHRANGE = 0x20
+    ADC_NORMALPROXIMITY = 0x00
+    ADC_RAWADC = 0x04
+
+#IRQ ENABLE
+class SI114X_IRQEN(IntEnum):
+    ALS = 0x01
+    PS1 = 0x04
+    PS2 = 0x08
+    PS3 = 0x10
+
+
+class grove_si114x(object):
+    def __init__(self,address = I2C_ADDR.SI114X):
+        self.bus = Bus()
+        self.addr = address
+        self._logger = logging.getLogger('grove_si114x')
+        assert self.Begin() , "Please check if the I2C device insert in I2C of Base Hat"
+    def __del__(self):
+        self._WriteByte(SI114X_REG.COMMAND, SI114X_CMD.RESET)
+        time.sleep(0.1)
+        self.bus.close()
+    def __exit__(self):
+        self.bus.close()
+    #Init the si114x and begin to collect data
+    def Begin(self):
+        if self._ReadByte(SI114X_REG.PART_ID) != 0X45:
+            return False
+        self.Reset()
+        #INIT
+        self.DeInit()
+        return True
+    #reset the si114x
+    #inclue IRQ reg, command regs...
+    def Reset(self):
+        self._WriteByte(SI114X_REG.MEAS_RATE0, 0)
+        self._WriteByte(SI114X_REG.MEAS_RATE1, 0)
+        self._WriteByte(SI114X_REG.IRQ_ENABLE, 0)
+        self._WriteByte(SI114X_REG.IRQ_MODE1, 0)
+        self._WriteByte(SI114X_REG.IRQ_MODE2, 0)
+        self._WriteByte(SI114X_REG.INT_CFG, 0)
+        self._WriteByte(SI114X_REG.IRQ_STATUS, 0xFF)
+        self._WriteByte(SI114X_REG.COMMAND, SI114X_CMD.RESET)
+        time.sleep(0.1)
+        self._WriteByte(SI114X_REG.HW_KEY, 0x17)
+        time.sleep(0.1)  
+
+    #default init  
+    def DeInit(self):
+        #ENABLE UV reading
+        #these reg must be set to the fixed value
+        self._WriteByte(SI114X_REG.UCOEFF0, 0x29)
+        self._WriteByte(SI114X_REG.UCOEFF1, 0x89)
+        self._WriteByte(SI114X_REG.UCOEFF2, 0x02)
+        self._WriteByte(SI114X_REG.UCOEFF3, 0x00)
+        self.WriteParamData(SI114X_PARAM.CHLIST, SI114X_CHLIST.ENUV | SI114X_CHLIST.ENALSIR | SI114X_CHLIST.ENALSVIS |
+                    SI114X_CHLIST.ENPS1)
+        #set LED1 CURRENT(22.4mA)(It is a normal value for many LED)
+        self.WriteParamData(SI114X_PARAM.PS1_ADCMUX, SI114X_ADCMUX.LARGE_IR)
+        self._WriteByte(SI114X_REG.PS_LED21, SI114X_LED_CURRENT.CUR22MA)
+        self.WriteParamData(SI114X_PARAM.PSLED12_SELECT, SI114X_LED_SEL.PS1_LED1)
+        #PS ADC SETTING
+        self.WriteParamData(SI114X_PARAM.PS_ADC_GAIN, SI114X_ADC_GAIN.DIV1)
+        self.WriteParamData(SI114X_PARAM.PS_ADC_COUNTER, SI114X_ADC_COUNTER.ADCCLK511)
+        self.WriteParamData(SI114X_PARAM.PS_ADC_MISC, SI114X_ADC_MISC.HIGHRANGE | SI114X_ADC_MISC.ADC_RAWADC)
+        #VIS ADC SETTING
+        self.WriteParamData(SI114X_PARAM.ALS_VIS_ADC_GAIN, SI114X_ADC_GAIN.DIV1)
+        self.WriteParamData(SI114X_PARAM.ALS_VIS_ADC_COUNTER, SI114X_ADC_COUNTER.ADCCLK511)
+        self.WriteParamData(SI114X_PARAM.ALS_VIS_ADC_MISC, SI114X_ADC_MISC.HIGHRANGE)
+        #IR ADC SETTING
+        self.WriteParamData(SI114X_PARAM.ALS_IR_ADC_GAIN, SI114X_ADC_GAIN.DIV1)
+        self.WriteParamData(SI114X_PARAM.ALS_IR_ADC_COUNTER, SI114X_ADC_COUNTER.ADCCLK511)
+        self.WriteParamData(SI114X_PARAM.ALS_IR_ADC_MISC, SI114X_ADC_MISC.HIGHRANGE)
+        #interrupt enable
+        self._WriteByte(SI114X_REG.INT_CFG, 1)
+        self._WriteByte(SI114X_REG.IRQ_ENABLE, SI114X_IRQEN.ALS)
+        #AUTO RUN
+        self._WriteByte(SI114X_REG.MEAS_RATE0, 0xFF)
+        self._WriteByte(SI114X_REG.COMMAND, SI114X_CMD.PSALS_AUTO)
+
+    #read param data
+    def ReadParamData(self,Reg):
+        self._WriteByte(SI114X_REG.COMMAND, Reg | SI114X_CMD.QUERY)
+        return self._ReadByte(SI114X_CMD.RD)
+
+    #writ param data
+    def WriteParamData(self,Reg,Value):
+        #write Value into PARAMWR reg first
+        self._WriteByte(SI114X_REG.WR, Value)
+        self._WriteByte(SI114X_REG.COMMAND, Reg | SI114X_CMD.SET)
+        #SI114X writes value out to PARAM_RD,read and confirm its right
+        return self._ReadByte(SI114X_REG.RD)
+
+    #Read Visible Value
+    @property
+    def ReadVisible(self):
+        return self._ReadHalfWord(SI114X_REG.ALS_VIS_DATA0)
+
+    #Read IR Value    
+    @property
+    def ReadIR(self):
+        return self._ReadHalfWord(SI114X_REG.ALS_IR_DATA0)
+
+    #Read UV Value
+    #this function is a int value ,but the real value must be div 100
+    @property
+    def ReadUV(self):
+        return self._ReadHalfWord(SI114X_REG.AUX_DATA0_UVINDEX0)
+    
+    #Read Proximity Value
+    def ReadProximity(self,PSn):
+         return self._ReadHalfWord(PSn)
+
+    # read 8 bit data from Reg
+    def _ReadByte(self,Reg):
+        try:
+            read_data = self.bus.read_byte_data(self.addr,Reg)
+        except OSError:
+            raise  OSError("Please check if the I2C device insert in I2C of Base Hat")
+        return read_data
+
+    # Write 8 bit data to Reg
+    def _WriteByte(self,Reg,Value):
+        try:
+            self.bus.write_byte_data(self.addr,Reg,Value)
+        except OSError:
+            raise OSError("Please check if the I2C device insert in I2C of Base Hat")
+
+    # read 16 bit data from Reg
+    def _ReadHalfWord(self,Reg):
+        try:
+            block = self.bus.read_i2c_block_data(self.addr,Reg, 2)
+        except OSError:
+            raise OSError("Please check if the I2C device insert in I2C of Base Hat")
+        read_data = (block[0] & 0xff) | (block[1] << 8)
+        return read_data   
+def handler(signalnum, handler):
+    print("Please use Ctrl C to quit")
+def main():
+    signal.signal(signal.SIGTSTP, handler) # Ctrl-z
+    signal.signal(signal.SIGQUIT, handler) # Ctrl-\
+    SI1145 = grove_si114x()
+    print("Please use Ctrl C to quit")
+    while True:
+        print('Visible %03d UV %.2f IR %03d' % (SI1145.ReadVisible , SI1145.ReadUV/100 , SI1145.ReadIR),end=" ")
+        print('\r', end='')
+        time.sleep(0.5)
+
+if __name__ == "__main__":
+    main()
```

## Comparing `seeed_python_si114x-1.0.1.dist-info/METADATA` & `seeed_python_si114x-1.1.0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,151 +1,275 @@
-Metadata-Version: 2.1
-Name: seeed-python-si114x
-Version: 1.0.1
-Summary: Python library for the Grove - Sunlight Sensor (si114x). 
-Home-page: https://github.com/Seeed-Studio/Seeed_Python_SI114X
-Author: Hansen
-Author-email: 595355940@qq.com
-License: MIT
-Keywords: seeed grove si114x  sensor i2c hardware
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/markdown
-Requires-Dist: Seeed-grove.py
-
-# Seeed_Python_SI114X
-
-![](https://camo.githubusercontent.com/0b16b004205798245778945edb73f36c7e5d7adf/68747470733a2f2f73746174696373332e736565656473747564696f2e636f6d2f696d616765732f70726f647563742f313031303230303839253230312e6a7067)
-
-Grove - Sunlight Sensor (si114x) is a multi-channel digital light sensor, which has the ability to detect UV-light, visible light and infrared light.
-
-This device is based on SI1145, a new sensor from SiLabs. The Si1145 is a low-power, reflectance-based, infrared proximity, UV index and ambient light sensor with I2C digital interface and programmable-event interrupt output. This device offers excellent performance under a wide dynamic range and a variety of light sources including direct sunlight.
-
-# Dependencies
-
-This driver depends on:
-- [***grove.py***](https://github.com/Seeed-Studio/grove.py)
-
-This is easy to install with the following command.
-
-```python
-pip3 install Seeed-grove.py
-```
-
-## Installing from PyPI
-
-On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally from PyPI. To install for current user:
-
-```
-
-pip3 install seeed-python-si114x
-
-```
-
-To install system-wide (this may be required in some cases):
-
-```
-
-sudo pip3 install seeed-python-si114x
-
-```
-
-if you want to update the driver locally from PyPI. you can use:
-
-```
-pip3 install --upgrade seeed-python-si114x
-```
-
-## Usage Notes
-
-First, Check the corresponding i2c number of the board:
-
-```
-
-(.env) pi@raspberrypi:~ $ ls /dev/i2c*
-/dev/i2c-1
-
-```
-
-Check if the i2c device works properly， 0x60 is the SI114x i2c address.
-```
-
-pi@raspberrypi:~/Seeed_Python_SI114X $ i2cdetect -y -r 1
-     0  1  2  3  4  5  6  7  8  9  a  b  c  d  e  f
-00:          -- 04 -- -- -- -- -- -- -- -- -- -- -- 
-10: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
-20: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
-30: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
-40: -- -- -- -- -- -- -- -- UU -- -- -- -- -- -- -- 
-50: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
-60: 60 -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
-70: -- -- -- -- -- -- -- --   
-
-```
-
-## Usage
-
-```python
-import seeed_si114x
-import time
-import signal
-def handler(signalnum, handler):
-    print("Please use Ctrl C to quit")
-def main():
-    SI1145 = seeed_si114x.grove_si114x()
-    print("Please use Ctrl C to quit")
-    signal.signal(signal.SIGTSTP, handler) # Ctrl-z
-    signal.signal(signal.SIGQUIT, handler) # Ctrl-\
-    while True:
-        print('Visible %03d UV %.2f IR %03d' % (SI1145.ReadVisible , SI1145.ReadUV/100 , SI1145.ReadIR),end=" ")
-        print('\r', end='')
-        time.sleep(0.5)
-if __name__  == '__main__':
-    main()
-```
-
-## API Reference
-
-## API Reference
-
-- uint16_t ReadVisible(void): return visible light of Ambient.
-
-```python
-    print("Visible %03d" % SI1145.ReadVisible)
-```
-
-- uint16_t ReadUV(void): return Ultraviolet (UV) Index.
-
-```python
-    print("UV %.2f" % SI1145.ReadUV / 100)
-```
-
-- uint16_t ReadIR(void): return infrared light of Ambient.
-
-```python
-    print("IR %03d" % SI1145.ReadIR)
-```
-----
-
-This software is written by seeed studio<br>
-and is licensed under [The MIT License](http://opensource.org/licenses/mit-license.php). Check License.txt for more information.<br>
-
-Contributing to this software is warmly welcomed. You can do this basically by<br>
-[forking](https://help.github.com/articles/fork-a-repo), committing modifications and then [pulling requests](https://help.github.com/articles/using-pull-requests) (follow the links above<br>
-for operating guide). Adding change log and your contact into file header is encouraged.<br>
-Thanks for your contribution.
-
-Seeed Studio is an open hardware facilitation company based in Shenzhen, China. <br>
-Benefiting from local manufacture power and convenient global logistic system, <br>
-we integrate resources to serve new era of innovation. Seeed also works with <br>
-global distributors and partners to push open hardware movement.<br>
-
-
-[![Analytics](https://ga-beacon.appspot.com/UA-46589105-3/Grove_LED_Bar)](https://github.com/igrigorik/ga-beacon)
-
+Metadata-Version: 2.1
+Name: seeed-python-si114x
+Version: 1.1.0
+Summary: Python library for the Grove - Sunlight Sensor (si114x,si115x). 
+Home-page: https://github.com/Seeed-Studio/Seeed_Python_SI114X
+Author: Hansen
+Author-email: 595355940@qq.com
+License: MIT
+Keywords: seeed grove si114x si115x sensor i2c hardware
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Seeed-grove.py
+
+# Seeed_Python_SI114X
+
+
+
+![](https://camo.githubusercontent.com/0b16b004205798245778945edb73f36c7e5d7adf/68747470733a2f2f73746174696373332e736565656473747564696f2e636f6d2f696d616765732f70726f647563742f313031303230303839253230312e6a7067)
+
+
+
+Grove - Sunlight Sensor (si114x) is a multi-channel digital light sensor, which has the ability to detect UV-light, visible light and infrared light.
+
+
+
+This device is based on SI1145, a new sensor from SiLabs. The Si1145 is a low-power, reflectance-based, infrared proximity, UV index and ambient light sensor with I2C digital interface and programmable-event interrupt output. This device offers excellent performance under a wide dynamic range and a variety of light sources including direct sunlight.
+
+
+
+# Dependencies
+
+
+
+This driver depends on:
+
+- [***grove.py***](https://github.com/Seeed-Studio/grove.py)
+
+
+
+This is easy to install with the following command.
+
+
+
+```python
+
+pip3 install Seeed-grove.py
+
+```
+
+ 
+
+## Installing from PyPI
+
+
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally from PyPI. To install for current user:
+
+
+
+```
+
+
+
+pip3 install seeed-python-si114x
+
+
+
+```
+
+
+
+To install system-wide (this may be required in some cases):
+
+
+
+```
+
+
+
+sudo pip3 install seeed-python-si114x
+
+
+
+```
+
+
+
+if you want to update the driver locally from PyPI. you can use:
+
+
+
+```
+
+pip3 install --upgrade seeed-python-si114x
+
+```
+
+
+
+## Usage Notes
+
+
+
+First, Check the corresponding i2c number of the board:
+
+
+
+```
+
+
+
+(.env) pi@raspberrypi:~ $ ls /dev/i2c*
+
+/dev/i2c-1
+
+
+
+```
+
+
+
+Check if the i2c device works properly， 0x60 is the SI114x i2c address.
+
+```
+
+
+
+pi@raspberrypi:~/Seeed_Python_SI114X $ i2cdetect -y -r 1
+
+     0  1  2  3  4  5  6  7  8  9  a  b  c  d  e  f
+
+00:          -- 04 -- -- -- -- -- -- -- -- -- -- -- 
+
+10: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
+
+20: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
+
+30: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
+
+40: -- -- -- -- -- -- -- -- UU -- -- -- -- -- -- -- 
+
+50: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
+
+60: 60 -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
+
+70: -- -- -- -- -- -- -- --   
+
+
+
+```
+
+
+
+## Usage
+
+
+
+```python
+
+import seeed_si114x
+
+import time
+
+import signal
+
+def handler(signalnum, handler):
+
+    print("Please use Ctrl C to quit")
+
+def main():
+
+    SI1145 = seeed_si114x.grove_si114x()
+
+    print("Please use Ctrl C to quit")
+
+    signal.signal(signal.SIGTSTP, handler) # Ctrl-z
+
+    signal.signal(signal.SIGQUIT, handler) # Ctrl-\
+
+    while True:
+
+        print('Visible %03d UV %.2f IR %03d' % (SI1145.ReadVisible , SI1145.ReadUV/100 , SI1145.ReadIR),end=" ")
+
+        print('\r', end='')
+
+        time.sleep(0.5)
+
+if __name__  == '__main__':
+
+    main()
+
+```
+
+
+
+## API Reference
+
+
+
+- uint16_t ReadVisible(void): return visible light of Ambient.
+
+
+
+```python
+
+    print("Visible %03d" % SI1145.ReadVisible)
+
+```
+
+
+
+- uint16_t ReadUV(void): return Ultraviolet (UV) Index.
+
+
+
+```python
+
+    print("UV %.2f" % SI1145.ReadUV / 100)
+
+```
+
+
+
+- uint16_t ReadIR(void): return infrared light of Ambient.
+
+
+
+```python
+
+    print("IR %03d" % SI1145.ReadIR)
+
+```
+
+----
+
+
+
+This software is written by seeed studio<br>
+
+and is licensed under [The MIT License](http://opensource.org/licenses/mit-license.php). Check License.txt for more information.<br>
+
+
+
+Contributing to this software is warmly welcomed. You can do this basically by<br>
+
+[forking](https://help.github.com/articles/fork-a-repo), committing modifications and then [pulling requests](https://help.github.com/articles/using-pull-requests) (follow the links above<br>
+
+for operating guide). Adding change log and your contact into file header is encouraged.<br>
+
+Thanks for your contribution.
+
+
+
+Seeed Studio is an open hardware facilitation company based in Shenzhen, China. <br>
+
+Benefiting from local manufacture power and convenient global logistic system, <br>
+
+we integrate resources to serve new era of innovation. Seeed also works with <br>
+
+global distributors and partners to push open hardware movement.<br>
+
+
+
+
+
+[![Analytics](https://ga-beacon.appspot.com/UA-46589105-3/Grove_LED_Bar)](https://github.com/igrigorik/ga-beacon)
+
```

