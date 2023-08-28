![](skins/mios/images/logo.png)

UI5 manual

  
---  
  
![](images/spacer.gif)[Install & System
Requirements](index.html#!docs5/installation_and_system_requirements_en_3Pro_all.md)

![](images/spacer.gif)[Basic System Setup ](index.html#!docs5/getting_started_en_3Pro_all.md)

![](images/plus.gif)[Guided Feature Walkthroughs ](index.html#!docs5/features_en_3Pro_all.md)

![](images/plus.gif)[Vera Web Portal](index.html#!docs5/web_portal_en_3Pro_all.md)

![](images/plus.gif)[Advanced
Configuration](index.html#!docs5/advanced_configuration_en_3Pro_all.md)

![](images/plus.gif)[Vera Compatible
Devices](index.html#!docs5/supported_hardware_en_3Pro_all.md)

![](images/minus.gif)[Diagnostics &
Troubleshooting](index.html#!docs5/troubleshooting_en_3Pro_all.md)

![](images/spacer.gif)[Network Troubleshooting](index.html#!docs5/network_troubleshooting_en_3Pro_all.md)

![](images/spacer.gif)[Initial Connection](index.html#!docs5/initial_connection_en_3Pro_all.md)

![](images/plus.gif)[Z-Wave Troubleshooting](index.html#!docs5/zwave_troubleshooting_en_3Pro_all.md)

![](images/spacer.gif)[Undetected Unit](index.html#!docs5/unit not detected_en_3Pro_all.md)

![](images/spacer.gif)[Remote access](index.html#!docs5/remote access_en_3Pro_all.md)

![](images/spacer.gif)[Device stopped communicating](index.html#!docs5/Device stopped communicating_en_3Pro_all.md)

![](images/spacer.gif)[Developer Resources](index.html#!docs5/developers_en_3Pro_all.md)

![](images/plus.gif)[Glossary & References](index.html#!docs5/reference_en_3Pro_all.md)

|

[Previous](index.html#!docs5/troubleshooting_en_3Pro_all.md)
[Next](index.html#!docs5/initial_connection_en_3Pro_all.md)

Network Troubleshooting

By default Vera automatically configures its network, if you connect it to
your router it will automatically configure in switch mode.  
If after plugging Vera into your network, you don't see your Vera on
cp.mios.com , please follow these steps to fix your networking:  

  * Unplug Vera from the power cord 
  * Unplug all the cables from Vera 
  * Plug a cable from your computer into Vera's LAN port
  * Plug Vera into the power cord 
  * Wait it to start and for your computer to get an IP address:
  * In windows you can type this in Start->Run to view it: cmd /K ipconfig 
  * In linux and mac you have to start a terminal and type there ifconfig | grep -B1 "inet addr"
  * By default you should receive an IP from Vera that should be in the range 192.168.81.100 - 192.168.81.254 
  * If you've changed the default LAN IP in Vera you'll receive an IP from that range 
  * If you've disabled Vera's dhcp server you won't receive an IP and you'll have to setup one manually on you pc 
    * In Windows 7
      * Open Control Panel
      * View by: Large icons -> Network and Sharing Center
      * View by: Category -> View netork status and tasks
      * Click on Change adapter settings
      * Right click on LAN connection to Vera , then click on Properties
        * Highlight the Internet Protocol Version 4 (TCP/IPv4) item, and click on Properties
        * In the IP address field enter 192.168.81.10
        * In the subnet mask field enter 255.255.255.0
        * In the Default gateway field enter 192.168.81.1
        * Click OK
      * Click OK Again  

    * In Windows XP  

      * Open Windows Start menu.
      * Open Control Panel.
      * Classic view: Open Network Connections
      * Category view: Select Network and Internet Connections, and then Network Connections.
      * Double-click on your the LAN connection to Vera.
      * Click Properties.
        * In the General tab, highlight the Internet Protocol (TCP/IP) item, and click Properties.   

        * In the IP address field enter 192.168.81.10
        * In the subnet mask field enter 255.255.255.0
        * In the Default gateway field enter 192.168.81.1  

        * Click OK
      * Click OK again
    * In Mac OS X
      * Open the Apple Menu(Top left corner of your screen)
      * Click System Preferences
      * Click Network
      * Click the Locations dropdown and select Edit Locations
      * Click the plus sign and call your new location "Vera system Troubleshooting"
      * Select "Ethernet" from the list on the left
      * Select "Manually" from the Configure IPv4 dropdown
        * Enter 192.168.81.10 in the IP address field
        * Enter 255.255.255.0 in the subnet mask field
        * Enter 192.168.81.1 in the Router field  

        * Hit "Apply"
  * after you have an ip on your PC and you can ping Vera's ip successfully open an web browser and type this in the address bar: 192.168.81.1 
  * Vera's web interface should open and then go to Setup->Net&Wi-Fi 
  * check the Internet settings: If Vera connects directly to your cable or DSL modem, select "Directly to the internet. Vera is a gateway" If Vera is plugged into your router, select "Through another gateway on my network. Vera is a switch" If you want Vera to connect wirelessly, you'll need to enter your wireless network information(ssid, key) and make sure to disconnect Vera's eth1 port from your network. 
  * In order to activate the MiOS service you'll first need to make an account on cp.mios.com, and add your Vera to your account while on the network with it from cp.mios.com

  

