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

Markers can be used to orient your model in world space or object space. World space orientation uses detected Marker positions to correct the XYZ position and Z rotation of your models. World space orientation is useful in scenarios where you want to ensure that your model is guaranteed not to rotate around X or Y axes, for instance if placing a model on a somewhat uneven flat surface (construction sites etc - see below).

![World Orientation Example]({{ site.baseurl}}/img/OrientToWorldExample.png "World Orientation Example")

Object orientation uses detected Marker positions to correct the XYZ position _and_ rotation of your model. Object space orientation is useful for scenarios where you are wanting to locate models on physical objects that may be in an unknown or changing position or orientation (see example below).

![Object Orientation Example]({{ site.baseurl}}/img/OrientToObjectExample.png "Object Orientation Example")

## Creating Markers from Coordinates

Enter the X, Y and Z coordinates that will be associated with the Marker and click Accept to add the Marker to the model. If you are planning to re-use existing physical Markers you can also edit the randomly generated ID.

## Creating Markers from model vertices

If you locating Markers on a physical object, use the Snap button in the Add Marker panel to snap the coordinates of the marker to a vertex in your model. Carefully choose a vertex where you will be able to locate the physical marker, then click the vertext to set the marker coordinates.

## Deleting Markers

If you need to delete or change the coordinates or ID of any existing Markers, click on the blue Marker label in the 3D viewport to open the Marker dialog. Make your changes and click accept to confirm them.

### Importing Markers from existing models

![Importing Markers]({{ site.baseurl}}/img/ImportRegistration.png "Importing Markers")

You can import Markers from any model that you have published to your Twinbuild account. Click on in the import icon to copy Marker positions from an existing model. This is useful when working with multiple digital models within the same physical space (e.g. a production line or workshop).
