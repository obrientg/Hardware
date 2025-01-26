# Google Wifi "puck" (AC-1304) and OpenWRT  
    
Note there are two verisnos of the "puck". There is also a "HD2" also known as a GJ2CQ. Unlike the AC-1304 it does not use a USB-C for power, but has a DC barrel input of 14V at 1.1A instead.   
According to the OpenWRT wiki, installation on the GJ2CQ requires soldering a USB port to four test points located on the PCB and using a screwdriver to short the unpopulated SW7 contacts at the appropriate time during installation.   
These GJ2CQ are more round/oval in shape, where the AC-1304 are sharp, round think white hockey pucks. Thankfully, I only have one of these GJ2CQ requiring the soldering skills, so I'll save it till last or pay it forward/give it away/sell it. These AC-1304 will be put to good use though.    
  
If you follow the directions between these two OpenWRT pages:    
The [information page with the older instructions at https://openwrt.org/toh/google/wifi]  
and with the updated details in [this forum post thread at https://forum.openwrt.org/t/finally-installed-openwrt-on-my-google-wifi-ac-1304/183541/2]( https://forum.openwrt.org/t/finally-installed-openwrt-on-my-google-wifi-ac-1304/183541/2) you can get OpenWRT installed on these "pucks" (AC-1304).  
  
Then, if you want to use thge puck as a repeater, then follow the [OpenWRT tutorial at https://openwrt.org/docs/guide-user/network/wifi/relay_configuration](https://openwrt.org/docs/guide-user/network/wifi/relay_configuration)      
and the [Youtube video at https://www.youtube.com/watch?v=Bfmx5NjIWLQ](https://www.youtube.com/watch?v=Bfmx5NjIWLQ)      
  
There are also directions on the OpenWRT web site/wiki/fourums on how to implement mesh, but I have not gone down that path as of yet. 
  
# Performance  
I will say, the boot process and intial webUI is sluggish. Once you get logged in, it works ok.   
  
These pucks have 802.11AC on the 5Ghz, and are working well as wiFi repeater for us using the 802.11N as the "backhaul" link to the main router AP.  
  
# Some notes from my install:   
You need the following items, and best gather and format/image first before starting:  
- Two (2) thumbdrives, 2GB or larger in size, and it helps if they have an activity light. When updating/flashing the Puck you are "flying blind" without any indicators; it really helps to have the indicator light on the USB drive letting you know things are still happening.   
- Chrome browser on a Windows endpoint, with the [OnHub Recovery utility add on installed, downloaded from https://chromewebstore.google.com/detail/onhub-recovery-utility/fmgkgdalfapcmjnanilfcpkhkhedmpdm?hl=en](https://chromewebstore.google.com/detail/onhub-recovery-utility/fmgkgdalfapcmjnanilfcpkhkhedmpdm?hl=en). Note the [OpenWRT install directions point you to the ChromeOS version](https://openwrt.org/toh/google/wifi) of OnHub Recovery, which only runs on a recent (non-EoL) version of ChromeOS.   
- Phillips screwdriver, to remove the screw holding the base of the puck from the rest of the outer case and the Write-Protect screw located inside.  
- [Spudger](https://en.wikipedia.org/wiki/Spudger) and/or small flathead screwdriver, to pop off the base of the case after removing the screw holding it secure to the rest of the puck. You need this access to remove the Write-Protect screw and the button to force Developer mode.  
- Some sort of non-conductive stick to press the Developer mode button  
- Two (2) Ethernet cables: one to conenct the puck WAN port to your internet connection, the other connected to the puck's LAN port and the laptop you are working from  
- A laptop to work from, with SCP and SSH capabilities (you will be logging into and uploading flies to the puck)  
- Power supply for said laptop  
- Power with USB C to power the Puck via the USB hub  
- A USB hub having USB C power in & able to power the puck, along with USB A to connect the USB thumbdrive with the firmware  
- Your beverage of choice, you need to stay hydrated  

# USB thumbdrive & firmware prep:   
  
Before we start the install, best get the thumbdrives imaged with the OnHub Recovery utility and the initial OpenWRT image:  
  
# To install:  
First you need to install the default, known good puck image via the OnHub Recovery utility  
  
