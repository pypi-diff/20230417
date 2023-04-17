# Comparing `tmp/pimoroni_ioexpander-0.0.4.tar.gz` & `tmp/pimoroni_ioexpander-0.0.5.tar.gz`

## Comparing `pimoroni_ioexpander-0.0.4.tar` & `pimoroni_ioexpander-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,42 @@
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/README.md
--rw-r--r--   0        0        0    46927 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/common.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/devices.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/encoder.md
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/encoder.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/ioe_regs.py
--rw-r--r--   0        0        0    15154 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/motor.md
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/motor.py
--rw-r--r--   0        0        0    17325 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/servo.md
--rw-r--r--   0        0        0    18673 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/servo.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/ioexpander/sioe_regs.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/LICENSE
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    12965 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/Makefile
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/README.md
+-rw-r--r--   0        0        0    14545 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/REFERENCE.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/check.sh
+-rwxr-xr-x   0        0        0     5533 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/install.sh
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tox.ini
+-rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/uninstall.sh
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/encoder.md
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/motor.md
+-rw-r--r--   0        0        0    17360 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/docs/servo.md
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/analog.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/basic-test-cycles.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/button.py
+-rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/mics6814.py
+-rwxr-xr-x   0        0        0     1295 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/pir.py
+-rwxr-xr-x   0        0        0     1444 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/potentiometer.py
+-rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/pwm.py
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/rgbled.py
+-rwxr-xr-x   0        0        0     1559 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/rotary.py
+-rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/servo.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-all-adc.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-all-pwm.py
+-rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/superio-pwm.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/examples/weather.py
+-rw-r--r--   0        0        0    47008 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/__init__.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/common.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/devices.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/encoder.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/ioe_regs.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/motor.py
+-rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/servo.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/ioexpander/sioe_regs.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_io.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_setup.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/tests/test_switch_counter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 pimoroni_ioexpander-0.0.5/PKG-INFO
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/__init__.py` & `pimoroni_ioexpander-0.0.5/ioexpander/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 
 from smbus2 import SMBus, i2c_msg
 
-from . import sioe_regs
-from . import ioe_regs
+from . import ioe_regs, sioe_regs
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 # These values encode our desired pin function: IO, ADC, PWM
 # alongside the GPIO MODE for that port and pin (section 8.1)
 # the 5th bit additionally encodes the default output state
 PIN_MODE_IO = 0b00000   # General IO mode, IE: not ADC or PWM
 PIN_MODE_QB = 0b00000   # Output, Quasi-Bidirectional mode
@@ -19,15 +18,15 @@
 PIN_MODE_OD = 0b00011   # Output, Open-Drain mode
 PIN_MODE_PWM = 0b00101  # PWM, Output, Push-Pull mode
 PIN_MODE_ADC = 0b01010  # ADC, Input-only (high-impedance)
 MODE_NAMES = ("IO", "PWM", "ADC")
 GPIO_NAMES = ("QB", "PP", "IN", "OD")
 STATE_NAMES = ("LOW", "HIGH")
 
-# More convinient names for the pin functions
+# More convenient names for the pin functions
 IN = PIN_MODE_IN
 IN_PULL_UP = PIN_MODE_PU
 IN_PU = PIN_MODE_PU
 OUT = PIN_MODE_PP
 PWM = PIN_MODE_PWM
 ADC = PIN_MODE_ADC
 
@@ -442,15 +441,15 @@
         return self._vref
 
     def enable_adc(self):
         """Enable the analog to digital converter."""
         self.set_bit(self.REG_ADCCON1, 0)
         self._adc_enabled = True
 
-    def disable_adc(void):
+    def disable_adc(self):
         """Disable the analog to digital converter."""
         self.clr_bit(self.REG_ADCCON1, 0)
         if self.REG_AINDIDS1 is not None:
             self.i2c_write16(self.REG_AINDIDS0, self.REG_AINDIDS1, 0)
         else:
             self.i2c_write8(self.REG_AINDIDS0, 0)
         self._adc_enabled = False
@@ -978,22 +977,22 @@
 
     def clear_watchdog_timeout(self):
         self.clr_bit(self.REG_WDCON, 3)  # Clear the WDTRF bit that may have been set from a previous watchdog timeout
 
     def set_watchdog_control(self, divider):
         try:
             wdtdiv = {
-                1: 0b000,
-                2: 0b001,
-                4: 0b010,
-                8: 0b011,
-                16: 0b100,
-                32: 0b101,
-                64: 0b110,
-                128: 0b111,
+                1: 0b000,    # 6.4ms
+                4: 0b001,    # 25.6ms
+                8: 0b010,    # 51.2ms
+                16: 0b011,   # 102.4ms
+                32: 0b100,   # 204.8ms
+                64: 0b101,   # 409.6ms
+                128: 0b110,  # 819.2ms
+                256: 0b111,  # 1.638s
             }[divider]
         except KeyError:
             raise ValueError("A clock divider of {}".format(divider))
 
         wdt = self.i2c_read8(self.REG_WDCON)
         wdt = wdt & 0b11111000  # Clear the WDPS bits
         wdt = wdt | wdtdiv  # Set the new WDPS bits according to our divider
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/common.py` & `pimoroni_ioexpander-0.0.5/ioexpander/common.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/devices.py` & `pimoroni_ioexpander-0.0.5/ioexpander/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import colorsys
+
 import ioexpander
 
 
 class RGBLED:
     def __init__(self, ioe=None, i2c_addr=None, pin_r=1, pin_g=3, pin_b=5, invert=False, brightness=0.05):
         """RGB LED Device.
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/encoder.md` & `pimoroni_ioexpander-0.0.5/docs/encoder.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Encoders <!-- omit in toc -->
 
-The Encoder library provides lets you read incremental rotary encoders from Nuvoton-based boards such as the [Pimoroni IO Expander Breakout](https://shop.pimoroni.com/products/io-expander).
+The Encoder library lets you read incremental rotary encoders from Nuvoton-based boards such as the [Pimoroni IO Expander Breakout](https://shop.pimoroni.com/products/io-expander).
 
 This library offers an `Encoder` class that wraps around the Nuvoton's built-in encoder support, giving access to additional information useful for motor control. Up to 4 encoders are supported.
 
 
-## Table of Content
+## Table of Contents <!-- omit in toc -->
 - [Encoder](#encoder)
   - [Getting Started](#getting-started)
   - [Count and Angle](#count-and-angle)
   - [Count Delta](#count-delta)
   - [Step and Turn](#step-and-turn)
   - [Changing the Direction](#changing-the-direction)
   - [Resetting to Zero](#resetting-to-zero)
   - [Capture](#capture)
-  - [State](#state)
   - [Function Reference](#function-reference)
   - [Constants Reference](#constants-reference)
-  - [Pin Limitations](#limitations)
+  - [Pin Limitations](#pin-limitations)
 
 
 ## Encoder
 
 ### Getting Started
 
 To start using encoders with your expander, you will need to first import the `IOE` and `Encoder` classes, then create your `IOE` object.
@@ -66,15 +65,15 @@
 Often you are not interested in the exact count that the encoder is at, but rather if the count has changed since the last time you checked. This change can be read by calling `.delta()` at regular intervals. The returned value can then be used with a check in code, for the value being non-zero.
 
 
 ### Step and Turn
 
 If using a rotary encoder with a physical direction marker, it can be useful to know its position in the form of which step it is at and how many turns have occurred. The current step can be read by calling `.step()`, which returns a value from zero up to the encoder's `counts_per_rev - 1`. The number of turns can be read by calling `.turn()`.
 
-These functions differ from reading the `.count()` or `.revolutions()` by using seperate counters, and so avoid the wrapping issue that these functions experience.
+These functions differ from reading the `.count()` or `.revolutions()` by using separate counters, and so avoid the wrapping issue that these functions experience.
 
 
 ### Changing the Direction
 
 The counting direction of an encoder can be changed either by providing `direction=REVERSED_DIR` when creating the `Encoder` object, or by calling `.direction(REVERSED_DIR)` at any time in code. The `REVERSED_DIR` constant comes from the `ioexpander.common` module. There is also a `NORMAL_DIR` constant, though this is the default.
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/encoder.py` & `pimoroni_ioexpander-0.0.5/ioexpander/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
-from sys import float_info
 from collections import namedtuple
-from ioexpander.common import NORMAL_DIR, REVERSED_DIR
 from math import pi
+from sys import float_info
+
+from ioexpander.common import NORMAL_DIR, REVERSED_DIR
 
 MMME_CPR = 12
 ROTARY_CPR = 24
 
 
 Capture = namedtuple("Capture", ["count",
                                  "delta",
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/ioe_regs.py` & `pimoroni_ioexpander-0.0.5/ioexpander/ioe_regs.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/motor.md` & `pimoroni_ioexpander-0.0.5/docs/motor.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# Motors with IO Expander<!-- omit in toc -->
+# Motors with IO Expander <!-- omit in toc -->
 
 The Motor library lets you drive DC motors from Nuvoton-based boards such as the [Pimoroni IO Expander Breakout](https://shop.pimoroni.com/products/io-expander) via connected h-bridge drivers.
 
 This library offers a `Motor` class that uses the Nuvoton's hardware PWM to drive a single motor, with support for up to 3 or 6 motors (depending on the chip size).
 
 
-## Table of Content
+## Table of Contents <!-- omit in toc -->
 - [Motor](#motor)
   - [Getting Started](#getting-started)
   - [Control by Speed](#control-by-speed)
     - [Full Speed](#full-speed)
     - [Stopping](#stopping)
     - [Calibration](#calibration)
   - [Control by Percent](#control-by-percent)
   - [Control by Duty Cycle](#control-by-duty-cycle)
     - [Duty Deadzone](#duty-deadzone)
   - [Frequency Control](#frequency-control)
   - [Configuration](#configuration)
     - [Direction](#direction)
     - [Decay Mode](#decay-mode)
-    - [Driver Type](#driver-type)
   - [Delayed Loading](#delayed-loading)
   - [Function Reference](#function-reference)
   - [Constants Reference](#constants-reference)
   - [PWM Limitations](#pwm-limitations)
 
 
 ## Motor
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/motor.py` & `pimoroni_ioexpander-0.0.5/ioexpander/motor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from sys import float_info
+
 from ioexpander import PWM
-from ioexpander.common import clamp, map_float, NORMAL_DIR, REVERSED_DIR
+from ioexpander.common import NORMAL_DIR, REVERSED_DIR, clamp, map_float
 
 FAST_DECAY = 0  # aka 'Coasting'
 SLOW_DECAY = 1  # aka 'Braking'
 
 
 class MotorState():
     DEFAULT_SPEED_SCALE = 1.0  # The standard motor speed scale
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/servo.md` & `pimoroni_ioexpander-0.0.5/docs/servo.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Servos with IO Expander <!-- omit in toc -->
 
 The Servo library lets you drive 3-pin hobby servo motors from Nuvoton-based boards such as the [Pimoroni IO Expander Breakout](https://shop.pimoroni.com/products/io-expander).
 
 This library offers a `Servo` class that uses the Nuvoton's hardware PWM to drive a single servo, with support for up to 6 or 12 servos (depending on the chip size). There is also a `Calibration` class for performing advanced tweaking of each servo's movement behaviour.
 
 
-## Table of Content
+## Table of Contents <!-- omit in toc -->
 - [Servo](#servo)
   - [Getting Started](#getting-started)
   - [Control by Value](#control-by-value)
     - [Common Values](#common-values)
   - [Control by Percent](#control-by-percent)
   - [Control by Pulse Width](#control-by-pulse-width)
   - [Frequency Control](#frequency-control)
@@ -28,38 +28,43 @@
 
 
 ## Servo
 
 ### Getting Started
 
 To start using servos with your expander, you will need to first import the `IOE` and `Servo` classes, then create your `IOE` object.
+
 ```python
 from ioexpander import IOE
 from ioexpander.servo import Servo
 
 ioe = IOE()
 ```
+
 If you are using an expander board that uses the larger Nuvoton chip, then `IOE` should be replaced with `SuperIOE`.
 
 To create your servo, choose which expander pin it will be connected to, and pass that into `Servo`.
+
 ```python
 SERVO = 19
 s = Servo(ioe, SERVO)
 ```
 
 You now have a `Servo` class called `s` that will control the physical servo connected to pin `19`. The pin chosen must support PWM (See [PWM Limitations](#pwm-limitations)).
 
 To start using this servo, simply enable it using:
+
 ```python
 s.enable()
 ```
 
 This activates the servo and moves it to it's last known position. Since this is the first time enabling the servo, there is no last known position, so instead it will move to the middle of its movement range instead.
 
 Once you have finished with the servo, it can be disabled by calling:
+
 ```python
 s.disable()
 ```
 
 From here the servo can be controlled in several ways. These are covered in more detail in the following sections.
 
 
@@ -125,14 +130,15 @@
 
 In addition, any function that performs a load, including the `.load()` function, can be made to wait until the new PWM value has been sent out of the pins. By default this is disabled as for a regular servo this would add up to a 20ms delay, but can be enabled by including `wait_for_load=True` in the relevant function calls.
 
 
 ### Function Reference
 
 Here is the complete list of functions available on the `Servo` class:
+
 ```python
 Servo(pin, calibration=ANGULAR, freq=50)        # calibration can either be an integer or a Calibration class
 pin()
 enable(load=True, wait_for_load=False)
 disable(load=True, wait_for_load=False)
 is_enabled()
 pulse()
@@ -155,14 +161,15 @@
 load(load=True, wait_for_load=False)
 ```
 
 
 ### PWM Limitations
 
 The IO expander chips have limitations on the number of PWM signals, which signals can be controlled independently, and which pins can be used together:
+
 * The regular IO expander has 6 PWM signals on a single hardware module.
 * The larger IO expander has 12 PWM signals split across four hardware modules, with 6 on the first one, then 2 each on the remaining three.
 
 A hardware module is a grouping of PWM signals that are synchronised with each other. This means that parameters such as frequency are shared, which can cause issues if you want one servo to operate at a different frequency to it's channel neighbour or to drive an LED with PWM at a high frequency. This can also be an advantage, by letting the values for multiple servos be "loaded" at the same moment.
 
 The PWM pinout for the regular IO expander is shown below. Note how some of the PWM channels are repeated:
 
@@ -198,14 +205,15 @@
 
 There are three common `type`s of servo's supported:
 * `ANGULAR` = `0` - A servo with a value that ranges from -90 to +90 degrees.
 * `LINEAR` = `1` - A servo with a value that ranges from 0 to +1.0.
 * `CONTINUOUS` = `2` - A servo with a value that ranges from -1.0 to +1.0.
 
 By default all `Servo` classes are `ANGULAR`. This can be changed by providing one of the other types as a parameter during their creation, as shown below:
+
 ```python
 angular = Servo(ioe, 19)  # ANGULAR is the default so does not need to be specified here
 linear = Servo(ioe, 20, LINEAR)
 continuous = Servo(ioe, 21, CONTINUOUS)
 ```
 
 
@@ -215,23 +223,24 @@
 
 ```python
 cal = Calibration()
 cal.apply_two_pairs(1000, 2000, -45, 45)
 s = Servo(ioe, 19, cal)
 ```
 
-This could be useful for example if the servo turning beyond those values would cause damage to whatever mechanism it is driving, since it would not be possible to go to angles beyond these unless limits were disabled (see [Limits](#limits)). Also it lets the exact pulse widths matching the angles be set (the `1000` and `2000` in the example). Discovering these values can take some trial and error, and will offen be different for each servo.
+This could be useful for example if the servo turning beyond those values would cause damage to whatever mechanism it is driving, since it would not be possible to go to angles beyond these unless limits were disabled (see [Limits](#limits)). Also it lets the exact pulse widths matching the angles be set (the `1000` and `2000` in the example). Discovering these values can take some trial and error, and will often be different for each servo.
 
 
 
-# Modifying a Calibration
+### Modifying a Calibration
 
 It is also possible to access and modify the calibration of a `Servo` after their creation. This is done by first getting a copy of the servo's calibration using `.calibration()` or `.calibration(servo)`, modifying its pulses or values, then applying the modified calibration back onto to the servo.
 
 Below, an angular servo is modified to increase its reported rotation range from 180 degrees to 270 degrees.
+
 ```python
 wide_angle = Servo(ioe, 19)
 cal = wide_angle.calibration()
 cal.first_value(-135)
 cal.last_value(+135)
 wide_angle.calibration(cal)
 ```
@@ -245,14 +254,15 @@
 
 Note, even with limits disables, servos still have hard limits of `400` and `2600` microsecond pulse widths. These are intended to protect servos from receiving pulses that are too far beyond their expected range. These can vary from servo to servo though, with some hitting a physical end-stop before getting to the typical `500` and `2500` associated with -90 and +90 degrees.
 
 
 ### Populating a Calibration
 
 To aid in populating a `Calibration` class, there are five helper functions that fill the class with pulse-value pairs:
+
 * `apply_blank_pairs(size)` - Fills the calibration with the specified number of zero pairs
 * `apply_two_pairs(min_pulse, max_pulse, min_value, max_value)` - Fills the calibration with two pairs using the min and max numbers provided
 * `apply_three_pairs(min_pulse, mid_pulse, max_pulse, min_value, mid_value, max_value)` - Fills the calibration with three pairs using the min, mid and max numbers provided
 * `apply_uniform_pairs(size, min_pulse, max_pulse, min_value, max_value)` - Fills the calibration with the specified number of pairs, interpolated from the min to max numbers provided
 * `apply_default_pairs(type)` - Fills the calibration with the pairs of one of the common types
 
 Once a `Calibration` class contains pairs (as checked `.size() > 0`), these can then be accessed by calling `.pair(index)` and can then be modified by calling `.pair(index, pair)`. The former function returns a list containing the pulse and value of the pair, and the latter accepts a list or tuple containing the pulse and value. For situations when only a single element of each pair is needed, `.pulse(index)` and `.value(index)` will return the current numbers, and `.pulse(index, pulse)` and `.value(index, value)` will override them.
@@ -264,14 +274,15 @@
 
 To aid in visualising a calibration's pulse-value mapping, the pulse for any given value can be queried by calling `.value_to_pulse(value)`. Similarly, the value for any given pulse can be queried by calling `.pulse_to_value(pulse)`. These are the same functions used by `Servo` when controlling their servos.
 
 
 ### Function Reference
 
 Here is the complete list of functions available on the `Calibration` class:
+
 ```python
 Calibration()
 Calibration(type)
 apply_blank_pairs(size)
 apply_two_pairs(min_pulse, max_pulse, min_value, max_value)
 apply_three_pairs(min_pulse, mid_pulse, max_pulse, min_value, mid_value, max_value)
 apply_uniform_pairs(size, min_pulse, max_pulse, min_value, max_value)
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/servo.py` & `pimoroni_ioexpander-0.0.5/ioexpander/servo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import namedtuple
+
 from ioexpander import PWM
 from ioexpander.common import clamp, map_float
 
 Pair = namedtuple("Pair", ["pulse", "value"])
 
 ANGULAR = 0
 LINEAR = 1
```

### Comparing `pimoroni_ioexpander-0.0.4/ioexpander/sioe_regs.py` & `pimoroni_ioexpander-0.0.5/ioexpander/sioe_regs.py`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.4/LICENSE` & `pimoroni_ioexpander-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pimoroni_ioexpander-0.0.4/pyproject.toml` & `pimoroni_ioexpander-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -45,53 +45,63 @@
 path = "ioexpander/__init__.py"
 
 [tool.hatch.build]
 include = [
     "/ioexpander",
     "/README.md",
     "/CHANGELOG.md",
+    "/REFERENCE.md",
+    "/docs",
     "LICENSE"
 ]
 
-[tool.hatch.build.targets.dist]
+[tool.hatch.build.targets.sdist]
 include = [
-    "/examples"
+    "*"
+]
+exclude = [
+    ".*",
+    "dist"
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 fragments = [
   { path = "README.md" },
   { text = "\n" },
-  { path = "REFERENCE.md" },
+  { text = "# Reference" },
+  { path = "REFERENCE.md", start-after = "<!-- pypa starts reference here -->" },  # Remove the TOC, since it doesn't work on PyPi
   { text = "\n" },
   { path = "CHANGELOG.md" }
 ]
 
 [tool.ruff]
 exclude = [
     '.tox',
     '.egg',
     '.git',
     '__pycache__',
     'build',
     'dist'
 ]
-line-length = 200
+line-length = 220
 
 [tool.codespell]
 skip = """
 ./.tox,\
 ./.egg,\
 ./.git,\
 ./__pycache__,\
 ./build,\
 ./dist.\
 """
 
+[tool.isort]
+line_length = 220
+
 [tool.check-manifest]
 ignore = [
     '.stickler.yml',
     'boilerplate.md',
     'check.sh',
     'install.sh',
     'uninstall.sh',
```

