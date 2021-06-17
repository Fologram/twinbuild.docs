---
layout: default
title: Publishing and Previewing Models
nav_order: 2
parent: Twinbuild Web Viewer
---

# Publishing and Previewing locally stored models in the web browser

![Twinbuild Model Preview]({{ site.baseurl}}/img/TwinbuildPreview.png "Twinbuild Model Preview")

Models can be previewed in the Twinbuild 3D view by dragging and dropping an .fbx, .ifc, .gltf or .glb file into https://app.twinbuild.com/ or publishing from Revit or Rhino.

The camera in the 3D preview is controlled by the mouse or tap gestures on touchscreens. Left click (or tap) and drag to orbit the model. Right click (or two finger tap) and drag to pan the model. Use the scroll wheel (or pinch gesture) to zoom the model.

If you model appears very small or the Twinbuild grid is very fine then you should consider moving your model geometry to the origin and removing any geometry that will not be used in the holographic experience. If your model takes a long time to load or camera motion is very slow you should consider simplifying or removing geometry in your model as the model will likely perform poorly on the HoloLens 2.

The Twinbuild 3D preview supports the GLTF physically based material specification. If your modelling application does not support PBR materials the Twinbuild integrations for Rhino and Revit will attempt to convert the native material specification to PBR. If publishing .fbx files, we recommend working with very simple coloured materials and avoid texture files as these may not be possible to load in the Twinbuild web viewer.

After confirming model scale, geometry and materials are working as expected you can sign in and upload your model.
