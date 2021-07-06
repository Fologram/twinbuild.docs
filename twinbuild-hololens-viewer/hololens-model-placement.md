---
layout: default
title: Placing Models with Registration Codes
nav_order: 4
parent: Twinbuild HoloLens Viewer
---

# Placing Models with Registration Codes

To view a downloaded model in your physical space, walk over to any one of your registration markers and look at the code with the HoloLens 2. When the code is detected, the scaled precision model will snap in place. Walk to a second code and repeat the scanning process. When the second code is detected, the model will scale to 1:1. Repeat this process with remaining codes. For optimal results, scan each code 2 or 3 times as this will also enable the HoloLens to build up tracking data within your workspace.

### Clearing cached code positions

Registration code positions are cached on the HoloLens 2 to allow loading different models into the same location in a physical space. If a physical registration code is moved to a new position after being scanned by Twinbuild you will need to clear all cached positions to prevent corruption of spatial data used to improve hologram drift. To clear all cached code positions, hold the power button on the Hololens 2 until you hear a beep and the device switches off. Turn the headset on and launch Twinbuild to rescan the new code positions.

### Notes on Code Detection

Code detection on the Hololens 2 runs as a background process and is 'always on'. Code detection will be impacted by the distance of the HoloLens from the code, and you may experience some slight jumps in hologram position if the HoloLens can detect a registration code several meters away as the position of the code will be relatively innacurate compared to if it is scanned when the device is nearby. For best results, regularly scan the nearest registration code to your workspace to ensure adequate drift corection, and keep your workspace as close to registration codes as possible. The materiality of the code will also affect scanning precision and matte surfaces like paper scan more successfully than screens or reflective laminate. Unevenly lit codes will also affect scanning precision and very bright or very dark spaces can be difficult to detect codes in. Finally take care that no objects are occluding any part of the code.
