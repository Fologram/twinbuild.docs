---
layout: default
title: Revit Visibility Settings
nav_order: 1
parent: Twinbuild For Revit
---

# Adjusting level of detail and visibility settings for Revit categories

![Revit Visibility Settings]({{ site.baseurl}}/img/RevitVisibility.png "Revit Visibility Settings")

Before publishing models with Twinbuild, ensure that you have disabled visibility for all Revit categories that will not be used in the holographic application. These typically include hiding furniture, small fixtures, landscaping elements etc.

![Revit LOD]({{ site.baseurl}}/img/RevitLOD.png "Revit LOD")

To ensure all parts of the model are visible in Twinbuild (including pipework and rebar previews), select the ‘Fine’ detail setting in the 3D View properties. You can optionally override the global detail level for specific categories in the Visibility / Graphics dialog box. Note that placeholder pipes will not appear even with the fine detail setting.
