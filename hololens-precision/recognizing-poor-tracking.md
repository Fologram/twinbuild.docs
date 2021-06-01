---
layout: default
title: Recognizing Poor Tracking or Miscalibration
nav_order: 1
parent: HoloLens Precision
---

# Learning to recognize sub-optimal tracking on the HoloLens

Poor tracking may not be immediately obvious to the user especially when viewing models located freely in 3D space.
{: .fs-6 .fw-300 }

### Methods for identifying poor tracking

_Total tracking loss:_ When the HoloLens loses tracking entirely, Twinbuild will exit and display a notification saying ‘Attempting to find your space’.

_Drift relative to physical space:_ Use a piece of tape to mark the position of a visible feature of the hologram (e.g. corner point of a wall) on the ground. Walk around and note how the corner of the hologram moves relative to the piece of tape. Any misalignment is the result of non-optimal tracking.

_Misalignment with registration points or objects:_ Align a holographic model of objects in a physical space (walls, columns, desks etc) with the physical space using registration points. If the digital model and registration points are precise, any misalignment between the hologram and physical objects is the result of non-optimal tracking.

_Measured tests:_ Use tape or pencil to mark the corner points of a 3000mm x 3000mm grid displayed on the HoloLens. Using a measuring tape, measure the distance between the marked points. Distances greater or smaller than 3000mm are due to non-optimal tracking or human error.

### Recognizing incorrect IPD calibration

The HoloLens 2 should prompt the user to ‘Adjust the device for your eyes’ whenever you switch the device between users. This process adjusts the IPD of the device to suit the new user. If the device has not been adjusted and the device IPD setting is significantly different to the user's IPD, holograms may be rendered at the incorrect depth and appear to drift very significantly. A quick visual check of hologram position relative to an easily observable fixed feature in the physical space (e.g. the corner of a desk or the edge of a floor board) is usually enough to recognize drift that may be the result of incorrect device IPD.

To ensure the HoloLens 2 is calibrated for your IPD, launch the Calibration app from the home menu on the HoloLens 2 and follow the instructions to complete the calibration.
