---
layout: default
title: Model Location
nav_order: 5
parent: Model Preparation
---

# Creating predictable experiences by working with the model origin

Twinbuild will maintain the coordinate space of any published models. Some BIM models contain geometry that is located a long distance from the origin (e.g. in GPS coordinates) and this coordinate space may be difficult to align with the coordinates of registration markers (that may be located relative to the 0,0,0 point of a LIDAR scanner for instance). If using Twinbuild within a fabrication or manufacturing space, it is generally useful to have the 0,0,0 point be a known physical location within this space (defined by the position of registration QR codes) so that digital models can easily be aligned with the physical environment (e.g. on a benchtop or within a work area). On construction sites, it is generally useful to locate models relative to the coordinate space of column grids or other feature points that will be used to place registration codes.
