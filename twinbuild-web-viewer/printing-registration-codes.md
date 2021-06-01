---
layout: default
title: Printing Registration Codes
nav_order: 5
parent: Twinbuild Web Viewer
---

# Creating and printing registration code PDFs

Click on any code label in the 3D viewport to open the code dialog, then click the Printer icon to create a PDF booklet of all codes in the model. You can adjust paper size and margins and download this PDF for printing.
{: .fs-6 .fw-300 }

![Twinbuild QR Codes]({{ site.baseurl}}/img/TwinbuildQR.png "Twinbuild QR Codes")

You can also use https://qr.twinbuild.com/ to create a booklet of markers for your work space ahead of time. To create a marker, select an available paper size and give each marker a simple and unique ID. These IDs are used in the Twinbuild web app to assign coordinates to each marker. Because the QR code of the marker contains only this ID information, markers can be used interchangeably on multiple projects. Click on the + button to add an additional marker to the booklet.

After creating the PDF booklet, print each marker at 1:1 scale. Avoid printing markers smaller than A4 as these may be difficult to detect on the HoloLens.

Each printed sheet can be cropped to a square using the grey cut line if required. Ensure not to crop the registration point for the marker (the upper left corner of the QR code indicated by the blue triangle).

If markers are intended to be reused or used in dirty environments, use a matte laminate to protect the paper.
