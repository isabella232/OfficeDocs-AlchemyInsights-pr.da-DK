---
title: Overvågning af adgangsstyring
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538735"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af adgangsstyring for Exchange

Brugere, der er målrettet med adgangsstyring modtager en besked via e-mail, hvis de ikke opfylder adgangskravene til din organisation. Du kan løse, anbefaler vi en eller flere af følgende løsninger:
  
- Hvis enheden antages at være tilmeldt, oplyse brugeren om at gå til firmaets Portal-app, og Kontroller, at det vises i firmaets Portal. Hvis det ikke er tilfældet, skal brugeren registrere enheden.
    
- Gå til portalen Azure **Intune \> enhed overholdelse af**. Klik på **enhed overholdelse**under **skærm** . Få vist rapporten til at kontrollere, at brugerens enhed er markeret som værende kompatibel enhed overholdes. 
    
- Gå til portalen Azure **Intune \> enhed overholdelse af**. Klik på **politikker**under **Administrer**. Kontroller, der er tildelt en profil til brugerens enhed på listen over overholdelse af politikker. Hvis der er tildelt nogen profil, derefter kunne Intune ikke bekræfte enhedens overholdelsesstatus. 
    
- Rediger brugerens adgangsstyring tildeling.
    
1. Gå til portalen Azure **Intune \> adgangsstyring \> politikker for**
    
2. Vælg en politik på listen
    
3. Klik på **brugere og grupper**
    
4. Hvis du vil målrette en bestemt politik på en person, kan du tilføje dem på **listen** . For at sikre, at en person, der er udeladt fra politikken, kan du føje dem til listen **udelades** . 
    
Læs mere: [Sådan skærm adgangsstyring enheder](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

