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

![](skins/mios/images/minus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3pro_all.md)

![](images/spacer.gif)[Supported IP Cameras](index.html#!docs5/supported_cameras_en_3pro_all.md)

![](images/spacer.gif)[VistaCam](index.html#!docs5/vistacam_en_3pro_all.md)

![](images/spacer.gif)[Panasonic IP Cameras](index.html#!docs5/panasonic_ip_cameras_en_3pro_all.md)

![](images/spacer.gif)[Foscam Pan/Tilt](index.html#!docs5/foscam_en_3pro_all.md)

![](images/spacer.gif)[Manually adding a camera](ip_camera_en_3pro_all.htmls)

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

[Previous](index.html#!docs5/vistacam_en_3pro_all.html) [Next](foscam_en_3pro_all.md)

Panasonic IP Cameras

For some unknown reason, Panasonic IP cameras will not obtain an IP address
automatically when you plug them into the network. We can provide no logical
explanation for this since nearly every user will want the camera to get an IP
address on the network. It is, after all, an IP device.

If you experience this issue, use one of the following methods to correct the
camera's settings:

Method #1:  Run the Windows CD that comes with the camera. Once you run
Panasonic's app and tell the camera to get an IP address, then the control
unit will find it and will integrate the camera automatically and setup will
be effortless.  However, because Panasonic only offers a Windows version of
the camera setup software, Linux and Mac users will have to use Method #2.

Method #2: Temporarily give your computer an IP address of 192.168.0.10, with
netmask 255.255.254.0, so that it joins the same subnet as the Panasonic
camera.  Open a web browser to [http://192.168.0.253](http://192.168.0.253/)
to get to the camera's admin page. Path:
/SnapshotJPEG?Resolution=640x480&Quality=Standard

When you first connect to the camera you need to pick a user name and
password. Entering the username: **dceadmin** and the password: **dcepass**
allows Vera to automatically integrate and control the camera. If you pick a
different username/password, then click the Camera Icon and provide the
username and password under the settings fieds.

Once issued the IP address to your camera, it will be on your home's network,
meaning the camera is only accessible from within the home and not accessible
to outsiders on the internet. Therefore you do not need to worry about a
secure password to prevent outsiders from gaining access. The camera's
password further serves to keep out casual users within your home.

So that you can view your IP camera when you're not home, the control unit
acts as a secure gateway to your camera.  Simply login remotely through the
cp.mios.com site using your username and password.  cp.mios.com is protected
by the same level of encryption used by banks for online banking. Through this
secure gateway you can view and control the cameras from anywhere in the
world!

If you buy the camera from Mi Casa Verde, we will use Panasonic's utility to
tell the camera to get an IP address automatically, and give the camera a
username/password of **dceadmin**/**dcepass**. So then the camera will be
automatically detected and used in the control unit. If you buy a wireless
camera, then we will also set the SSID/WPA2 passphrase to match your
particular configuration so that the camera works out of the box wirelessly as
well.  



###  **Configuring the Panasonic IP camera to connect wirelessly to your
unit**

The Panasonic IP Cameras have a switch on the bottom: WIRED/WIRELESS. In order
to connect your camera wirelessly, you'll need to follow these steps:

    
    
       - set the switch to WIRED  
       - connect your camera to your unit's LAN port using an Ethernet cable  
       - turn the camera on, confirm control unit's LAN LED turns orange, and wait for the IP Cam LED to turn green  
       - wait for the camera to be detected and displayed in the Devices toolbar  
       - assign the camera to a 'Room' and click 'Save'  
    (for the camera to be detected it should have the default username/password: dceadmin/dcepass and listen on port 80)  
       - confirm that you can see images from the camera  
       - click on the camera icon and note its IP address (e.g. 192.168.81.200) from the Advanced tab  
       - connect your computer to the same network as your camera  
       - open your web browser and type in:[ ](http://findvera.com/)[http://camera1_ip](http://camera1_ip/) (in this example, [http://192.168.81.200](http://192.168.81.200/))  
       - login with the default camera username: dceadmin and password: dcepass  
       - go to Setup -> Wireless and set SSID, Cipher and Password to control unit's wireless settings  
    which can be found an the bottom of unit. (default Cipher is WPA2-PSK)  
       - click 'Save Settings'  
       - turn the camera's bottom switch to WIRELESS and reboot your camera by cycling its power  
    

Your camera should now connect wirelessly to the control unit. If you change
your unit's wireless settings you'll have first to update them on your
cameras, so you won't lose connection to them.

  

