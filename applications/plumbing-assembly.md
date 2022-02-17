---
layout: default
title: Plumbing Assembly
nav_order: 3
parent: Applications
---

# Plumbing Assembly and Installation

Twinbuild can assist with pre-fabrication and install of drainage systems and pipework
{: .fs-6 .fw-300 }

Twinbuild can be used to prefabricate plumbing modules such that pipes, fittings and traps meet requirements for falls and perfectly fit with on site conditions such as slab penetrations and ceiling cavities. For on-site installation, Twinbuild can be used to visualize where pipes run through existing structures to minimize material usage, setout time and mistakes.

### Model Preparation

![Plumbing Installation]({{ site.baseurl}}/img/applications/PlumbingInstallation.png "Plumbing Installation")

_Assembly_ Create a low-polygon mesh of pipes and fittings (under 10,000 faces) of the assembly and any critical connection points such as slab penetrations. Use outline rendering in Twinbuild on the HoloLens to create virtual templates of pipework to assist with 3D placement and orientation during assembly.

_Installation_ For installation, use linework to describe pipe centerlines where possible and avoid publishing mesh models of fittings if possible. Where 3D meshes are required - for instance to describe more complex connections - keep these to under 10,000 faces to work with outlines in Twinbuild. It is often useful to publish some reference geometry of as built conditions such as finished faces of walls or structure as a visual reference for hologram drift during install.

### Marker Setout

_Assembly_ Two markers are usually sufficient for precision of small modules. For larger modules use a grid of four or more markers. These can be permanently set up in an offsite work environment and re-imported into each new module design model for expediency.

_Installation_ For installation, locate markers at known physical reference points as near as possible to the installation work area. For instance, markers may be located at the corners of interior wall edges defining the installation work area.

![Setout from existing walls]({{ site.baseurl}}/img/Precision_ObjectFeatures.png "Setout from existing walls")

### Task Guidance

Follow best practice for [user behaviour]({{site.baseurl}}/hololens-precision/user-behaviour) before performing set out. Walk around the site for 5 minutes and ensure all markers have been scanned. Before starting setout, ensure the closest marker has been recently scanned.

_Assembly_ Enable outlines in Twinbuild on the HoloLens to create a virtual template within which to locate physical parts. Viewing the hologram in elevation can be used to precisely assemble correct falls. Viewing the hologram in plan can be used to precisely connect to existing conditions such as slab penetrations. Remember that the true position of the hologram is easiest to perceive when viewed in the center of the field of view and front-on to the model.

_Installation_ Perform quick visual checks to ensure minimal drift by comparing the holographic model of as built surfaces to the existing conditions on site. If installing small pipework, use centerlines to guide installation and bore holes in existing framing or cladding as required.
