![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3lite_all.md)

![](skins/mios/images/minus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Network Troubleshooting](index.html#!docs5/network_troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Initial Connection](index.html#!docs5/initial_connection_en_3lite_all.md)

![](skins/mios/images/minus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Migrate To Z-wave version 452](index.html#!docs5/migrate_to__z-wave_version_452_en_3lite_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit_en_3lite_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote_en_3lite_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device_en_3lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3lite_all.md)

|

[Previous](index.html#!docs5/initial_connection_en_3lite_all.html) [Next](migrate_to__z-wave_version_452_en_3lite_all.md)

Z-Wave Troubleshooting

**How does Z-Wave works ?  
**

Z-Wave has a range for **indoor** use of **25 to 30 meters**  **(82 to 100
feet)** from node to node so some devices have longer range and others
shorter. The **range** of a Z-Wave signal is strongly influenced by the
environment and depends on many factors, from the antenna and implementation
of the device to the materials the product is encased in, and the materials
that the radio signal has to go through (concrete walls or metal doors). So if
a node is more than **24-28 meters (80-90 feet)** from the gateway you put a
repeater node (like an plug-in on/off switch) in between and the signal will
go from the gateway to the repeater node, to the end device. The signal will
hop up to 4 times until the 5th device and you can create scenes,
associations, etc. between any of those nodes (devices) in the network.
Depending on how your house is set-up, we recommend for indoor use that the
distance should be about **12-15 meters** (**40-50 feet)**.

Because **door locks** are a special breed of z-wave devices which require an
exchange of security keys when they communicate with the Vera  unit we
recommend that the distance should be about **6-9 meters (20-30 feet)**.

For **outdoor** z-wave devices that range can go up to **100 meters (300
feet)** for line of sight .

**Things to consider regarding Z-Wave range:**  
\- Each wall or obstacle (i.e.: refrigerator, big screen TV, etc.) between the
remote or a Z-Wave device and the destination device will reduce the maximum
range by approximately 25-30%.  
\- Brick, tile or concrete walls block more of the Z-Wave signal than walls
made of wooden studs and plasterboard (drywall).  
\- Wall mounted Z-Wave devices installed in metal junction boxes will suffer a
significant loss of range (approximately  
20%) since the metal box blocks a large part of the Z-Wave signal.

  
If you are experiencing issues with your z-wave network's responsiveness or
reliability, you should repair the network to let the z-wave chip in Vera
rebuild it's mesh network. To repair your network:

  1. Go to Setup -> Z-Wave Settings.
  2. Click the "Repair" tab
  3. Click "GO"
  4. Don't do anything else with your system. It's best to do a repair overnight, because repairing your network prevents Vera from polling your nodes, detecting events, reporting when your door locks open, etc.
  5. After the repair finishes, from Z-Wave Device>Repair, you can view a repair report that can identify which nodes on your network have weaker connections to the mesh and can help you identify locations where you might need to add a module to improve the network

  

