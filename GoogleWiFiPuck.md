#Google Wifi "puck" (AC-1304) and OpenWRT 
  
There is also a "HD2" also known as a GJ2CQ. Unlike the AC-1304 it does not use a USB-C for power, but a DC barrel input (14V@1.1A) instead.   
According to the OpenWRT wiki installation on the GJ2CQ requires soldering a USB port to four test points located on the PCB and using a screwdriver to short the unpopulated SW7 contacts at the appropriate time during installation.   
These GJ2CQ are more round/oval in shape, where the AC-1304 are sharp, round pucks. Thankfully I only have one of these GJ2CQ requiring the soldering skills, so I'll save it till last or pay it forward/give it away/sell it.   
  
If you follow the directions between these links:    
https://openwrt.org/toh/google/wifi   
and with the updated details in this thread https://forum.openwrt.org/t/finally-installed-openwrt-on-my-google-wifi-ac-1304/183541/2 you can get OpenWRT installed on these "pucks" (AC-1304).  
  
Then, if you want to use some of those as repeaters, then follow this tutorial   
https://openwrt.org/docs/guide-user/network/wifi/relay_configuration   
and the video at  
https://www.youtube.com/watch?v=Bfmx5NjIWLQ  
  
I will say, the boot process and intial webUI is sluggish. Once you get logged in, it works ok.   
  
These pucks have 802.11AC on the 5Ghz, and are working well as wiFi repeater for us using the 802.11N as the "backhaul" link to the main router AP.  
  
# Some notes from my install:   
You need the following, and best gather and format/image first before starting:  
- Two (2) thumbdrives, 2GB or larger in size, and it helps if they have an activity light. When updating/flashing the Puck you are "flying blind" without any indicators; it really helps to have the indicator light on the USB drive letting you know things are still happening.   
- Chrome browser on a Windows endpoint, with the OnHub Recovery utility add on installed: https://chromewebstore.google.com/detail/onhub-recovery-utility/fmgkgdalfapcmjnanilfcpkhkhedmpdm?hl=en Noe the OpenWRT install directions point you to the ChromeOS version, which only runs on a recent (non-EoL) version of ChromeOS.   
- Phillips screwdriver, to remove the screw holding the outer case together and the Write-Protect screw  
- spunger and/or smalelr flathead screwdriver, to pop off the base ofthe case to access the Write-Protect screw and the button to force Developer mode.   
  
# To install: 

