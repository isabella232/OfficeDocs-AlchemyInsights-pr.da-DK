---
title: Fejlfinding af adgang nægtede meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939877"
---
# <a name="troubleshoot-access-denied-messages"></a>Fejlfinding af adgang nægtede meddelelser

Hvis nogen fik meddelelsen "Adgang nægtet" til en delt mappe i SharePoint, har administratoren af gruppen af websteder muligvis aktiveret "Låst tilstand for brugere med tilladelsen Begrænset adgang". Sådan slår du dette fra: 
  
1. Gå til webstedet, klik på ikonet Indstillinger, og klik derefter **på** Indstillinger .
    
2. Under Administration **af gruppe af websteder skal** du klikke på Funktioner for grupper af **websteder.**
    
3. Ud for **Låst tilstand for brugere med tilladelsen Begrænset adgang skal du klikke** på **Deaktiver.**
    
Meddelelsen Adgang nægtet kan også forekomme for delte mapper, hvis webstedet er et publiceringswebsted. Du kan få mere at vide [under Adgang nægtet ved adgang til en delt mappe](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Hvis en person fik meddelelsen "Adgang nægtet", når han eller hun forsøger at få vist anmodninger om adgang, skal brugeren tilføjes som administrator for en gruppe af websteder eller som medlem af gruppen Ejere for webstedet. Du kan få mere at vide [under Listen Adgang nægtet adgang til anmodninger](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Hvis en bruger fik en meddelelse med "Adgang nægtet", efter at han/hun blev fjernet fra Active Directory i det lokale miljø og derefter tilføjet igen, skal du se Adgang nægtet, når en brugerkonto synkroniseres med [en Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

