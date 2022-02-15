---
layout: default
title: Marker Setup
nav_order: 4
parent: HoloLens Precision
---

# How Marker visibility affects Precision

The visibility of Markers in the work environment will impact hologram precision.
{: .fs-6 .fw-300 }

Twinbuild uses detected Marker positions to correct for ordinary drift in hologram position over time. The frequency and relative position from which these markers are scanned will affect tracking and corresponding precision. An appropriate distribution of Markers should be designed to ensure optimal precision for a given work site and task, see [this guide]({{site.baseurl}}/model-placement) for more detail in designing marker distributions.

### Issues with infrequently scanning markers

_Cause:_ A work space may contain many markers but Twinbuild will locate models at 1:1 after only two markers are scanned. The closest marker to where work is being completed may therefore not be scanned.

_Impact:_ Drift and imprecision if markers near work space are not scanned.

_Identification:_ Appearance of drift during work. See [this article]({{site.baseurl}}/hololens-precision/recognizing-poor-tracking) for help identifying drift.

_Solution:_ Encourage users to scan all markers in a work area before starting work. When moving from one area of a work area to another encourage re-scanning the most proximate three markers before returning to work.

### Issues with detecting markers from far away or at oblique angles

_Cause:_ The HoloLens will automatically correct for drift with all tracked markers. Reliability in the tracked position of markers decreases with distance and angle to the camera (due to the decrease in the number of pixels of the marker available for tracking) and drift correction may therefore be performed sub-optimally.

_Impact:_ Incorrect drift correction leading to imprecise hologram position

_Identification:_ Small jumps in hologram position during work.

_Solution:_ Ensure that markers nearest to the work area are scanned before beginning work - this will reduce the impact of any markers detected further away. Avoid positioning markers near the work area on oblique angles. Because only the origin (top left corner) of the marker is used for tracking it is usually possible to change the orientation of the marker so they are perpendicular to the HoloLens during work.
