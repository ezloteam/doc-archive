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

![](skins/mios/images/minus.gif)[IR devices](index.html#!docs5/infrared_en_3pro_all.md)

![](images/spacer.gif)[SQBlaster](index.html#!docs5/sqblaster_en_3pro_all.md)

![](images/spacer.gif)[USB UIRT](index.html#!docs5/USB_en_3pro_all.md)

![](images/spacer.gif)[GC100](index.html#!docs5/gc100_en_3pro_all.md)

![](images/spacer.gif)[iTach](index.html#!docs5/itach_en_3pro_all.md)

![](images/spacer.gif)[Remotec IRBlaster](index.html#!docs5/remotec_en_3pro_all.md)

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

[Previous](index.html#!docs5/itach_en_3pro_all.html) [Next](Insteon_en_3pro_all.md)

Remotec IRBlaster

The Remotec IRBlasters are partially supported in firmware versions 1.5.346
and higher.

1\. If you haven't already included them in your network, go to Device, Add
Devices, Add Z-Wave devices, and include the Remotec like any other Z-Wave
device. The 'z-wave include' button is marked PROG on the side of the 6-port
blaster, and it's the big black round button on the top of the single port
blaster.

2\. After it is included, go to Devices, Add Device, and choose Add IR Device.

3\. Choose the IR Blaster from the 'use transmitter' pull-down. If you have a
6-port blaster, you will see the blaster + 6 ports. NOTE: In firmware 1.5.346
you should choose the blaster itself, not one of the 6 ports.

4\. Choose 'Manual setup' because the Remotec blasters have their own
codesets.

5\. You will then need to enter the codeset number. Do not enter the 0 in
front of a codeset. If the manual says 0251, use 251. If you have multiple
codesets, or are not sure which one is best, you can enter several codesets
separated with a comma. For example, if you have a Samsung TV, you'll see
there are 6 possible codesets. If you don't know which one to use, enter them
all like this: 251,261,351,1191,1311,1911

6\. After you click 'Create Device', your new device will appear on the
Devices, A/V Gear. Choose the 'control' button to bring up the remote control
to test your new device.

7\. If you entered multiple codesets, and the remote isn't working, there's a
button in the upper right corner of the remote to toggle through all the
codesets. It will say #1 at first, meaning, we'll be using the first codeset
you entered. Click it to try the second codeset, third, etc., until you've
tried them all and it comes back to #1. Try each one until you find the one
that works best. It will continue to use whatever is the last codeset you
selected, so you only need to do this once. If you only entered one codeset,
this button will not be there.

NOTE: Due to a bug in 1.5.346, it won't automatically program the remotec with
the codeset you entered until you hit the button described in step 7. So if
you add a device with only 1 codeset it won't work. A temporary workaround is
that if you you must enter at least 2 codesets. If the codeset is 251, then
enter codesets 1,251 in step #5. This way you can hit the #1 button in step 7
to cycle to the 2nd codeset, and it will program the Remotec to use codeset
#251. This bug only affects release 1.5.346.

Note that once you have confirmed the device is working, you can include this
A/V device in scenes.

  

