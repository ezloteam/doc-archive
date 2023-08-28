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

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/reference_en_3pro_all.md)

Manual Z-Wave Routing

### Manual Routing  

In order to do a manual routing (this applies to the Z-Wave version 3.20) you
should go to advanced settings of a device, add a variable with the service
id: urn:micasaverde-com:serviceId:ZWaveDevice1 and the variable name:
ManualRoute and the value is a dot separated list of Z-Wave node ID's, just
like the AutoRoute variable.  

The Auto route variable may be something like this: "2-20x,7-59x,2.7-78". This
means there are 3 routes found. #1 uses node 2 as an intermediary, and it has
a 'score' of 20.  

The score is a measure of latency and accuracy,the lower number is better. The
'x' that follows means the last attempt to use it failed, so it won't be used
anymore.  

The next route uses node #7, it scored worse, and also failed. The 3rd route
uses node 2 & 7\. It had the worst score (78), but it's currently working (no
x).

  

