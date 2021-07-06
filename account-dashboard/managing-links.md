---
layout: default
title: Managing Models with Persistent Links
nav_order: 5
parent: Twinbuild Account Dashboard
---

# Managing Models with Persistent Links

![Twinbuild Link]({{ site.baseurl}}/img/16_Twinbuild_App_ModelQR.png "Twinbuild Link")

Users can view models in Twinbuild on the HoloLens by scanning a Link containing a temporary access token to a model displayed on a mobile or PC screen. These temporary tokens expire after 5 minutes, maintaining security by preventing anyone from viewing the model without signing in to their account and creating a new Link.

![Persistent Link warning]({{ site.baseurl}}/img/17_Twinbuild_App_ModelAccessWarning.png "Persistent Link warning")

However it is often convenient to print Links to include with other printed documents or for access offline. To print a Link with a one year long access token, click View in AR to create a Link, then click Print.

> **Note:** Anyone with access to the physical print of the Link will be able to view this model by scanning with the HoloLens 2, so exercise caution when printing Links to sensitive data.

![Twinbuild Persistent Link]({{ site.baseurl}}/img/18_Twinbuild_App_ModelQRPDF.png "Twinbuild Persistent Link")

Note: Links printed by view capture / print screen or other methods will still include the default access token and will expire after 5 minutes.

### Viewing and editing persistent links

![Manage Links view]({{ site.baseurl}}/img/19_Twinbuild_Account_OfflineCode_crop.png "Manage Links view")

Click on the Edit button next to Manage Persistent Links on your account dashboard to expand the Persistent Links view. The table shows all models with a persistent access token, when each model was last accessed (viewed on the HoloLens) and when the Link will expire. Each of these models can be viewed on the HoloLens 2 by anyone with access to the printed Link. You can open a model in the web viewer by clicking the button next to the model name. To revoke the access token for a Link, click the cross button and acknowledge the prompt.
