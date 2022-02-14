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

![Two Marker Precision]({{ site.baseurl}}/img/Precision_2Markers.png "Two Marker Precision")

### Two Markers

_Implementation:_ Using a tape measure / disto, align markers with the workspace at a known measured distance apart.

_Precision:_ High (along marker line - indicated by green in the above diagram), very poor beyond the line.

_Applications:_ 1:1 visualization and for linear applications up to 4000mm long and up to 2000mm high (e.g. wall construction). Larger applications should work with linear marker arrays (see below).

_Work Area:_ Maximum precision at each marker, with drift correction along the line between markers. Normal HoloLens drift at any distance from this line.

![Linear Marker Precision]({{ site.baseurl}}/img/Precision_LinearMarkers.png "Linear Marker Precision")

### Linear Markers

_Implementation:_ Using a tape measure (and stringline if necessary), align markers with the workspace at a known measured intervals.

_Precision:_ High (along marker line - indicated by green in the above diagram), very poor beyond the line.

_Applications:_ 1:1 visualization and for linear applications up to 2000mm high (e.g. wall construction).

_Work Area:_ Maximum precision at each marker, with drift correction along the line between markers. Normal HoloLens drift at any distance from this line.

![2D Grid Precision]({{ site.baseurl}}/img/Precision_2DGrid.png "2D Grid Precision")

### 2D Grids

_Implementation:_ Using a tape measure / disto and laser level, locate a square grid of markers at a known measured distance apart. Alternatively, place markers at known locations e.g. along intersecting lines of column grids or at corners of interior walls.

_Precision:_ Moderate to high (due to human error in setting out grid and imprecision in built features). Precision is best near markers and within the contained boundary.

_Applications:_ Setout applications contained within the marker perimeter and up to 2000mm high, where floor mounted markers will not be occluded during the course of the application.

_Work Area:_ Maximum precision at each marker, with drift correction within the area between any three markers. Normal drift outside of the marker perimeter.

![Workpiece Corners Precision]({{ site.baseurl}}/img/Precision_ObjectCorners.png "Workpiece Corners Precision")

### Workpiece Corners

_Implementation:_ Locate markers at the corners of a workpiece to define a bounding volume.

_Precision:_ Low to Moderate. Precision relies on equal precision in the workpiece and is best near markers.

_Applications:_ Setout and fabrication applications on small moving objects up to 4x4x4m where markers are accessible during work.

_Work Area:_ Maximum precision at each marker, with drift correction within the bounding volume. Normal drift outside of the marker volume.

![Workpiece Grid Precision]({{ site.baseurl}}/img/Precision_ObjectGrid.png "Workpiece Grid Precision")

### Workpiece Grid

_Implementation:_ Locate markers at approximately repeating intervals on known locations on a workpiece.

_Precision:_ High. Precision relies on equal precision in the workpiece and can be increased by reducing the intervals between markers.

_Applications:_ Setout and fabrication applications on large moving objects of any scale where markers are accessible during work.

_Work Area:_ Maximum precision at each marker, with drift correction within the bounding volume. Normal drift outside of the marker volume.

![Workpiece Features Precision]({{ site.baseurl}}/img/Precision_ObjectFeatures.png "Workpiece Features Precision")

### Workpiece Features

_Implementation:_ Locate markers at known locations on a workpiece on close proximity to the area where a task will be performed.

_Precision:_ High. Precision relies on equal precision in the workpiece and can be increased by adding markers as close as possible to the work area.

_Applications:_ Setout and fabrication applications on existing building sites and structures e.g. for MEP installation.

_Work Area:_ Maximum precision at each marker, with drift correction within the bounding volume. Normal drift outside of the marker volume.
