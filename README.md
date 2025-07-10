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

## What do I need to put it together?

### Bill of Materials (BOM)
- Qty 1: 9x1 Pin male (straight through) IDC header or hooded/keyed IDC header (2.54mm pitch) - such as an [XH 2.54mm](https://www.aliexpress.us/item/3256805407027838.html?spm=a2g0o.order_list.order_list_main.62.35a618021c0Zqn&gatewayAdapt=glo2usa) or [shrouded male DuPont](https://www.aliexpress.us/item/3256805243290163.html?spm=a2g0o.order_list.order_list_main.123.35a618021c0Zqn&gatewayAdapt=glo2usa): Aliexpress.
- Qty 1: 9 x 1 pin male (right angle) IDE header or hooded/keyed IDC header (2.54mm pitch) of whatever you got for the previous step (either XH or Dupont) - the previous links have those versions as well.  This is for the SmartPort SD side (you use this instead of the DE25 connector.)
- Qty 1: A female to female 9 conductor to 9 conductor opposite direction cable [XH to XH](https://www.aliexpress.us/item/2251832672911708.html?spm=a2g0o.order_list.order_list_main.183.35a618021c0Zqn&gatewayAdapt=glo2usa) or [Dupont to Dupont](https://www.aliexpress.us/item/2255800932917997.html?spm=a2g0o.order_list.order_list_main.108.35a618021c0Zqn&gatewayAdapt=glo2usa) - depending on the type of connectors you used.  
- Qty 9: DB type 1.0mm pins, you might wants spares too - https://www.aliexpress.us/item/3256802431271655.html
- Qty 2: M2.5 Nuts - https://www.aliexpress.us/item/2255800799473326.html
- Qty 2: M2.5x12mm Countersunk Screws - https://www.aliexpress.us/item/2251832747871730.html
- (three pieces): 3D print the "DB-19M-Adapter-Male-Rev1" STL files from the FujiNet Apple II project: https://github.com/FujiNetWIFI/fujinet-hardware/tree/master/AppleII/DB-19M-Adapter-Male-Rev1
- note: For the above, I highly suggest you male a slightly larger hole than the pin header to get the pins to go through.  I use a Wiha screwdriver only slightly bigger than the hole in the DE19 print to widen the nine pins slightly.  It makes the pins push in slightly easier.

## Assembly

Before you begin soldering, carefully read the entire set of instructions below to understand how the components fit together. Proper assembly sequence is essential for a successful build.

1. **Solder the 9-pin IDC header first (computer side).**  
   - This is the connector that faces the Apple II computer.  
   - Solder this connector first for easiest access, otherwise you're going to be trying to solder between 3D printed plastic.  
   - The 9 pin header should face away from the computer; this is where you'll later plug in the 9-pin cable from the SmartPort SD Nano Shield.  
   - The silkscreen labels on the PCB help confirm correct orientation.

2. **Install the DE-19 connector pins.**  
   - Insert the 9 individual pins into the DE-19 footprint **from the back** of the DE19 3D print, as shown in the image above.  
   - These should match the same 9-pin layout as the SmartPort SD Nano Shield cable.  Make sure you don't get it backward.
   - Double-check the pin alignment using the clearly labeled silkscreen on the PCB, if you're using the correct pins you'll know if you're reversed or not.

3. **Prepare to solder the DE-19 pins.**  
   - Place the PCB over the pins but **do not press it down fully yet** as to leave a gap between the PCB and the 3D part of the DE19 connectdor.
   - **Important:** Slide the "shoulder piece" (the alignment spacer) in behind the PCB before seating the PCB all the way down.  
   - Once everything is aligned properly, solder all nine DE-19 pins.

4. **Complete the assembly with the case.**  
   - Install the top part of the 3D printed case over the assembly.
   - Secure it using the included nuts and bolts.  
   - If the pins and the shoulder piece were positioned correctly, the case should fit cleanly with no force.

## Contributing

Contributions, bug reports, and improvements are welcome! Please use GitHub Issues to suggest changes or open a pull request with your proposed enhancements.

## License and Credits

This hardware design is licensed under the **CERN Open Hardware Licence Version 2 – Strongly Reciprocal (CERN OHL v2-S)**.  
You may copy, modify, and distribute this design under the terms of the license. Source files must be made available when distributing physical products or derived works.

This adapter is based in part on the excellent work by the FujiNet team. It borrows from the [Apple II FujiNet adapter](https://github.com/FujiNetWIFI/fujinet-hardware/tree/master/AppleII), also licensed under CERN OHL v2-S.
