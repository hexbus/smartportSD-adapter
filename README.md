# SmartPortSD Adapter

An open hardware adapter designed by [hexbus](https://github.com/hexbus) to connect the [SmartPort SD Nano Shield](https://github.com/djtersteegc/smartportsd/tree/main/smartportsd-nano-shield) by [@djtersteegc](https://github.com/djtersteegc) to Apple II systems using the 19-pin (DB19/DE-19) SmartPort interface.

## Overview

The SmartPort SD Nano Shield is a compact and powerful SmartPort-based SD card solution for Apple II computers. While the original board uses a 25-pin Duodisk connector, it also includes a more accessible 9-pin header that can be repurposed for DB19-compatible systems.

This adapter bridges the 9-pin connector on the SmartPort SD Nano Shield to a DE-19 connector suitable for direct connection to an Apple IIGS or Apple IIc.

![Adapter Image](https://github.com/hexbus/smartportSD-adapter/blob/main/db19%20to%209%20pin%20Smartport%20SD%20Adapter.png)
![Adapter Image](https://github.com/hexbus/smartportSD-adapter/blob/main/IMG_2669.jpg)
![Adapter Image](https://github.com/hexbus/smartportSD-adapter/blob/main/IMG_2670.jpg)
![Adapter Image](https://github.com/hexbus/smartportSD-adapter/blob/main/IMG_2671.jpg)
![Adapter Image](https://github.com/hexbus/smartportSD-adapter/blob/main/IMG_2672.jpg)

## Why This Adapter?

While the SmartPort SD Nano Shield is designed with flexibility in mind, most Apple II users (especially Apple IIGS and IIc owners) need a DE-19 port for SmartPort functionality. This adapter enables direct plug-and-play connectivity using the 9-pin header, eliminating the need for custom cables or bulky DB25 adapters.

Tested and confirmed working on an Apple IIGS. It should also work with the Apple IIc, but please verify pinout compatibility before use.

## Contributing

Contributions, bug reports, and improvements are welcome! Please use GitHub Issues to suggest changes or open a pull request with your proposed enhancements.

## License and Credits

This hardware design is licensed under the **CERN Open Hardware Licence Version 2 – Strongly Reciprocal (CERN OHL v2-S)**.  
You may copy, modify, and distribute this design under the terms of the license. Source files must be made available when distributing physical products or derived works.

This adapter is based in part on the excellent work by the FujiNet team. It borrows from the [Apple II FujiNet adapter](https://github.com/FujiNetWIFI/fujinet-hardware/tree/master/AppleII), also licensed under CERN OHL v2-S.
