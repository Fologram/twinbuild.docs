---
layout: default
title: System Load and Device Condition
nav_order: 4
parent: HoloLens Precision
---

# How system load and device condition affect precision

### Issues with working with detailed 3D models (>500K polygons)

_Cause:_ Detailed models take longer to render on the HoloLens leading to lower frame rates and fewer computational resources available for tracking algorithms.

_Impact:_ Non-optimal tracking together with user discomfort due to low frame rates.

_Identification:_ If you are experiencing poor tracking performance together with a low device frame rate then this is mostly likely due to model detail.

_Solution:_ Twinbuild will display a model health warning notifying users if the model contains over the recommended number of objects, polygons, textures and materials. Check to make sure that your model does not contain unnecessary detailed geometry, and that simple geometry is not being automatically meshed at greater than necessary resolution. As a general rule of thumb, limit the detail of all geometry displayed on the HoloLens during setout applications.

### Issues with infrequently clearing spatial mapping data

_Cause:_ Infrequent use of the HoloLens 2 in the same space may lead to old spatial data being used to track feature points that no longer exist in that space (typically due to the movement of objects in the space over time)

_Impact:_ Non-optimal tracking.

_Identification:_ Poor tracking in a space after infrequent use of the HoloLens 2

_Solution:_ Open the settings menu on the HoloLens 2 and navigate to System > Holograms > Remove All Holograms to clear the spatial data on the HoloLens 2. Spend a few minutes walking around the space to rebuild tracking data before working in the space.

### Issues with working with dirty or scratched headsets

_Cause:_ Dirt, dust and scratches on the acrylic material covering the onboard RGB and depth cameras can occlude or blur visible feature points and reduce tracking performance.

_Impact:_ Non-optimal tracking.

_Identification:_ Check the condition of your HoloLens 2 for dirt and scratches before use.

_Solution:_ Take care when using the HoloLens 2 in working environments to eliminate exposure to dirt, sharp or abrasive objects. Wipe the surface of the HoloLens 2 with a microfibre cloth to clean the acrylic before use.

### Issues with low battery life

_Cause:_ The HoloLens 2 will throttle CPU and GPU performance to extend battery life when limited power is available.

_Impact:_ Non-optimal tracking.

_Identification:_ Check the battery level before using the Hololens 2 in tasks that require optimal tracking.

_Solution:_ Use a high power portable battery pack to keep the HoloLens 2 fully charged during operation. Keep the HoloLens 2 plugged in using the USB C cables supplied with the headset when not in use to ensure the device is always fully charged.
