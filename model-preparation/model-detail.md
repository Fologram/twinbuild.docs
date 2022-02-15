---
layout: default
title: Model Detail
nav_order: 1
parent: Model Preparation
---

# Simplifying models for augmented reality

Viewing very detailed models (>1M polygons) on the hololens can limit CPU / GPU resources available for tracking and reduce hologram precision. In almost all cases highly detailed models are not necessary for construction and manufacturing tasks, and application performance can be significantly improved by simply eliminating details that are extraneous to the task at hand. Avoid showing details that will not be visible, remove textures from materials and work with simple model formats (boxes, curves and linework) where possible.

## Example: Pipework

Default mesh settings for parametric and NURBS pipework geometry may produce high resolution meshes that are unnecessary for mixed reality and lead to compromised performance. When exporting curved geometry such as pipework work with centerlines alone if possible, and when 3D models are required, take care to minimize meshing parameters to produce as little geometry as possible. For instance, a NURBS model of pipework may export to a mesh with 300K vertices by default, while 10K is sufficient to perform layout, QA and visualization.

![NURBS Pipework]({{ site.baseurl}}/img/PipeworkNURBS.png "NURBS Pipework")
_Nurbs Pipework native to modelling software_

![High Detail Pipework]({{ site.baseurl}}/img/PipeworkHighDetail.png "High Detail Pipework")
_Default Meshing settings - 300,000 vertices_

![Low Detail Pipework]({{ site.baseurl}}/img/PipeworkLowDetail.png "Low Detail Pipework")
_Ideal settings - 10,000 vertices_
