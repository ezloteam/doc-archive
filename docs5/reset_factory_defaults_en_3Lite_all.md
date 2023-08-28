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

![](skins/mios/images/plus.gif)[Z-Wave Device Properties](index.html#!docs5/add_device_zwave_properties_options_en_3Lite_all.md)

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

[Previous](index.html#!docs5/advanced_settings_downloads_en_3Lite_all.md)
[Next](index.html#!docs5/zwave_options_en_3Lite_all.md)

Reset Vera to Factory Defaults

You can return Vera to the factory default state, wiping out all the
configuration changes you have made.  
  
First, if you want to reset the Z-Wave network, that is the list of Z-Wave
devices that you have paired, openVera 's Setup page and click 'Z-Wave
settings', then 'Advanced' and then 'Go' on the 'Reset Z-Wave Network' option.  
  
![](/images/mios/UI5_resetZnet1.PNG)  
  
Next, if you also want to reset everything else in Vera, including any changes
you've made to Vera's networking, any rooms or scenes or users you've added,
your location settings, and so on, then from Vera's SETUP page click 'Backup'
and click 'Restore Factory Defaults'. Alternatively, you can press the  button
on the front of Vera marked 'Reset' twice in rapid succession, then watch the
power light on the front of Vera. The power light will go out when Vera is
doing a reset. In order to avoid accidentally resetting Vera and losing your
data, you have to double press the button quickly. So if the power light
doesn't go out, try again until it does.

**NOTE:** This means if you have paired devices they will no longer work after you do a factory reset. Any devices that were paired with Vera before the reset will still be "remembering" the z-wave ID after the reset.  You have to remove them from the Z-Wave network, and then add them again.  

  

