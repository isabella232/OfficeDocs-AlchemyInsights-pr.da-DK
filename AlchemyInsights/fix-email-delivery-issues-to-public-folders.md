---
title: Løs problemer med levering af mail til mailaktiverede offentlige mapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068806"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løs problemer med levering af mail til mailaktiverede offentlige mapper

Hvis eksterne afsendere ikke kan sende meddelelser til dine mailaktiverede offentlige mapper, og afsenderne modtager fejlen: kunne ikke findes **(550 5.4.1),** skal du bekræfte, at maildomænet for den offentlige mappe er konfigureret som et internt relædomæne i stedet for et autoritativt domæne:

1. Åbn [Exchange Administration (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Gå til **Mailflow** \> **Accepterede domæner**, vælg det accepterede domæne, og klik derefter på **Rediger**.

3. På siden med egenskaber, der åbnes, skal du ændre værdien til Intern videresendelse, hvis domænetypen er angivet til **Autoritativ,** **og** derefter klikke på **Gem**.

Hvis eksterne afsendere modtager fejlen, du ikke har tilladelse **til (550 5.7.13),** skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for at få vist tilladelser for anonyme brugere i den offentlige mappe:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` F.eks. `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Hvis du vil tillade eksterne brugere at sende mails til denne offentlige mappe, skal du tilføje CreateItems-adgang direkte til brugeren Anonym. F.eks. `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
