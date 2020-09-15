---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699513"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Opdater DNS-poster for at beholde dit websted hos din nuværende udbyder

1. I Microsoft 365 administration skal du gå til siden **konfigurations**  >  [domæner](https://portal.office.com/adminportal/home#/Domains) og vælge det domæne, du vil bruge til dit websted, på listen over domæner.

2. Vælg **+ ny brugerdefineret post** , og angiv følgende:

  - For **DNS-type** skal du skrive: **A (adresse)**

  - For **værtsnavn eller alias**skal du skrive følgende: **@**

  - For **IP-adresse**skal du skrive den statiske IP-adresse på dit websted, hvor den er hostet (f. eks. 172.16.140.1).

    Det skal være en  *statisk*  IP-adresse for webstedet, ikke en  *dynamisk*  IP-adresse. Kontrollér med det websted, hvor dit websted er hosted, for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.

3. Vælg **Gem**.

Derudover kan du oprette en CNAME-post for at hjælpe kunder med at finde dit websted.
  
1. Vælg **+ ny brugerdefineret post** , og angiv følgende:

  - For **DNS-type** skal du skrive: **CNAME (alias)**

  - For **værtsnavn eller alias**skal du skrive følgende: **www**

  - For **Point to Address skal du**skrive det fulde domænenavn (FQDN) til dit websted (f. eks. contoso.com).

2. Vælg **Gem**.
