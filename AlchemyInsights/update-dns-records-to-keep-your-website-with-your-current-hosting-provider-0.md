---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665754"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder

1. Gå til **installation**i Microsoft 365 admin center, > [domæner](https://portal.office.com/adminportal/home#/Domains) side, og vælg det domæne, du bruger til dit websted på listen over domæner.

2. Vælg **+ ny brugerdefineret post** , og Skriv følgende:

  - Angiv for **DNS-type** : **(adresse)**

  - For **Host-navn eller Alias**, skal du skrive følgende:**@**

  - Skriv den statiske IP-adresse på dit websted, hvor den aktuelt er placeret (f.eks, 172.16.140.1) til **IP-adresse**.

    Det skal være en *statisk* IP-adresse for webstedet, ikke en *dynamisk* IP-adresse. Spørg websted, hvor webstedet er vært for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.

3. Vælg **Gem**.

Desuden kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.
  
1. Vælg **+ ny brugerdefineret post** , og Skriv følgende:

  - Angiv for **DNS-type** : **CNAME (Alias)**

  - **Host-navn eller Alias**, skal du skrive følgende: **www**

  - Skriv det fuldt kvalificerede domænenavn (FQDN) på dit websted (for eksempel contoso.com) for **peger på adresse**.

2. Vælg **Gem**.
