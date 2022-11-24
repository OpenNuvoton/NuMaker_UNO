- [NuMaker UNO board package for Arduino IDE](#numaker-uno-board-package-for-arduino-ide)
- [Supported Boards & Features](#supported-boards--features)
- [Board Package Installation Steps](#board-package-installation-steps)
- [VCOM Driver Installation Steps (Optional for M032BT)](#vcom-driver-installation-steps-optional-for-m032bt)
- [NuLink Driver Installation Requirements (For M460)](#nulink-driver-installation-requirements-for-m460)
- [Compatible Versions of Arduino IDE](#compatible-versions-of-arduino-ide)
- [Disclaimer](#disclaimer)
- [Important Notice](#important-notice)

# NuMaker UNO board package for Arduino IDE
This repository contains the package descriptor for NuMaker UNO boards

# Supported Boards & Features

| NuMaker Boards | Rich peripherals | Bluetooth Low Energy<br>ArduinoBLE(***1.2.1***) | Debugger(Arduino IDE 2.0) |
| -------------- | ---------------- | ----------------------------------------------- |---------------------------|
| **NUC131**     | ✔️                | ❌                                            | ✔️                        |
| **M032BT**     | ✔️                | ✔️                                            | ✔️                        |
| **M252**       | ✔️                | ❌                                            | ✔️                        |
| **M467**       | ✔️                | ❌                                            | ✔️                        |
| **M487**       | ✔️                | ❌                                            | ✔️                        |


# Board Package Installation Steps
1. Download and Install Arduino IDE from https://www.arduino.cc/en/Main/Software
2. Double-click arduino.exe, and then go to **File->Preferences**
3. Paste following URL to 'Additional Boards Manager URLs' input field: 
`https://raw.githubusercontent.com/OpenNuvoton/NuMaker_UNO/master/package_nuvoton_index.json`
4. Under **Tools->Board->Boards Manger**, search `NuMaker UNO`, click **Install**
5. You can now select NuMaker UNO and install it in Arduino IDE.

# VCOM Driver Installation Steps (Optional for M032BT)
The Virtual COM (VCOM) interface requires a VCOM driver to be installed on PC first. 
The driver "Nu-Link_USB_Driver 1.x.exe" can be found at: http://www.nuvoton.com/opencms/resource-download.jsp?tp_GUID=SW0520150729202535
1. Execute "Nu-Link_USB_Driver 1.x.exe" after the USB cable is un-plugged.
2. Follow the steps of installation wizard to select setup language and installation location.
3. Plug in USB cable after driver installation complete.
4. Connect the NuMaker UNO with PC using a USB cable. If the driver is successfully installed, the Windows shall find a new device and then automatically find the correct driver. A virtual COM port named "Nuvoton Virtual Com Port" can be found in "Device Manager".

# NuLink Driver Installation Requirements (For M460)
To support M460 firmware upload, it requires: 
1. NuLink USB Driver Version: 1.9 and above
2. NuLink Command Tool: 3.09 and above

# Compatible Versions of Arduino IDE
* 2.0.0

# Disclaimer
The Software is furnished "AS IS", without warranty as to performance or results, and
the entire risk as to performance or results is assumed by YOU. Nuvoton disclaims all
warranties, express, implied or otherwise, with regard to the Software, its use, or
operation, including without limitation any and all warranties of merchantability, fitness
for a particular purpose, and non-infringement of intellectual property rights.

# Important Notice
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


**Copyright (C) 2022 Nuvoton Technology Corp. All rights reserved**
