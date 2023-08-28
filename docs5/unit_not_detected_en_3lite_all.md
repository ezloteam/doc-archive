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

![](skins/mios/images/plus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3lite_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit_en_3lite_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote_en_3lite_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device_en_3lite_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3lite_all.md)

![](skins/mios/images/plus.gif)[Glossary &
References](index.html#!docs5/reference_en_3lite_all.md)

![](images/spacer.gif)[Manual Z-Wave Routing](index.html#!docs5/ManualRoute_en_3lite_all.md)

|

[Previous](index.html#!docs5/zwave_troubleshooting_en_3lite_all.md)
[Next](index.html#!docs5/remote_en_3lite_all.md)

Undetected Unit

If your unit is not detected by <http://cp.mios.com/firmware> can be caused by
the followings:  
  
1\. _Your unit doesn't have Internet access_. (You should see WAN led
blinking.)  
FIX: Connect your computer directly to your unit and manually adjust the
network settings after you check the network connections and power cycle the
unit.  
  
2\. _After the upgrade to UI5, your Vera didn't get the new corresponding
servers_.  
Connect directly to your LAN port of your Vera and type this in your web
browser:<http://192.168.81.1/cgi-bin/cmh/sysinfo.sh>  
If you see this line: **"evtserver": "",** then you should enable Remote
Assistance and submit a ticket.  
FIX: Contact tech support after enabling remote assistance.  
Please go to Setup -> Tech support and click the Enable full access button and
send us the text information from the left side of this button (button now
shows Disable). (Ex: Tech support full control enabled, access code xxxxx-
xxxxxx (ssh reference: SSH_22=xxxxx
TS_SRV=[ts2.tssrv.com](http://ts2.mios.com/)) ). Fill in your contact
information and the details of your problem and press the submit button. We
need to have full access to verify your whole logs to see what's happening
with your unit.  
  
3\. _Your ip address and your unit ip address are different._  
Point your pc browser to [http://whatismyip.org](http://whatismyip.org/) .Note
the number, then connect to Vera's LAN port and go to Setup->Net&Wi-
Fi->Troubleshoot Network and note the External IP.  
If the numbers aren't the same your unit won't be detected to be in the same
network.  
FIX: Connect your computer to the Internet through Vera's LAN port or wireless
Vera network.  
  
*Note:1) Check your proxy settings also, if you're connecting through a proxy, your ip will be different than your Vera unit. Disable proxy for the setup part.  
2) If you have a GSM card/modem in your pc, this will have a higher priority,
and you'll connect through it to the internet, not through your home
router/Vera unit.  
  
4\. _Your unit is detected but you can't connect to it (ERROR: Cannot
communicate with your Vera.)_  
*Note: This applies only if you connect to the internet through the same network as your Vera unit (your pc and your Vera WAN port are plugged into the same router/switch).  
      \- You've manually configured your Vera unit network settings and setup the Firewall to ON.  
FIX: Change Vera's firewall to OFF.  
  
      \- You're network configurations are wrong. I've encountered cases when people configured their routers internal private network to 192.169.xxx.xxx or 172.35.xxx.xxx, etc.  
*Note: Your internal network should have valid private ip addresses from A, B or C class. More info here: <http://en.wikipedia.org/wiki/Private_network>  
If your Vera unit doesn't have a private ip address it will be directly
accessed from the Internet and will have its firewall ON.  
FIX: Correct your network settings or if they are correct, connect to the
Internet through your Vera's LAN port for the setup part.  

  

