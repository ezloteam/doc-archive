![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3Pro_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Pro_all.md)

![](skins/mios/images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3Pro_all.md)

![](skins/mios/images/minus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3Pro_all.md)

![](images/spacer.gif)[Supported IP Cameras](index.html#!docs5/supported_cameras_en_3Pro_all.md)

![](images/spacer.gif)[VistaCam](index.html#!docs5/vistacam_en_3Pro_all.md)

![](images/spacer.gif)[Panasonic IP Cameras](index.html#!docs5/panasonic_ip_cameras_en_3Pro_all.md)

![](images/spacer.gif)[Foscam Pan/Tilt](index.html#!docs5/foscam_en_3Pro_all.md)

![](images/spacer.gif)[Manually adding a camera](index.html#!docs5/ip_cameras_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3Pro_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Alarm panels](index.html#!docs5/alarm,panel_en_3Pro_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon hem_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Pro_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Pro_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Pro_all.md)

|

[Previous](index.html#!docs5/foscam_en_3Pro_all.html) [Next](infrared_en_3Pro_all.md)

Manually adding a camera

**Manually adding a camera**

  
To add a camera manually please go to your Dashboard > Devices > Add Devices >
"I want to add an IP Camera" > click on the "Manually add" .

  
![](/images/mios/man_add.png)  
  
Then on the next screen select the IP of your camera and press next .  
  
![](/images/mios/man_add_1.jpg)  
  
Then on the next screen select the type of camera you want to add (Generic IP
Camera/VistaCam/Panasonic/Foscam), then type in the username and password for
your camera .  
  
Note: If the camera is not detected automatically, power-cycle the Vera unit
and once it finishes to boot up, power-cycle the camera and it should be
detected. If not please type the IP address for the camera.  
  
![](/images/mios/man_add_2.png)  
  
Once you click next you will be able to see a picture from your camera and you
will be able to add it. If you are not able to see the camera after you added
it go to Devices > Cameras > click on View > Settings and follow the steps
below to change the URL of the camera with the correct one as it is shown
below, and if it's in the Supported Cameras list you can find the URL
[here](/supported_cameras_en_all_all.html).  
  

In most cases, IP cameras have a URL method for obtaining a SNAPSHOT or JPG
image from the camera. If your camera supports this method, you can then use
it to see image on the UI and Vera can archive these snapshots over time for
security purposes. Most IP/Network cameras made in the past few years will
have a JPG Snapshot mode. Some examples from Linksys are WVC54GCA,
WVC200/WVC210.  D-link, Trend-Net, and many others make similar cameras.

If your camera is not a 'Plug and Play' model or not on the supported list,
you need to specify the settings for the camera in the camera device control
panel, on the Settings or Advanced tab.

You will need to specify:

1\. the IP address or domain name of the camera;  
2\. the URL or path to retrieve the current image from the camera as a JPEG
file;  
3\. the username and password if the camera requires it.  

The URL (your camera's manual may denote this as "path" or "snapshot address")
needs to retrieve the actual JPEG file, not just an HTML page that has the
JPEG file somewhere on it. For example, if you can view a JPEG file from your
camera with this URL: **<http://192.168.81.5/Snapshot.JPG?Quality=Standard>**,
then put in these settings:

IP Address: **192.168.81.5**  
Path: **Snapshot.JPG?Quality=Standard**

Note: If your IP camera uses a different port then the default 80 port, you
have to type in the IP address of the camera followed by a colon and the port
number: for example:  10.0.1.152:9080 and be sure to provide the
username/password if one is needed. After you specify this information, click
the red 'Save' button, and then you can see the camera by clicking the 'View'
button.  

Note: To store pictures from your camera on our servers, the 12 digit MAC
address of the camera must be added into the MAC field.

![](/images/mios/UI5_IPconfCam.jpg)  

###  Example of using a Linksys WVC54GCA or WVC210 camera with your control
unit

For example, if you can view a JPEG file from your camera with this URL:
<http://192.168.81.5/img/snapshot.cgi>, then put in these settings:  
Domain or IP: 192.168.81.5 (or _YourDomain.MyLinksysCam.com_ if remote access
is enabled)  
Path: img/snapshot.cgi  
A username and password must be used unless all users are allowed in the USERS
section.  

  * If you have more than one camera, you will be using the PORT as part of the URL. If your second camera is on PORT 1024 and the IP is 192.168.81.6, you would use 192.168.81.6:1024 or YourDomain.MyLinksysCam.com:1024 

###  iCAMView and some Lorex network cameras

For [iCAMView](http://www.icamview.co.uk/) based cameras, including a few
Lorex-branded ones, the path would be:  
`showimg_pda.cgi?cam=1 for the first camera`  
`showimg_pda.cgi?cam=2 for the second camera`  

Older models may require slightly different path:  

`pda.cgi?cam=1 for the first camera`

`pda.cgi?cam=2 for the second camera`

Other parameters would be the same as above.

###  Axis IP Cameras

Path: axis-cgi/jpg/image.cgi (or _lastshot.jpg_ depending of the model)  
More information here:  
[Axis live_snapshots](http://www.axis.com/techsup/cam_servers/tech_notes/live_
snapshots.htm)  
[Axis techoverview](http://www.axis.com/techsup/cam_servers/cam_200p/techoverv
iew.htm)

  

