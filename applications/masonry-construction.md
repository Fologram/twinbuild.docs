---
layout: default
title: Masonry Construction
nav_order: 5
parent: Applications
---

# Complex Brickwork and Masonry Construction

Twinbuild can dramatically simplify setout tasks for curving brickwork, non-standard bonds and non-repeating brick patterns.
{: .fs-6 .fw-300 }

![Masonry Design]({{ site.baseurl}}/img/applications/Masonry_DesignModel.png "Masonry Design")

Twinbuild enables highly expressive designs from brick to be built in construction time similar to conventional straight walls. Twinbuild can reduce reliance on physical templates or measured setout by replacing these tasks with holographic models describing the exact position of each brick in the design. Twinbuild enables structures to be built in parallel by teams working from the same holographic model, without introducing the risk of inconsistent bonds.

### Model Preparation

![Masonry Setup]({{ site.baseurl}}/img/applications/Masonry_Courses.png "Masonry Setup")

Linework describing the outline of the top face of each brick should first be generated from design models. This linework should be grouped into courses. Each course should then be placed on a Layer / Category with names defining the construction sequence (e.g. 01,02,03,04 etc). The model should also include low-polygon reference geometry (existing wall or floor structures) to use to perform visual checks of hologram alignment during construction and marker setout.

### Marker Setout

Markers should be located as close to the brickwork as possible. The location of markers should be carefully considered to ensure that sufficient markers remain visible during construction as any obscured markers will no longer be detected by Twinbuild and used for drift correction. For instance, if constructing a brick veneer (as above), markers may be located in a grid on the studwork behind the wall up to the height of the wall.

### Task Guidance

Follow best practice for [user behaviour]({{site.baseurl}}/hololens-precision/user-behaviour) before performing set out. Walk around the site for 5 minutes and ensure all markers have been scanned. Before starting setout, ensure the closest marker has been recently scanned.

Perform quick visual checks to ensure minimal drift by comparing the holographic model of as built structures or previously laid courses of bricks to the existing conditions on site. Use the Layer Isolate button in Twinbuild for HoloLens to select the current course of bricks. Stand directly above the brick course so that the course is visible in plan. Position each brick by locating the physical brick within the matching holographic outline. Remember that the true position of the hologram is easiest to perceive when viewed in the center of the field of view and front-on to the model. Avoid attempting to place bricks that cannot be viewed in plan and use scaffolding to accomodate for this if necessary.
