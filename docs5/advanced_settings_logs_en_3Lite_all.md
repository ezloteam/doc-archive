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

![](skins/mios/images/minus.gif)[Logs](advanced_settings_en_3Lite_all.html_logs)

![](images/spacer.gif)[Archive Logs](index.html#!docs5/archive_logs_en_3Lite_all.md)

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

[Previous](index.html#!docs5/advanced_settings_backup_en_3Lite_all.md)
[Next](index.html#!docs5/archive_logs_en_3Lite_all.md)

Logs

  
Here you can view and configure Vera's logs. Tech support staff may ask you a
question about your logs or to enable "Verbose Logging" before reproducing an
issue.  
  

Show polling activity:  
  
Show individual jobs:  
  
Verbose logging:  
 Check it only before reproducing an issue. Verbose logging can cause a slow
down of the engine.  
It is automatically disable after 24hours  

  
Lock Log Levels:  
Prevents automatically disabling the Verbose Logs after 24 hours  
  
Archive old logs on Server  

Vera regularly runs into abnormal circumstances that require special handling;
your Internet connection may go down, there may be interference on the Z-Wave
network, and so on. Vera stores all this information in a log. Because Vera
does not have a hard drive or permanent storage, the logs are lost every time
you turn Vera off and on, or when Vera is running low on memory. If you leave
the "Archive old logs on Server", then the logs will be sent to the online
server instead. The logs do not contain any personally identifiable
information.

Each day automated processes go through all the logs are uploaded looking for
patterns and other abnormalities, which are sent to the developers for
analysis and possibly bug fixes. Also, if you leave this option checked, and
you later call technical support to report a problem, your support rep will be
able to look over the logs to see if there were any errors encountered around
the time.

We recommend you leave this feature on as it improves the quality control
process. The amount of data uploaded to the MiOS server is small, and the
uploads are infrequent, generally once every 12 hours. So, for users with
normal high speed Internet connections like Cable or DSL, the data usage is
insignificant. If you use Vera on a high-cost Internet connection, like, say a
boat with a satellite uplink, you can disable this option to reduce the amount
of traffic Vera generates on the network.  



![](/images/mios/UI5_logspage.PNG)  

  

