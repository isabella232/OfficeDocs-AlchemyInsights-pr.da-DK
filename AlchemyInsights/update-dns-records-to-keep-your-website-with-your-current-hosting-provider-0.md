---
title: Opdatere DNS-poster for at beholde dit websted hos din nuværende hostingudbyder
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007676"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Opdatere DNS-poster for at beholde dit websted hos din nuværende hostingudbyder

1. I Microsoft 365 Administration skal du gå til siden **Konfiguration** af domæner og vælge det domæne, du bruger til dit websted, på  >  [](https://admin.microsoft.com/Adminportal#/Domains) listen over domæner.

2. Vælg **+ Ny brugerdefineret** post, og angiv følgende:

  - Til **DNS-type** skal du **skrive: A (adresse)**

  - For **Værtsnavn eller Alias** skal du skrive følgende: **@**

  - For **IP-adresse** skal du skrive den statiske IP-adresse til dit websted, hvor det aktuelt hostes (f.eks. 172.16.140.1).

    Dette skal være en  *statisk*  IP-adresse til webstedet, ikke en  *dynamisk*  IP-adresse. Kontakt webstedet, hvor dit websted hostes, for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.

3. Vælg **Gem**.

Desuden kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.
  
1. Vælg **+ Ny brugerdefineret** post, og angiv følgende:

  - Til **DNS-type** skal du **angive: CNAME (Alias)**

  - For **Værtsnavn eller Alias** skal du skrive følgende: **www**

  - For **Peger på adresse** skal du skrive det fulde domænenavn for dit websted (f.eks. contoso.com).

2. Vælg **Gem**.
