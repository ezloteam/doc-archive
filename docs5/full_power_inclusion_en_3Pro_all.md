![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3Pro_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Pro_all.md)

![](skins/mios/images/minus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Advanced Settings](index.html#!docs5/advanced_settings_en_3Pro_all.md)

![](images/spacer.gif)[Add Z-Wave Dongle With Different Frequency](index.html#!docs5/changing_zwave_port_en_3Pro_all.md)

![](images/spacer.gif)[Z-Wave Advanced Options](index.html#!docs5/zwave_device_advanced_en_3Pro_all.md)

![](images/spacer.gif)[Full/Low Power Inclusion/Exclusion](index.html#!docs5/full_power_inclusion_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Pro_all.md)

|

[Previous](index.html#!docs5/zwave_device_advanced_en_3Pro_all.md)
[Next](index.html#!docs5/supported_hardware_en_3Pro_all.md)

Full/Low Power Inclusion/Exclusion

In order to use Z-Wave devices, those devices must be "paired" or "included"
into the unit Z-Wave network. Generally this is done by bringing the zwave
unit within 3 feet (1 meter) of the Z-Wave device you want to include and then
turn on/off or otherwise activating the Z-Wave device. This is called "low
power inclusion" because the wireless signals used to talk with the Z-Wave
device are intentionally sent at a very low power so that only devices that
are very close to the dongle will get included. This way if you live in an
apartment, and your neighbors also have Z-Wave devices, you do not need to
worry that one of their Z-Wave devices might get activated and thereby
included in your Z-Wave network by mistake. The other advantage to the
standard low power inclusion is that you get immediate feedback if the new
Z-Wave device was successfully paired because the blinking light momentarily
stops blinking. This is particularly useful if you're having trouble pairing a
node because you can [Reset Node|reset the node] and get instant feedback that
it's working.  
  
If there are no neighbors within a 20 foot (about 6 meter) range of your
Z-Wave unit, you might also try "full power inclusion". This means you leave
the Z-Wave unit at its place, you don' need to disconnect it and bring it
closer to the Z-Wave devices, and it will use the normal, full power setting
of the Z-Wave network to try to include nodes.  
| ![](/images/mios/UI5_includeFULL.PNG)![](/images/mios/UI5_excludeFull.PNG)  
---  
To do this, go to Devices->Add Devices, scroll at the bottom of the page and
choose 'Advanced Z-Wave devices' .  Scroll down on to the bottom of the next
page.  
Using the pull-down menu to the left of the "Go" button, change 'low power' to
'full power'.  
If you want to reset/exclude nodes, instead of including them, change the
first pull-down menu to 'Exclude'.  
If you leave the 2nd pull-down at 'one', then as soon as the Z-Wave Gateway
has included/excluded one node, it will stop trying. If you change it to say
'Multiple', then for however many seconds you specify in the 'Timeout' box
(default 30 seconds) you can include/exclude as many nodes as you want.  
You can also change the 'Type' pull down if you want to limit the type of
nodes being included/excluded.  
When you're all done, click "Go".  
  
Full power inclusion doesn't always work. Only newer Z-Wave devices support
it, and, they don't always support the full 'mesh network' functions needed to
reliably include. So you can use full power inclusion to pick up as many nodes
as you can, and then carry the Z-Wave unit around to pick up the nodes that
you couldn't get with full power inclusion.

  

