---
layout: default
title: Admin setup for Microsoft Accounts
nav_order: 7
parent: Creating an Account
grand_parent: Twinbuild Account Dashboard
---

# Setup instructions for Microsoft Active Directory

If you see a "Need Admin Approval" popup when signing in to Twinbuild for the first time using a Microsoft email, ask your Global Active Directory Administrator to check if your Active Directory tenant is configured to require admin consent for User.Read permission.

![Need Admin Approval]({{ site.baseurl}}/img/Need_Admin_MS.png "Need Admin Approval")

If you're not prompted at login to request consent from your tenant's Global Admin, you can send them this link: https://login.microsoftonline.com/common/adminconsent?client_id=97b04478-b065-44e6-a810-636a4dc59d35

Your administrator will then be able to log in and grant permission with the following screen:

![Request Permissions]({{ site.baseurl}}/img/Request_Permission_MS.png "Request Permissions")

(Note you may receive an invalid redirect after accepting the permission, however it will be granted and can be verified in the Azure admin panel)
