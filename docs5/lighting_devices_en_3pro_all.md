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

![](skins/mios/images/minus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Door locks](index.html#!docs5/door_locks_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Lighting Devices](index.html#!docs5/lighting_devices_en_3pro_all.md)

![](images/spacer.gif)[Smart Switch](index.html#!docs5/smart_switch_en_3pro_all.md)

![](images/spacer.gif)[Plug and Receptacle Devices](index.html#!docs5/plug_devices_en_3pro_all.md)

![](images/spacer.gif)[Thermostats](index.html#!docs5/thermostats_en_3pro_all.md)

![](images/spacer.gif)[Window Coverings](index.html#!docs5/window_coverings_en_3pro_all.md)

![](images/spacer.gif)[Sensors](index.html#!docs5/sensors_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Scene Controllers](index.html#!docs5/scene_controllers_en_3pro_all.md)

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

[Previous](index.html#!docs5/door_locks_en_3pro_all.html) [Next](smart_switch_en_3pro_all.md)

Lighting Devices

Lighting devices are in-wall switches that let you control scenes, local
loads, and any other device through Vera.  
  
Supported Lighting Devices

  * Light Switches
    * [Smart Switch](index.html#!docs5/smart_switch_en_all_all.md)  

  * [Scene Controllers](index.html#!docs5/scene_controllers_en_all_all.md)
    * [Leviton Scene Controller](index.html#!docs5/leviton_scene_controller_en_all_all.md)
  * Also see user-maintained [wiki page](http://wiki.micasaverde.com/index.php/Supported_Hardware#Lighting_Devices)
Scene Controller Commands  

  * Set LED x ON
  * Set LED x OFF
Scene Controller Events  

  * A Scene is Activated  

    * Event fires when the scene number you specified is turned on
  * A Scene is De-Activated
    * Note: Different scene controllers implement this differently. Some scene controllers activate scenes 1-4, but de-activate scene 0. Check your scene controller's manual for more detail
Lighting Device Commands  

  * Set ON
    * Turns a switch on
    * Sets a dimmer to full brightness
  * Set OFF
    * Turns a switch off
    * Turns a dimmer completely off
  * Set level to x%
    * Dimmers only
    * Sets the dimmer to x% 
Lighting Device Events  

  * A device is turned on
    * This event happens whenever a device was off and is now on.
    * Note: sometimes we won't know that a device has turned on or off until we've polled it, which could take minutes or more depending on your network size.
  * A device is turned off

  

