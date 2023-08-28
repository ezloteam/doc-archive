![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3Lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Advanced Settings](index.html#!docs5/advanced_settings_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Net & Wi-Fi](setup_en_3Lite_all.html_network_settings_connect_to_the_internet)

![](images/spacer.gif)[Backup](index.html#!docs5/advanced_settings_backup_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Logs](advanced_settings_en_3Lite_all.html_logs)

![](images/spacer.gif)[Firmware Upgrades](index.html#!docs5/advanced_settings_downloads_en_3Lite_all.md)

![](images/spacer.gif)[Reset Vera to Factory Defaults](index.html#!docs5/reset_factory_defaults_en_3Lite_all.md)

![](images/spacer.gif)[Z-Wave Options](index.html#!docs5/zwave_options_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Z-Wave Device Properties](index.html#!docs5/add_device_zwave_properties_options_en_3Lite_all.md)

![](images/spacer.gif)[Advanced](index.html#!docs5/add_device_zwave_properties_advanced_en_3Lite_all.md)

![](images/spacer.gif)[Device Options](index.html#!docs5/add_device_zwave_properties_dev_option_en_3Lite_all.md)

![](images/spacer.gif)[Logs](index.html#!docs5/add_device_zwave_properties_logs_en_3Lite_all.md)

![](images/spacer.gif)[Notifications](index.html#!docs5/add_device_zwave_properties_notifications_en_3Lite_all.md)

![](images/spacer.gif)[Settings](index.html#!docs5/add_device_zwave_properties_settings_en_3Lite_all.md)

![](images/spacer.gif)[Add Z-Wave Dongle With Different Frequency](index.html#!docs5/changing_zwave_port_en_3Lite_all.md)

![](images/spacer.gif)[Z-Wave Advanced Options](index.html#!docs5/zwave_device_advanced_en_3Lite_all.md)

![](images/spacer.gif)[Full/Low Power Inclusion/Exclusion](index.html#!docs5/full_power_inclusion_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Lite_all.md)

|

[Previous](index.html#!docs5/add_device_zwave_properties_advanced_en_3Lite_all.md)
[Next](index.html#!docs5/add_device_zwave_properties_logs_en_3Lite_all.md)

Device Options

##  Configuration settings

Some Z-Wave devices allow you to manually set configuration variables to do
things like adjust ramp rate and so on. This is unique for each device, and
each manufacturer handles this differently.  

If the manual for your Z-Wave device indicates that you can set a
configuration variable or setting to change the default behavior, do it by
clicking the 'Add Configuration Setting' button. Indicate which variable
number to set, and what value to set it to.  

The value can be a '1 byte hex', '1 byte dec', '2 byte hex', '2 byte dec', '4
byte hex' or '4 byte dec'. If you do not know what this means and the
manufacturer did not tell you which one they want you to choose, then choose
'4 byte dec'.  

Put the setting you want in 'Desired Value'. Vera will attempt to configure
the node after you click the red 'Save' button, and if successful, you'll see
the [[Device_Control_Status#Job_icons|green 'Configure Job' OK icon]. If it's
a battery operated device and Vera can't configure it right away, read the
comments above about the **Configure node right now**.  

Once Vera has configured the Z-Wave device, Vera will ask the device again for
the value of the configuration setting and show it under 'Current Value'. If
you set a value, configured the device, and the current value is something
other than your desired value, that means the Z-Wave device did not accept the
'Desired Value' you gave it, and you may need to contact the manufacturer for
clarification.  

If you change the 'Data Size' option to say 'Monitor only', then when the
device is next configured Vera will not change the value, but Vera will ask
the device for the current value and show it in the 'Current Value' column.  

If you change it to 'Default', then the next time Vera configures the device,
Vera will tell the device to go back to the default value for this setting,
and you'll see the value in the 'Current Value' column.  

![](/images/mios/UI5_devOptTab.PNG)

##  Associations

**Note:** Leave _By default Vera should automatically configure devices_ checked as explained above, and leave each device's _Automatically configure_ set to 'Default Behavior'. If you tell Vera not to configure the device, Vera will leave the device alone and will not set the associations for you. 

These are also unique for each device according to the manufacturer.
Associations are commonly used to tell sensors to turn on lights, and to
associate devices. Refer to the manufacturer's users manual that came with the
Z-Wave device to learn how they handle associations. Associations are given an
ID or group ID.  

To add an association, type in the group ID, which is a number, click 'Add
Group' and then check off the Z-Wave devices you want to be associated. Vera
will attempt to configure the node after you click the red 'Save' button, and
if successful, you'll see the [[Device_Control_Status#Job_icons|green
'configure job' ok icon].  

If it's a battery operated device and Vera can't configure it right away, read
the comments above about the **Configure node right now**.

##  Scene Assignments

If this is a Z-Wave controller, then you will have another section on this
page to assign scenes to the controller's buttons, as explained [here](http://
wiki.micasaverde.com/index.php/ZWave_Add_Controller#Scene_Assignments_for_cont
rollers). You won't see this for other types of Z-Wave devices.

  

