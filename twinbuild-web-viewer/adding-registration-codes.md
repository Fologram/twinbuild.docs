---
layout: default
title: Locating Models with Markers
nav_order: 4
parent: Twinbuild Web Viewer
---

# Locating Models with Markers

Markers are QR codes that fix holograms to precisely known coordinates in 3D space.
{: .fs-6 .fw-300 }

![Adding Markers]({{ site.baseurl}}/img/AddMarker.png "Adding Markers")

### Adding Markers

The coordinates of Markers can be defined using the TwinbuildQR command in Rhino or entered manually by clicking on the Marker button in the Twinbuild web application after uploading a model. These Markers will be used to place your holographic model in physical space, and correct for drift in the hologram as users move between Markers.

## World and Object orientation

![Marker Orientation]({{ site.baseurl}}/img/MarkerOrientation.png "Marker Orientation")

Markers can be used to orient your model in world space or object space. World space orientation uses detected Marker positions to correct the XYZ position and Z rotation of your models, while Object space orientation will updated the XYZ position and XYZ rotation of the model to match the orientation of detected Markers.

![Orientation Mode Diagram]({{ site.baseurl}}/img/OrientationModeDiagram.png "Orientation Mode Diagram")

## Creating Markers from Coordinates

Enter the X, Y and Z coordinates that will be associated with the Marker and click Accept to add the Marker to the model. If you are planning to re-use existing physical Markers you can also edit the randomly generated ID.

## Creating Markers from model vertices

If you locating Markers on a physical object, use the Snap button in the Add Marker panel to snap the coordinates of the marker to a vertex in your model. Carefully choose a vertex where you will be able to locate the physical marker, then click the vertext to set the marker coordinates.

## Deleting Markers

If you need to delete or change the coordinates or ID of any existing Markers, click on the blue Marker label in the 3D viewport to open the Marker dialog. Make your changes and click accept to confirm them.

### Importing Markers from existing models

![Importing Markers]({{ site.baseurl}}/img/ImportRegistration.png "Importing Markers")

You can import Markers from any model that you have published to your Twinbuild account. Click on in the import icon to copy Marker positions from an existing model. This is useful when working with multiple digital models within the same physical space (e.g. a production line or workshop).
