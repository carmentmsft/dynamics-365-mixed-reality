---
author: MattHoag-MS
description: Learn how to enable or disable Azure Object Anchors (Preview) in a Dynamics 365 Guides environment 
ms.author: v-mhoag
ms.date: 11/15/2021
ms.topic: article
title: Enable or disable Azure Object Anchors (Preview) for a Dynamics 365 Guides environment
ms.reviewer: v-bholmes
---

# Enable or disable Azure Object Anchors (Preview) in a Dynamics 365 Guides environment

> [!IMPORTANT]
> Some or all of the functionality noted in this article is available as part of a preview release. The content and the functionality are subject to change.

As of the July 2021 release of Dynamics 365 Guides, an author has the option to anchor a guide with Azure Object Anchors. The November 2021 release allows administrators 
to control if Azure Object Anchors can be selected as the guide anchor type in the PC app or accessed in the Guides model-driven app.  Azure Object Anchors can be enabled or 
disabled for each Dynamics 365 environment.

Azure Object Anchors uses sensing and processing on HoloLens 2 to recognize a physical object and match it with a digital twin that has been imported into Dynamics 365 Guides, 
converted to an object anchor, and assigned to a guide. [Learn more about Azure Object 
Anchors](/dynamics365/mixed-reality/guides/pc-app-anchor-azure-object).

If you're an administrator for Dynamics 365 Guides, you can enable or disable Azure Object Anchors in a specific Dynamics 365 Guides environment. If Azure Object Anchors 
is disabled, authors cannot update a guide's anchor type to an Object Anchor. [Learn more about converting 3D objects to Azure Object 
Anchors](/dynamics365/mixed-reality/guides/pc-app-anchor-azure-object#convert-the-file-in-the-guides-model-driven-app).

## Enable or disable Object Anchors

1. Sign in to the instance by using your admin or author credentials.

    > [!TIP]
    > To find the URL for the instance, select the **Analyze** tab in the PC app. The URL is shown in the **Instance URL** field at the bottom of the page. Copy this URL, 
    and paste it into the address bar of your web browser.
    >
    > ![Instance URL field.](media/instance-url.PNG "Instance URL field")

2. In Power Apps, select the **Guides** app tile.

    ![Guides app tile.](media/guides-app-tile.PNG "Guides app tile")

3. In the left pane, use the area picker at the bottom of the screen to switch the area selection from **Main** to **Settings** to view all settings for the instance.

    ![Settings highlighted in the left pane.](media/Admin-EnableCalling01__Background-GuidesMDA-AreaPicker-Settings.png "Settings highlighted in left pane")

4. In the left pane, select **Environment**, and then move the **Enable Object Anchor (Preview)** slider to enable or disable Object Anchors for the environment.

    ![New command highlighted at top of Power Apps screen.](media/Admin-EnableCalling02__Background-GuidesMDA-AreaSettings-Environment.png "New command highlighted at top of 
    Power Apps screen")
    
    When Object Anchors are turned off, authors will see a **Try Preview** button in the Anchor wizard. If an author selects this button, they'll see a notification to contact their admin if they want to use Object Anchors. Authors will not be able to select an Object Anchor when creating a new guide, or switch the anchor type to an Object Anchor for an existing guide. Any existing guides that already use Object Anchors will not be affected by disabling Object Anchors. 

    ![Try Preview button highlighted in Anchor wizard.](media/anchor-wizard-try-preview.jpg "Try Preview button highlighted in Anchor wizard")

    > [!NOTE]
    > Enabling or disabling Object Anchors is not immediate. A change can take time to propagate. [Learn how to revoke user access in an emergency in 
    Azure Active Directory](/azure/active-directory/enterprise-users/users-revoke-access).

## See also

[Anchor a guide in Dynamics 365 Guides by using Azure Object Anchors Preview](pc-app-anchor-azure-object.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]
