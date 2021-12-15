---
layout: default
title: Model Placement
nav_order: 10
has_children: true
---

# Best practice for working with Markers

Users should determine a strategy for locating Markers by balancing the overheads of setup time with the required holographic precision.
{: .fs-6 .fw-300 }

Imprecision in marker locations will lead to corresponding error in drift correction of holographic models. For maximum precision it is important to ensure your workspace is set up within a perimiter defined by 3 or more registration codes as Twinbuild will interpolate between the tracked positions of the nearest three registration codes to corect for drift.

Maximum hologram precision will be exactly equal to the precision in the location of the registration code when standing directly above that code, high when within a volume defined by 3 or more codes, moderate when along a linear axis defined by only two codes, and low (e.g. normal drift) at all other locations. Drift will worsen as you move further and further from the code bounding volume. [See here for more information on factors affecting precision.]({{ site.baseurl}}/hololens-precision)

![Linear Marker Precision]({{ site.baseurl}}/img/LinearMarkerDiagram.png "Linear Marker Precision")

### Linear Markers

_Implementation:_ Using a tape measure / disto, align markers (white crosses in above diagram) with the workspace at a known measured distance apart.

_Precision:_ High (along marker line - indicated by green in the above diagram), very poor beyond the line.

_Applications:_ 1:1 visualization and for linear applications up to 4000mm long and up to 2000mm high (e.g. wall construction)

_Work Area:_ Maximum precision at each marker, with drift correction along the line between markers. Normal HoloLens drift at any distance from this line.

![Marker Grid Precision]({{ site.baseurl}}/img/GridMarkerDiagram.png "Marker Grid Precision")

### Marker Grids

_Implementation:_ Using a tape measure / disto and laser level, locate a square grid of markers (white crosses in above diagram) perpendicular to a wall in the work space at a known measured distance apart. Alternatively, place markers at known locations e.g. along intersecting lines of column grids or at corners of interior walls.

_Precision:_ Moderate to high (due to human error in setting out grid and imprecision in built features). Precision is best near markers and within the contained boundary.

_Applications:_ Setout applications contained within the marker perimeter and up to 2000mm high, where floor mounted markers will not be occluded during the course of the application.

_Work Area:_ Maximum precision at each marker, with drift correction within the area between any three markers. Normal drift outside of the marker perimeter.

![Distributed Marker Precision]({{ site.baseurl}}/img/DistributedMarkerDiagram.png "Distributed Marker Precision")

### Distributed Markers

_Implementation:_ Distribute markers within the workspace such that they are frequently visible while working with the HoloLens. Maintain approximately 4000mm spacing between markers (white dots in above diagram). After placement, digitize the positions of the markers using LIDAR scans or alternative methods.

_Precision:_ Highest (within contained boundary as indicated by green area in above diagram)

_Applications:_ Manufacturing environments with recurring use.

_Work Area:_ Maximum precision at each marker, with drift correction within the area between any three markers. Normal drift outside of the marker perimeter.
