---
layout: default
title: Publishing and Previewing Models
nav_order: 1
parent: Twinbuild Web Viewer
---

# Publishing and Previewing models in the web browser

![Twinbuild App Dashboard]({{ site.baseurl}}/img/14_Twinbuild_App_NoModels.png "Twinbuild App Dashboard")

You can publish models to Twinbuild from the Twinbuild App Dashboard or directly from our Revit and Rhino plugins. To publish a model from the dashboard, sign in to https://app.twinbuild.com/ and select or drag and drop an .fbx, .ifc, .gltf or .glb file into the drop zone. To publish from Revit or Rhino, follow the guides below.

[Revit Guide]({{ site.baseurl}}/twinbuild-for-revit){: .btn } [Rhino Guide]({{ site.baseurl}}/twinbuild-for-rhino){: .btn }

![Twinbuild Model Preview]({{ site.baseurl}}/img/15_Twinbuild_App_ModelPreview.png "Twinbuild Model Preview")

The camera in the 3D preview is controlled by the mouse or tap gestures on touchscreens. Left click (or tap) and drag to orbit the model. Right click (or two finger tap) and drag to pan the model. Use the scroll wheel (or pinch gesture) to zoom the model.

If you model appears very small or the Twinbuild grid is very fine then you should consider moving your model geometry to the origin and removing any geometry that will not be used in the holographic experience. If your model takes a long time to load or camera motion is very slow you should consider simplifying or removing geometry in your model as the model will likely perform poorly on the HoloLens 2.

The Twinbuild 3D preview supports the GLTF physically based material specification. If your modelling application does not support PBR materials the Twinbuild integrations for Rhino and Revit will attempt to convert the native material specification to PBR. If publishing .fbx files, we recommend working with very simple coloured materials and avoid texture files as these may not be possible to load in the Twinbuild web viewer.

After confirming model scale, geometry and materials are working as expected you can sign in and upload your model.
