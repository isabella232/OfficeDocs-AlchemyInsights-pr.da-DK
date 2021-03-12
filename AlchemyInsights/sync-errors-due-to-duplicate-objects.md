---
title: 902 (synkroniseringsfejl på grund af dublerede objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708056"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="e7636-102">Synkroniseringsfejl på grund af dublerede objekter</span><span class="sxs-lookup"><span data-stu-id="e7636-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="e7636-103">Du modtager muligvis en af følgende fejlmeddelelser, når katalogsynkronisering afsluttes i Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="e7636-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="e7636-104">Dette objekt kan ikke opdateres i Microsoft Online Services, fordi følgende attributter, der er knyttet til dette objekt, har værdier, der muligvis allerede er knyttet til et andet objekt i dit lokale katalog.</span><span class="sxs-lookup"><span data-stu-id="e7636-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="e7636-105">Der findes allerede et synkroniseret objekt med den samme proxyadresse i Microsoft Online Services-kataloget.</span><span class="sxs-lookup"><span data-stu-id="e7636-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="e7636-106">Dette objekt kan ikke opdateres, fordi følgende attributter, der er knyttet til dette objekt, har værdier, der måske allerede er knyttet til et andet objekt i dine lokale katalogtjenester: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="e7636-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="e7636-107">For at identificere og rette problemet skal du hente og køre Værktøjet til afhjælpning af [problemer med IdFix DirSync.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="e7636-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="e7636-108">Du kan finde flere oplysninger i [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="e7636-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
