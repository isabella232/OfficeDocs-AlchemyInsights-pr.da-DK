---
title: Fejlfinding i forbindelse med adgang nægtet-meddelelser
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050699"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding i forbindelse med adgang nægtet-meddelelser

Hvis en person har fået meddelelsen "adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "begrænset adgang til bruger tilladelses låsning". Sådan deaktiverer du dette: 
  
1. Gå til webstedet, klik på ikonet indstillinger, og klik derefter på **Indstillinger for websted**.
    
2. Klik på **funktioner for gruppen af**websteder under **administration af gruppe af**websteder.
    
3. Klik på **Deaktiver**ud for **tilstanden begrænset adgang til bruger tilladelse**.
    
Der kan også forekomme en meddelelse om adgang nægtet for delte mapper, hvis webstedet er et udgivelseswebsted. Du kan finde flere oplysninger under [adgang nægtet, når du får adgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Hvis en person har fået meddelelsen "adgang nægtet", når du forsøger at få vist anmodninger om adgang, skal brugeren tilføjes enten som administrator af en gruppe af websteder eller som medlem af Ejergruppen for webstedet. Du kan finde flere oplysninger under [adgang nægtet på listen over anmodninger om adgang](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Hvis en bruger har fået meddelelsen "adgang nægtet", efter at de blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, [skal du se adgang nægtet, når en brugerkonto er synkroniseret med Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

