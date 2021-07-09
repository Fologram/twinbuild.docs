---
layout: default
title: Locating Models with Markers
nav_order: 3
parent: Twinbuild Web Viewer
---

# Locating Models with Markers

Markers are QR codes that fix holograms to precisely known coordinates in 3D space.
{: .fs-6 .fw-300 }

![Adding Markers]({{ site.baseurl}}/img/AddRegistration.png "Adding Markers")

### Adding and editing Markers

The coordinates of Markers can be defined using the TwinbuildQR command in Rhino or entered manually by clicking on the Add Marker in the Twinbuild web application after uploading a model. These Markers will be used to place your holographic model in physical space, and correct for drift in the hologram as users move between Markers. Enter the X, Y and Z coordinates that will be associated with the Marker and click Accept to add the Marker to the model. If you are planning to re-use existing physical Markers you can also edit the randomly generated ID.

If you need to delete or change the coordinates or ID of any existing Markers, click on the blue Marker label in the 3D viewport to open the Marker dialog. Make your changes and click accept to confirm them.

![Importing Markers]({{ site.baseurl}}/img/ImportRegistration.png "Importing Markers")

### Importing Markers from existing models

You can import Markers from any model that you have published to your Twinbuild account. Click on in the import icon to copy Marker positions from an existing model. This is useful when working with multiple digital models within the same physical space (e.g. a production line or workshop).
