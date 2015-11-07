# expresscard-breakout
Simple breakout board for an expresscard socket

## Schematic and board

![Schematic](https://raw.githubusercontent.com/HokieGeek/expresscard-breakout/master/expresscard-breakout.png)
![Board](https://raw.githubusercontent.com/HokieGeek/expresscard-breakout/master/expresscard-breakout.brd.png)

# ExpressCard Pinouts

http://www.usb.org/developers/expresscard/EC_specifications/ExpressCard_2_0_FINAL.pdf

![Pinout Ref Image](http://www.mikrocontroller.net/attachment/35641/Express-Card-Slots-Blockschaltbild-5103.gif)

## Pin groups

### Power

 #  | Name | Function
--- | ---- | --------
 1  |  GND | Ground pin closest to the USB pins
 9  | 1.5v | Not sure what I would use these for, but nice to have access to them
10  | 1.5v | 
14  | 3.3v | Again, not sure if I should break out both of these...
15  | 3.3v | 
20  |  GND | These next three are closest to the PCI Express pins
23  |  GND |
26  |  GND |

I probably don't need to break out these individually. Probably need at most two GND, one 1.5v and one 3.3v

### USB

 #  | Name | Function
--- | ---- | -------- 
 2  | USB D- | USB Data line
 3  | USB D+ | USB Data line
 4  | CPUSB# | Indicate presence of USB module by wiring to GND

### PCI Express

 #  | Name | Function
--- | ---- | --------
 13 | PERST# | A reset?
 16 | CLKREQ# | Request that REFCLK be enabled
 17 | CPPE# | Indicates presence of PCI Express module by wiring to GND
 18 | REFCLK- | 
 19 | REFCLK+ |
 21 | PERn0 | Receive differential pair
 22 | PERp0 |
 24 | PETn0 | Transmit differential pair
 25 | PETp0 |
 
### SMBus

 #  | Name | Function
--- | ---- | --------
 7  | SMBDATA |
 8  | SMBCLK |

### Others

 #  | Name | Function
--- | ---- | --------
 11 | WAKE# | Turns the host on
 12 | 3.3v AUX | Voltage reference source for WAKE#

