![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3pro_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3pro_all.md)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3pro_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Alarm panels](index.html#!docs5/alarm_en_3pro_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/infrared_en_3pro_all.html) [Next](alarm_en_3pro_all.md)

Insteon Devices

Here's a quick walkthrough of how to get started with Insteon/X10 in Vera.

1\. Connect a SmartLabs 2413U **PowerLinc Modem** to one of Vera's USB ports.
Alternatively, you can use a 2412S (RS-232) version and this Serial to USB
adapter: <http://www.futureelectronics.com/en/Technologies/Product.aspx?Produc
tID=UC232R10FUTURETECHNOLOGYDEVICES2297802>

2\. Go to Vera's Setup page in your browser and click 'Setup', 'Insteon
Settings'. If you see the message: "Insteon interface not found, do you want
to enable it?", click the 'Enable it' button. Wait a minute for Vera to enable
the Insteon/X10 module and find the PowerLinc.

3\. To add Insteon devices, click the 'Add INSTEON or X10 devices, like light
switches, thermostats, sensors, etc' button. To add X10 devices, choose the
device type, house code and unit code in the 'Add an X10 device' section, then
click 'go'.

4\. When you've added new Insteon devices and Vera doesn't yet know what room
they're in, you will see the 'unassigned devices' page, which shows you the
new devices and asks you to pick the room the device is in. Do this and click
continue.

5\. If Vera was successfully able to talk to your Insteon device, you should
see it on your dashboard. You can click the wrench key on that device to see
more detailed information, including it's ID.

Refer to the page [Insteon Supported
Hardware](http://wiki.micasaverde.com/index.php/Insteon_Supported_Hardware)
for notes on specific Insteon devices and how they work.  
  

  * **NOTE**: To control Insteon devices you need a Power Link MODEM (not a controller). For example the 2414U won't work because it's an Insteon controller (not a modem) and uses a different protocol. 
  * **NOTE**: The Insteon devices use a mix of proprietary RF signals and powerline signal. In most cases Insteon devices run over powerline, and should connect to the Insteon Modem using the electrical wiring. However, if your house has a main breaker and one or more subpanels and Vera is tied to one subpanel and the devices are on another subpanel or on the main power panel, will not receive signals of the Insteon devices. PLM communications do not go across power panels! So you should have your Vera and the Insteon devices on the same circuit breaker panel. 

  

