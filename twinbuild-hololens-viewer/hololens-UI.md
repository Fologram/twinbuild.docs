---
layout: default
title: Twinbuild Menu and UI
nav_order: 1
parent: Twinbuild HoloLens Viewer
---

# Twinbuild for HoloLens User Interface

The Twinbuild user interface is designed to be as simple and unintrusive as possible.
{: .fs-6 .fw-300 }

When a model is loaded in Twinbuild for the first time, Twinbuild will enter preview mode and display the model at scale for quick visual checks. The model preview will appear approximately one meter in front of the HoloLens and scaled to a 1x1m bounding volume. To interact with the model preview, you can use two-handed pinch and drag gestures on the HoloLens to move, scale and rotate the bounding volume of the preview. After locating the model with a Marker, the model will be scaled to 1:1 and interaction will be locked.

Note that Preview mode is not recommended for production or demonstration scenarios due to the likelihood of accidental model manipulation.

![Twinbuild UI]({{ site.baseurl}}/img/TwinbuildUI.png "Twinbuild UI")

The Twinbuild UI contains tools for easily accessing HoloLens settings, Twinbuild models and editing layer properties. To open the Twinbuild user interface on the HoloLens, look at your palm. You can grab and drag the menu to move it in your space and can close the menu at any time by tapping the Exit icon.

The layer panel displays all layers in the model. Layers visibility can be toggled on and off with the icon to the right of the layer name. Toggling visibility for a parent layer will hide all child layers. Individual layers can also be isolated (hiding all other layers) by tapping the isolate button to the far right of the layer name. Note that isolating a child layer will not hide geometry on the parent layer.

Layers can be isolated in sequence by tapping the Next Layer or Previous Layer buttons. This allowsa user to quickly step view individual layers one at a time for completing task sequences (e.g. displaying courses of bricks). All layers can be made visible by tapping the Show All button.

## Recording screengrabs and video

You can take a screengrab of the composite view of holograms and your physical space using the Windows Home menu. Tap the Windows icon on your wrist to open the Windows Home menu in Twinbuild, then tap the camera icon to launch the screengrab tool. Perform the tap gesture to save a screengrab. You can start and stop recording a video with the Video icon from the Windows home menu.

To save screengrabs and videos to your PC, connect your HoloLens with USB and navigate to the Camera Roll folder in Windows Explorer. For more information, see [Microsoft's docs](https://docs.microsoft.com/en-us/hololens/holographic-data).

## Exiting Twinbuild

To exit Twinbuild, say the voice command _Admin Force Quit_, Alternatively you can tap the Home button from the Windows Home menu to minimize Twinbuild then close any visible Twinbuild tiles in your space.
