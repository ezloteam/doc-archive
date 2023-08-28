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

[Previous](index.html#!docs5/dsc_en_3pro_all.md)
[Next](index.html#!docs5/honeywell_alarm_panel_ad2usb_en_3pro_all.md)

Elk M1 Alarm Panel

# Connecting the panel to Vera

There are 3 ways to connect the panel to Vera:

  * Using an **USB RS-232 Serial Adapter** like [​this one](http://www.usbgear.com/computer_cable_details.cfm?sku=USBG-232MM&cats=199&catid=199%2C461%2C106%2C1009%2C601). For best compatibility with Vera, I recommend a serial adapter with **FTDI** or **Prolific** chipset. 
  * Using a wired Ethernet connection with the [​Elk-M1XEP Ethernet Interface](http://www.elkproducts.com/_webapp_2981439/ELK-M1XEP_M1_Ethernet_Interface). 
  * Using a **WiFi RS-232 Serial Adapter** like [​this one](index.html#!docs5/http://www.gridconnect.com/wi232.md). 

The first 2 options are preferable because they are easier to setup and more
reliable.  

# Installation and Setup

## Preliminary steps

### USB RS-232 Serial Adapter

If the panel has been connected to Vera using an USB RS-232 Serial Adapter,
first check to see if the serial port has been detected by Vera:

  1. Open the Vera UI. 
  2. Navigate to **Apps** >> **Develop Apps** >> **Serial Port Configuration**. 
  3. If you don't see the serial port in the list, restart Luup. 
  4. Configure the serial port: 
    * Set the **Baud** to _115200_. 
    * Optionally you can give a name to this serial port in the **Name** field. 
  5. Save. 

### Elk M1XEP

Follow the installation and configuration procedure in the **M1XEP
Installation Manual**.

### WiFi RS-232 Serial Adapter

Follow the installation and configuration procedure from its manual. The
serial port must be configured to use a **Baud rate** of _115200_.

## Setup

First go to **Apps** >> **Install Apps** and install the plugin, then follow
the steps below:

### Panel connected to Vera on **USB** port using an USB RS-232 Serial Adapter

  1. Go to **Apps** >> **Develop Apps** >> **Serial port configuration** and select the alarm panel device from the **Used by device** drop-down list. 
  2. Save. 
  3. After Luup has restarted reload the UI. 

![](/images/mios/UI_5_en_mios_elk1.png)  

### Panel connected to Vera on **Ethernet** port using Elk-M1XEP or
**wireless** using WiFi RS-232 Serial Adapter

  1. Open the alarm panel device control panel >> **Advanced** tab. In the **ip** input field enter the IP address of the Ethernet adapter and the port on which it is connected. (e.g. if the IP address of the Ethernet adapter is _192.168.8.164_ and it is connected on port _5000_, the **ip** value should be _192.168.8.164:5000_) 
  2. Save. 
  3. After Luup has restarted reload the UI. 

![](/images/mios/UI_5_en_mios_elk2.png)



For more information please visit:

<http://code.mios.com/trac/mios_elk-alarm-panel/wiki/WikiStart>

  

  

