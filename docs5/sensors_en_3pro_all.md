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

![](skins/mios/images/minus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Door locks](index.html#!docs5/door_locks_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Lighting Devices](index.html#!docs5/lighting_devices_en_3pro_all.md)

![](images/spacer.gif)[Plug and Receptacle Devices](index.html#!docs5/plug_devices_en_3pro_all.md)

![](images/spacer.gif)[Thermostats](index.html#!docs5/thermostats_en_3pro_all.md)

![](images/spacer.gif)[Window Coverings](index.html#!docs5/window_coverings_en_3pro_all.md)

![](images/spacer.gif)[Sensors](index.html#!docs5/sensors_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Scene Controllers](index.html#!docs5/scene_controllers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3pro_all.md)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3pro_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Alarm panels](index.html#!docs5/alarm_en_3pro_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3pro_all.md)

|

[Previous](index.html#!docs5/window_coverings_en_3pro_all.md)
[Next](index.html#!docs5/scene_controllers_en_3pro_all.md)

Sensors

Motion detectors support 2 types of events: "when a sensor is tripped" or
"when an armed sensor is tripped". This is called an event. There can be two
types of events for sensors:

  * when a sensor is tripped: this means that motion sensors will generate an event whenever it is tripped regardless of it's armed state. You can use this setting to get an alert or run a scene whenever the sensor is tripped even when it's on Bypass   

  * when an Armed sensor is tripped:this means the motion sensors will generate an event whenever it is tripped and only when set on armed state.You can use this setting to get an alert or run a scene ONLY when the sensor is ARMED and it detects motion 

For example : If you select a sensor (door,window,motion/etc) is tripped",
"device is tripped" you will receive a notification when the sensor is tripped
(the door is opened) despite the sensor's state is SET on ARM or BYPASS. If
you select "an armed sensor is tripped", "device armed is tripped" you will
receive a notification when the state of the sensor is ARM and the sensor is
tripped (the door is opened ).  

How do I arm or bypass the device? To arm/bypass your sensor you have to go to
Devices -> motion sensor -> click on Arm/Bypass

|  Manufacturer  |  Device Type  |  Model no.  |  Version  |  Frequency  |
Specs  |  Notes  
---|---|---|---|---|---|---  
ACT  |  Motion Sensor  |  ZIR000 / ZIR010  |  
|  EU (ZIR010) or US (ZIR000)  |  [Link](http://www.act-
solutions.com/HomePro/pdfs/HomePro/Specs/ZIR000_spec.pdf) [Link](http://www
.act-solutions.com/HomePro/pdfs/HomePro/Inst/ZIR000_instr.pdf)
[Link](http://www.act-
solutions.com/HomePro/pdfs/HomePro/Specs/ZIR010_spec.pdf) [Link](http://www
.act-solutions.com/HomePro/pdfs/HomePro/Inst/ZIR010_instr.pdf) |  Remove the
cover, pair to the Vera system using the push-button on the left of the
circuit board. The Vera system must configure it to work, and it can only be
configured within less of a minute (30 sec best) of inserting the batteries.
With the Vera system idle, remove/reinsert the batteries, and within 30
seconds put the Vera system in include mode. Within a few minutes confirm the
"configure" icon for the device is green on the Vera system's setup page  
Express Controls aka HomeSeer  |  3-in-1 sensor (light/temperature/motion)  |
HSM100 / EZMotion  |  
|  EU or US  |
[Link](http://www.expresscontrols.com/pdf/EZMotionOwnerManual.pdf) |  See [Exp
ressControls3in1](http://wiki.micasaverde.com/index.php/ExpressControls3in1)  
If the motion sensor does not work right after inclusion and configuration,
remove the batteries for a few seconds.  
EverSpring/Hawking/Home Manageables  |  Door/window sensor  |  SM103  |
6,2,9,1,0  |  EU or US  |  [Link](http://www.everspring.com/Products/Home_Auto
mation_Detail.asp?parentUID=83&UID=355&CateUIDList=0,83)
[Link](http://www.everspring.com/Archive/Image/File/A501110873R01_SM103_-
ECR.pdf) |  Pair using the intrusion button. The sensor will accept
configuration within a few minutes of the initial pairing, or of pressing the
intrusion button on the back even after it's paired. Pair the device, or if
it's already paired, press the intrusion button, and within 30 seconds put the
Vera system in include mode. Within a few minutes confirm the "configure" icon
for the device is green on the Vera system's setup page. NOTE: There is some
confusion about the orientation of the sensor. The main sensor body has a back
(where the intrusion is), a front (where the logo and LED is), and the 2 other
surfaces, one of which has a curved edge, and the other is flat. The magnet
needs to go against the flat surface. And the flat surface on the magnet
should be as close as possible to the flat surface on the sensor, lined up in
the middle so the line which passes through the LED lines up with the sensor.  
EverSpring/Home Manageables  |  Humidity + Temperature sensor  |  HM-TS001  |
|  |  [Link](http://www.asihome.com/ASIshop/product_info.php?products_id=3946)
[Link](http://www.homeseer.com/pdfs/guides/HM_TD001.pdf) |  Pair or unpair the
device by tapping the CF button 3 times very quickly. Once it's paired and
shows up in the UI as a generic device, press the CF button 3 times again
quickly to make it wakeup and get configured. Then it will correctly be
identified as 3 devices (combo device + temperature + humidity).  
Everspring  |  Motion Detector  |  SP103  |  6,2,9,1,0  |  EU or US  |  [Link]
(http://www.everspring.com/Products/Home_Automation_Detail.asp?parentUID=83&UI
D=354&CateUIDList=0,83) [Link](http://www.everspring.com/Archive/Image/File/A5
01110874R01_SP103_%20-%20ECR.pdf) |  Works well  
Fortrezz  |  Water /Freeze  |  WWA-001  |    |  US  |
[Link](http://www.fortrezz.com/)
[Link](http://www.fortrezz.com/resources/WWA_manual_01May2009.pdf) |  Works
great I would place a few in your house. Bathrooms, laundry , kitchen ,
basement. Great product!  
Fortrezz | Water /Freeze  | WWA-002 |   |   |
[Link](http://wiki.micasaverde.com/index.php/Fortrezz_WWA-002) | Works great I
would place a few in your house. Bathrooms, laundry , kitchen , basement.  
  
Intermatic  |  Motion Sensor  |  CA-9000  |  |  US  |
[Link](http://www.smarthomeusa.com/Products/CA9000/manuals/CA9000.pdf) |  This
device has limited functionality as a sensor. It can only be used to turn on
and off a light directly by setting an association, which the Vera system
supports. It does not fire events, so you cannot use it as an event on a
scene.  
Merten  |  4-gang radio transmitter, flush-mounted  |  506004  |  2,2,27,1,4
|  EU  |  [Link](http://www.merten.de/download/DL_doku/V5060_581_02_web.pdf) |  
  
  

