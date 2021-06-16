---
title: Active Directory synkroniseres ikke
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930969"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="7efa6-102">Active Directory synkroniseres ikke</span><span class="sxs-lookup"><span data-stu-id="7efa6-102">Active Directory not syncing</span></span>

<span data-ttu-id="7efa6-103">Hvis du modtager synkroniseringsfejl, f.eks. "ingen seneste synkronisering", eller bemærker status for katalogsynkronisering i Office-administrationsportalen, hvor der står "Senest synkroniseret for mere end 3 dage siden", kan det være, at AADConnect har forkerte indstillinger eller utilstrækkelige tilladelser til at udføre en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="7efa6-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="7efa6-104">Hvis du geninstallerer AADConnect ved hjælp af hurtig konfiguration, kan problemet muligvis løses hurtigt:</span><span class="sxs-lookup"><span data-stu-id="7efa6-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="7efa6-105">[Download den nyeste version af AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="7efa6-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="7efa6-106">[Følg vejledningen for hurtig installation.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="7efa6-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="7efa6-107">Azure AD Connect skal installeres på Windows Server 2012 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="7efa6-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="7efa6-108">Denne server skal være tilknyttet et domæne, og det kan være domænecontroller eller en medlemsserver.</span><span class="sxs-lookup"><span data-stu-id="7efa6-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="7efa6-109">Du kan se en komplet liste over Forbind og forudsætninger for Azure AD ved at gennemgå [Forudsætninger for Azure AD Forbind.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="7efa6-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="7efa6-110">Du kan finde flere oplysninger om AADConnect-tjenestekonti [i Azure AD Forbind: Konti og tilladelser](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="7efa6-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
