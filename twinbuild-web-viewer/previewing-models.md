---
layout: default
title: Previewing Models
nav_order: 2
parent: Twinbuild Web Viewer
---

# Previewing models in the web browser

![Twinbuild Model Preview]({{ site.baseurl}}/img/15_Twinbuild_App_ModelPreview.png "Twinbuild Model Preview")

The camera in the 3D preview is controlled by the mouse or tap gestures on touchscreens. Left click (or tap) and drag to orbit the model. Right click (or two finger tap) and drag to pan the model. Use the scroll wheel (or pinch gesture) to zoom the model.

![Twinbuild Model Layouts]({{ site.baseurl}}/img/Twinbuild_LayoutsMenu.png "Twinbuild Model Layouts")

If you have published a model with multiple Views (Revit) or Layer States (Rhino) then you can switch between these using the Layouts dropdown menu located above the Markers button in the bottom left of the Twinbuild Web Viewer. You can switch between these same Layouts while viewing the model on the HoloLens.

If you model appears very small or the Twinbuild grid is very fine then you should consider moving your model geometry to the origin and removing any geometry that will not be used in the holographic experience. If your model takes a long time to load or camera motion is very slow you should consider simplifying or removing geometry in your model as the model will likely perform poorly on the HoloLens 2.

The Twinbuild 3D preview supports the GLTF physically based material specification. If your modelling application does not support PBR materials the Twinbuild integrations for Rhino and Revit will attempt to convert the native material specification to PBR. If publishing .fbx files, we recommend working with very simple coloured materials and avoid texture files as these may not be possible to load in the Twinbuild web viewer.

After confirming model scale, geometry and materials are working as expected you can sign in and upload your model.
