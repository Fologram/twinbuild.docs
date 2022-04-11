---
layout: default
title: Model Materiality
nav_order: 2
parent: Model Preparation
---

# Selecting appropriate materials for augmented reality

Holograms rendered as surfaces can obscure parts of the physical environment that need to be visible to carry out a task. Rendering surface models on the hololens with textures or reflective materials can also distract workers from following spatial guides and reduce the immersion of the experience by creating screendoor effects or the appearance of pixelated surfaces. To address this issue, Twinbuild provides an outline display mode that allows both physical and virtual objects to be visible at the same time. When viewing a model in outline mode, all geometry will be rendered as white linework and materials / textures will be ignored.

## Preparing models to be rendered as outlines in Twinbuild

Twinbuild creates outlines automatically from all unwelded edges in model mesh geometry. If outline mode is displaying _all_ edges in your model, use your CAD software to check whether mesh faces should be welded before publishing (In Rhino you can use the _Weld_ command and specify an angle tolerance for weld angles. Angles between faces larger than this tolerance will be displayed as outlines). Conversely, if outline mode is not displaying any edges then you may need to unweld your geometry before publishing (In Rhino use the _Unweld_ command).

## Hiding holograms with black materials

Outline mode will display all geometry in your model as simple white linework. In some cases it is necessary to more precisely control what is displayed in Twinbuild, while still enabling both physical and virtual objects to be viewed at the same time.

A common challenge to working entirely with vector geometry (curve and lines) in mixed reality is the lack of occlusion, and virtual objects will be visible even when they are "behind" physical objects in a workspace. This increases the difficulty of following virtual objects as spatial guides as users need to constantly check to ensure they are working with the correct guide and not some linework that is in the background some distance away. To address this issue, physical objects can be approximately modelled and assigned black materials in order to obscure virtual content in mixed reality. Black materials will be rendered to the depth buffer while appearing transparent on the HoloLens 2, creating an effective (albeit fake) experience of virtual content being hidden by physical objects.

### Example: Preparing a Model

![Solid Surfaces on the HoloLens]({{ site.baseurl}}/img/SolidSurfacesHoloLens.jpg "Solid Surfaces on the HoloLens")

The default export from most CAD software will be a solid white mesh model. Because the HoloLens optimizes rendering for performance, these tend to appear as flat objects and details are difficult to perceive.

![Wireframe model on the HoloLens]({{ site.baseurl}}/img/WireframeModelHoloLens.jpg "Wireframe model on the HoloLens")

Rendering the entire model as curves (e.g. as a wireframe) addresses this issue but means that the entire model is visible all at once which can be difficult to follow as a guide

![Adding occlusion geometry or hiding layers]({{ site.baseurl}}/img/OcclusionHoloLens.jpg "Adding occlusion geometry or hiding layers")

By assigning a black material to the surface of the model we can hide geometry behind our work surface. In some cases it is also possible to place geometry on seperate layers and toggle the display of these layers based on the requirements of the work task. Note that images captured on the HoloLens will still display materials as black (as above), though the appearance for the viewer is of a transparent surface (indicated below).

![Transparent black surfaces]({{ site.baseurl}}/img/OcclusionExample.png "Transparent black surfaces")

### Example: Applying Graphics

![Pattern Curves]({{ site.baseurl}}/img/PatternCurves.png "Pattern Curves")

Consider the example of applying painted or stencilled graphics to an existing 3D object such as a sculpture. Holograms of curves on the back side of the object are always visible and make it difficult to infer the location of the graphics on the front side of the object.

![Pattern on solid white material]({{ site.baseurl}}/img/PatternCurvesWhite.png "Pattern on solid white material")

Assigning a white material to the 3D model of the object that the graphics are being applied to solves this problem, but the white material occludes the physical object and makes it more challenging to correctly perform the task.

![Pattern on transparent black material]({{ site.baseurl}}/img/PatternCurvesBlack.png "Pattern on transparent black material")

Assigning a solid black material to the 3D model of the object occludes virtual objects but appears transparent on the HoloLens so that the physical object is still visible.
