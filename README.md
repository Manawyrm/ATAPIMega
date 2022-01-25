ATAPIMega
=============================
![PCB render](https://screenshot.tbspace.de/gljmedvurbk.png)

### Overview

[ATAPIMega](https://github.com/Manawyrm/ATAPIMega) is a hardware project which allows regular (P)ATA CD/DVD drives to be used as a standalone Audio-CD player.  
This repository contains KiCAD PCB design and schematic for the CD player.  

The PCB accepts (regulated!) 12V DC power via a 5.5mm/2.1mm barrel jack and outputs 12V/5V for the CD drive.  
The microcontroller is an ATmega2560 (Arduino Mega-compatible), chosen for 5V-I/O voltage and high pin-count (and bad availability of STM32's in the component shortage of 2021).

### Manufacturing
The PCB can be fully assembled at [JLCPCBs](https://jlcpcb.com/DDE) assembly service, including through-hole parts. Only the LCD will have to be installed manually.
Manufacturing files for automatic assembly service can be found at `gerbers/RevA/ATAPIMega/`.  

Due to the high amount of extended components, setup fees are quite high (~30$).  
Price will decrease significantly with higher board count (~15$/board).

### Additional info 

[Schematic](gerbers/RevA/ATAPIMega/ATAPIMega.pdf)  
[Interactive BOM](https://tbspace.de/content/downloads/atapimega-ibom-reva.html)  
[Firmware](https://github.com/Manawyrm/ATAPIMega-Firmware)  

### Errata
Rev.A: FTDI / UART connector reset circuitry is wrong, needs bodge resistor!

### Future improvements
- mounting holes
- labeling of audio ports (LGGR, etc.)
- power switch

### Credits
5V Step-Down switch-mode regulator was designed with a lot of help from [@Toble_Miner](https://github.com/TobleMiner)! Thanks!
