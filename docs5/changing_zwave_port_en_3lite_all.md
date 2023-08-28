![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3lite_all.md)

![](skins/mios/images/minus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Advanced Settings](index.html#!docs5/advanced_settings_en_3lite_all.md)

![](images/spacer.gif)[Add Z-Wave Dongle With Different Frequency](index.html#!docs5/changing_zwave_port_en_3lite_all.md)

![](images/spacer.gif)[Z-Wave Advanced Options](index.html#!docs5/zwave_device_advanced_en_3lite_all.md)

![](images/spacer.gif)[Full/Low Power Inclusion/Exclusion](index.html#!docs5/full_power_inclusion_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3lite_all.md)

|

[Previous](index.html#!docs5/advanced_settings_en_3lite_all.md)
[Next](index.html#!docs5/zwave_device_advanced_en_3lite_all.md)

Add Z-Wave Dongle With Different Frequency

  
Installing the dongle  
If you have an external Z-Wave dongle with different frequency or you want to
use a dongle instead of the built-in Z-Wave module, you can easily do that by
changing a variable on the Z-Wave Device setting in the Dashboard.  
  
This setting is located in Setup -> Z-Wave settings -> Options -> Port. (see
picture below)  
  
By default, Vera comes with a built-in z-wave chip, which is available at port
/dev/ttyS0 .  
  
If you attach an External Z-Wave dongle, you need to change this port to be
/dev/ttyUSB0  
  
Important: After you make this change, just save the settings and the Z-Wave
network will restart and re-configure.  
  
  
Functionality  
  
When the dongle is inserted in Vera you will see it blinking constantly. This
means it has been detected and is functioning.  
Whenever you try to include a new device without removing the dongle from the
USB port you will have to use the same button on the Vera and check the status
of the Z-Wave LED on the gateway, and not on the dongle.  
  
Note:  While the dongle is connected to Vera, the LED on the dongle should be
blinking constantly, wether the unit is in include mode or not and pressing
the dongle button, shouldn't have any effect.  
  
  
  
![](/images/mios/UI5_port1.PNG)

  

