---
title: OneDrive for Business Web OneDrive omdirigerer til Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722804"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="b8d93-102">Omdirigeret til Delve, når du har klikket på OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8d93-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="b8d93-103">Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="b8d93-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="b8d93-104">For at løse dette problem skal administratoren give brugerne ret til at oprette webstedet Mine websteder.</span><span class="sxs-lookup"><span data-stu-id="b8d93-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="b8d93-105">Det skyldes, at onedrive for business-siden er oprettet på Mine websteder.</span><span class="sxs-lookup"><span data-stu-id="b8d93-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="b8d93-106">Følg disse trin for at give denne rettighed:</span><span class="sxs-lookup"><span data-stu-id="b8d93-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="b8d93-107">Klik på **brugerprofiler**i SharePoint Administration.</span><span class="sxs-lookup"><span data-stu-id="b8d93-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="b8d93-108">Klik på Administrer **brugertilladelser**i sektionen **Personer** .</span><span class="sxs-lookup"><span data-stu-id="b8d93-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="b8d93-109">Tilføj brugere, der har brug for tilladelser til at oprette deres websted Mine websteder.</span><span class="sxs-lookup"><span data-stu-id="b8d93-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="b8d93-110">Denne indstilling er som standard angivet til **Alle undtagen eksterne brugere**.</span><span class="sxs-lookup"><span data-stu-id="b8d93-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="b8d93-111">Når du har tilføjet brugeren, brugerne eller gruppen, skal du sørge for, at den tilføjede bruger, brugere eller gruppe er markeret, rulle til **afsnittet tilladelser** og derefter markere afkrydsningsfeltet ud for **Opret personligt websted (kræves til personlig lagring, nyhedsopdatering og fulgt indhold).**</span><span class="sxs-lookup"><span data-stu-id="b8d93-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="b8d93-112">Klik på **OK**, og få derefter brugeren til at gå til OneDrive-siden for at oprette webstedet.</span><span class="sxs-lookup"><span data-stu-id="b8d93-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
