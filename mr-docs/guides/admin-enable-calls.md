---
author: MattHoag-MS
description: Learn how to enable or disable calling in a Dynamics 365 Guides environment 
ms.author: v-mhoag
ms.date: 11/08/2021
ms.topic: article
title: Enable or disable calling for a Dynamics 365 Guides environment
ms.reviewer: v-bholmes
---

# Enable or disable calling (Preview) in a Dynamics 365 Guides environment

> [!IMPORTANT]
> The Calling feature for Dynamics 365 Guides is in Preview, so not all functionality is available yet. We're working to bring additional features such as chat and text scaling in later Dynamics 365 Guides releases. Please be aware of these limitations before using the Calling Preview.

As of the November 2021 release of Dynamics 365 Guides, calling is enabled by default. When calling is enabled, a Microsoft Dynamics 365 Guides HoloLens user can make a one-to-one call to a remote collaborator. The remote collaborator can join the call using the Microsoft Teams desktop app or the mobile app. During the call, the remote collaborator can see everything seen by the Dynamics 365 Guides user, including holograms and the real world behind the holograms.

If you're an admin for Dynamics 365 Guides, you can enable or disable calling for a user in a specific Dynamics 365 Guides environment. Enabling or disabling calling by environment is useful when operators or authors do not need to work with remote collaborators. Or if it is preferred that HoloLens users are not able to start a call and allow remote collaborators to see everything that they see while working in Dynamics 365 Guides.  

[Learn about licensing requirements and limitations when making calls in Dynamics 365 Guides](requirements.md)

## Enable or disable calling

1. Sign in to the instance by using your admin or author credentials.

    > [!TIP]
    > To find the URL for the instance, select the **Analyze** tab in the PC app. The URL is shown in the **Instance URL** field at the bottom of the page. Copy this URL, and paste it into the address bar of your web browser.
    >
    > ![Instance URL field.](media/instance-url.PNG "Instance URL field")

2. In Power Apps, select the **Guides** app tile.

    ![Guides app tile.](media/guides-app-tile.PNG "Guides app tile")

3. In the left pane, use the area picker at the bottom of the screen to switch the area selection from **Main** to **Settings** to view all settings for the instance.

    ![Settings highlighted in the left pane.](media/Admin-EnableCalling01__Background-GuidesMDA-AreaPicker-Settings.png "Settings highlighted in left pane")

4. In the left pane, select **Environment**, and then move the **Enable calls** slider as needed to enable or disable calling for the environment.

    ![New command highlighted at top of Power Apps screen.](media/Admin-EnableCalling02__Background-GuidesMDA-AreaSettings-Environment.png "New command highlighted at top of Power Apps screen")

    If a user tries to start a call while working in an environment where calling is disabled, the user will see the following error message:

    "**Your admin may have disabled calling or you may not have a Microsoft Teams or Remote Assist license.**"
    
    > [!NOTE]
    > Enabling or disabling calling is not immediate. A change can take time to propagate. [Learn how to revoke user access in an emergency in Azure Active Directory](/azure/active-directory/enterprise-users/users-revoke-access).

## See also

- [Make a call in Dynamics 365 Guides](make-call.md)
- [Licensing and product requirements for making calls in Dynamics 365 Guides](requirements.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]