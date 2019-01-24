---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464116"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder

1. Vælg det domæne, du bruger til dit websted, og vælg derefter **DNS-indstillingerne** i ruden management på listen over domæner, på siden [domæner](https://portal.office.com/adminportal/home#/Domains) . 
    
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
    

