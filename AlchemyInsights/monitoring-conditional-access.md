---
title: Overvågning af betinget adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713712"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af betinget adgang til Exchange

Brugere, der er målrettet mod betinget adgang, modtager en e-mail med en meddelelse, hvis de ikke opfylder organisationens adgangskrav. Vi anbefaler en eller flere af følgende løsninger for at løse problemet:
  
- Hvis enheden formodes at være tilmeldt, skal du råde brugeren til at gå til appen Firmaportal og bekræfte, at den vises i virksomhedsportalen. Hvis det ikke er tilfældet, skal brugeren tilmelde enheden.
    
- I Azure-portalen skal du gå til **Intune \> Device Compliance**. Klik på **Enhedsoverholdelse af enhed**under **Skærm** . Få vist rapporten om overholdelse af enheden for at kontrollere, at brugerens enhed er markeret som kompatibel. 
    
- I Azure-portalen skal du gå til **Intune \> Device Compliance**. Klik på **Politikker**under **Administrer**. På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed. Hvis der ikke er tildelt en profil, kan Intune ikke bekræfte enhedens overholdelsesstatus. 
    
- Rediger brugerens tildeling med betinget adgang.
    
1. På Azure-portalen skal du gå til **Intune-politikker \> for \> betinget adgang**
    
2. Vælg en politik på listen
    
3. Klik på **Brugere og grupper**
    
4. Hvis du vil målrette mod en bestemt politik mod en person, skal du føje dem til listen **Medtag.** Hvis du vil sikre, at en person udelades fra politikken, skal du føje vedkommende til listen **Udeluk.** 
    
Læs mere: [Sådan overvåges Betingede Access-enheder](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

