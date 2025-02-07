---
author: Mamaylya
description: Learn about the device and licensing requirements for installing and using Microsoft Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 08/10/2022
ms.topic: article
title: Device and licensing requirements for Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Device and licensing requirements for Dynamics 365 Guides

The following table lists technical requirements for deploying and using [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] throughout your organization.

> [!Note] 
> Dynamics 365 Guides might not be available in your country. For more information, see [Dynamics 365 Guides availability](faq.md) and
> [Geographical availability for Power Apps](https://dynamics.microsoft.com/availability-reports/georeport/) (filter the view by **Dynamics 365** > **Operations Apps**, and then scroll the table to see Dynamics 365 Guides availability).

## Device requirements
| Device | Platform | Operating system requirements | Details |
|---|---|---|---|
| [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] | x86, ARM | Build 10.0.17134 or later.<p>[!include[pn-hololens](../includes/pn-hololens.md)] build 10.0.17134 is the earliest build that supports [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. We recommend that you update [!include[pn-hololens](../includes/pn-hololens.md)] to newer versions when they become available.</p> | For information about how to use [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Update for Business, Mobile Device Management, and [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Server Update Services (WSUS), see [Manage updates to HoloLens](/HoloLens/hololens-updates).<p>**Note:** HoloLens includes the Microsoft Edge browser. You can't use Internet Explorer with HoloLens.</p> |
| A computer (PC) that is running [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 (required to create guides) | x64 | A PC that runs [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 with build 10.0.17134 (April 2018 Update 1803) or later.<br><br>**Minimum resolution**. Dynamics 365 Guides supports a minimum effective resolution of 800 x 600 pixels before information loss.  | A PC that runs [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 is used to create and edit guides that will then be available on [!include[pn-hololens](../includes/pn-hololens.md)]. |

> [!TIP]
> [You can set up a device license for multiple operators on a shared HoloLens device](device-license.md). 

## Requirements for services, apps, and features

The following table lists product requirements for services, apps, and features related to Dynamics 365 Guides.

| Service, app, or feature | Product required| Learn more |
|---|---|---|
|Purchase a Dynamics 365 Guides subscription and assign licenses|Azure Active Directory (Azure AD) account<br><br>You'll need an Azure AD account for each licensed user so they can sign in to the app.</li></ul> | [Get started with Azure AD](/azure/active-directory/fundamentals/active-directory-whatis) |
|PC authoring app and HoloLens app| Dynamics 365 Guides| [Buy and deploy Dynamics 365 Guides](setup.md)<p><p>-Or-<p>[Sign up for a free trial subscription](setup.md)</p> |
|Microsoft Dataverse and Power Apps service|Dynamics 365 Guides (included with subscription)|[Buy and deploy Dynamics 365 Guides](setup.md) |
|Outbound calling from Dynamics 365 Guides| Microsoft Teams or Dynamics 365 Remote Assist<br><br>A Microsoft Teams license *is not* included with a Dynamics 365 Guides license. A Microsoft Teams license *is* included with a Dynamics 365 Remote Assist license.</p> | [Learn more about calling from Dynamics 365 Guides](https://powerbi.microsoft.com/desktop/) |
|Analytics dashboard| Power BI Desktop app ([available as a free download](https://powerbi.microsoft.com/desktop/)).</p> | [Learn more about Power BI](https://powerbi.microsoft.com/desktop/) |

## Making and receiving calls

You must have a Microsoft Teams license to make outgoing calls from the Dynamics 365 Guides HoloLens app. This section describes specific Microsoft Teams requirements and describes limitations for the calling feature. 

### Microsoft Teams requirements

| Device                             | OS requirement                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Microsoft Teams app on Windows 10 PC | Any Windows 10 build                                       | A Windows 10 PC running the Teams PC application can collaborate with a Dynamics 365 Guides user on HoloLens 2. |
| Microsoft Teams app on a mobile device | Any iOS or Android phone or tablet running  Microsoft Teams | A phone or tablet running the Microsoft Teams mobile app can collaborate with a Dynamics 365 Guides user on HoloLens 2.|

The Microsoft Teams user can be in the same organization as the Dynamics 365 Guides user, in a federated organization, or a guest in the organization.

### Calling feature limitations

The calling feature in Dynamics 365 Guides does not support:

- Access to the Dynamics 365 Remote Assist model-driven app. Outbound calls from Dynamics 365 Guides are not included in Dynamics 365 Remote Assist call record analytics/insights.
- [Creating and managing assets](/dynamics365/mixed-reality/remote-assist/asset-capture-overview) either within or outside a Dynamics 365 Guides call.
- Creating and sharing one-time-call links.
- Creating or viewing analytics and insights based on call records. 

Dynamics 365 Remote Assist and Dynamics 365 Guides do not currently comply with Microsoft Teams policies.

The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Azure AD member](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Azure AD B2B](/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Azure AD guest account. 

## See also

- [Setup overview](setup.md)
- [Set up a device license for multiple operators on a shared HoloLens device](device-license.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
