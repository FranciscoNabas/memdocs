---
# required metadata

title: In development - Windows 365 Enterprise
titleSuffix: 
description: Windows 365 Enterprise features in development
keywords:
author: ErikjeMS 
ms.author: erikje
manager: dougeby
ms.date: 04/13/2023
ms.topic: conceptual
ms.service: windows-365
ms.subservice: 
ms.assetid: 

# optional metadata

#audience:

ms.reviewer: traceyadams
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: seodec18, references_regions
ms.collection:
- M365-identity-device-management
- tier2
---

# In development for Windows 365 Enterprise

To help in your readiness and planning, this page lists Windows 365 updates and features that are in development but not yet released. In addition to the information on this page:

- If we anticipate that you'll need to take action before a change, we'll publish a complementary post in Office message center.
- When a feature enters production, the feature description will move from this page to [What's new](whats-new.md).
- This page and the [What's new](whats-new.md) page are updated periodically. Check back for more updates.
- Similar features may be announced at different times for Windows 365 Business.

> [!NOTE]
> This page reflects our current expectations about Windows 365 capabilities in an upcoming release. Dates and individual features might change. This page doesn't describe all features in development.

**This article was last updated on the date listed under the title above.**

<!-- Common categories:  
## App management
## Device configuration
## Device provisioning
## Device management
## Intune apps
## Monitor and troubleshoot
## Role-based access control
## Security
## End-user experience

-->

<!-- ***********************************************-->
## Device management

### Support for symmetric NAT with RDP Shortpath<!--43602619-->

In a future update, RDP Shortpath in Windows 365 will support establishing an indirect UDP connection using Traversal Using Relays around NAT (TURN) for symmetric NAT.  TURN is a popular standard for device-to-device networking for low latency, high-throughput data transmission with Azure Communication Services. For more information about TURN and Azure Communication Services, see [Network Traversal Concepts](/azure/communication-services/concepts/network-traversal). For more information about RDP Shortpath, see [Use RDP Shortpath for public networks with Windows 365](rdp-shortpath-public-networks.md).

### Move Cloud PC<!--43450234-->

Today, when changing the region definition or Azure network connection (ANC) in a provisioning policy, only newly provisioned Cloud PCs are created in the new region. Existing Cloud PCs remain in the original region or ANC.

In a future release, a new option will be added to provisioning policies. This new option will let you define a new region or ANC for the provisioning policy, and trigger existing Cloud PCs to move to the updated region. When you initiate the move:

1. All Cloud PCs in the provisioning policy that no longer match the updated region or ANC will be shut down.
2. All such Cloud PCs will be moved to the new region or ANC.

It may take several hours for the moves to complete.

New Cloud PCs created by the provisioning policy will be created in the new region or ANC.

### Group-based license support for Cloud PC resizing<!--41357690-->

In a future update, both single and bulk resizing will support Cloud PCs that were provisioned with group-based licenses.


<!-- ***********************************************-->
<!--## Device provisioning-->

<!--***********************************************-->
## End user experience

### Windows 365 web client keyboard shortcut redirection<!--43951825-->

Windows 365 web client users will be able to use keyboard shortcuts (like Alt + Tab) on their Cloud PC. These shortcuts would normally be intercepted by the host operating system and not sent to the Cloud PC.

<!-- ***********************************************-->
## Monitor and troubleshoot

### End user manual connectivity check<!--37679345 -->

End users will be able to manually run connectivity checks on their Cloud PCs from [windows365.microsoft.com](https://windows365.microsoft.com).

<!-- ***********************************************-->
## Miscellaneous

### Windows 365 Government setup tool<!--43461105-->

A new Windows 365 Government setup tool will replace the current PowerShell scripts that are used to setup tenant mapping and permissions.

<!-- ***********************************************-->
<!-- ## Provisioning -->

<!-- ***********************************************-->
<!--## Role-based access control-->

## Next steps

For details about recent developments, see [What's new in Windows 365](whats-new.md).
