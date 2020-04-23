---
title: Fejlfinding i forbindelse med meddelelser, der er nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759794"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding i forbindelse med meddelelser, der er nægtet adgang

Hvis nogen har fået meddelelsen "Adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "Låsning af begrænset adgang til brugertilladelse". Sådan slår du dette fra: 
  
1. Gå til webstedet, klik på ikonet Indstillinger, og klik derefter på **Indstillinger for websted**.
    
2. Klik på Funktioner for **gruppe af websteder under**Administration af gruppe **af**websteder .
    
3. Klik på **Deaktiver**ud for **låsning af begrænset adgangstilladelse**.
    
Der kan også forekomme en meddelelse nægtet adgang for delte mapper, hvis webstedet er et publiceringswebsted. Du kan finde oplysninger under [Access Denied, når du får adgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Hvis en person fik meddelelsen "Adgang nægtet", når vedkommende forsøger at få vist adgangsanmodninger, skal brugeren tilføjes som enten administrator af en gruppe af websteder eller medlem af gruppen Ejere for webstedet. Du kan finde flere oplysninger på [listen Access Denied to Access Requests](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Hvis en bruger fik meddelelsen "Adgang nægtet", efter at vedkommende blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, skal du se [Adgang nægtet, når en brugerkonto synkroniseres med Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

