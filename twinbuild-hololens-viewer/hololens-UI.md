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

![Twinbuild UI]({{ site.baseurl}}/img/Twinbuild_HoloLensUI.png "Twinbuild UI")

The Twinbuild UI contains tools for easily accessing HoloLens settings, restarting the application, toggling between outline and solid rendering and viewing Layouts or Layers. To open the Twinbuild user interface on the HoloLens, look at your palm. You can grab and drag the menu to move it in your space and can close the menu at any time by tapping the Exit icon.

The UI panel will display a paginated list of buttons for controlling the visibility of elements in the model. Buttons will display the Layer table of a model by default, and switch to displaying Layouts if the model contains multiple Views (Revit) or Layer States (Rhino). Tapping on a button will toggle the visibility of the Layer / Layout. Use the pagination arrows on the left side of the menu to navigate through all Layouts / Layers in the model. The "Next" and "Previous" buttons can be used to step through the Layout / Layer sequence for the purposes of following assembly guides or other sequential task information.

## Recording screengrabs and video

You can take a screengrab of the composite view of holograms and your physical space using the Windows Home menu. Tap the Windows icon on your wrist to open the Windows Home menu in Twinbuild, then tap the camera icon to launch the screengrab tool. Perform the tap gesture to save a screengrab. You can start and stop recording a video with the Video icon from the Windows home menu.

To save screengrabs and videos to your PC, connect your HoloLens with USB and navigate to the Camera Roll folder in Windows Explorer. For more information, see [Microsoft's docs](https://docs.microsoft.com/en-us/hololens/holographic-data).

## Exiting Twinbuild

To exit Twinbuild, say the voice command _Admin Force Quit_, Alternatively you can tap the Home button from the Windows Home menu to minimize Twinbuild then close any visible Twinbuild tiles in your space.
