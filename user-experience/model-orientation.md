---
layout: default
title: Model Orientation
nav_order: 5
parent: Optimizing User Experience
---

# Choosing an appropriate model orientation for your application

It may be challenging to accurately align physical and digital objects when the two objects are positioned in different orientations in 3D space. Twinbuild can correct for position in world XYZ axes and for rotation around the world Z axis by interpolating between the correction vectors of the nearest three registration markers. Orientation is not corrected for rotation around the X or Y axes, meaning that physical objects that are not positioned with a precisely known orientation may be difficult to overlay with holographic information for layout or QA applications. Design applications where physical and digital objects can be located with only XYZ position aligned with two points in the XY plane.
