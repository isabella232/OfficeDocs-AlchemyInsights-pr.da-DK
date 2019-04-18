---
title: Løse problemer med e-mail-levering til postaktiverede offentlige mapper
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910587"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Løse problemer med e-mail-levering til postaktiverede offentlige mapper

Hvis eksterne afsendere kan ikke sende meddelelser til dine offentlige mapper med e-mail-aktiveret og afsendere modtager fejl: **ikke fundet (550 5.4.1)**, kontrollere e-mail-domæne til den offentlige mappe er konfigureret som en intern relay domæne i stedet for en autoritative domæne:

1. Åbn [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Gå til **Poststrøm** \> **godkendte domæner**, Vælg det accepterede domæne, og klik derefter på **Rediger**.

3. Side, der åbnes, hvis domænetype er indstillet til **Authoritative**i egenskaberne, ændre værdien til **interne relay** , og klik derefter på **Gem**.

Hvis eksterne afsendere modtager fejlen **du ikke har tilladelse (550 5.7.13)**, skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) til at få vist tilladelser for anonyme brugere i den offentlige mappe:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

For at give eksterne brugere at sende e-mail til denne offentlige mappe, kan du tilføje adgang CreateItems ret til brugertypen Anonym. For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
