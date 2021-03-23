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
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="6e30f-102">Rediger Microsoft Edge ved hjælp af datamappevariabler i stedet for hard-coded stier</span><span class="sxs-lookup"><span data-stu-id="6e30f-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="6e30f-103">Hvis du f.eks. i Windows vil gemme profildataene under en brugers lokale programdata i stedet for på standardplaceringen, skal du angive *politikken UserDataDir* til **${local_app_data}\Edge\Profile.**</span><span class="sxs-lookup"><span data-stu-id="6e30f-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="6e30f-104">Du kan finde flere oplysninger i [Opret Microsoft Edge-variabler for brugerdatamapper.](https://docs.microsoft.com/deployedge/microsoft-edge-policies)</span><span class="sxs-lookup"><span data-stu-id="6e30f-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>