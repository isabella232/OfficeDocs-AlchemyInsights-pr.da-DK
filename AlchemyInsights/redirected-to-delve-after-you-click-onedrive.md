---
title: OneDrive for Business Web OneDrive omdirigerer til Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799983"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="0923a-102">Omdirigeret til Delve, når du har klikket på OneDrive</span><span class="sxs-lookup"><span data-stu-id="0923a-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="0923a-103">Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="0923a-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="0923a-104">For at løse dette problem skal administratoren give brugerne ret til at oprette deres Mit websted-websted.</span><span class="sxs-lookup"><span data-stu-id="0923a-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="0923a-105">Dette skyldes, at siden OneDrive for Business oprettes på Mine websteder.</span><span class="sxs-lookup"><span data-stu-id="0923a-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="0923a-106">Hvis du vil tildele denne ret, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="0923a-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="0923a-107">Klik på brugerprofiler i SharePoint **Administration.**</span><span class="sxs-lookup"><span data-stu-id="0923a-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="0923a-108">I sektionen **Personer** skal du klikke **på Administrer brugertilladelser**.</span><span class="sxs-lookup"><span data-stu-id="0923a-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="0923a-109">Tilføj brugere, der skal have tilladelse til at oprette deres Mit websted-websted.</span><span class="sxs-lookup"><span data-stu-id="0923a-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="0923a-110">Denne indstilling er som standard indstillet til **Alle undtagen eksterne brugere.**</span><span class="sxs-lookup"><span data-stu-id="0923a-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="0923a-111">Når du har tilføjet brugeren, brugerne eller gruppen, skal du kontrollere, at den tilføjede bruger, brugere eller gruppe er markeret, rulle ned til **tilladelsessektionen** og derefter markere afkrydsningsfeltet ud for Opret personligt websted (påkrævet til personligt **lager, nyhedsstrøm** og fulgte indhold).</span><span class="sxs-lookup"><span data-stu-id="0923a-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="0923a-112">Klik **på OK,** og få derefter brugeren til at gå til OneDrive-siden for at oprette webstedet.</span><span class="sxs-lookup"><span data-stu-id="0923a-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
