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

![](skins/mios/images/minus.gif)[Door locks](index.html#!docs5/door_locks_en_3pro_all.md)

![](images/spacer.gif)[Kwikset Door Lock](index.html#!docs5/kwikset_lock_en_3pro_all.md)

![](images/spacer.gif)[Schlage Door Lock](index.html#!docs5/schlage_lock_en_3pro_all.md)

![](images/spacer.gif)[Yale Door Lock](index.html#!docs5/yale_door_lock_en_3pro_all.md)

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

[Previous](index.html#!docs5/zwave_devices_en_3pro_all.md)
[Next](index.html#!docs5/kwikset_lock_en_3pro_all.md)

Door locks

The supported locks are the Schlage lock, Kwikset and Yale.  
  
Door locks are a special breed of Z-Wave devices which require an exchange of
security keys with Vera during the 'Include' ("pairing") process.
Accordingly, the normal 'Include' procedure - carrying Vera to the devices -
will work with locks.  
When you include a door lock please make sure that you have Vera at about 3
feet - 5 feet from it. If you can bring your Vera while still connected to the
Internet, and try the[ Full Power
Inclusion](index.html#!docs5/full_power_inclusion_en_all_all.md) and follow the steps for the
specific door lock.  
If you're not able to have Vera connected to the Internet, make sure you
follow the [inclusion process](/include_mode_en_all_all.html) steps and that
Vera is at 3 feet from the door lock.  
  
IMPORTANT: After pairing the door lock with Vera, please make sure you bring
Vera out of inclusion mode by tapping the Z-Wave button once more, having the
Z-Wave light stable and please leave Vera about 5 minutes close to the door
lock to let it finish the configuration process.  
  
Adding Range to your lock  

  * For Z-Wave to route properly to your lock, you must make sure there is at least one security compatible (enabled) Z-Wave device in direct range of it.
  * Many newer Z-Wave devices support Beaming, including any GE/Jasco lamp modules/switches with the following versions:
    * 2.0a
    * 3.0a
    * 2.0b
    * 3.0b
    * NOT 2, 2.0, 3, or 3.0
  
To add a pin code to a lock  

  * Click the ![Wrench](/images/mios/setup_icon_UI5.png)button for the lock
  * Click the "Pin Codes" tab
  * Enter a name for the pin code you want to add
    * Note: Once you add a pin code, you won't be able to see the code, you'll only be able to refer to it by the name you give it here.
  * Enter the pin code you want to add
    * Check your lock's manual to see how many digits you can have in your pin code
To add a timer for a pin code  

  * Click the ![Wrench](/images/mios/setup_icon_UI5.png)button for the lock
  * Click the "Pin Codes" tab
  * Select "Daily" or "Weekly" from Add Schedule dropdown next to the pin code you want to schedule
To add a notification for a pin code  

  * Click the ![Wrench](/images/mios/setup_icon_UI5.png)button for the lock 
  * Click the "Notifications" tab 
  * Select "Add notification for:"
  * Select "A pin code is entered"
  * Fill in the "Notification Name:"
  * Fill in the field "Which pin code number" with the number of order of the pin code desired to create a notification for. You can check the number of order in the "Pin Codes tab" in front of each pin code preceded by a "#"
  * Click the "Add" button, close the Door lock settings and click on "Save"

## Reverse the Lock/Unlock Status

If the lock/unlock status of your door lock is backwards, meaning Vera's
'Dashboard' shows it is locked when it's really unlocked and vice-versa, it's
possible the lock was oriented upside-down when mounted. To solve this issue:

  * Click the ![Wrench](/images/mios/setup_icon_UI5.png)button for the lock
  * Click the "Advanced" tab
  * At "New service:" enter "urn:micasaverde-com:serviceId:HaDevice1"
  * At "New variable:"  enter "ReverseOnOff"
  * At "New value:" enter "1"
  * Click the "Add" button, close the Door lock settings and click on "Save".



  

  

