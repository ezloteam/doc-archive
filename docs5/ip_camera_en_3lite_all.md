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

![](skins/mios/images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3lite_all.md)

![](skins/mios/images/minus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3lite_all.md)

![](images/spacer.gif)[Supported IP Cameras](index.html#!docs5/supported_cameras_en_3lite_all.md)

![](images/spacer.gif)[VistaCam](index.html#!docs5/vistacam_en_3lite_all.md)

![](images/spacer.gif)[Panasonic IP Cameras](index.html#!docs5/panasonic_ip_cameras_en_3lite_all.md)

![](images/spacer.gif)[Foscam Pan/Tilt](index.html#!docs5/foscam_en_3lite_all.md)

![](images/spacer.gif)[Manually adding a camera](ip_camera_en_3lite_all.htmls)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3lite_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Alarm panels](index.html#!docs5/alarm_en_3lite_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3lite_all.md)

|

[Previous](index.html#!docs5/zwave_devices_en_3lite_all.md)
[Next](index.html#!docs5/supported_cameras_en_3lite_all.md)

Network Cameras

  
Table of Contents:  
  
1\. General (Works for Panasonic IP Cameras and others)  
[2\. VistaCam](index.html#!docs5/vistacam_en_all_all.md)  
[3\. Panasonic IP Camera](/panasonic_ip_cameras_en_all_all.html)  
  
  
A list of supported cameras is [here](/supported_cameras_en_all_all.html).  
  
Vera is compatible with any network camera that is able to snap a still
picture using the standard picture format (JPEG).  Most cameras are capable of
doing this although some were explicitly designed to be proprietary and to
only work with their manufacturer's own software or with a proprietary web
plugin.  Assuming you have a standard network camera, Vera will be able to
snap pictures whenever events occur, like a sensor being tripped, and store
them in an archive.  You can also view what's in front of the camera using
nearly any smartphone since all of them can display still pictures.  The image
is usually refreshed every 1 second or so depending on your network speed.  
  
Your Vera system also has limited support for full-motion live video.  This is
more difficult because there are a lot of incompatible formats, and many web
browsers and phones cannot display live video at all or only using video
formats that are different from what the cameras use.  But, with a few
combinations of cameras and browsers/phones, you will get real full-motion
video.  
  
Some cameras may be plug-and-play and get detected and setup automatically as
soon as you turn them on, but that depends on several factors.  If your camera
is not automatically detected, you can add it manually either at Step 1 in the
Setup Wizard, or by clicking the Add Device icon on the Dashboard.  The Setup
Wizard is a bit easier since it guides you step by step.  Either way, Vera
needs 3 pieces of information to make your camera work: 1) It's IP address, 2)
the username+password, if any, to access the camera, 3) the URL (ie the
http://.... in your web browser) to get a snapshot image as a JPEG file.  
  
The link at the top of the page shows you URL's for common cameras.  If your
camera is not on the list, you might still be able to get it to work.  Try
viewing the camera in your web browser on your home network.  When you see an
image from the camera try saving that image location.  For example, in
Internet Explorer, you right click on an image and, if it's a standard still
image, you have the option "Copy Image" and "Copy Image Location".  If you can
copy the image location, you'll end up with something like:
http://192.168.1.115/SnapshotJPEG?Resolution=320x240&Quality=Standard.  In
that case, your IP 192.168.2.115, the URL is:
SnapshotJPEG?Resolution=320x240&Quality=Standard.  
  
Note: If your IP camera uses a different port then the default 80 port, you
have to type in the IP address of the camera followed by a colon and the port
number: for example:  10.0.1.152:9080  
  

  

