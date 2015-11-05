# expresscard-breakout
Simple breakout board for an expresscard socket


## ExpressCard Pinouts

See issue #1, annoyingly

## Pins of interest

### Power and others

 #  | Name | Function
--- | ---- | --------
 1  |  GND | Ground pin closest to the USB pins
 9  | 1.5v | Not sure what I would use these for, but nice to have access to it
10  | 1.5v | 
11  | WAKE# | Hmm...
12  | 3.3v AUX | Available for limited operations such as creating wake requests when the host is suspended
14  | 3.3v | My bread and butter, I guess... I wonder if I want to include a booster circuit for 5v?
15  | 3.3v | 
20  |  GND | These next three are closest to the PCI Express pins
23  |  GND |
26  |  GND |

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
 
 
