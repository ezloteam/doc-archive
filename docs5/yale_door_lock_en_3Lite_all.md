![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3Lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Door locks](index.html#!docs5/door_locks_en_3Lite_all.md)

![](images/spacer.gif)[Kwikset Door Lock](index.html#!docs5/kwikset_lock_en_3Lite_all.md)

![](images/spacer.gif)[Schlage Door Lock](index.html#!docs5/schlage_lock_en_3Lite_all.md)

![](images/spacer.gif)[Yale Door Lock](index.html#!docs5/yale_door_lock_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Lighting Devices](index.html#!docs5/lighting_devices_en_3Lite_all.md)

![](images/spacer.gif)[Plug and Receptacle Devices](index.html#!docs5/plug_devices_en_3Lite_all.md)

![](images/spacer.gif)[Thermostats](index.html#!docs5/thermostats_en_3Lite_all.md)

![](images/spacer.gif)[Window Coverings](index.html#!docs5/window_coverings_en_3Lite_all.md)

![](images/spacer.gif)[Sensors](index.html#!docs5/sensors_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Scene Controllers](index.html#!docs5/scene_controllers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3Lite_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Alarm panels](index.html#!docs5/alarm_en_3Lite_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Lite_all.md)

|

[Previous](index.html#!docs5/schlage_lock_en_3Lite_all.md)
[Next](index.html#!docs5/lighting_devices_en_3Lite_all.md)

Yale Door Lock

###  Adding/pairing the door lock into a Z-Wave network:

Please note that when pairing secure devices like door locks you will have to
use the [full power inclusion
mode](index.html#!docs5/http://docs5.mios.com/full_power_inclusion_en_all_all.md) from the
Dashboard.

I. Put Vera in include mode by using the full power inclusion mode:

1\. Go to Vera's Dashboard

2\. Click on Add button from Devices -> Add devices -> Advanced Z-Wave devices

3\. Scroll all the way down and select: Include, one node, with full power and
timeout after 90 or 120 seconds and hit Go

II. Do the include procedure on the door lock:  
1\. Enter the 4-8 digit Master PIN code followed by the # key  
2\. Press 7 followed by the # key. (*This function appears only with network
module installed)  
3\. Press 1 followed by the # key to include the door lock.  
      
CAUTION: When joining a network your controller may or may not be aware of any
previously saved user codes stored in the lock. It is recommended that all
user codes be deleted from the lock prior to joining a network.

  

###  Deleting/Removing the door lock from a Z-Wave network:

1\. Put Vera in exclude mode, by using the full power exclude mode (same as
above, only instead of Include, select Exclude)

2\. Enter the 4-8 digit Master PIN code followed by the # key

3\. Press 7 followed by the # key. (*This function appears only with network
module installed)

4\. Press 3 followed by the # key to exclude the door lock.  



### Adding a pin code  

To add a pin code, you will need to click on the 'wrench icon', click on the
'Pin codes' tab, check the check-box near 'Keep a copy of my pin codes', then
enter the name 'New code name: ', after that enter the actual pin code next to
'4-8 digit code: ', then click 'Set', and click the Save button in top right
corner of the Dashboard.

  

