![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3pro_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Advanced Settings](index.html#!docs5/advanced_settings_en_3pro_all.md)

![](images/spacer.gif)[Add Z-Wave Dongle With Different Frequency](index.html#!docs5/changing_zwave_port_en_3pro_all.md)

![](images/spacer.gif)[Z-Wave Advanced Options](index.html#!docs5/zwave_device_advanced_en_3pro_all.md)

![](images/spacer.gif)[Full/Low Power Inclusion/Exclusion](index.html#!docs5/full_power_inclusion_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/changing_zwave_port_en_3pro_all.md)
[Next](index.html#!docs5/full_power_inclusion_en_3pro_all.md)

Z-Wave Advanced Options

Here you have various advanced Z-Wave options. Use these options only if you
understand what they mean. Most users will not need these options.  
  

**Reset Z-Wave network** purges all data in Vera's Z-Wave chip, which also clears out the list of Z-Wave devices paired to Vera. You will then need to [reset any devices](http://wiki.micasaverde.com/index.php/Reset_Node) you previously paired, and pair them again. If you also want to get rid of your scenes, network settings, users, network devices, etc., you can do a full [factory reset](http://wiki.micasaverde.com/index.php/Factory_Reset). 

**WARNING**: This process is **IRREVERSIBLE**, you cannot restore your devices from a backup, you have to pair each of them again. Before proceeding you have to manually unpair all the devices, otherwise you will create duplicate nodes which will compromise your Z-Wave network. 

  
If you already have another Z-Wave controller that you want to be the master,
and you want Vera to be the secondary controller, bring the master controller
and Vera close to each other, tell the current master controller to start
sending network data or to add another Z-Wave controller, and then click
**Copy Z-Wave network from a master controller**. You will see the status of
the transfer in blue at the top of the page, and Vera will tell you if it was
successful. The "Role" shown on the 'Options' tab will then also change a
minute or so later.

**Controller shift** tells Vera to transfer the role of primary controller to another Z-Wave controller. After you click 'Controller Shift,' proceed to add the other Z-Wave controller the same way you normally would, as explained [here](http://wiki.micasaverde.com/index.php/ZWave_Add_Controller). The difference between adding the controller by clicking 'Controller Shift' versus adding the controller the normal way by clicking 'Add ZWave controller', is that if you choose 'Controller Shift', at the end when the other Z-Wave controller gets added, that other ZWave controller will become the 'Master controller', and Vera will be a secondary controller. This means the other Z-Wave controller will then be responsible for healing the networking and being the SIS/SUC (a technical Z-Wave term). Normally, by default, Vera is the master controller and is SIS/SUC.   

Reset Z-Wave chip will send a software reset to the Z-Wave chip. This will
restart the code written on it. It will not cause any loose of data.

Backup Z-Wave network:

The Z-Wave chip maintains the master list of all the other Z-Wave devices that
you have included into your Z-Wave network. Vera also maintains its own
database with a list of devices, and Vera's database has a lot more detail,
such as the name of the device, the room that it's in and so on. Vera
continually syncs its database with the master list of devices in the Z-Wave
chip. This is why you can carry it around to pair and unpair devices, and Vera
will show any new or removed devices. If change your Z-Wave unit, then all
your devices will disappear since the new one doesn't have any devices paired
to it and so Vera deletes the ones in its database.

Vera also has the ability to restore, or clone, this backup into another unit.

For example, if you receive a replacement unit, you can restore a backup of
your old dongle's data to the new dongle so you don't have to rebuild your
network.

To do this follow these steps:

  1. Be sure that you have not made any changes to Vera within the past 2 hours.  
Vera will backup the dongle's configuration whenever the list of devices in
the dongle changes. The backup process is slow, so Vera does it in small
increments when there is no activity on the Z-Wave network. In Vera's toolbar,
go to Setup->Z-Wave Settings->Options, and look at the value for Last Z-Wave
network backup. This will show the date & time that Vera last completed a
successful backup of the dongle. Be sure that this is not empty or "_N/A_". If
it is, go to Setup->Z-Wave Settings->Advanced and click Go on "Backup Z-Wave
network "  

  2. Once you've confirmed that Vera has a backup of your dongle, go to _Advanced_, _Backup_ and choose **Create backup**.  
Your browser will prompt you to save a file. Save it to your computer
somewhere, such as on the Desktop. Be sure to wait until your browser has
finished downloading.  That backup file contains both Vera's database as well
as the dongle's.

  3. Connect your new Z-Wave unit. Wait a minute to be sure that it boots up.
  4. Go to Advanced, Backup and in the restore section, click 'choose file' and locate the backup file.  
Check the box 'Restore Dongle Firmware'. Then click Restore.

  5. Leave Vera alone for 15 minutes.  
Vera will restore its database, which has all the detailed information on the
device, and will also restore the dongle's data from the backup file, which
takes several minutes.

  6. Confirm your new Z-Wave unit is working and that you have a complete list of devices. 

**NOTE ** In case you forgot to backup your existing settings and you have the "Backup my configuration on server" service activated from Setup->Backup Auto-Backup section, your Vera will backup your data once per day. So, login with your account, go to Setup->Backup and you will see there the backups. Select the last one and restore it to your Vera unit. Read here about the restore process: [Backup / Restore](http://wiki.micasaverde.com/index.php/Advanced#Backup.2FRestore)

  

