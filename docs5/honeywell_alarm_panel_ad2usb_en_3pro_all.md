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

![](skins/mios/images/minus.gif)[Alarm panels](index.html#!docs5/alarm_en_3pro_all.md)

![](images/spacer.gif)[DSC Alarm Panel](index.html#!docs5/dsc_en_3pro_all.md)

![](images/spacer.gif)[Elk M1 Alarm Panel](index.html#!docs5/elk_m1_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Honeywell Ademco Vista Alarm Panels via AD2USB](index.html#!docs5/honeywell_alarm_panel_ad2usb_en_3pro_all.md)

![](images/spacer.gif)[Honeywell / Ademco Alarm Panels with RS-232 Interface](index.html#!docs5/honeywell_alarm_panel_rs232_en_3pro_all.md)

![](images/spacer.gif)[Paradox EVO Alarm Panels](index.html#!docs5/paradox_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Visonic Powermax Alarm Panel](index.html#!docs5/visonic_powermax_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/elk_m1_alarm_panel_en_3pro_all.md)
[Next](index.html#!docs5/honeywell_alarm_panel_rs232_en_3pro_all.md)

Honeywell Ademco Vista Alarm Panels via AD2USB

## Connecting the panel to Vera[ ](http://code.mios.com/trac/mios_vista-alarm-
panel-ad2usb#ConnectingthepaneltoVera)

The panel must be connected to Vera using the AD2USB keypad emulator. You will
need a **Mini USB B** to **USB A** cable to connect the AD2USB to Vera.

Follow the instructions in the AD2USB guide to connect the AD2USB to the alarm
panel. Here are some useful links:

  * [​http://www.nutech.com/index.php?option=com_fireboard&Itemid=74&func=view&catid=4&id=13](http://www.nutech.com/index.php?option=com_fireboard&Itemid=74&func=view&catid=4&id=13)
  * [​http://www.nutech.com/index.php?parent_id=1&option=com_easyfaq&Itemid=84](http://www.nutech.com/index.php?parent_id=1&option=com_easyfaq&Itemid=84)

# Installation and Setup

## Setup

First go to **Apps** >> **Install Apps** and install the plugin, then follow
the steps below:

  1. In the alarm panel device control panel open the **Advanced** tab and enter the number of active partitions in the **NumPartitions** input field. 

**Warning:** The plugin might not work correctly if this number is incorrect. 

![](/images/mios/UI_5_en_mios_ademco1.png)  

  2. Save. After restart, a device for each partition is created (e.g _Ademco Vista Partition 1_). 
  3. In the partition's control panel, open the **Advanced** tab and in the **KeypadAddresses** input field enter the addresses of the keypads assigned to this partition. If there are more than one keypad for a partition, enter the addresses of each keypad separated by a comma (e.g. If the keypads at addresses 17, 19 and 23 are assigned to this partition, the _KeypadAddresses_ will be _17,19,23_). Repeat this for all the partition devices. 

**NOTE #1:** The AD2USB's address should be added to the keypad addresses list for any partition. 

**NOTE #2:** If the _KeypadAddresses_ field doesn't exist, reload the web page. 

**WARNING**: The plugin won't work correctly if these variables aren't correctly set.   

![](/images/mios/UI_5_en_mios_ademco2.png)

  

  4. Save. 
  5. Go to **Apps** -> **Develop Apps** -> **Serial Port configuration**. Set the **Baud** to _115200_ and select the alarm panel device from the **Used by device** drop-down list. Optionally, you can enter a name for the serial port in the **Name** field. 

**NOTE:** If the port is not on the serial port list, first make sure that the AD2USB is connected to Vera, then restart Luup. After restart, try this step again. 

![](/images/mios/UI_5_en_mios_ademco3.png)  

  6. Save. If everything works OK you should see the partition status updating. 

For more information please visit:

[http://code.mios.com/trac/mios_vista-alarm-panel-
ad2usb](javascript:void\(0\);/*1333037280155*/)  

  

