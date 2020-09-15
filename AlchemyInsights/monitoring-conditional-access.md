---
title: Overvågning af betinget adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702897"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af betinget adgang for Exchange

Brugere, der er målrettet med betinget adgang, modtager en mailbesked, hvis de ikke opfylder din organisations adgangs krav. Vi anbefaler en eller flere af følgende løsninger for at løse problemet:
  
- Hvis enheden anses for at være tilmeldt, skal du bede brugeren om at gå til appen Firmaportal og bekræfte, at den vises på Firmaportalen. Hvis det ikke er den, skal brugeren tilmelde enheden.
    
- I Azure-portalen skal du gå til **Intune \> Device Compliance**. Klik på **enheds overholdelse**under **overvågning** . Se din enheds kompatibilitetsrapport for at bekræfte, at brugerens enhed er markeret som kompatibel. 
    
- I Azure-portalen skal du gå til **Intune \> Device Compliance**. Under **Administrer**skal du klikke på **politikker**. På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens overholdelses status. 
    
- Redigere brugerens betingede adgangs tildeling.
    
1. I Azure-portalen skal du gå til ** \> \> politikker for betinget adgang til Intune**
    
2. Vælg en politik på listen
    
3. Klik på **brugere og grupper**
    
4. Hvis du vil målrette en bestemt politik til en anden, skal du føje dem til listen **Medtag** . Hvis du vil sikre dig, at en person udelades fra politikken, skal du føje dem til listen **Udelad** . 
    
Læs mere: [Sådan overvåges enheder med betinget adgang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

