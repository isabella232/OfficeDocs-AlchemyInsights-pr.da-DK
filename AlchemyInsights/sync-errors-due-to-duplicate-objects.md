---
title: 902 (Synkroniseringsfejl på grund af dublerede objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767113"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="8b423-102">Synkroniseringsfejl på grund af dublerede objekter</span><span class="sxs-lookup"><span data-stu-id="8b423-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="8b423-103">Du kan få vist en af følgende fejlmeddelelser, når katalogsynkroniseringen afsluttes i Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="8b423-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="8b423-104">Dette objekt kan ikke opdateres i Microsoft Online Services, fordi følgende attributter, der er knyttet til dette objekt, har værdier, der muligvis allerede er knyttet til et andet objekt i den lokale mappe.</span><span class="sxs-lookup"><span data-stu-id="8b423-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="8b423-105">Der findes allerede et synkroniseret objekt med den samme proxyadresse i mappen Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="8b423-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="8b423-106">Dette objekt kan ikke opdateres, fordi følgende attributter, der er knyttet til dette objekt, har værdier, der allerede er knyttet til et andet objekt i de lokale katalogtjenester: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8b423-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="8b423-107">Du kan identificere og løse problemet ved at hente og køre [IdFix DirSync-fejloprydningsværktøjet](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="8b423-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="8b423-108">Yderligere oplysninger finder du i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="8b423-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
