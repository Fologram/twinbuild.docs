---
layout: default
title: Framing Assembly
nav_order: 1
parent: Applications
---

# Timber and Steel Frame Assembly

Twinbuild can be used measure off and layout timber and steel frames manually, or perform QA on automated framing processes.
{: .fs-6 .fw-300 }

Working from holographic guides in Twinbuild for framing fabrication can minimize mistakes and improve set out productivity, and maintain a digital design to production workflow. Twinbuild can help with set out on frames with multiple unique parts / lengths / joints, as well as guide during prefabrication of cabling, pipework and other services.

When working with automated processes for framing fabrication, Twinbuild can assist with assembly and help workers perform quick visual checks using object-aligned holographic models. QA can be performed during fabrication, offsite and onsite before install.

### Model Preparation

![Frame Assembly 2D]({{ site.baseurl}}/img/applications/FramingAssembly2d.png "Frame Assembly 2D")

For simple frame designs a 2D drawing is sufficient for setout. If working from Revit, export and insert a DXF of the frame drawing into a 3D view to publish to Twinbuild. Assign different colours to framing and services for clarity.

![Frame Assembly]({{ site.baseurl}}/img/applications/FramingAssembly.png "Frame Assembly")

For QA or more complex models (for instance with multiple profiles or complex services) export a low-polygon 3D model of the frame. Model sections as single surface extrusions rather than as solids when possible. When viewing the model in Twinbuild on the HoloLens, enable Outlines to overlay physical frames with virtual content without occluding the physical frame with a solid hologram. Model all services (cables and pipes) as linework.

Replace surface trims with curve outlines to avoid creating high-polygon meshes in Twinbuild. For instance, bores for cabling should be modelled as curve outlines rather than booleans to ensure you can still use the Outline display for the frame geometry without introducing artifacts.

![The effect of booleaned bores]({{ site.baseurl}}/img/applications/MeshCompare.png "The effect of booleaned bores")

_Above: Steel section modelled as a simple extrusion with linework indicating bore geometry. Below: bores booleaned from steel section and the resulting mesh geometry_

### Marker Setout

_Fabrication:_ For optimal precision setup a marker grid in the production space with spacing of maximum 3000x3000mm. In the Twinbuild Web Viewer, use Orient To World and add the marker positions. These markers can be imported into any model published to Twinbuild when fabricating multiple frame designs.

_QA:_ In the Twinbuild Web Viewer, use Orient to Object and locate a marker on each of the four corners of the frame. Fix these markers precisely on the physical frame by folding the tab of the Marker.

### Task Guidance

_Fabrication:_ Follow best practice for [user behaviour]({{site.baseurl}}/hololens-precision/user-behaviour) before performing set out or fabrication. When setting out or placing framing, ensure the hologram is viewed in plan and at arms length. Use physical templates for setting out precise right angles where required.

_QA:_ For reliable perception of precision, observe the hologram in plan at approximately arms length. Reliability will be best in close proximity to Markers.
