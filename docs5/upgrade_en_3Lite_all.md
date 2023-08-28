![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Guided Feature Walkthroughs
](features_en_3Lite_all.html)

![](images/spacer.gif)[Walkthrough: Keyless Go](index.html#!docs5/keyless_en_3Lite_all.md)

![](images/spacer.gif)[Walkthrough: Video Archiving](index.html#!docs5/video_archiving_en_3Lite_all.md)

![](images/spacer.gif)[Walkthrough: Energy Logging](index.html#!docs5/energy_logging_en_3Lite_all.md)

![](images/spacer.gif)[Walkthrough: Bridged Z-Wave with Multiple Vera](index.html#!docs5/multiple_units_en_3Lite_all.md)

![](images/spacer.gif)[Include and Exclude](index.html#!docs5/include_mode_en_3Lite_all.md)

![](images/spacer.gif)[Upgrade from Vera 2 to Vera 3/Vera Lite](index.html#!docs5/upgrade_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Lite_all.md)

|

[Previous](index.html#!docs5/include_mode_en_3Lite_all.md)
[Next](index.html#!docs5/web_portal_en_3Lite_all.md)

Upgrade from Vera 2 to Vera 3/Vera Lite

To upgrade from Vera 2 to Vera 3/Vera Lite you must first make sure you have
the latest UI5 firmware. If, on Vera 2, you have UI4 you must upgrade to the
latest firmware of UI4, and after that, to upgrade to UI5, you must go from
the same network as your Vera to:

<https://cp.mios.com/firmware>

After the upgrade, you must go to Setup -> Backup, click "Backup Z-Wave
network", then click "Create backup", save the file on the computer. Then, on
your Vera 3/Vera Lite you must go to Setup -> Backup, select "Restore Z-Wave
network", click "Browse", select the backup file saved on the computer, then
click "Restore".

Note: If you select Restore Z-Wave network, all the data stored on the Z-Wave
chip will be restored including the Z-Wave version, role, home id, devices,
etc.

Please make sure that, when you go on the Dashboard of Vera 3/Vera Lite to
Setup -> Z-Wave Settings, you have next to Port: /dev/ttyS0

If you don't have this please modify it and click the Save button.  



  

