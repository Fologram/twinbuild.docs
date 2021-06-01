---
layout: default
title: User Behaviour
nav_order: 3
parent: HoloLens Precision
---

# How user calibration and behaviour affects precision

User behaviour will affect tracking performance as the user controls which parts of the work space are visible to the RGB cameras on the HoloLens used for tracking.
{: .fs-6 .fw-300 }

Users should be trained in appropriate use of the HoloLens to minimize adverse impact on tracking and precision during work.

### Issues with covering cameras

_Cause:_ Covering HoloLens cameras with clothing, protective equipment, welding helmets, dirt / dust / scratches or with hands during use will all reduce tracking performance as feature points used for tracking will no longer be visible or will become blurred.

_Impact:_ Covering cameras can lead to unpredictable tracking performance or total tracking loss.

_Identification:_ After losing tracking the position of holograms may appear to jump dramatically as the HoloLens attempts to correct for newly visible feature points. This can be especially disruptive when sharing devices between multiple users.

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
