---
layout: default
title: Layer State Management in Rhino
nav_order: 1
parent: Twinbuild For Rhino
---

# Creating task sequences

![Rhino Layer State Manager]({{ site.baseurl}}/img/Twinbuild_LayerStates.png "Rhino Layer State Manager")

The best way to create task sequences in Rhino 7 using the Layer State Manager. The Layer State Manager allows you to save the current state of the layer table metadata (visibility, materials, line types and so on) and switch between these states instantly. The list of layer states can then be published to Twinbuild to represent a sequence of tasks.

Place geometry needed for each task on a new Rhino layer. Toggle the visibility of the layers in the model that should be visible to complete the first task, then open the _LayerStateManager_ and save this state with a name that users can use to identify the task. To create an ordered list of tasks, specify a number at the start of the task name e.g. 00_Task1, 01_Task2 etc. Layer States will be sorted alphabetically when publishing to Twinbuild.

_Note: In some applications it may be possible to automate the creation of layers and assignment of geometry using parametric models like Grasshopper. For example, in masonry applications each course of bricks is placed on a layer identifying that course._

A user wearing the HoloLens can then use Twinbuild to switch between published Layouts using the Next and Previous buttons in the Twinbuild UI, or by switching directly to a selected layout by tapping it's name from the list.

# Creating task sequences with Rhino 6

Rhino 6 does not include the Layer State Manager. To create task sequences with Rhino 6, put all geometry necessary for a task on a single layer and give the layer a name that will help a user identify the task. Avoid publishing any layers that do not contain task information.

A user wearing the HolOlens can then switch between visibility of layers using the same UI as above.
