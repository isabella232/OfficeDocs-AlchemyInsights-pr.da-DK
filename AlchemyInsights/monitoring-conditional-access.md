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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708668"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af betinget adgang til Exchange

Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav. For at løse dette anbefaler vi en eller flere af følgende løsninger:

- Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til appen Firmaportal og kontrollere, at den vises i firmaportalen. Hvis det ikke er muligt, skal brugeren tilmelde enheden.
- I Azure-portalen skal du gå til Intune > overholdelse af enhed. Klik på Enhedsoverholdelse under Skærm. Få vist overholdelsesrapporten for enheden for at bekræfte, at brugerens enhed er markeret som kompatibel.
- I Azure-portalen skal du gå til Intune > overholdelse af enhed. Klik på Politikker under Administrer. Kontrollér, at der er tildelt en profil til brugerens enhed på listen over politikker for overholdelse af regler og standarder. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.
- Rediger brugerens betingede adgangstildeling.

1. I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune.**  >    >  
2. Vælg en politik på listen.
3. Klik på Brugere og grupper.
4. Hvis du vil målrette en bestemt politik mod en person, kan du føje dem til listen Medtag. For at sikre, at en person udelades fra politikken, kan du føje dem til listen Udelad.

Nyttige links:

[Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindingspolitik](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Overvågning af overholdelse af intune-enhed](https://docs.microsoft.com/intune/compliance-policy-monitor)

Bemærk! Disse trin er kun nyttige ved fejlfinding af funktionen Betinget adgang til Azure Active Directory. Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang med Exchange-politik. Du kan finde flere oplysninger om administration af exchange-enheder [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
