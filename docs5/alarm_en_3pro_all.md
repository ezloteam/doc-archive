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

![](skins/mios/images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3pro_all.md)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3pro_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3pro_all.md)

![](skins/mios/images/minus.gif)[Alarm panels](index.html#!docs5/alarm_en_3pro_all.md)

![](images/spacer.gif)[DSC Alarm Panel](index.html#!docs5/dsc_en_3pro_all.md)

![](images/spacer.gif)[Elk M1 Alarm Panel](index.html#!docs5/elk_m1_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Honeywell Ademco Vista Alarm Panels via AD2USB](index.html#!docs5/honeywell_alarm_panel_ad2usb_en_3pro_all.md)

![](images/spacer.gif)[Honeywell / Ademco Alarm Panels with RS-232 Interface](index.html#!docs5/honeywell_alarm_panel_rs232_en_3pro_all.md)

![](images/spacer.gif)[Paradox EVO Alarm Panels](index.html#!docs5/paradox_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Visonic Powermax Alarm Panel](index.html#!docs5/visonic_powermax_alarm_panel_en_3pro_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/Insteon_en_3pro_all.html) [Next](dsc_en_3pro_all.md)

Alarm panels

###  Supported Alarm Panel:

|  Manufacturer  |  Model(s)  |  Required module  |  Plugin  |  Notes  
---|---|---|---|---  
DSC  |

  * [PowerSeries PC1616](http://www.dsc.com/index.php?n=products&o=view&id=1)
  * [PowerSeries PC1832](http://www.dsc.com/index.php?n=products&o=view&id=2)
  * [PowerSeries PC1864](http://www.dsc.com/index.php?n=products&o=view&id=3)
|  [IT-100](http://www.dsc.com/index.php?n=products&o=view&id=22) |
[Link](http://code.mios.com/trac/mios_dscalarmpanel/wiki/WikiStart) |  
Elk  |

  * [M1 Gold](http://www.elkproducts.com/_webapp_2981420/M1_Gold_Cross_Platform_Control%C2%AE)
  * [M1EZ8](http://www.elkproducts.com/_webapp_3127911/M1EZ8_Cross_Platform_Control%C2%AE)
|  The M1EZ8 panel requires the [ELK-
M1EZ8MSI](http://www.elkproducts.com/_webapp_2981423/elk-
m1ez8msi__m1ez8_main_serial_interface) Main Serial Port Interface.  |
[Link](http://code.mios.com/trac/mios_elk-alarm-panel/wiki/WikiStart) |  You
can use the ELK-M1XEP Ethernet Interface to connect the panels to Vera on the
Ethernet port.  
GE Security / Interlogix / Caddx  |

  * [NetworX NX-4](http://www.interlogix.com/resources/intrusion/906-3179_NetworX_brochure.pdf)
  * [NetworX NX-6](http://www.interlogix.com/resources/intrusion/906-3179_NetworX_brochure.pdf)
  * [NetworX NX-8](http://www.interlogix.com/resources/intrusion/906-3179_NetworX_brochure.pdf)
  * [NetworX NX-8E](http://www.interlogix.com/resources/intrusion/906-3179_NetworX_brochure.pdf)
|  [NX-584](http://utcfssecurityproducts.com/ProductsAndServices/Pages/NX-584.
aspx) |  [Link](http://code.mios.com/trac/mios_caddxnx584/wiki/WikiStart) |
NetworX NX-8E already has a RS-232 interface, so it doesn't require the NX-584
module.  
Honeywell / Ademco  |  VISTA-50P, VISTA-128BP, VISTA-128BPT, VISTA-128BPE,
VISTA-128FBP, VISTA-250BP, VISTA-250BPT, VISTA-250BPE and VISTA-250FBP  |
VISTA-50P, VISTA-128BP, VISTA-128FBP, VISTA-250BP, and VISTA-250FBP panels
require the [4100SM](http://www.security.honeywell.com/me/intrusion/products/e
xp/ac/138478.html) module.  |  [Link](http://code.mios.com/trac/mios_ademco-
panels-plugin/wiki/WikiStart) |  If your Vista panel is not on this list, look
at the next row.  
Honeywell / Ademco  |  10SE, 20SE, 10P, 15P, 20P, 50P, etc.  |
[AD2USB](index.html#!docs5/http://www.nutech.com/online-store/18.md) |
[Link](http://code.mios.com/trac/mios_vista-alarm-panel-ad2usb/wiki/WikiStart)
|  
Paradox  |

  * Digiplex DGP-848 
  * EVO48 
  * [EVO192](http://www.paradox.com/Products/default.asp?CATID=7)
|  [PRT3 Integration Module](http://www.paradox.com/Products/default.asp?CATID
=7&SUBCATID=75&PRD=234) |  [Link](http://code.mios.com/trac/mios_paradox-
alarm/wiki/WikiStart) |  
Visonic  |

  * [PowerMax](http://www.visonic.com/Products/Wireless-Property-Protection/PowerMax)
  * [PowerMax+](http://www.visonic.com/Products/Wireless-Property-Protection/PowerMaxPlus)
  * [PowerMaxComplete](http://www.visonic.com/Products/Wireless-Property-Protection/PowerMaxComplete)
  * [PowerMaxPro](http://www.visonic.com/Products/Wireless-Property-Protection/PowerMaxPro)
|  RS-232 Interface Module  |  [Link](http://code.mios.com/trac/mios_visonic-
powermax/wiki/WikiStart) |  
  
  

