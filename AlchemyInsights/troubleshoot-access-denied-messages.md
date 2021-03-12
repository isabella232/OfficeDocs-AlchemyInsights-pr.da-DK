---
title: Fejlfinding af adgang nægtet meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704888"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding af adgang nægtet meddelelser

Hvis nogen fik meddelelsen "Adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "Låst tilstand for brugere med tilladelsen Begrænset adgang". Sådan slår du dette fra: 
  
1. Gå til webstedet, klik på ikonet Indstillinger, og klik derefter på **Indstillinger for websted.**
    
2. Klik **på Funktioner for grupper af** websteder under Administration af gruppe af **websteder.**
    
3. Ud for **låst tilstand for brugere med tilladelsen Begrænset adgang skal du** klikke på **Deaktiver.**
    
En Adgang nægtet-meddelelse kan også forekomme for delte mapper, hvis webstedet er et publiceringswebsted. Du kan få mere at vide [under Adgang nægtet, når du åbner en delt mappe.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Hvis en person fik meddelelsen "Adgang nægtet", når han eller hun forsøger at få vist anmodninger om adgang, skal brugeren tilføjes som administrator for en gruppe af websteder eller som medlem af gruppen Ejere for webstedet. Du kan finde flere oplysninger på [listen Anmodninger om adgang nægtet adgang.](https://go.microsoft.com/fwlink/?linkid=2004220)
  
Hvis en bruger fik meddelelsen "Adgang nægtet", efter brugeren blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, skal du se Adgang nægtet, når en brugerkonto synkroniseres med [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

