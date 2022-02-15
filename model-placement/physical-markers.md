---
layout: default
title: Physical Markers
nav_order: 4
parent: Model Placement
---

# Best practice for working with physical Markers

Twinbuild registration codes can be printed, laminated and reused from project to project.
{: .fs-6 .fw-300 }

It is important to follow best practice when creating printed QR codes to ensure they are easily detectable by the hololens and precisely located in physical space.

### Printing Markers

Location codes should be printed at a size that ensures they are easily visible to the hololens during typical occupation of a site or workspace. Generally speaking A4 or A3 prints are appropriate for most use cases. Larger codes will be detected by the HoloLens from greater distance but do not track more precisely than smaller codes detected nearer to the HoloLens camera.

When printing markers, ensure that there is at least 10mm of white padding around the edge of the QR code. If you are cutting the prints down to size before using the markers, take care not to remove this extra white space to ensure optimal tracking.

### Placing Markers

When placing markers in physical space, fold over the top left corner of the code (indicated by the black dog ear on the printed page) so that the corner of the code can be exactly positioned in physical space. This will allow you to keep a white margin around the code while still being able to position the origin point of the code hard against physical objects like columns or walls.

### Handling Markers

Take care that the printed surface of the code remains as flat as possible when handling markers. Any undulation in the surface of the code can introduce noise and result in imprecision in the detected marker position. Where possible, print codes on heavy stock material or laminate. Reprint any markers that have become folded, torn or otherwise damaged. You should be able to precisely position the newly printed marker in the same location as the damaged code by folding over the corner of the code sheet as before.

### Reusable Markers

Registration codes can be laminated for durability and reusability across projects. Use a matte surface laminate to reduce reflection and glare and improve detection on the HoloLens. Note: The HoloLens will cache the position of all detected markers and will not detect markers that have moved from these cached positions. If you are planning to move markers, take care to restart the HoloLens before re-scanning the markers to ensure that this cache has been cleared.

### Codes on objects - magnets, etching and stickers

Registration codes can be printed on any surface to make placement on objects simpler. Printing on magnetized surfaces allows registration codes to be quickly fixed to steel benches and parts, and QR codes can be etched or stencilled on timber pieces for precise registration. Stickers can also be used to permanently fix QR codes in manufacturing spaces.

### Codes on moving objects

Ensure your model is set to ["Orient To Object"]({{ site.baseurl}}/twinbuild-web-viewer/adding-registration-codes) when positioning markers on objects that will be in unknown or changing physical orientations.
