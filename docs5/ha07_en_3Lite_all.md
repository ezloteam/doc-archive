![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Lite_all.md)

![](images/plus.gif)[Guided Feature Walkthroughs ](index.html#!docs5/features_en_3Lite_all.md)

![](images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Lite_all.md)

![](images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Lite_all.md)

![](images/minus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](images/minus.gif)[Z-Wave Devices](index.html#!docs5/zwave_devices_en_3Lite_all.md)

![](images/plus.gif)[Door locks](index.html#!docs5/door_locks_en_3Lite_all.md)

![](images/plus.gif)[Lighting Devices](index.html#!docs5/lighting_devices_en_3Lite_all.md)

![](images/spacer.gif)[Plug and Receptacle Devices](index.html#!docs5/plug_devices_en_3Lite_all.md)

![](images/spacer.gif)[Thermostats](index.html#!docs5/thermostats_en_3Lite_all.md)

![](images/spacer.gif)[Window Coverings](index.html#!docs5/window_coverings_en_3Lite_all.md)

![](images/spacer.gif)[Sensors](index.html#!docs5/sensors_en_3Lite_all.md)

![](images/minus.gif)[Scene Controllers](index.html#!docs5/scene_controllers_en_3Lite_all.md)

![](images/spacer.gif)[Leviton Scene Controller](index.html#!docs5/leviton_scene_controller_en_3Lite_all.md)

![](images/spacer.gif)[Intermatic Handheld Remotes](index.html#!docs5/ha07_en_3Lite_all.md)

![](images/spacer.gif)[Intermatic CA5100](index.html#!docs5/Intermatic_CA5100_en_3Lite_all.md)

![](images/plus.gif)[Network Cameras](index.html#!docs5/ip_camera_en_3Lite_all.md)

![](images/plus.gif)[IR devices](index.html#!docs5/infrared_en_3Lite_all.md)

![](images/spacer.gif)[Insteon Devices](index.html#!docs5/Insteon_en_3Lite_all.md)

![](images/plus.gif)[Alarm panels](index.html#!docs5/alarm_en_3Lite_all.md)

![](images/spacer.gif)[Aeon Home Energy Monitor](index.html#!docs5/aeon_en_3Lite_all.md)

![](images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](images/plus.gif)[Glossary & References](index.html#!docs5/reference_en_3Lite_all.md)

|

[Previous](index.html#!docs5/leviton_scene_controller_en_3Lite_all.md)
[Next](index.html#!docs5/Intermatic_CA5100_en_3Lite_all.md)

Intermatic Handheld Remotes

Add Intermatic Handheld Controller (HA07 and HA09 )  
  
If the remote has already been included in another Z-Wave network, you need to
do a factory reset on it first, as explained below, before you can add it to
Vera.  
  
Adding the remote to your Z-Wave network  
  
1\. Be sure the remote is not already paired with another network. Do a
factory reset as explained below if you're not sure.  
  
2\. Take the remote near Vera and choose Devices -> Add Devices -> Advanced
Z-Wave devices -> and here you will find the option for remotes and scene
controllers Add one.  
  
3\. On the HA07, press and hold 'include' for a few seconds until it says
'copy', and then press the '1 off' button. It should say 'Copy RA' while
transferring to Vera, and then say 'successful' when it's done.  
On the HA09 (no screen) press and hold 'include' for 5 seconds. Both the red
and green LEDs at the top will flash. Press and release Scene 1 'off'. The
green LED will flash while configuration is transferred. The green LED will
turn solid for 2 seconds upon successful transfer, or both will flash for 2
seconds on failure.  
  
4\. After a few seconds you should see the remote show up as an unassigned
device on the Devices tab in Vera's setup site. If not, reload the web page.
Pick the room the remote is in, and give the remote a name if you want.  
  
If you do not want Vera to assign scenes to the remote, but will do that using
another device, you can stop here. If you want Vera to assign scenes, keep
going with step 5.  
  
5\. On the scenes tab in Vera's Dashboard, create the scenes you want assigned
to the scene controller. Click the red 'save' button to save your scenes. If
you haven't yet added all the lights and other Z-Wave devices you want in the
scene you'll have to do that first, of course, and come back to this step
later. When you create a new scene on the triggers tab click the 'Add Trigger'
button for your scene. For 'Device:' select the remote controller, 'What type
of event is trigger?' select 'A scene is activated'. Then enter a name and the
scene button you want to trigger the scene, a number between 1 and 5 for the 5
scene buttons.  
  
After you save your changes, turning on the scene button triggers the scene.
Note that the scene can include delays. For more information please check this
[page](http://faq.mios.com/content/2/10/en/how-to-create-a-scene-with-
schedules-and-delays.html).  
  
The 5 scene buttons on the scene controller can be turned 'on' or 'off'.
Turning the scene on triggers the scenes 1 through 5. Turning the scene off
does not turn the devices in the scene off as you would expect. Rather,
turning off any of the 5 buttons causing Vera to trigger scene 0. So if you
create a scene with the event for 'scene 0', it will be triggered whenever you
turn off any scene. You can create a scene as described above, and in step 5
choose button #0. But this means that no matter which of the 5 scene buttons
you turn off, they all trigger the scene for button #0.  
If this is confusing, just stick to the normal usage of buttons 1-5, but be
aware that if scene 2, for example, is 'on' (ie the LED is lit), you will need
to press '2' twice to get it to run the scene again. So, using this method,
the normal way to turn off the lights is to have a scene which turns the
devices off and assigns it to a button. For example, scene '1' could be your
'bright' scene, scene '2' could be your 'dinner scene', and scene '3' could be
your 'living room lights off' and scene 4 could be your 'all lights off'
scene.  
  
  
Removing the remote from your Z-Wave network  
  
If you already paired the remote and want to remove it:  
  
1\. On Vera's setup page go to Devices -> Add devices -> Advanced Z-Wave
Devices  
2\. Chose 'Exclude' from the drop-down menu and full power  
3\. Click 'Go'  
4\. Then press the same sequence as in Step #3 during the 'Add' process
(above).  
  
Doing a Factory Reset  
  
Intermatic HA07 Remote  
  
1\. Press and hold [Include]+[Delete] for several seconds until it says
'Reset'.  
2\. Then press and hold 'Scene 1' [On] and 'Scene 1' [Off] for several seconds
it says 'all clear'.  
  
Intermatic HA09 Remote  
  
Reset Scenes and Network:  
1\. Press and hold [Include]+[Delete] for 10 seconds until the red and green
lights blink alternately.  
2\. Press and hold [1 ON]+[1 OFF] until the green light remains solid.  
Reset Scenes Only:  
1\. Press and hold [Include]+[Delete] for 10 seconds until the red and green
lights blink alternately.  
2\. Press and hold [2 ON]+[2 OFF] until the green light remains solid.

  

