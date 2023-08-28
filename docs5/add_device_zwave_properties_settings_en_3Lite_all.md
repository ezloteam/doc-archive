![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Lite_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Guided Feature Walkthroughs
](features_en_3Lite_all.html)

![](skins/mios/images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Advanced Settings](index.html#!docs5/advanced_settings_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Net & Wi-Fi](setup_en_3Lite_all.html_network_settings_connect_to_the_internet)

![](images/spacer.gif)[Backup](index.html#!docs5/advanced_settings_backup_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Logs](advanced_settings_en_3Lite_all.html_logs)

![](images/spacer.gif)[Firmware Upgrades](index.html#!docs5/advanced_settings_downloads_en_3Lite_all.md)

![](images/spacer.gif)[Reset Vera to Factory Defaults](index.html#!docs5/reset_factory_defaults_en_3Lite_all.md)

![](images/spacer.gif)[Z-Wave Options](index.html#!docs5/zwave_options_en_3Lite_all.md)

![](skins/mios/images/minus.gif)[Z-Wave Device Properties](index.html#!docs5/add_device_zwave_properties_options_en_3Lite_all.md)

![](images/spacer.gif)[Advanced](index.html#!docs5/add_device_zwave_properties_advanced_en_3Lite_all.md)

![](images/spacer.gif)[Device Options](index.html#!docs5/add_device_zwave_properties_dev_option_en_3Lite_all.md)

![](images/spacer.gif)[Logs](index.html#!docs5/add_device_zwave_properties_logs_en_3Lite_all.md)

![](images/spacer.gif)[Notifications](index.html#!docs5/add_device_zwave_properties_notifications_en_3Lite_all.md)

![](images/spacer.gif)[Settings](index.html#!docs5/add_device_zwave_properties_settings_en_3Lite_all.md)

![](images/spacer.gif)[Add Z-Wave Dongle With Different Frequency](index.html#!docs5/changing_zwave_port_en_3Lite_all.md)

![](images/spacer.gif)[Z-Wave Advanced Options](index.html#!docs5/zwave_device_advanced_en_3Lite_all.md)

![](images/spacer.gif)[Full/Low Power Inclusion/Exclusion](index.html#!docs5/full_power_inclusion_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3Lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3Lite_all.md)

|

[Previous](index.html#!docs5/add_device_zwave_properties_notifications_en_3Lite_all.md)
[Next](index.html#!docs5/changing_zwave_port_en_3Lite_all.md)

Settings

  
Here are all the settings that an user has to apply to an device and all the
information about that device that are relevant to the end user.  
  
![](/images/mios/UI5_devSettTab.PNG)  
  
  
Automatically Configure:  

Normally you should leave the default behavior, as specified on the 'Z-Wave
device' -> 'Z-Wave Options' page from the Toolbox, by leaving 'By default Vera
should automatically configure devices' checked, with all your devices set to
'Use the default'.  
This way Vera will automatically configure all your devices. In many cases,
the devices will not work unless Vera configures them, and generally you will
always want Vera to do this for you. The only exception is when you have
another Z-Wave controller configuring your devices, and you've made some
special settings there, and you don't want Vera to change them.

Even you do have have another Z-Wave controller, it's still okay to let Vera
configure your Z-Wave devices. The only problem may arise when it comes to
associations. If you don't know what Z-Wave associations are, just accept the
default settings, which are necessary if you want certain types of devices,
like sensors, to work with Vera.

For those interested in an explanation of what this means, read on...

In a Z-Wave network, some of your devices support what are called
"Associations" (also called the Z-Wave command class association).  
This is how a device that sends messages knows where to send those messages.
For example, motion sensors send messages when the sensor is tripped,
thermometers may send messages when the temperature changes, and so on. Often
times these devices have their own proprietary mechanism for setting
associations, which is not standardized.  

For example, a motion sensor may provide instructions in the user's manual for
how to associate it with a light switch so it turns the light switch on when
the sensor is tripped. Generally, it's much easier to let Vera manage the
associations for you.  
If you let Vera do this, Vera will associate all devices that send messages
with Vera, telling them all to send the messages to Vera so she can process
them for you.  

For example, Vera can tell any motion sensors and thermometers to send all
messages to Vera, and that way, you can attach events to your scenes so Vera
will run a scene, like turning on a light, when a motion sensor is tripped, or
closing the blinds when the temperature is over 90 degrees to save energy.  
If these devices are not associated with Vera, Vera will never get the
messages. The catch is that if you have previously set up associations, those
associations will be lost when Vera configures the device, because Vera will
manage the associations.  
The recommended solution is still to let Vera handle the configuring, but just
tell Vera what extra associations you want as explained in the 'Associations'
section below. Then Vera will set her own associations, and will also add
whatever associations you specify.  
You can also disable automatic configuration, either for an individual device
or globally, with this check box, and then Vera won't do anything with the
device's associations.

When you have added new devices and they appear on the 'Unassigned Devices'
page, you have the option of turning off Vera's configuration in case you have
already set up the associations before getting Vera, and you don't want Vera
to take over this and change the associations you previously set up.

Polling Interval

Polling is the process where Veratries to ask a Z-Wave device for its current
status, like if it's On or Off, at what temperature, and so on. This is how
Vera knows when the status of a device changes, such as when the temperature
has changed if it's a thermostat, or if you manually turned a light on or off.
Normally Vera attempts to poll one Z-Wave device every 10 seconds, and Vera
polls the devices in order until Vera has polled all of them. So the delay
between polling nodes depends on how many nodes you have. If you have 6 nodes,
each node will be polled once a minute, and if you manually turn a light off,
within a minute or so Vera's dashboard will show the light is off. But, if you
have 100 Z-Wave devices, it can take 16 minutes before Vera has polled them
all. You can change the polling behavior from here.

Watts:

Very few Z-Wave devices are actually able to report how much energy they are
using, so Vera generally estimates this based on the device's wattage. By
default each light will have 100 watts. If the light really is a 100 watt
light, you can leave it. If not, put in the actual wattage, which is usually
printed on the bulb. Remember that if multiple lights are on the same Z-Wave
switch you should add their wattages. You can also specify the wattages for
appliance modules; for example, if you have a 200-watt fan plugged into an
appliance module, you would type "200" for this device's wattage. Vera will
constantly poll all the Z-Wave devices in your home to see if they are on, off
or dimmed to a certain level, and Vera will use this to estimate the
electricity being used. Also see: [Energy](index.html#!docs5/energy_en_all_all.md)

Capabilities: The Z-Wave capabilities (classes) that this device reports to be
able to implement.

Neighbors: The other zwave devices to which this device is in direct
communication. On a zwave network a message can be relayed 4 times until it
receives its destination.

Configure at: The date and time when the device was last time configured. If
it appears N/A it means that the device wasn't yet configured. If it's a
battery operated device you should first wake it up and then press the
"Configure node right now" button.

Configure node right now: This causes Vera to attempt to configure the device
immediately. After clicking this button you see the job icon for 'Configuring
the Device' next to the device description and it will turn green if Vera was
able to configure the device, or red if Vera was not. (See [diagram of job
icons](index.html#!docs5/diagram_of_jobs_icons_en_all_all.md)) Some devices, like
motion/door/window sensors, are generally not functional until they are
configured.  
If they are not configured, you will see the configure job icon in red. But if
the device is battery operated, it's quite possible that, in order to conserve
battery life, the device goes into a 'sleep mode' during which the Z-Wave
radio is turned off, and Vera cannot configure it.  
These battery operated devices typically wake up every few hours and announce
that they're going to be awake for a few seconds. When this happens, Vera will
use that opportunity to configure the device.  
So, if you added a battery operated device and you see the red 'Configure Job'
icon, indicating the device is not configured and is not usable, you can check
back the next day and it probably will be configured. Often times, the sensors
allow you to remove and reinsert the batteries, or to press a button, and this
will force them to listen to the Z-Wave network for a minute or two.  
If you have a sensor like this, you can then manually 'wake it up', and then
you can promptly click the 'Configure Node Right Now' button to make Vera try
to configure the device. This button is also useful if you have changed
specific Z-Wave configuration and association settings and want to see them
applied right away, as explained below.

  

