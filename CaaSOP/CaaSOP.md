---
layout: default
title: CaaS for OctoPrint
description: "Calibration as a Service Plugin for OctoPrint."
has_children: true
nav_order: 3
---

# Calibration as a Service for OctoPrint
Ulendo has developed a plugin for OctoPrint called Ulendo-CaaS. This plugin allows for the a seamless experience, simplifying the process of calibrating a printer, and finding the optimal vibration compensation parameters.
 

## How it works
The  Calibration as a Service plugin generates a frequency sweep for on the printer, and collects the data using an attached accelerometer. The data is then sent via internet to a centralized cloud service which analyzes the data and generates the optimal parameters when is then returned the printer.

## Supported Platforms

### Devices
The Ulendo-CaaS plugin has been tested on the the Raspberry Pi 3b, Raspberry Pi 4.  

### Accelerometers
ADXL345

#### Printers
Currently, Ulendo has pre-built firmware for the [Ender 3] V2 Neo, and the Taz Pro printers. To add support for your printer, ask your printer's manufacturer about adding support for Ulendo's FTM.


### Fixed Time Motion
Currently, this plugin only works with plugins with printers that have support for Ulendo's Fixed Time Module developed for the Marlin Firmware. To find out how to add support for this module, contact your OEM.

The data collection, and application of the shapers require support at the firmware level, and is not available for all machines. Contact your OEM to find out more about adding support for Ulendo's FTM.


## Printer operation
For the Calibration as a Service Plugin to work effectively, an accelerometer needs to be attached to the printer, and connected to a support version of the Raspberry Pi. 

The diagram below provides and overview of the connections required on the accelerometer and the host device. 

After the accelerometer is connected to the Pi and mounted to the printer. Users can use the CaaS plugin to initiate the calibration process. 


[Ulendo-CaaS]: https://just-the-docs.github.io/just-the-docs/
[Ulendo-CaaS Github]: https://github.com/S2AUlendo/UlendoCaaS
[Ender 3]: https://github.com/S2AUlendo/Ender3-FT