---
title: Rediger Microsoft Edge ved hjælp af datamappevariabler i stedet for hard-coded stier
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035281"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Rediger Microsoft Edge ved hjælp af datamappevariabler i stedet for hard-coded stier

Hvis du f.eks. i Windows vil gemme profildataene under en brugers lokale programdata i stedet for på standardplaceringen, skal du angive *politikken UserDataDir* til **${local_app_data}\Edge\Profile.**

Du kan finde flere oplysninger i [Opret Microsoft Edge-variabler for brugerdatamapper.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)