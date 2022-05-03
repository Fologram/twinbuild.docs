---
layout: default
title: Twinbuild For Rhino
nav_order: 8
has_children: true
---

# Installing Twinbuild for Rhino

Publish models directly from Rhino with our integration
{: .fs-6 .fw-300 }

[Get Twinbuild](https://twinbuild.com/download){: .btn }

Installing the Twinbuild for Rhino plugin from twinbuild.com/download adds the _Twinbuild_ and _TwinbuildQR_ commands to Rhino.

Use the _Twinbuild_ command to publish all supported and visible objects to the web browser. The _Twinbuild_ command compresses curves, mesh geometry and texture files and creates a GLB object that is then opened in the Twinbuild web application. For best results, ensure that Google Chrome is set as your PCs default web browser.

### Creating Task Sequences using Layer States

You can use the Rhino 7 Layer State manager to save the visibility of all layers in your model as a custom view in Twinbuild called a Layout. Task sequences can be created by publishing models with multiple layouts that can then be stepped through one by one on the Hololens.

![Layer State Manager]({{ site.baseurl}}/img/Twinbuild_LayerStates.png "Layer State Manager")

Use the _LayerStateManager_ command to open the layer state window, then click on the Save icon to save the current visibility state of layers in your model. Repeat this process after changing layer visibility to create your layer states, then use the _-Twinbuild_ command with the hypen included and select the _LayerStates_ option to publish the model containing all of your Layouts.

![Twinbuild Rhino Command]({{ site.baseurl}}/img/Twinbuild_RinoCommand.png "Twinbuild Rhino Command")

### Working at the Origin

To ensure a predictable experience for the end user, it is generally useful to keep models located at the origin. Use the ExportWithOrigin command in Rhino to export selected objects to a new Rhino file with a specified origin point. Open the exported model to continue working with Twinbuild.

### Publishing Curves

Twinbuild renders curves with a uniform thickness regardless of distance to the HoloLens to ensure maximum precision and minimal visual occlusion during setout tasks. If you wish to export curves with a world-space thickness that renders like other 3D objects in the model you can create mesh pipes from your curve geometry.

![Curve Piping]({{ site.baseurl}}/img/RhinoCurvePiping.png "Curve Piping")

Use the Rhino curve piping properties to create low polygon mesh pipes from curve geometry. Run the _ExtractPipedCurve_ command to extract the mesh object from the preview of the curve pipe. This object can then be published with with the rest of the model as normal.

### Publishing Text

Twinbuild does not export Rhino's Text or Dot objects. Text objects need to be converted to curve or Mesh geometry to export and view on the HoloLens. Text can be converted to curves using the _Explode_ command. If you wish to view the text as a solid surface, select the exploded curves and use the _PlanarSrf_ to create a planar surface model. Then use the _Mesh_ command to create a low poly mesh from this surface. Delete the surface geometry before publishing.

Dots can be converted to Text objects using the _ConvertDot_ command, after which you can follow the steps above.

### Unsupported Objects

Text, Lights, Dimensions and Hatches are not currently supported natively in Twinbuild. Text can be meshed before publishing using the steps outlined above. Remove any geometry in the model that will not be used in the holographic application (e.g. superficial elements like models of people, trees etc). Remove any materials with textures to simplify the experience for the end user.
