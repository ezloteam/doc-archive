![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Guided Feature Walkthroughs
](features_en_3pro_all.html)

![](images/spacer.gif)[Walkthrough: Keyless Go](index.html#!docs5/keyless_en_3pro_all.md)

![](images/spacer.gif)[Walkthrough: Video Archiving](index.html#!docs5/video_archiving_en_3pro_all.md)

![](images/spacer.gif)[Walkthrough: Energy Logging](index.html#!docs5/energy_logging_en_3pro_all.md)

![](images/spacer.gif)[Walkthrough: Bridged Z-Wave with Multiple Vera](index.html#!docs5/multiple_units_en_3pro_all.md)

![](images/spacer.gif)[Including and Excluding](index.html#!docs5/include_mode_en_3pro_all.md)

![](images/spacer.gif)[Upgrade from Vera 2 to Vera 3/Vera Lite](index.html#!docs5/upgrade_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/energy_logging_en_3pro_all.md)
[Next](index.html#!docs5/include_mode_en_3pro_all.md)

Walkthrough: Bridged Z-Wave with Multiple Vera

There are several reasons why you might want to have multiple Vera in one
home.  For example, you might want a Vera to be physically located next to an
alarm panel. You can connect it to the alarm panel with a serial cable.  
  
One of the most common reasons is to improve the reliability of Z-Wave
devices.  Z-Wave devices are 'mesh networks'. This means if device a needs to
control device b, but they're not in direct range for the wireless radio
signal to reach, then other Z-Wave devices in between a and b will act as
relays.  However, there are limitations to this, such as a limit to the number
of hops a message can make. The signal may not travel through some barriers
like brick walls, you may have a 'dead zone' area in your home where there are
no nodes or other interference, or you may have separate areas like a main
house and a guest house.  
  
Z-Wave is quite reliable when you have several Z-Wave devices in a small area
so the number of hops is kept to a minimum.  You may want to put one Vera in
the main house, another in the guest house, or divide the main house in 2
halves with a Vera right in the middle of each half so that most Z-Wave
devices are in direct range of the Vera.  There is no limit to the number of
Vera you can have in your home and, so long as they are all connected to the
same home LAN (ie Ethernet network), multiple Vera's can be bridged so they
act as one.  
  
The way bridging works is that you go to one Vera and "import" or add the
other one.  So, Vera #1 can import the devices from Vera #2 and Vera #3, and
that way on Vera #1 you will see all devices from all 3 Vera systems together
as though it was one system.  You can create scenes and events on Vera #1 that
control devices from all 3 Vera, and you can attach events to those scenes
that are triggered by devices on all 3 Vera systems.  When you control Vera #1
from the web interface or a mobile phone interface, you will have control over
all devices from all 3 Veras.  
  
There are no limitations on importing other Vera systems.  So, technically if
you had 3 systems, #1 could import the devices on #2 and #3, and #3 could
import the devices on #1 and #2, and in that way both #1 and #3 would have all
the devices.  This, however, might lead to confusion, particularly if you have
scenes and events on both #1 and #3. You might see things happening and not
know which Vera is actually doing what.  To keep it simple, the best solution
is to generally think of one Vera as the "Master" and have it import the
devices from all the other "Slaves", and then create scenes and events only on
the "Master".  You won't need to do anything with the "Slaves" except include
the devices and modify the device settings for those devices. On the "Master",
the 'setup' icon on the dashboard ![](images/mios/setup_icon_UI5.png) will
only let you change settings for the Master's native devices.  To change
settings for a device, such as Z-Wave variables, you will need to use whatever
Vera included those devices natively.  
  
To import the devices from another Vera:

  * Click Devices and go to "Add devices" tab  

  * Scroll down in Add/remove device window and click Add "UPnP devices"
![Addupnp](/images/mios/UI5_Addupnp2\(1\).png)

  * Check the checkbox "Scan for UPnP devices" and "Save"
  * Wait 10 minutes for Vera to scan the device's from the other Vera's Z-Wave network
  * Click the Next button under Devices/Add Devices/UPnP devices "Add control over another UPnP device, such as another Vera."
![ADD_UPNP2](/images/mios/UI5_Addupnp2.png)  

  * Click add for the Vera system that you want to be able to control from this Vera
  * You're done. You've successfully bridged two Z-Wave networks with Vera

  

