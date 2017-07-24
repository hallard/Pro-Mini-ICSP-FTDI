Arduino Pro Mini ICSP and FTDI Programming Board
================================================

This shield is used to flash my Arduino Pro Mini with [OptiBoot](https://github.com/Optiboot/optiboot) bootloader and to upload sketch to it. Optiboot is less Flash consuming than classic one.

Also, for 3.3V device upload at 57600 is slow so I'm using 250000 BPS upload. So I can upload faster and more than that bootloader is using 0.5K of flash instead of 2K, it's a double win configuration, especially with huge sketch like LMIC for my [Mini LORA Board](https://www.thethingsnetwork.org/forum/t/8059/).

I'm using PCB boards with pogo pins and this avoid soldering any headers to the Mini Boards. 

**Features**   

- ICSP 6 pins connector
- FTDI 6 pins connector
- Power LED
- Reset button

**Got V1.0 Boards from [PCBs.io](https://PCBs.io). I tested them, all is fine**

Detailed Description
====================

Schematics
==========

Click on image to zoom   
![schematic](https://raw.githubusercontent.com/hallard/Pro-Mini-ICSP-FTDI/master/pictures/Pro-Mini-ICSP-FTDI-sch.png)  


Boards
====== 

**Top**
<img src="https://raw.githubusercontent.com/hallard/Pro-Mini-ICSP-FTDI/pictures/Pro-Mini-ICSP-FTDI-top.jpg" alt="Top">

**Bottom**
<img src="https://raw.githubusercontent.com/hallard/Pro-Mini-ICSP-FTDI/master/pictures/Pro-Mini-ICSP-FTDI-bot.jpg" alt="Bottom">


You can order PCB at [PCBs.io](https://PCBs.io/share/rm2v2). PCBs.io give me reward when you order my designed boards from their site. This is pretty good, because I can use these rewards to create and design new boards and order boards for a discounted price and share new boards. So if you don't care about PCB manufacturer please use PCBs.io.

Assembled boards (V1.0)
=======================

TBD

Bootloaders
===========

I've compiled some [bootloaders](https://raw.githubusercontent.com/hallard/Pro-Mini-ICSP-FTDI/master/bootloaders/) for you, use the one you prefer, I'm using:

- optiboot_flash_atmega328p_250000_8MHZ.hex (250KBPS) on 3V3 8MHz Mini
- optiboot_flash_atmega328p_250000_16MHZ.hex on 5V 16MHz Mini

I tested the 1MB ones, works fine also

License
=======

<img src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons Attribution-NonCommercial 4.0">
This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International [License](http://creativecommons.org/licenses/by-nc/4.0)

If you want to do commercial stuff with this project, please contact [CH2i company](https://ch2i.eu) so we can organize an simple agreement.

Misc
====
See news and other projects on my [blog](https://hallard.me)
 
