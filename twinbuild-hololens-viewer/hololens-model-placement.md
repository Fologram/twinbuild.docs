---
layout: default
title: Placing Models with Markers
nav_order: 5
parent: Twinbuild HoloLens Viewer
---

# Placing Models with Markers

To view a loaded model in your physical space, walk over to any one of your Markers and scan it with the HoloLens 2. When the Marker is detected, the scaled precision model will snap in place. Walk to a second Marker and repeat the scanning process. When the second Marker is detected, the model will scale to 1:1. Repeat this process with remaining Markers. For optimal results, scan each Marker 2 or 3 times as this will also enable the HoloLens to build up tracking data within your workspace.

### Clearing cached Marker positions

Marker positions are cached on the HoloLens 2 to allow loading different models into the same location in a physical space. If a physical Marker is moved to a new position after being scanned by Twinbuild you will need to clear all cached positions to prevent corruption of spatial data used to improve hologram drift. To clear all cached Marker positions, hold the power button on the Hololens 2 until you hear a beep and the device switches off. Turn the headset on and launch Twinbuild to rescan the new code positions.

### Notes on Marker Detection

Marker detection on the Hololens 2 runs as a background process and is 'always on'. Marker detection will be impacted by the distance of the HoloLens from the Marker, and you may experience some slight jumps in hologram position if the HoloLens can detect a Marker several meters away as the position of the Marker will be relatively innacurate compared to if it is scanned when the device is nearby. For best results, regularly scan the nearest Marker to your workspace to ensure adequate drift corection, and keep your workspace as close to Markers as possible. The materiality of the Marker will also affect scanning precision and matte surfaces like paper scan more successfully than screens or reflective laminate. Unevenly lit Markers will also affect scanning precision and very bright or very dark spaces can be difficult to detect Markers in. Finally take care that no objects are occluding any part of the Marker.
