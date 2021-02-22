---
title: Skjule offentlige mapper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315338"
---
# <a name="hide-public-folders"></a><span data-ttu-id="518b1-102">Skjule offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="518b1-102">Hide public folders</span></span>

<span data-ttu-id="518b1-103">**Sådan skjuler du hele træet til offentlige mapper:**</span><span class="sxs-lookup"><span data-stu-id="518b1-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="518b1-104">Brug trinnene i denne [artikel til](https://aka.ms/ControlPF) at skjule hele træet i offentlige mapper for selektive brugere eller alle brugere.</span><span class="sxs-lookup"><span data-stu-id="518b1-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="518b1-105">**Sådan skjuler du en bestemt offentlig mappe:**</span><span class="sxs-lookup"><span data-stu-id="518b1-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="518b1-106">Tilføje tilladelser for brugere, der skal have adgang til den offentlige mappe</span><span class="sxs-lookup"><span data-stu-id="518b1-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="518b1-107">Fjern **brugerstandarden** fra **tilladelseslisten:**</span><span class="sxs-lookup"><span data-stu-id="518b1-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
