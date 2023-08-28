![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3pro_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Network Troubleshooting](index.html#!docs5/network_troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Initial Connection](index.html#!docs5/initial_connection_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit_en_3pro_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote_en_3pro_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/unit_en_3pro_all.html) [Next](Device_en_3pro_all.md)

Remote access

To remotely access your Vera from another computer please visit:  
  
<https://cp.mios.com/>

  

If you are unable to access your unit remotely, it may be that your firewall
is very restrictive and your Vera is unable to initiate the connection with
our servers. In normal situations where the Vera unit is able to connect to
the Internet like a normal computer would, there should be no issues at all,
but if you have a very restrictive firewall you might want to open a port for
the unit to let it connect to our servers.

First you have to make sure you set up a static ip for the Vera unit
preferably directly on your main router, based on its MAC address which you
can find on the back of the box itself or in the DHCP table on your router.
After you've successfully set up the static IP address you can safely go and
open port 232 for that IP address for outbound connections. Assuming this has
been successfully set, the Vera should be able to reach to our servers and you
should be able to access it remotely from anywhere.

  

