---
title: Active Directory synkroniserer ikke
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697623"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="50bc8-102">Active Directory synkroniserer ikke</span><span class="sxs-lookup"><span data-stu-id="50bc8-102">Active Directory not syncing</span></span>

<span data-ttu-id="50bc8-103">Hvis du modtager synkroniseringsfejl, f. eks "ingen seneste synkronisering", eller opdager status for katalogsynkronisering i Office-administrations portalen, siger "senest synkroniseret for mere end 3 dage siden" det kan være, at AADConnect har forkerte indstillinger eller utilstrækkelige tilladelser til at udføre en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="50bc8-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="50bc8-104">Hvis du geninstallerer AADConnect ved hjælp af hurtig indstillinger, kan du muligvis løse problemet hurtigt:</span><span class="sxs-lookup"><span data-stu-id="50bc8-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="50bc8-105">[Hent den nyeste version af AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="50bc8-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="50bc8-106">[Følg vejledningen til hurtig installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="50bc8-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="50bc8-107">Du kan finde flere oplysninger om AADConnect-tjenestekonti under [Azure ad Connect: konti og tilladelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="50bc8-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
