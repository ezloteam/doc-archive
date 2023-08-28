![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3lite_all.md)

![](skins/mios/images/minus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Network Troubleshooting](index.html#!docs5/network_troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Initial Connection](index.html#!docs5/initial_connection_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit_en_3lite_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote_en_3lite_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device_en_3lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3lite_all.md)

|

[Previous](index.html#!docs5/remote_en_3lite_all.html) [Next](developers_en_3lite_all.md)

Device stopped communicating

**Device stopped communicating with Vera ?**

Please know that the possible reasons for your z-wave device(s) to lose
communication with Vera is caused by one of the following :

-a battery operated device has the batteries discharged so can you please check the batteries and see if it works?

-is the distance between Vera and the device larger than 15 feet ? If so do you have any other z-wave device between Vera and the device to increase the Z-Wave range ? If you do have you added a new device in your Z-Wave network and forgot to do a heal to repair the network ? Please run a repair from Z-Wave Settings > Repair and see if it solves the issue.

-is that device a door lock? If so you will need to add in your z-wave network a security compatible (encryption capable) device which can relay the encrypted signal that the door lock needs to communicate with the Vera unit. 

-are there any devices that use the 900 MHz frequency band like old cellular phones, baby monitoring devices or weather stations ? If so they will interfere with the Z-Wave network and thus cause your devices to stop communicating with Vera so we advise that you move those devices outside of the z-wave network.

-it is recommended that Vera is in a central position of your Z-Wave network so it will do less hops to get to the device you want to control. Is there any way you can re-organize your z-wave network and move your Vera unit in a central position ?

**How to fix the issue ?**

This issue is easily fixed by excluding and re-including the device that is
causing issues in your Z-Wave network. To do this you will need to put Vera in
Exclude mode to remove them and Include mode to add them. You can do this
either by taking your Vera unit with the battery provided to your devices or
if you can bring your devices closer to Vera you can use the Full Power
Inclusion method explained [here](http://docs5.mios.com/doc.php?language=1&man
ual=1&platform=3Pro&page=full_power_inclusion).

  

