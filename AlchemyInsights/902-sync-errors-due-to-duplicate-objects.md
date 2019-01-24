---
title: 902 (synkroniseringsfejl skyldes duplikerede objekter)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464589"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="655d0-102">Synkroniseringsfejl skyldes duplikerede objekter</span><span class="sxs-lookup"><span data-stu-id="655d0-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="655d0-103">Du modtager muligvis en af følgende fejlmeddelelser, når directory-synkroniseringen er fuldført:</span><span class="sxs-lookup"><span data-stu-id="655d0-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="655d0-104">Du kan ikke opdatere dette objekt i Microsoft Online Services, fordi følgende attributter, der er tilknyttet dette objekt har værdier, der allerede er knyttet til et andet objekt i den lokale mappe.</span><span class="sxs-lookup"><span data-stu-id="655d0-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="655d0-105">Der findes allerede et objekt, der er synkroniseret med den samme proxyadresse i din Microsoft Online Services-mappe.</span><span class="sxs-lookup"><span data-stu-id="655d0-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="655d0-106">Kan ikke opdatere dette objekt, fordi følgende attributter, der er tilknyttet dette objekt har værdier, der allerede er knyttet til et andet objekt i din lokale katalogtjenester: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="655d0-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="655d0-107">Identificere og løse problemet ved at hente og køre [Værktøj til afhjælpning af IdFix DirSync fejl](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="655d0-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="655d0-108">Yderligere oplysninger finder du under [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="655d0-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

