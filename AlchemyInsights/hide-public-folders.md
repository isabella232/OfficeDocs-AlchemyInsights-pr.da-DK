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
# <a name="hide-public-folders"></a>Skjule offentlige mapper

**Sådan skjuler du hele træet til offentlige mapper:**

Brug trinnene i denne [artikel til](https://aka.ms/ControlPF) at skjule hele træet i offentlige mapper for selektive brugere eller alle brugere.

**Sådan skjuler du en bestemt offentlig mappe:**

1. Tilføje tilladelser for brugere, der skal have adgang til den offentlige mappe

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Fjern **brugerstandarden** fra **tilladelseslisten:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
