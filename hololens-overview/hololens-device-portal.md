---
layout: default
title: HoloLens Device Portal
nav_order: 5
parent: HoloLens Overview
---

# Setting up HoloLens device portal

Device portal allows you to manage your device over WiFi or USB.
{: .fs-6 .fw-300 }

Common uses of the device portal are to:

- Live-stream video to a computer or projector
- Access and download saved images and video from the device
- Manually set calibration data (IPD) without re-running the calibration app

### Enabling Developer Mode and Device Portal

On your HoloLens, select 'Settings'
Select Update and Security
Select the For Developers option in the side bar
Turn on Developer Mode
Scroll down and enable Device Portal
Click the Remove icon in the corner of the Settings tile to save and exit

### Accessing the HoloLens Device Portal

Ensure that your HoloLens and computer are connected to the same WiFi network
On your HoloLens, check your IPV4 Address. You can find this under:
`Settings > Network & Internet > Wi-Fi > Advanced Options`
In an internet browser, type the IPV4 address and press enter
Depending on your browser, you will receive a different prompt to proceed with the connection. In Edge, click on Details, then Go to Webpage. In Chrome, click on Advanced, then Proceed. See notes below on accepting security certificates.

### Creating Credentials

When accessing device portal for the first time, you will be asked to create credentials. It is important that you remember these credentials as you may be required to reset the device if they are lost. Also consider creating credentials that can be shared with other users of the device, so that they too can share their experiences.

On your computer, after completing the "Accessing the Device Portal", request a pin from your device. It will be shown on the HoloLens
Enter the pin, and set your username and password
Click Pair
Log in with your credentials on your computer.

For further reference see [Using the Windows Device Portal](https://docs.microsoft.com/en-us/windows/mixed-reality/develop/platform-capabilities-and-apis/using-the-windows-device-portal)
