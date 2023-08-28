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

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Network Troubleshooting](index.html#!docs5/network_troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Initial Connection](index.html#!docs5/initial_connection_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Migrate To Z-wave version 452](index.html#!docs5/migrate_to__en_3Lite_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit_en_3Lite_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote_en_3Lite_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Lite_all.md)

|

[Previous](index.html#!docs5/zwave_troubleshooting_en_3Lite_all.md)
[Next](index.html#!docs5/unit_en_3Lite_all.md)

Migrate To Z-wave version 452

## Introduction

Inside your Vera there is a Z-Wave chip which is upgradeable, meaning Vera can
automatically load either the newer or older Z-Wave firmware into the chip.
Z-Wave has its own firmware, separate from Vera's firmware.  
This means that its routing capabilities are improved and gives Vera the
ability to optimize the Z-Wave network. This is particularly useful in a large
and complex network with lots of Z-Wave devices.  
As of version 3.20 Vera  no longer supports inclusion controllers (ie
SUC/SIS). This feature allowed you to add a secondary, handheld (USB)
controller to the Z-Wave network, and then include additional Z-Wave nodes
using this controller. We recommend new customers to always use the newer
version of Z-Wave.  

You can change which version Vera uses by going to Setup -> Z-Wave Settings
and checking the "Use Z-Wave version 3.20 instead of 2.78" box to use the
newer Z-Wave, or unchecking it to use the older Z-Wave (2.78), and then saving
your changes.  

## Prerequisites

Officially you have to reset your Z-Wave network and rebuild your network from
scratch. While this is not an issue for a new user or a really small network,
some Vera users have large Z-Wave networks already setup with lots of scenes
and will not want to redo everything. Therefore we have developed the
following different methods which should work most of the time, and they
include making a backup so you can go back if it doesn't work.

Before you upgrade it is recommended you run a Z-Wave repair/heal network,
since this will create a reliability rating, or "health score", for all your
Z-Wave nodes. Then after upgrading you can run it again and see if the
reliability has improved. To do this go to Setup -> Z-Wave Settings -> Repair,
and click 'Go'.  
Depending on the size of your network the process will take anywhere from 1
hour for smaller networks, up to 8 hours for networks with 80+ Z-Wave devices.
It's best to start it at night before going to bed so nobody will be manually
using the Z-Wave devices during the test as this can throw the profiling off
so the health score is not accurate. Once the process has completed, return to
the Repair tab and you should be able to view the Repair report using the
pull-down menu. You can save this and compare after you migrate to the newer
Z-Wave firmware.

## Instructions

There are two ways to upgrade your z-wave firmware. The first way is to update
the firmware and build your network from scratch. The second way is to upgrade
the firmware using the "Hack to convert 2.78 to 3.20" option under the
Advanced tab of the Z-Wave Settings page. This second option allows you to
keep your devices and settings without going through the reset z-wave network
procedure.

***NOTE, Before continuing, please make sure to backup your Z-Wave network!**

  1. After upgrading your Vera to the latest firmware go to Setup -> Backup and click on 'Backup Z-Wave network'. Confirm that within a minute or so you get a Backup: Backup done message in the info panel in the top central part of the dashboard. 
  2.  Go to Setup -> Backup. Choose the option "Create Backup". This will give you the option of saving a file called "backup.MiOS2...something". Save this file on your computer somewhere and hold onto it.  

### Update z-wave firmware to the new firmware and build the z-wave network
from scratch

After Vera has finished changing the Z-Wave firmware, you should choose the
"Reset Z-Wave network" button which is in Setup -> Z-Wave Settings ->
Advanced.  
This will clear out your entire Z-Wave network, removing all your devices, and
starting clean. The reason for this is that the way the newer Z-Wave firmware
stores the Z-Wave network data is slightly different.  

If you move from the older to the newer version without doing a reset it is
likely you will not be able to add or remove any nodes.  
This "Reset Z-Wave network" resets the network data in either the newer or
older format from scratch, so the Z-Wave chip will be ready to go.

  1. Go into the Z-Wave option in the toolbox, click the Options tab and choose "Use Z-Wave version 3.20 instead of 2.78". 
  2. You should also check the box "Use MiOS routing instead of Z-Wave (requires 4.5)" and "Limit neighbors to Z-Wave discovery (requiries MiOS routing)". 
  3. Close the popup and click Save. Wait about 5 minutes for Vera to finish flashing the firmware, then go to Setup -> Z-Wave Settings and choose the Options tab and confirm at the top it says "Version: 3.20". 

### Update the z-wave firmware using the "Hack to convert 2.78 to 3.20" option

Using this method will allow you to keep you current settings, included
devices etc. However, if you only have a limited network it's safer
(possibility of corrupting data) to build the 3.20 network from scratch.  
If you build from scratch, Reset Z-Wave network anyway, this will produce a
new House ID and start you with a clean state. You will have to unpair all
your devices in order to include them again.  

  1. Go to Setup -> Z-Wave Settings, click the Options tab and choose "Use Z-Wave version 3.20 instead of 2.78". 
  2. You should also check the box "Use MiOS routing instead of Z-Wave (requires 4.5)" and "Limit neighbors to Z-Wave discovery (requries MiOS routing)". 
  3. Close the popup and click Save. Wait about 5 minutes for Vera to finish flashing the firmware, then go to Setup -> Z-Wave Settings and choose the Options tab and confirm at the top it says "Version: 3.20". 
  4. Reboot or power-cycle your Vera.
  5. Go back into the z-wave devices settings as you did at step 1. click the options tab and tick the "Hack to convert 2.78 to 3.20" box and you will see above "452: 4.52 upgrade ok".  

  6. Click on the Reload button to restart the engine.  

After updating Vera should show this at the top of your options tab of the
z-wave device:

    
    
    Version	3.20 L:1   
    House/Node	   
    Role	Master SIS:NO PRI:YES 

If your role is not shown as above (for instance Role: Suc SIS:YES PRI:NO) you
could try a "Shift controller" from the Advanced tab of the Z-Wave Settings.

### Downgrading to z-wave version 2.78

  1. Unplug Vera's power and reconnect it. 
  2. When Vera starts up, uncheck the "Use Z-Wave version 3.20 instead of 2.78" box, close the popup and save. 
  3. Wait a couple minutes and confirm that the Z-Wave version is now 2.78. 

  

