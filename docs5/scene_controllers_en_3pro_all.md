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

![](skins/mios/images/plus.gif)[Lighting Devices](index.html#!docs5/lighting_devices_en_3pro_all.md)

![](images/spacer.gif)[Plug and Receptacle Devices](index.html#!docs5/plug_devices_en_3pro_all.md)

![](images/spacer.gif)[Thermostats](index.html#!docs5/thermostats_en_3pro_all.md)

![](images/spacer.gif)[Window Coverings](index.html#!docs5/window_coverings_en_3pro_all.md)

![](images/spacer.gif)[Sensors](index.html#!docs5/sensors_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Scene Controllers](index.html#!docs5/scene_controllers_en_3pro_all.md)

![](images/spacer.gif)[Leviton Scene Controller](index.html#!docs5/leviton_scene_controller_en_3pro_all.md)

![](images/spacer.gif)[Intermatic Handheld Remotes](index.html#!docs5/ha07,_ha09,_intermatic_en_3pro_all.md)

![](images/spacer.gif)[Intermatic CA5100](index.html#!docs5/Intermatic_CA5100_en_3pro_all.md)

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

[Previous](index.html#!docs5/sensors_en_3pro_all.md)
[Next](index.html#!docs5/leviton_scene_controller_en_3pro_all.md)

Scene Controllers

If you want to use a secondary controller with Vera you should keep in mind
that there are two ways of adding scenes on the secondary controller.  
Some controllers support copying the scenes directly from the Vera unit and
you can easily click on the Setup button on the scene controller itself, go to
the Scenes tab and assign each button to one of the scenes you already saved
on the Vera unit.  
With other types of controllers which are not supporting this capability, you
will have to create the scenes and in each scene you want to use with that
controller, you have to create a [trigger](index.html#!docs5/triggers_en_all_all.md), select
the scene controller and choose as event **'A scene is activated'**, then fill
in the scene number you want to activate on the scene controller itself.

Note: Please keep in mind that #2 Scene Controller (Device number 2) is Vera's
own integrated Scene controller. To set up a trigger for your scene controller
you have to make sure to choose the right device.

  

