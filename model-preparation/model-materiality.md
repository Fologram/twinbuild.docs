---
layout: default
title: Model Materiality
nav_order: 2
parent: Model Preparation
---

# Selecting appropriate materials for augmented reality

Holograms rendered as surfaces can obscure parts of the physical environment that need to be visible to carry out a task. Rendering surface models on the hololens with textures or reflective materials can also distract workers from following spatial guides and reduce the immersion of the experience by creating screendoor effects or the appearance of pixelated surfaces. Generally speaking, avoid surface models and the use of textures on the HoloLens to ensure the physical environment is always visible to the user.

## Hiding holograms with black materials

A common challenge to working entirely with vector geometry (curve and lines) in mixed reality is the lack of occlusion, and virtual objects will be visible even when they are "behind" physical objects in a workspace. This increases the difficulty of following virtual objects as spatial guides as users need to constantly check to ensure they are working with the correct guide and not some linework that is in the background some distance away. To address this issue, physical objects can be approximately modelled and assigned black materials in order to obscure virtual content in mixed reality. Black materials will be rendered to the depth buffer while appearing transparent on the HoloLens 2, creating an effective (albeit fake) experience of virtual content being hidden by physical objects.
