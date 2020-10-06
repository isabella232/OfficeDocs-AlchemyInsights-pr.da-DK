---
title: Løs problemer med levering af mail til offentlige mapper, der er aktiveret til mail
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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366458"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løs problemer med levering af mail til offentlige mapper, der er aktiveret til mail

Hvis eksterne afsendere ikke kan sende meddelelser til dine mailaktiverede offentlige mapper, og afsenderen modtager fejlen: **blev ikke fundet (550 5.4.1)**, skal du kontrollere, at mail domænet for den offentlige mappe er konfigureret som et internt Relay-domæne i stedet for et autoritativt domæne:

1. Åbn [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **mail flow** \> **accepterede domæner**, Vælg det accepterede domæne, og klik derefter på **Rediger**.

3. På siden med egenskaber, der åbnes, hvis domæne typen er angivet til **autoritativ**, skal du ændre værdien til **intern relæ** og derefter klikke på **Gem**.

Hvis eksterne afsendere modtager den fejl, **du ikke har tilladelse (550 5.7.13)**, skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for at få vist tilladelserne for anonyme brugere i den offentlige mappe:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Hvis du vil tillade, at eksterne brugere sender mails til denne offentlige mappe, skal du føje CreateItems adgang til anonyme brugere. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
