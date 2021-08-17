---
title: Hvad du skal gøre, hvis Azure-funktioner ikke fungerer korrekt i Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117082"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Hvad du skal gøre, hvis Azure-funktioner ikke fungerer korrekt i Microsoft Edge

Microsoft Edge har [kendte problemer,](https://go.microsoft.com/fwlink/?linkid=2140608) der er relateret til sikkerhedszoner og kan påvirke, hvordan Azure-brugere logger på Windows Administration. Hvis du har problemer med at bruge Azure-funktioner med Microsoft Edge, kan du prøve følgende trin:

1. Søg efter Internetindstillinger i **menuen** **Start,** og vælg det.
2. Gå **til fanen** Sikkerhed i dialogboksen **Internetegenskaber.**
3. Vælg **zonen Websteder, der** er tillid til, og vælg **derefter knappen** Websteder.
4. I dialogboksen **Websteder, der** er tillid til skal du også tilføje URL-adressen til [https://login.microsoftonline.com](https://login.microsoftonline.com) gatewayen [https://login.live.com](https://login.live.com) og , og derefter vælge **Luk**.
5. I dialogboksen **Egenskaber for** internet skal du gå til fanen Beskyttelse **af personlige** oplysninger.
6. I sektionen **Blokering af pop op-vindue** skal du vælge **Indstillinger**. I den dialogboks, der åbnes, skal du også tilføje URL-adressen til din gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) og , og derefter vælge [https://login.live.com](https://login.live.com) **Luk**.
