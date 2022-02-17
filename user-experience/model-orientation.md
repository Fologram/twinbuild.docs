---
layout: default
title: Model Orientation
nav_order: 5
parent: Optimizing User Experience
---

# Choosing an appropriate model orientation for your application

If Twinbuild is used for green field construction, setout or fabrication from scratch then use Orient to Site to ensure that holograms remain perfectly level during setout. If Twinbuild is used for fabrication and setout on or with existing objects where precise orientation is not known ahead of time or is expected to change, use Orient to Object to ensure hologram orientation can be updated dynamically to match the precise orientation of physical objects.

World space orientation is useful in scenarios where you want to ensure that your model is guaranteed not to rotate around X or Y axes, for instance if placing a model on a somewhat uneven flat surface (construction sites etc - see below).

![World Orientation Example]({{ site.baseurl}}/img/OrientToWorldExample.png "World Orientation Example")

Object orientation uses detected Marker positions to correct the XYZ position _and_ rotation of your model. Object space orientation is useful for scenarios where you are wanting to locate models on physical objects that may be in an unknown or changing position or orientation (see example below).

![Object Orientation Example]({{ site.baseurl}}/img/OrientToObjectExample.png "Object Orientation Example")
