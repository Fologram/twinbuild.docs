---
layout: default
title: Twinbuild For Rhino
nav_order: 7
has_children: true
---

# Installing Twinbuild for Rhino

Publish models directly from Rhino with our integration
{: .fs-6 .fw-300 }

[Get Twinbuild](https://twinbuild.com/download){: .btn }

Installing the Twinbuild for Rhino plugin from twinbuild.com/download adds the _Twinbuild_ and _TwinbuildQR_ commands to Rhino.

Use the _Twinbuild_ command to publish all supported and visible objects to the web browser. The _Twinbuild_ command compresses mesh geometry and texture files and creates a GLB object that is then opened in the Twinbuild web application. For best results, ensure that Google Chrome is set as your PCs default web browser.

### Working at the Origin

To ensure a predictable experience for the end user, it is generally useful to keep models located at the origin. Use the ExportWithOrigin command in Rhino to export selected objects to a new Rhino file with a specified origin point. Open the exported model to continue working with Twinbuild.

### Publishing Curves

![Curve Piping]({{ site.baseurl}}/img/RhinoCurvePiping.png "Curve Piping")

Use the Rhino curve piping properties to create low polygon mesh pipes from curve geometry for publishing with Twinbuild. The settings above (0.5mm radius, 4 segments and a flat cap type) are well suited to layout tasks. If creating pipes from curves, adjust the Accuracy slider to create a pipe with appropriate mesh resolution for the task. Run the _ExtractPipedCurve_ command to extract the mesh object from the preview of the curve pipe. This object can then be published with the _Twinbuild_ command.

### Unsupported Objects

Curves, Text, Lights, Dimensions and Hatches are not currently supported natively in Twinbuild. Curves and text can be meshed before publishing using the steps outlined above. Remove any geometry in the model that will not be used in the holographic application (e.g. superficial elements like models of people, trees etc). Remove any materials with textures to simplify the experience for the end user.
