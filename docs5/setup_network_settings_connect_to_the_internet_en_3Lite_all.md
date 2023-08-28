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

![](skins/mios/images/minus.gif)[Net & Wi-Fi](setup_en_3Lite_all.html_network_settings_connect_to_the_internet)

![](images/spacer.gif)[Wifi client mode](index.html#!docs5/Wifi_client_mode_en_3Lite_all.md)

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

[Previous](index.html#!docs5/advanced_settings_en_3Lite_all.md)
[Next](index.html#!docs5/Wifi_client_mode_en_3Lite_all.md)

Net & Wi-Fi

  
Vera automatically detects various facts about your network and attempts to
configure your network for you. Most users will never have to use this page.
You have 2 options to configure your network:

  1. Automatically Configure
    * This is all most users will ever need to do. Vera will detect whether it is connected directly to the Internet or to a router and configure itself accordingly.
  2. Manually Configure
    * Select this if you want to setup your network using a static IP or PPPoE  

![](/images/mios/UI5_net&wifi_vera_lite\(1\).png)  
For option 2 you can configure these settings:

  * What type of network connection do you have?
    * DHCP
      * Most common. Select this if you don't know what DHCP vs Static IP means.
    * Static IP
      * If you need Vera to have a static IP on your network, select this.
    * PPPoE
      * Use this for a VPN connection only if you know what you are doing. We don't support debugging issues with your VPN.
  * IP Address
    * The IP that you want Vera to have on your network.
  * Subnet mask
    * Unless you know otherwise, it should be 255.255.255.0
  * Gateway
    * The IP address of your router. Most of the time this is 192.168.1.1
  * DNS
    * The DNS servers that Vera should use. 208.67.222.222 and 8.8.8.8 are both good DNS servers to use.
  * Lan
    * You should leave the options in the LAN section to the default value unless you know what you are doing. Do not setup the LAN ip address to the same WAN ip as this might prevent you from accessing your Dashboard. If you only want to setup a static ip, use the options in the WAN settings.

![](/images/mios/UI5_netSettings1_vera_lite.PNG)  

  

