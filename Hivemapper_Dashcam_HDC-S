Hivemapper_Dashcam_HDC-S 

Hivemapper Dashcam HDC S 
Model: HDC-S-0HE1-001
S/N: HDCS 807

Well, this is an “interesting” device, I grabbed it from ewaste thinking this could be a good webcam or security camera. And it is, in a way – a dashcam that they supposedly paid you in cryptocurrency to drive around while this documented the scenery and road. In short, some custom hardware for mapping roads as you drive, so you can earn their custom cryptocurrency which has devalued. These HDC-S models are recently EOL, and are not recognized in windows or OS X (I have not tried Linux or BSD). They are listed for stupid money on eBay, but I was unable to get them to work for anything.

Friends in the Retro community let me know that some Hivemappers a great source of raspberry pi compute modules and HQ cameras, or perhaps movidius powered compute modules (which are far less usable). The models they disassembled had Raspberry Pi CM4 and a HQ camera. 

Before ripping it apart, I looked intro reuse as is – could it be used intact. Unfortunately, the Hivemapper support is via Discord. I reached out, and their support said you could still use it as a dashcam, saving the footage to the SD card.  

Ripped this model S apart, and did not find a media card slot at all. 

I found the proprietary Hivemapper board with the following annotations: 
NG2391C-HM
R7M4E2
On this board are two larger chips: 

TAOGLAS
SGGP-12A 

(RF antennae) https://www.taoglas.com/datasheets/SGGP.12.4.A.02.pdf
https://www.mouser.com/ProductDetail/Taoglas/SGGP.12.4.A.02 

Blox
NEO-M9N-00B-00
G6200573718
2223
0501 32

(GNSS module) https://www.u-blox.com/en/product/neo-m9n-module 
https://www.digikey.com/en/products/detail/u-blox/NEO-M9N-00B/12149174
 

There were three “daughter” cards attached, one being the Intel WiFi module which as the super sticky heat absorption pad on the face, but on the reverse is: 
PB#: J39770-001
Connected to a Molex 2.4/5GHz antennae #146153 

Per https://techinfodepot.shoutwiki.com/wiki/Intel_Dual_Band_Wireless-AC_9260_(9260NGW) this is a Intel Dual Band Wireless-AC 9260 
https://www.intel.com/content/www/us/en/products/sku/99445/intel-wirelessac-9260/specifications.html 

There is the Hellbender LoRa radio card, on the reverse is: 
1923
94V0
ASM: 4602-000002
https://hellbender.com/product/lora-radio/ 

The other “daughtercard” is the brains of this device, the Luxonis OAK-SoM-Pro – Myriad SoM with eMMC flash
On the board: OAK-SoM-Pro-KeemBay DM2399 R1M0E1 
I found the GitHub for their documentation at https://github.com/luxonis/oak-hardware/blob/master/SoMs/OAK-SoM-Pro-S3/DM2399_R1M0E1_Production.step 

And this great PDF with the full breakdown, with this great description https://files.luxonis.com/store-files/oak-som-pro-s3.pdf 
“OAK-SoM-Pro is a System on Module (SoM) designed for integration into top-level systems with a need for a low-power, high performance, real-time AI, and depth perception. It is ideal for use in industrial automation, robotics, and security systems.” 
Per this PDF this board is an OAK-SoM-Pro-S3 (RVC3), 
And the datasheet https://github.com/luxonis/oak-hardware/blob/master/SoMs/OAK-SoM-Pro/OAK-SoM-Pro_Datasheet.pdf  

This is the 2nd generation Hivemapper per their web site 
https://docs.hivemapper.com/contribute/driving 
“The Hivemapper Dashcam S (“HDC-S”) was the second-generation model. It provided additional functionality such as 4K video for personal use. The HDC-S was discontinued in 2024…”

And possibly sold for $649?!?! https://heliumdeploy.com/products/hivemapper-dashcam-s


Documentation:
https://docs.hivemapper.com/cameras/hdc-and-hdc-s/start-driving-and-mapping-hdc-hdc-s 
https://docs.hivemapper.com/cameras/hdc-and-hdc-s/install-an-hdc-s
https://www.youtube.com/watch?v=q5Fagw8oGbc 


Thoughts: 
Pay to purchase the hardware for a system that “gifts” crypto which is devalued (and likely worthless at this point). While further impacting our ecosystem and global warming by driving around AND the mining of the currency. Create more ewaste with devices that are EoL after a short while, are unable to be reused – and do not support updating the firmware for that reuse. 
Utter trash, IMHO. 

Posted with some images: https://defcon.social/@Irishmasms/116342774349223612 

EOF

