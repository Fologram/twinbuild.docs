---
layout: default
title: User Behaviour
nav_order: 3
parent: HoloLens Precision
---

# How user calibration and behaviour affects precision

User behaviour will affect tracking performance as the user controls which parts of the work space are visible to the RGB cameras on the HoloLens used for tracking.
{: .fs-6 .fw-300 }

Users should be trained in appropriate use of the HoloLens to minimize adverse impact on tracking and precision during work. For more information see [Microsoft's documentation](https://docs.microsoft.com/en-us/hololens/hololens-spaces).

### Issues with inferring position of far away or peripheral objects

_Cause:_ Holograms can be seen at any arbitrary distance from the viewer. However, attempting to use holograms at greater than arms length from the viewer may introduce apparent drift due to incorrect perception of the location of the object. Incorrect perception is usually caused by lever arm effects when rendering depth on stereo displays: small movement in the position of the display relative to the eyes can result in large apparent motion in objects far away.

_Impact:_ Incorrect perception of hologram position resulting in apparent drift / imprecision. See [this article]({{site.baseurl}}/user-experience/model-reach) for more information.

_Identification:_ After moving to within arms length of the hologram in question it will appear to have moved.

_Solution:_ The true position of the hologram can be more accurately perceived at arms length and directly within the field of view of the stereo display.

### Issues with inferring position of objects on oblique angles

_Cause:_ When holograms are viewed on oblique angles the limited visibility of the object makes it difficult to accurately infer the position the object in XYZ space. For instance, a bricklaying application requires holographic models of each course of bricks to be viewed in plan to determine the position of each brick. However, as courses reach eye height the view of the hologram becomes increasingly oblique and introduces error.

_Impact:_ Incorrect perception of hologram position resulting in apparent drift / imprecision, especially from incorrectly judging depth.

_Identification:_ After moving to a "front on" view of the hologram the object appears to have moved.

_Solution:_ The true position of the hologram can be more accurately perceived when viewed "front on" e.g. when the face of the object is perpendicular to the direction of view. If necessary view holograms from scaffolding / ladders etc to maintain a front on view.

### Issues with covering cameras

_Cause:_ Covering HoloLens cameras with clothing, protective equipment, welding helmets, dirt / dust / scratches or with hands during use will all reduce tracking performance as feature points used for tracking will no longer be visible or will become blurred.

_Impact:_ Covering cameras can lead to unpredictable tracking performance or total tracking loss.

_Identification:_ After losing tracking the position of holograms may appear to jump dramatically as the HoloLens attempts to correct for newly visible feature points. This can be especially disruptive when sharing devices between multiple users.

_Solution:_ Keep cameras clean and unobscured during use.

### Issues with working in close proximity to surfaces

_Cause:_ Working in close proximity to blank walls, floors and ceilings can reduce the number of visible feature points available for tracking.

_Impact:_ Complete tracking loss that may require leaving the workspace to recover.

_Solution:_ Keep objects at arms length and avoid working very close to small or detailed objects. Remain aware of how much of the work space is visible to the Hololens cameras. If necessary add patterns or objects to blank surfaces to minimize the chance of tracking loss.

### Issues with device motion

_Cause:_ Placing the device down upside down, or moving the device rapidly can lead to tracking loss.

_Impact:_ Complete tracking loss that may require clearing spaces to recover.

_Solution:_ Avoid rapid motion when manually moving devices and train users to place the HoloLens the right way up when not in use.

### Issues with sharing devices between users

_Cause:_ Passing the HoloLens to another user may occlude the HoloLens cameras and lead to tracking loss. The new user’s IPD may vary significantly from the current user and without adjusting the device IPD can lead to the appearance of hologram drift.

_Impact:_ Non-optimal tracking or drift due to miscalibration.

_Solution:_ If requiring optimal tracking and precision, always adjust the device for your eyes when prompted by the HoloLens. If you know the users who will be using the HoloLens, setup Azure Active Directory to store user profiles and automatically adjust IPD for each new user.

### Issues with headset fit

_Cause:_ Loose headset fit results in movement of the display relative to the users eyes and associated appearance of movement in hologram position.

_Impact:_ Incorrect or unreliable perception of hologram position.

_Solution:_ Ensure headset display is tilted all the way down and rests just above the wearer's nose, the display is centered on the users nose and level and the the head strap is firmly tightened before beginning work.
