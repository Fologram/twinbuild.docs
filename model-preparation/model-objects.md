---
layout: default
title: Model Objects
nav_order: 4
parent: Model Preparation
---

# Improving performance by removing and joining objects in models

Twinbuild will scale model geometry to fit a 1500mm bounding box on initial load. If the model contains any objects that are distributed a long distance apart this may result in a very large bounding box and correspondingly small objects on initial load. Be sure to remove any unnecessary geometry to ensure a predictable experience for the end user.

Performance can be improved by joining meshes in the model to reduce draw calls. Twinbuild will automatically join objects if they are on the same layer and have the same material. If your model contains many small objects that will be viewed together place them on the same layer of manually join them into a single mesh to take advantage of these performance optimizations.
