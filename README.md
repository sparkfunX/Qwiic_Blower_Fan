Qwiic Blower Fan
========================================

[![Qwiic Blower Fan](https://cdn.sparkfun.com//assets/parts/1/8/0/1/2/18561-Qwiic_Blower_Fan-01.jpg)

[*Qwiic Blower Fan (SPX-18561)*](https://www.sparkfun.com/products/18561)

The unmistakable sounds of a tiny cooling fan spooling up usually means you've sat your laptop on a soft surface, or launched one too many tabs in your browser. It's a textbook cry for help from all of our favorite consumer electronics but what if your next hardware project could also complain about overheating? Well now it can!

In all seriousness, though, sometimes you need to move a little air around. Whether for active cooling or ventilation, a tiny fan can make a big difference. However, a tiny fan also has tiny wires which can make it difficult to work with. We've remedied this issue by mounting it to a board along with the mating flat-flex connector, a voltage booster and an ATtiny-based driver so you can power and control the fan over the Qwiic bus.

The control firmware monitors the tachometer output of the fan in order to implement PI Control over the fan speed, allowing you to set your desired speed in real units. It's also possible to disable the PI control loop and set the speed as a proportion of the maximum. The accompanying Arduino library includes example code for controlling the fan, tweaking settings, and even setting the fan speed based on an attached Qwiic Temperature Sensor and a lookup table.

We're unable to find a datasheet for this fan in particular (which is intended to replace the OEM fan in a Nintendo Switch)

Heads Up! This device draws enough power that it operates at the upper limit of the Qwiic bus. If there are few other devices on the bus and the fan is not allowed to rapidly change throttle, it is possible to power this fan directly from the bus. In some applications, however, it may be necessary to provide the blower fan with a dedicated 3.3V supply.

Repository Contents
-------------------

* **/Firmware** - Control firmware for the ATtiny
* **/Hardware** - Eagle design files (.brd, .sch)
* **/Production** - Panelized hardware files for production

License Information
-------------------

This product is _**open source**_! 

Please review the LICENSE.md file for license information. 

If you have any questions or concerns on licensing, please contact technical support on our [SparkFun forums](https://forum.sparkfun.com/viewforum.php?f=152).

Distributed as-is; no warranty is given.

- Your friends at SparkFun.

_<COLLABORATION CREDIT>_

