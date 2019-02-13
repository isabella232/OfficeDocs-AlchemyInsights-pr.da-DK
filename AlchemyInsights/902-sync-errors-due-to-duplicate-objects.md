---
title: 902 (synkroniseringsfejl skyldes duplikerede objekter)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919866"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d242a-102">Synkroniseringsfejl skyldes duplikerede objekter</span><span class="sxs-lookup"><span data-stu-id="d242a-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d242a-103">Du modtager muligvis en af følgende fejlmeddelelser, når directory-synkroniseringen er fuldført:</span><span class="sxs-lookup"><span data-stu-id="d242a-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="d242a-104">Du kan ikke opdatere dette objekt i Microsoft Online Services, fordi følgende attributter, der er tilknyttet dette objekt har værdier, der allerede er knyttet til et andet objekt i den lokale mappe.</span><span class="sxs-lookup"><span data-stu-id="d242a-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="d242a-105">Der findes allerede et objekt, der er synkroniseret med den samme proxyadresse i din Microsoft Online Services-mappe.</span><span class="sxs-lookup"><span data-stu-id="d242a-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="d242a-106">Kan ikke opdatere dette objekt, fordi følgende attributter, der er tilknyttet dette objekt har værdier, der allerede er knyttet til et andet objekt i din lokale katalogtjenester: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="d242a-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="d242a-107">Identificere og løse problemet ved at hente og køre [Værktøj til afhjælpning af IdFix DirSync fejl](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="d242a-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="d242a-108">Yderligere oplysninger finder du under [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="d242a-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

