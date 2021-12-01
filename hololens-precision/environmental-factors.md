---
layout: default
title: Environmental Factors
nav_order: 2
parent: HoloLens Precision
---

# How the work environment affects HoloLens precision

A work environment that is well suited to hololens tracking can be created by minimizing factors that adversely affect the ability of the hololens to detect and track static feature points in the space.
{: .fs-6 .fw-300 }

### Issues with moving objects

_Cause:_ Large objects will likely include features that the HoloLens uses for tracking. Lots of moving objects (e.g. crowded spaces) can occlude tracked feature points and reduce tracking performance.

_Impact:_ As a result holograms can appear to move when these large objects are moved as the Hololens cannot differentiate between motion of tracked features and motion of the HoloLens device.

_Identification:_ If you are experiencing ‘jumps’ in hologram position as you move around a space this may be due to the spatial tracking data being corrupted by the movement of larger objects.
Moving just a few small objects should not noticeably affect tracking performance.

_Solution:_ Avoid working around large moving objects or in crowded spaces. If these cannot be avoided, reset tracking data after moving large objects by opening the Settings menu on the HoloLens 2 and navigating to System > Holograms > Remove All Holograms. Then spend a few minutes walking around the space to rebuild tracking data.

### Issues with black and reflective materials

_Cause:_ The RGB cameras on the HoloLens are typically unable to track feature points on black surfaces due to the limited contrast on black surfaces visible to the cameras. Reflective surfaces also reflect tracked features.

_Impact:_ As the HoloLens cannot easily differentiate between a reflected feature and the feature itself, the position of the reflected feature will appear incorrect relative to other non-reflected features in the tracked space and reduce tracking performance.

_Identification:_ Very glossy materials and reflective glass are common causes of poor tracking. Wet environments will also typically become reflective and reduce tracking performance.

_Solution:_ If working in reflective or black environments is unavoidable, consider temporarily covering reflective materials with matte sheet (canvas, cardboard etc) and dry any wet and reflective surfaces.

### Issues with empty spaces

_Cause:_ Large warehouse spaces, empty factories and workshops, halls, board rooms and some outdoor spaces e.g. car parks or green field sites will all track poorly due to the absence of unique feature points.

_Impact:_ As a result you may experience drift due limited available tracking data. Complete tracking loss is also more likely when fewer feature points are visible to the Hololens cameras.

_Solution:_ Work in the presence of objects (tools, furniture, plants etc) where possible, and add objects or non-repeating drawn patterns to the work space if necessary to improve tracking.

### Issues with variable light conditions

_Cause:_ Very light or dark spaces will negatively affect tracking as the RGB cameras on the HoloLens will not have sufficient contrast to detect feature points. Spaces with changing light conditions (such as by switching lights on or off) can also track poorly as shadows cast by lights may have been relied on as tracked feature points. Moving lights or shadows in the workspace can also negatively affect tracking for the same reason as moving objects.

_Impact:_ Working in spaces with variable light conditions may lead to unpredictable tracking performance.

_Identification:_ If you experience a reduction in tracking quality over time without physically altering the environment (e.g. moving objects) then this may be due to a change in lighting conditions.

_Solution:_ Avoid working outdoors when requiring high precision, or create a shaded environment where light conditions can be controlled. Establish static and even lighting conditions in the work area and use multiple lights to avoid creating temporary or moving shadows that may be relied on for tracking.

### Issues with repeating patterns

_Cause:_ Repeating tiles, carpet, panels and structure all negatively affect tracking performance through the absence of unique features.

_Solution:_ Cover repeating patterns or avoid working in these spaces if possible.

For more information see [Microsoft's documentation](https://docs.microsoft.com/en-us/hololens/hololens-environment-considerations).
