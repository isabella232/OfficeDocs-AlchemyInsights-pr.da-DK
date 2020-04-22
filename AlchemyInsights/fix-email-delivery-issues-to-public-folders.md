---
title: Løs problemer med levering af mail til mailaktiverede offentlige mapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716346"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løs problemer med levering af mail til mailaktiverede offentlige mapper

Hvis eksterne afsendere ikke kan sende meddelelser til dine e-mail-aktiverede offentlige mapper, og afsenderne får vist fejlen: **Blev ikke fundet (550 5.4.1),** skal du kontrollere, at maildomænet for den offentlige mappe er konfigureret som et internt relædomæne i stedet for et autoritativt domæne:

1. Åbn [Exchange Administration (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **Mailflow** \> **Accepterede domæner**, vælg det accepterede domæne, og klik derefter på **Rediger**.

3. Hvis domænetypen er angivet til **Autoritativ**på siden egenskaber, der åbnes, skal du ændre værdien til **Internt relæ** og derefter klikke på **Gem**.

Hvis eksterne afsendere får vist den **fejl, du ikke har tilladelse til (550 5.7.13),** skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for at få vist tilladelserne for anonyme brugere i den offentlige mappe:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`F.eks.

Hvis du vil give eksterne brugere tilladelse til at sende mail til denne offentlige mappe, skal du føje adgangsrettigheden CreateItems til brugeren Anonym. `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`F.eks.
