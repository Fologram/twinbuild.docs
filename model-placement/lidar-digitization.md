---
layout: default
title: Digitizing Markers from LIDAR Scans
nav_order: 3
parent: Model Placement
---

# How to determine Marker locations from high resolution LIDAR scans

Optimal precision can be obtained by distributing Markers within the work space at approximately 4000mm apart in locations that are easily visible by workers wearing the HoloLens.
{: .fs-6 .fw-300 }

An efficient way to achieve this is to arbitrarily place markers within the work space and then use a high precision LIDAR scan to measure the relative locations of each marker. Alternatively you can use professional surveying equipment (Total Stations etc) or consumer laser measuring tools (Disto 3D) to digitize marker positions.

### Deciding where to locate markers

Markers can be placed arbitrarily within the environment with an approximate spacing between markers of 4000mm. Where possible place markers near work areas and avoid placement of markers in locations where viewing the marker on the HoloLens could lead to tracking loss (due to the occlusion of feature points e.g. close to a large wall). If you are outsourcing the scanning process to a third party, you should also attach visual information to indicate the marker ID in a manner that will be easily visible on the LIDAR scan (e.g. large temporary labels or colour coding etc).

### LIDAR Scan Setup

Locate the scanner at the center of the workspace so all (or as many as possible) of the codes are visible. Multiple scans can be used but may introduce imprecision due to misalignment of individual scans. Use the highest precision settings available for your scanner. Precision will be affected by noise in scan depth data (typically increasing with points further from the scanner) together with human error introduced from picking the QR code registration point from available points. This human error is usually introduced due to low resolution scans or points a long distance from the scanner.

### Estimating Positions from Point Clouds

After completing the scan, import the point cloud data to a CAD package such as Rhino and fit rectangles to points in the scan indicating QR codes. Use the corner of the rectangle nearest to the registration point of the marker (indicated by the blue triangle) to determine the location of the code.

### Preparing and saving registration point coordinates for Twinbuild

After digitizing all of the marker positions, move the entire collection of points such that 0,0,0 is located on the floor of your workspace in your point cloud and roughly in the middle of the area you plan to work within using the HoloLens. Keep note of each of these coordinates (after moving) and associated marker ID in a text file for input to Twinbuild.
