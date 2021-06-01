---
layout: default
title: HoloLens Tracking
nav_order: 1
parent: HoloLens Overview
---

# How does the HoloLens fix models in place?

The HoloLens 2 uses ‘inside out’ tracking to estimate headset pose from the position and motion of feature points within the work environment that are visible to the onboard cameras.
{: .fs-6 .fw-300 }

![HoloLens 2 Cameras](https://docs.microsoft.com/en-us/hololens/images/hololens2-front-view.png "HoloLens 2 Cameras")

The HoloLens has 4 greyscale cameras that are used to detect high contrast features and estimate their depth. As you and the HoloLens move, the relative position of the feature points is tracked by SLAM algorithms running on the headset and used to update the camera pose. Holograms are then rendered on the stereo display of the Hololens using this camera position.

![SLAM Example](https://www.andreasjakl.com/wp-content/uploads/2018/08/Davison-MonoSLAM-Map.jpg "SLAM Example")
_Example of tracked feature points. Image credits: Davison, A. J., Reid, I. D., Molton, N. D., & Stasse, O. (2007). MonoSLAM: Real-time single camera SLAM. IEEE Transactions on Pattern Analysis & Machine Intelligence, (6), 1052-1067._
{: .fs-2 .fw-300 }

The reliability of holographic models for set out tasks will be impacted by the precision with which registration markers can be located (LIDAR or survey precision), the GPU load on the HoloLens (model polygon, object and texture count), user behaviour in maintaining positions where tracking features are visible (covering cameras or moving too close to blank walls), device calibration for the user and the availability of suitable features to track within the work space.
