---
layout: default
title: Publishing Settings
nav_order: 9
parent: Twinbuild Web Viewer
---

# Editing Twinbuild publishing settings file

The default publishing settings can be manually adjusted using the Twinbuild settings file located at `%appdata%/twinbuild/rhino/settings.json` for Rhino and `%appdata%/twinbuild/Revit/settings.json` for Revit if required.

### Global Settings

```json
"SettingsVersion": 1
The version of the Twinbuild settings file
"ServeAddress": "http://app.twinbuild.com/preview"
The default address for previewing models
"ServePort": 9099
The port used for locally previewing models
"Binary": true
Whether a .glb file should be generated (alternative is .gltf)
"ServeTimeout": 10000
Time the file should be available for the server to retrieve
"VertexColors": true
Whether mesh vertex colours should be included in exports
"Normals": true
Whether mesh normals should be included in exports
"TextureCoordinates": true
Whether mesh texture coordinates should be included in exports
"MinVerticesForDraco": 64
The minimum number of vertices a mesh should have to be considered compressable
"JpgQuality": 70
The quality of JPGs after resizing
"MaxImageDimension": 1024
The maximum dimension of resized images
"ForcePowerOfTwoImages": true
Whether images should be fit into nearest power of two dimensions, i.e. 899x100 would resize to 1024x768
"AllowTransparentImages": false
Whether transparent images are supported
"DracoCompression": 7
The amount of draco compression. 0 (off) - 10 (maximum)
"PrettyPrint": true
Whether .gltf (non-binary) files should be human readable (larger file sizes)
```

### Revit Settings

```json
"LevelOfDetail": 0.5
The level of detail for the meshing algorithm. 0 is minimum detail and 1 is maximum
"ReduceDrawCalls": true
If true, objects that share similar layer and material properties will be merged into a single mesh
```

### Rhino Settings

```json
"UseInstanceDefinitionLayer": false
Whether block instances should be placed on their definition layer or on their original layer
"UseFineMesh": false
Mesh resolution
"CurveLinearTolerance": 1.0
The maximum distance between midpoints of polyline segments and converted curves
"CurveAngleTolerance": 0.5
The maximum angle between polyline segments
```
