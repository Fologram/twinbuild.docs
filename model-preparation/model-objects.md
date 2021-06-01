---
layout: default
title: Model Objects
nav_order: 4
parent: Model Preparation
---

# Improving performance by removing and joining objects in models

Twinbuild will scale model geometry to fit a 1500mm bounding box on initial load. If the model contains any objects that are distributed a long distance apart this may result in a very large bounding box and correspondingly small objects on initial load. Be sure to remove any unnecessary geometry to ensure a predictable experience for the end user.

Performance can be improved by joining meshes in the model to reduce draw calls. If your model contains many small objects that will be viewed together (e.g. the experience does not require viewing objects one at a time in a sequence), join these into a single mesh before publishing.
