---
title: Hvad du skal gøre, hvis Azure-funktionerne ikke fungerer korrekt i Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583309"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Hvad du skal gøre, hvis Azure-funktionerne ikke fungerer korrekt i Microsoft Edge

Microsoft Edge har [kendte problemer](https://go.microsoft.com/fwlink/?linkid=2140608) , der er relateret til sikkerhedszoner og kan påvirke, hvordan Azure-brugere logger på Windows administration. Hvis du har problemer med at bruge Azure-funktioner med Microsoft Edge, kan du prøve følgende trin:

1. I menuen **Start** skal du søge efter **Internet indstillinger** og vælge den.
2. Gå til fanen **sikkerhed** i dialogboksen **Egenskaber for internettet** .
3. Vælg zonen **websteder, du har tillid** til, og vælg derefter knappen **websteder** .
4. I dialogboksen websteder, du **har tillid til** , skal du tilføje din gateway-URL samt [https://login.microsoftonline.com](https://login.microsoftonline.com) og [https://login.live.com](https://login.live.com) derefter vælge **Luk**.
5. Gå til fanen **beskyttelse af personlige oplysninger** i dialogboksen **Egenskaber for internettet** .
6. Vælg **Indstillinger** i sektionen **blokering af pop op-vinduer** . I den dialogboks, der åbnes, skal du tilføje din gateway-URL samt [https://login.microsoftonline.com](https://login.microsoftonline.com) og [https://login.live.com](https://login.live.com) derefter vælge **Luk**.
