---
title: OneDrive for Business Web OneDrive omdirigerer til Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776373"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="5f543-102">Omdirigeret til Delve, når du har klikket på OneDrive</span><span class="sxs-lookup"><span data-stu-id="5f543-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="5f543-103">Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="5f543-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="5f543-104">For at løse dette problem skal administratoren give brugerne tilladelse til at oprette webstedet mit websted.</span><span class="sxs-lookup"><span data-stu-id="5f543-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="5f543-105">Dette skyldes, at OneDrive for Business-siden er oprettet på mine websteder.</span><span class="sxs-lookup"><span data-stu-id="5f543-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="5f543-106">Hvis du vil tildele denne rettighed, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="5f543-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="5f543-107">I SharePoint administration skal du klikke på **Brugerprofiler**.</span><span class="sxs-lookup"><span data-stu-id="5f543-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="5f543-108">Klik på **Administrer brugertilladelser**i sektionen **personer** .</span><span class="sxs-lookup"><span data-stu-id="5f543-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="5f543-109">Tilføj brugere, der skal have tilladelse til at oprette deres websted for mit websted.</span><span class="sxs-lookup"><span data-stu-id="5f543-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="5f543-110">Denne indstilling er som standard angivet til **alle undtagen eksterne brugere**.</span><span class="sxs-lookup"><span data-stu-id="5f543-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="5f543-111">Når du har tilføjet brugeren, brugerne eller gruppen, skal du sørge for, at den tilføjede bruger, brugerne eller gruppen er markeret, rulle ned til sektionen **tilladelser** og derefter markere afkrydsningsfeltet ud for **Opret et personligt websted (påkrævet til personligt lager, nyhedsstrøm og følge af indhold)**.</span><span class="sxs-lookup"><span data-stu-id="5f543-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="5f543-112">Klik på **OK**, og få brugeren til at gå til siden OneDrive for at oprette webstedet.</span><span class="sxs-lookup"><span data-stu-id="5f543-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
