# Comparing `tmp/edgepi-python-sdk-1.2.5.tar.gz` & `tmp/edgepi-python-sdk-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgepi-python-sdk-1.2.5.tar", last modified: Fri Jul 21 00:20:06 2023, max compression
+gzip compressed data, was "edgepi-python-sdk-1.2.6.tar", last modified: Wed Aug  2 23:31:42 2023, max compression
```

## Comparing `edgepi-python-sdk-1.2.5.tar` & `edgepi-python-sdk-1.2.6.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/edgepi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_query_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/calibration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/edgepi_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/digital_input_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/edgepi_digital_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/digital_output_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/edgepi_digital_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/eeprom_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/proto_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/edgepi_leds.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/led_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/edgepi_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/pwm_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/relay/edgepi_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/test_edgepi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/test_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/test_led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/test_tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.050837 edgepi-python-sdk-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 23:31:42.050837 edgepi-python-sdk-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.022836 edgepi-python-sdk-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.026836 edgepi-python-sdk-1.2.6/src/edgepi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.026836 edgepi-python-sdk-1.2.6/src/edgepi/adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_query_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/adc/edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/calibration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/calibration/edgepi_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/dac/edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/digital_input_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_input/edgepi_digital_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/digital_output_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/digital_output/edgepi_digital_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/eeprom_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.030836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/proto_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/edgepi_leds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/led/led_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/peripherals/spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/edgepi_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/pwm/pwm_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.034836 edgepi-python-sdk-1.2.6/src/edgepi/relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/relay/edgepi_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/edgepi/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 23:31:42.000000 edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.022836 edgepi-python-sdk-1.2.6/src/test_edgepi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/test_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.038836 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/test_led.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/test_tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.042837 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:42.046836 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-02 23:31:23.000000 edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
```

### Comparing `edgepi-python-sdk-1.2.5/LICENSE` & `edgepi-python-sdk-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/PKG-INFO` & `edgepi-python-sdk-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.2.5
+Version: 1.2.6
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edgepi-python-sdk-1.2.5/README.md` & `edgepi-python-sdk-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/setup.py` & `edgepi-python-sdk-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="edgepi-python-sdk",
-    version="1.2.5",
+    version="1.2.6",
     author="S.Park",
     author_email="spark@osensa.com",
     description="EdgePi Python SDK package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EdgePi-Cloud/edgepi-python-sdk",
     project_urls={
```

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_commands.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_conv_time.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_exceptions.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_multiplexers.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_query_lang.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_query_lang.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_state.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_status.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_voltage.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/adc/edgepi_adc.py` & `edgepi-python-sdk-1.2.6/src/edgepi/adc/edgepi_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/calibration/calibration_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/calibration/calibration_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/calibration/edgepi_calibration.py` & `edgepi-python-sdk-1.2.6/src/edgepi/calibration/edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_commands.py` & `edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/dac/dac_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/dac/edgepi_dac.py` & `edgepi-python-sdk-1.2.6/src/edgepi/dac/edgepi_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/digital_input/edgepi_digital_input.py` & `edgepi-python-sdk-1.2.6/src/edgepi/digital_input/edgepi_digital_input.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/digital_output/edgepi_digital_output.py` & `edgepi-python-sdk-1.2.6/src/edgepi/digital_output/edgepi_digital_output.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom_data.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/edgepi_eeprom_data.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/eeprom_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/eeprom_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py` & `edgepi-python-sdk-1.2.6/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio.py` & `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_chip.py` & `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_chip.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.6/src/edgepi/gpio/edgepi_gpio_expander.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_configs.py` & `edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_configs.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/gpio/gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/led/edgepi_leds.py` & `edgepi-python-sdk-1.2.6/src/edgepi/led/edgepi_leds.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/gpio.py` & `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/i2c.py` & `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/pwm.py` & `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/spi.py` & `edgepi-python-sdk-1.2.6/src/edgepi/peripherals/spi.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/pwm/edgepi_pwm.py` & `edgepi-python-sdk-1.2.6/src/edgepi/pwm/edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/pwm/pwm_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/pwm/pwm_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/reg_helper.py` & `edgepi-python-sdk-1.2.6/src/edgepi/reg_helper/reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/relay/edgepi_relay.py` & `edgepi-python-sdk-1.2.6/src/edgepi/relay/edgepi_relay.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 from edgepi.gpio.gpio_constants import GpioPins
 from edgepi.gpio.edgepi_gpio import EdgePiGPIO
 
 _logger = logging.getLogger(__name__)
 
 class EdgePiRelay():
     """A class to control the relay"""
-    def __init__(self, normally_open : bool = True):
+    def __init__(self):
         # To limit access to input functionality, using composition rather than inheritance
         self.gpio = EdgePiGPIO()
-        if normally_open:
-            self.gpio.clear_pin_state(GpioPins.RELAY.value)
-        else:
-            self.gpio.set_pin_state (GpioPins.RELAY.value)
 
     def get_state_relay(self):
         """
         Method to get the current state of the relay
         Arg:
             N/A
         Return:
```

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/tc/edgepi_tc.py` & `edgepi-python-sdk-1.2.6/src/edgepi/tc/edgepi_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_commands.py` & `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_constants.py` & `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_conv_time.py` & `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_faults.py` & `edgepi-python-sdk-1.2.6/src/edgepi/tc/tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/utilities/crc_8_atm.py` & `edgepi-python-sdk-1.2.6/src/edgepi/utilities/crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi/utilities/utilities.py` & `edgepi-python-sdk-1.2.6/src/edgepi/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/PKG-INFO` & `edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.2.5
+Version: 1.2.6
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/SOURCES.txt` & `edgepi-python-sdk-1.2.6/src/edgepi_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/test_dac.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_dac/test_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/test_gpio.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_gpio/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/test_led.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_led/test_led.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/test_tc.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/integration_tests/test_tc/test_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_status.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/test_relay.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_relay/test_relay.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,60 +7,38 @@
 if sys.platform != 'linux':
     sys.modules['periphery'] = mock.MagicMock()
 
 import pytest
 from edgepi.gpio.gpio_constants import GpioPins
 from edgepi.relay.edgepi_relay import EdgePiRelay
 
-@pytest.mark.parametrize("normally_open, pin_name", [(True, GpioPins.RELAY.value),
-                                                    (False, GpioPins.RELAY.value)])
-def test_edgepi_relay_init(mocker, normally_open, pin_name):
-    mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
-    pin_set = mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.set_pin_state')
-    pin_clear = mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.clear_pin_state')
-    EdgePiRelay(normally_open)
-    if normally_open:
-        pin_clear.assert_called_once_with(pin_name)
-    else:
-        pin_set.assert_called_once_with(pin_name)
-
 @pytest.mark.parametrize("normally_open, result", [(True, True),
                                                     (False, False)])
 def test_get_state_relay(mocker, normally_open, result):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
     mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.read_pin_state',
                   return_value = normally_open)
-    relay = EdgePiRelay(normally_open)
+    relay = EdgePiRelay()
     assert relay.get_state_relay() == result
 
-@pytest.mark.parametrize("normally_open, pin_name", [(True, GpioPins.RELAY.value),
-                                                     (False, GpioPins.RELAY.value)])
-def test_toggle_relay(mocker, normally_open, pin_name):
+@pytest.mark.parametrize("pin_name", [(GpioPins.RELAY.value),
+                                                     (GpioPins.RELAY.value)])
+def test_toggle_relay(mocker, pin_name):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
     toggle_pin = mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.toggle_pin')
-    relay = EdgePiRelay(normally_open)
+    relay = EdgePiRelay()
     relay.toggle_relay()
     toggle_pin.assert_called_once_with(pin_name)
 
-@pytest.mark.parametrize("normally_open", [(True),
-                                           (False)])
-def test_close_relay(mocker, normally_open):
+def test_close_relay(mocker):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
     set_pin = mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.set_pin_state')
-    relay = EdgePiRelay(normally_open)
+    relay = EdgePiRelay()
     relay.close_relay()
-    if normally_open:
-        assert set_pin.call_count == 1
-    else:
-        assert set_pin.call_count == 2
+    assert set_pin.call_count == 1
 
-@pytest.mark.parametrize("normally_open", [(True),
-                                           (False)])
-def test_open_relay(mocker, normally_open):
+def test_open_relay(mocker):
     mocker.patch('edgepi.gpio.edgepi_gpio.EdgePiGPIO')
     clear_pin = mocker.patch('edgepi.relay.edgepi_relay.EdgePiGPIO.clear_pin_state')
-    relay = EdgePiRelay(normally_open)
+    relay = EdgePiRelay()
     relay.open_relay()
-    if normally_open:
-        assert clear_pin.call_count == 2
-    else:
-        assert clear_pin.call_count == 1
+    assert clear_pin.call_count == 1
```

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_utilities.py` & `edgepi-python-sdk-1.2.6/src/test_edgepi/unit_tests/test_utilities/test_utilities.py`

 * *Files identical despite different names*

