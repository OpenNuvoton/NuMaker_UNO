# NuMaker UNO board package for Arduino IDE
This repository contains the package descriptor for NuMaker UNO board

## Board Package Installation Steps
1. Download Arduino 1.8.5 IDE from https://www.arduino.cc/en/Main/Software
2. Extract arduino-1.8.5-windows.zip
3. Double-click arduino.exe, and then go to **File->Preferences**
4. Paste following URL to 'Additional Boards Manager URLs' input field: 
https://raw.githubusercontent.com/OpenNuvoton/NuMaker_UNO/master/package_nuvoton_index.json
5. Under **Tools->Board->Boards Manger**, search NuMaker UNO by Nuvoton, click **Install**
6. You can now select NuMaker UNO in Arduino IDE

## VCOM Driver Installation Steps
The Virtual COM (VCOM) interface requires a VCOM driver to be installed on PC first. 
The driver "Nu-Link_USB_Driver 1.2.exe" can be found at: http://www.nuvoton.com/hq/support/tool-and-software/development-tool-hardware/numaker-uno?__locale=zh_TW

1. Execute "Nu-Link_USB_Driver 1.2.exe" after the USB cable is un-plugged.
2. Follow the steps of installation wizard to select setup language and installation location.
3. Plug in USB cable after driver installation complete.
4. Connect the NuMaker UNO with PC using a USB cable. If the driver is successfully installed, the Windows shall find a new device and then automatically find the correct driver. A virtual COM port named "Nuvoton Virtual Com Port" can be found in "Device Manager".

## Disclaimer
The Software is furnished "AS IS", without warranty as to performance or results, and
the entire risk as to performance or results is assumed by YOU. Nuvoton disclaims all
warranties, express, implied or otherwise, with regard to the Software, its use, or
operation, including without limitation any and all warranties of merchantability, fitness
for a particular purpose, and non-infringement of intellectual property rights.

## Important Notice
Nuvoton Products are neither intended nor warranted for usage in systems or equipment,
any malfunction or failure of which may cause loss of human life, bodily injury or severe
property damage. Such applications are deemed, "Insecure Usage".

Insecure usage includes, but is not limited to: equipment for surgical implementation,
atomic energy control instruments, airplane or spaceship instruments, the control or
operation of dynamic, brake or safety systems designed for vehicular use, traffic signal
instruments, all types of safety devices, and other applications intended to support or
sustain life.

All Insecure Usage shall be made at customer's risk, and in the event that third parties
lay claims to Nuvoton as a result of customer's Insecure Usage, customer shall indemnify
the damages and liabilities thus incurred by Nuvoton.

Please note that all data and specifications are subject to change without notice. All the
trademarks of products and companies mentioned in this datasheet belong to their respective
owners.


**Copyright (C) 2016 Nuvoton Technology Corp. All rights reserved**
