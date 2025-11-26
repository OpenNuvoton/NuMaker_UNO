- [NuMaker UNO board package for Arduino IDE](#numaker-uno-board-package-for-arduino-ide)
- [NuMaker M4 board package for Arduino IDE](#numaker-m4-board-package-for-arduino-ide)
- [Board Package Installation Steps](#board-package-installation-steps)
- [VCOM Driver Installation Steps (Optional for M032BT)](#vcom-driver-installation-steps-optional-for-m032bt)
- [Compatible Versions of Arduino IDE](#compatible-versions-of-arduino-ide)
- [Disclaimer](#disclaimer)
- [Important Notice](#important-notice)

# NuMaker UNO board package for Arduino IDE
This package contains the NuMaker UNO board descriptors.

## Supported Boards & Features

| NuMaker Boards | Rich GPIO |Embedded CAN<br>nvtCAN(*Note) |Bluetooth Low Energy<br>ArduinoBLE(***1.2.1***) |
| -------------- | ---------------- | ----------------------------------------------- |----------------------------------------------- |
| **[NuMaker-NUC131U](https://direct.nuvoton.com/en/numaker-nuc131u)**     | ✔️              | ✔️                                               | ❌                                          |
| **[NuMaker-M032BT](https://direct.nuvoton.com/en)**     | ✔️              | ❌                                               | ✔️                                           |
| **[NuMaker-M032KG](https://direct.nuvoton.com/en/numaker-m032kg)**     | ✔️              | ❌                                               | ️❌                                         |
| **[NuMaker-M252SD](https://direct.nuvoton.com/en/numaker-m252sd)**       | ✔️              | ❌                                               | ❌                                           |
| **[NuMaker-PFM-M487](https://direct.nuvoton.com/en/numaker-pfm-m487)**       | ✔️              | ❌                                               | ❌                                           |

Note: Compatible to [Seeed_Arduino_CAN](https://github.com/Seeed-Studio/Seeed_Arduino_CAN)

# NuMaker M4 board package for Arduino IDE
This package contains the NuMaker M4 board descriptors.

## Supported Boards & Features

| NuMaker Boards | Rich GPIO | Embedded SD |Embedded CAN/FD<br>nvtCAN(*Note1)  | RS485 | Ethernet | Firmware Upload<br>by ISP(*Note2) | Keyboard/Mouse |
| ------------------ | ---------------- | ------|----------------------------------------------- |------|----|----|----|
| **[NuMaker-IOT-M467](https://direct.nuvoton.com/en/numaker-iot-m467)**       | ✔️  | ✔️| ✔️| ✔️| ✔️ | ✔️ |  ❌                                            ||
| **[NuMaker-UNO-M4](https://www.nuvoton.com/products/iot-solution/arduino-compatible-platform/numaker-uno-m4/)**       |✔️ | ✔️| ❌  | ✔️| ✔️| ✔️| ❌  ||
| **[NuMaker-UNO-M4KB](https://www.nuvoton.com/products/iot-solution/arduino-compatible-platform/numaker-uno-m4/)**       |✔️ | ✔️| ❌  | ✔️| ✔️| ✔️| ✔️  ||


Note1: Compatible to [Seeed_Arduino_CAN](https://github.com/Seeed-Studio/Seeed_Arduino_CAN)

Note2: ISP programming flow [demo video](https://youtube.com/shorts/vcT7D0wLV94). Operation mode(APP/LDR) is indicated by LED lightings.


# Board Package Installation Steps
1. Download and Install Arduino IDE from https://www.arduino.cc/en/Main/Software.
2. Check your network connection works fine. Sometimes intra-net would block Arduino IDE start-up downloads. <br>
   After checking, double-click arduino.exe, and then go to **File->Preferences**
4. Paste following URL to 'Additional Boards Manager URLs' input field: 
`https://raw.githubusercontent.com/OpenNuvoton/NuMaker_UNO/master/package_nuvoton_index.json`
5. For NuMaker UNO package, under **Tools->Board->Boards Manger**, search `NuMaker UNO`, click **Install**;<br>
   For NuMaker M4 package, under **Tools->Board->Boards Manger**, search `NuMaker M4`, click **Install**
6. You can now select NuMaker UNO/M4 and install it in Arduino IDE.

# VCOM Driver Installation Steps (Optional for M032BT)
The Virtual COM (VCOM) interface requires a VCOM driver to be installed on PC first. 
The driver "Nu-Link_USB_Driver 1.x.exe" can be found at: http://www.nuvoton.com/opencms/resource-download.jsp?tp_GUID=SW0520150729202535

1. Execute "Nu-Link_USB_Driver 1.x.exe" after the USB cable is un-plugged.
2. Follow the steps of installation wizard to select setup language and installation location.
3. Plug in USB cable after driver installation complete.
4. Connect the NuMaker UNO with PC using a USB cable. If the driver is successfully installed, the Windows shall find a new device and then automatically find the correct driver. A virtual COM port named "Nuvoton Virtual Com Port" can be found in "Device Manager".

# Compatible Versions of Arduino IDE
* 2.4.3 up

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


**Copyright (C) 2025 Nuvoton Technology Corp. All rights reserved**


