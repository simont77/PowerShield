# PowerShield
 This design is an extension board for any Raspberry Pi based astronomy tool, like Astroberry or StellarMate.
 The repository contains the electrical (ECAD) and mechanical (MCAD) design files.
 
# Electrical Design (ECAD)
 ![Alt text](./ECAD/pics/Astroberry_assembled_PCB_ISO_back.png?raw=true "Title")
 ![Alt text](./ECAD/pics/Astroberry_assembled_PCB_ISO_front.png?raw=true "Title")
 
## Features
* One power input
* 4pcs switchable (ON/OFF) not regulated outpus, each has maximum 3A load capability (CH1 ... CH4 - DC jack)
* 2pcs switchable (ON/OFF) or PWM controlled outputs, also with maximum 3A load capability for dew heaters (DEW1 and DEW2 - RCA)
* Fuse monitoring signals for each outputs, to detect fuse burn
* Integrated 5V/3A SMPS to power Raspberry Pi
* Integrated BME280 to measure, temperature, pressure and humidity
* Integrated GPS module with integrated antenna
* Connecting external GPS antenna
* Fan connector, supports 3,3V and 5V fans, fan can be switched ON/OFF.
* Input voltage monitoring, maximal range 20V
* Total output current monitoring, maximal range 16A, allowed total ouput curren is 15A
* Reverse polarity protection
* 4 pin 3,5mm jack to connect external sensors, or extension boards, communication interface can be selected with jumpers, I2C or one wire
* LED feedback for each outputs
* LED for GPS, e.g. show 3D fix (usage of this LED is SW dependent)

List of used ports and their funtions will be available in the Wiki section.

## What works
 Every features listed above are tested and working. Testing was done with terminal commands, like "gpio" or with testing scripts.

## What is not working
 Check the "Issues" section.

## What is needed
* INDI driver is not available.
* I am planning to perform thermal measurement, to see what is board thermal behaviour under maximal load condition.

# Mechanical Design (MCAD)
 Mechanical design was done based on Hammond Extruded Aluminum Enclosures design.
 
 ![Alt text](./Astroberry_assembly_ISO_front.png?raw=true "Title")
 ![Alt text](./Astroberry_assembly_ISO_back.png?raw=true "Title")
 
 The "extruded" part of the housing is prepared for 3D printing.
 The front and back plates are design in KiCAD as well and manufactured from 1,6mm thick PCB, the panelized gerber files are uploaded in the repository.

# Licence
 The licence is the CERN Open Hardware Licence version 2, and variant CERN-OHL-S
 Check the "LICENCE" file or original location of the licence:
 https://ohwr.org/cern_ohl_s_v2.txt
 
# Donation
If you like the design, think about to support me with a cup of coffee, a glas of beer...
This could help to develop further this design.

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=PK5PGMN5WKTRN&source=url)
