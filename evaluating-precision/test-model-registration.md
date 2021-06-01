---
layout: default
title: Registering the Test Model
nav_order: 2
parent: Evaluating Precision
---

# Adding registration markers to the test model

To locate the Precision Test model relative to your physical workspace you will need to attach the coordinates of your Registration markers. This process will need to be completed once for each workspace where you plan to use Twinbuild, as registration marker positions can be shared between published models.

Click on Register to add the coordinates of a registration marker to the model. Enter the ID and coordinates (in meters) then click Accept to register the point. If you make a mistake, you can click on the ID of the point within the 3D viewport to edit the ID or coordinates. Repeat this process for each Registration Marker in your workspace.

If your Registration Points are not located in the correct position relative to the test grid geometry, check to make sure you have moved the coordinates of each Registration Point in CAD so that the 0,0,0 point is on the floor roughly in the area where you plan to use the HoloLens.

If you are performing a simple test from a linear collection of markers, then the y and z coordinates of the markers can remain 0. Only the x coordinate will be required to capture the relative distances between the markers. Keep in mind that precision will only be optimal along the line of the markers and it is not recommended to attempt to perform the precision test at locations off this axis.
