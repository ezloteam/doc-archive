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

[Previous](index.html#!docs5/alarm_en_3pro_all.html) [Next](troubleshooting_en_3pro_all.md)

Aeon Home Energy Monitor

If you have version 3.58 or later of the HEM firmware (unrelated toVera 's
firmware), it supports the ability to report in real-time whenever there is a
change in the energy consumption.  It generates a report for Vera whenever
there is a change.

For versions 3.57 and lower, the only way to get real time energy reporting
was to have the HEM send Vera reports constantly, whether or not there was a
change.  This required powering the HEM with USB power.  So we recommend using
the USB port on the HEM to upgrade to firmware 3.58 or newer, as per the
instructions on aeon-labs.com

There have been reported issues with HEM firmware less than 3.61. If you don't
have 3.61, download this file:

US Version: [HEM361](http://wiki.micasaverde.com/images/0/0c/HEM361.zip)

## [Inclusion ](http://wiki.micasaverde.com/index.php?title=Aeon_HomeEnergyMon
itor&action=edit&section=1)

When including the HEM to the Vera unit you should have the HEM powered with
the USB AC adapter.

## [Note ](http://wiki.micasaverde.com/index.php?title=Aeon_HomeEnergyMonitor&
action=edit&section=2)

You need to have it plugged in through the USB AC adapter for it to report the
KWH accurately, because when it is battery operated it sleeps most of the time
and it cannot accurately track KWH.

  

