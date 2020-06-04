---
title: Opdatere DNS-poster for at holde dit websted hos din nuværende udbyder
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665754"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Opdatere DNS-poster for at holde dit websted hos din nuværende udbyder

1. I Microsoft 365 Administration skal **Setup**du gå til siden  >  [Installationsdomæner,](https://portal.office.com/adminportal/home#/Domains) og vælg det domæne, du bruger til dit websted, på listen over domæner.

2. Vælg **+ Ny brugerdefineret post,** og angiv følgende:

  - For **DNS-type** enter: **A (Adresse)**

  - Skriv følgende under **Værtsnavn eller Alias:****@**

  - For **IP-adresse**skal du skrive den statiske IP-adresse for dit websted, hvor det aktuelt er hostet (f.eks. 172.16.140.1).

    Dette skal være en *statisk* IP-adresse til webstedet, ikke en *dynamisk* IP-adresse. Check med websted, hvor dit websted er hostet for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.

3. Vælg **Gem**.

Derudover kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.
  
1. Vælg **+ Ny brugerdefineret post,** og angiv følgende:

  - For **DNS-type** skal du indtaste: **CNAME (Alias)**

  - Skriv følgende under **Værtsnavn eller Alias:** **www:**

  - For **point til adresse**skal du skrive det fuldt kvalificerede domænenavn (FQDN) for dit websted (f.eks. contoso.com).

2. Vælg **Gem**.
