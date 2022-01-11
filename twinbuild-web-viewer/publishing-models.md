---
layout: default
title: Publishing Models
nav_order: 1
parent: Twinbuild Web Viewer
---

# Drag and Drop model publishing

You can publish models to Twinbuild by dragging and dropping a supported file to app.twinbuild.com or directly from our Revit and Rhino plugins. To learn how to publish from Revit or Rhino, follow one of these guides:

[Revit Guide]({{ site.baseurl}}/twinbuild-for-revit){: .btn } [Rhino Guide]({{ site.baseurl}}/twinbuild-for-rhino){: .btn }

![Twinbuild App Dashboard]({{ site.baseurl}}/img/14_Twinbuild_App_NoModels.png "Twinbuild App Dashboard")

To publish a model from the dashboard, sign in to https://app.twinbuild.com/ and select or drag and drop an .fbx, .ifc, .gltf or .glb file into the drop zone. You can also drag and drop a supported file directly into the 3D web viewer to load the new model. Note that files in zipped or compressed folders should be extracted to an uncompressed folder before using the drag and drop interface.

## Considerations for drag and drop publishing

Twinbuild's native Revit and Rhino plugins will automatically optimize and compress models for better performance in mixed reality. Models exported from CAD software may not have been intended to be viewed on the HoloLens and we recommend the following export workflow when working with .FBX or .IFC files:

- Locate models at 0,0,0
- Ensure models are exported in meters
- Use low-polygon meshing settings for NURBS geometry
- Work with curves rather than surface geometry where possible
- Hide or reduce the detail of high-polygon models
- Use simple colours for materials and avoid exporting texture files
