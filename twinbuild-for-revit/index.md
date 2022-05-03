---
layout: default
title: Twinbuild For Revit
nav_order: 9
has_children: true
---

# Installing Twinbuild for Revit

Publish models directly from Revit with our integration
{: .fs-6 .fw-300 }

[Get Twinbuild](https://twinbuild.com/download){: .btn }

You will need admin rights on your machine and Revit 2019 or newer to install the plugin. Run the installer and accept the default installation location to install the plugin. Once the installation is complete, you should see the Twinbuild ribbon added to the Add-Ins tab in Revit.

![Twinbuild for Revit]({{ site.baseurl}}/img/TwinbuildForRevit.png "Twinbuild for Revit")

To publish the current active view, click on the Publish button in the Twinbuild ribbon. To publish multiple views in a single model, click on the Publish Multiple button then select the views to publish. Drag and drop the selected views to change the publishing order and create guides from model geometry that can be stepped through in sequence using Twinbuild on the HoloLens.

![Publishing Multiple Views]({{ site.baseurl}}/img/Twinbuild_PublishMultiple.png "Publishing Multiple Views")

Once the views have been selected, click on Publish to export the geometry and open a preview in the web browser. Note that large models or multiple views may take some time to export and for best results ensure that Google Chrome is set as your PCs default web browser.
