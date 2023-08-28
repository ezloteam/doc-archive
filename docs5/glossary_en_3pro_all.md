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

![](skins/mios/images/minus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Tech Support](index.html#!docs5/tech_support_en_3pro_all.md)

![](images/spacer.gif)[Glossary](index.html#!docs5/glossary_en_3pro_all.md)

![](images/spacer.gif)[Factory Reset](index.html#!docs5/factory_reset_en_3pro_all.md)

![](images/spacer.gif)[Security](index.html#!docs5/security_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/tech_support_en_3pro_all.md)
[Next](index.html#!docs5/factory_reset_en_3pro_all.md)

Glossary

**Exclude / Exclusion / Reset a device / Remove a device / Un-pair :** These all mean the same thing and refer to resetting a device, or removing it from whatever Z-Wave network it is currently in. 

**Include / Inclusion / Pair / Add Device:** These all mean the same thing and refer to adding a new device to the current Z-Wave network stored in the primary controller. 

**Mesh network:** The range that a Z-Wave can transmit information to another Z-Wave device is between 30 and 100 feet. However, Z-Wave is a mesh network, meaning if there are nodes in between, they can act as relays or repeaters. In this way, if you have 5 Z-Wave devices, each is 30' apart, and the 2 furthest are 120' feet apart, the 2 furthest nodes can still talk to each other because the 3 nodes in the middle act as repeaters. Z-Wave supports a maximum of 4 hops, meaning there can be up to 4 repeaters. 

**Primary Controller:** In a Z-Wave network, there needs to be 1 device that is designated as the "Primary" controller. This is the device that keeps a database of all the other Z-Wave devices in your network. The primary controller also has responsibility for ensuring the health of your Z-Wave network by regularly checking what nodes are working and what other nodes are close to them to act as relay points. By default, the Vera system comes as your primary controller, and you add your other Z-Wave devices to the Vera system. If you already have another primary controller and don't want to rebuild your Z-Wave network, the Vera system can become a secondary controller. On Vera's devices, Z-Wave settings page it shows which role the Vera system has. 

**Replication / Replicating, copying, or transferring a Z-Wave network, adding a secondary controller:** These mean the same thing and refer to sending a copy of the master database of Z-Wave devices contained in the primary controller to some new, secondary controller, which will now become part of the Z-Wave network and have a list of all the other Z-Wave devices so it can control them too. 

  

