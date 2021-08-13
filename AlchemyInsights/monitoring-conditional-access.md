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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975095"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af betinget adgang for Exchange

Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav. For at løse problemet anbefaler vi en eller flere af følgende løsninger:

- Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til Firmaportal-appen og kontrollere, at den vises i Firmaportal. Hvis den ikke gør det, skal brugeren tilmelde enheden.
- I Azure-portalen skal du gå til Intune > overholdelse af enhed. Klik på Enhedsoverholdelse under Skærm. Få vist overholdelsesrapporten for enheden for at bekræfte, at brugerens enhed er markeret som kompatibel.
- I Azure-portalen skal du gå til Intune > overholdelse af enhed. Klik på Politikker under Administrer. Kontrollér, at en profil er tildelt til brugerens enhed på listen over politikker for overholdelse af regler og standarder. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.
- Rediger brugerens betingede adgangstildeling.

1. I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune**  >    >  .
2. Vælg en politik på listen.
3. Klik på Brugere og grupper.
4. Hvis du vil målrette en bestemt politik på en person, skal du føje dem til listen Medtag. For at sikre, at en person udelades fra politikken, kan du føje dem til listen Udelad.

Nyttige links:

[Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindingspolitik](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Overvågning af overholdelse af Intune-enhed](https://docs.microsoft.com/intune/compliance-policy-monitor)

Bemærk! Disse trin er kun nyttige i forbindelse med fejlfinding Azure Active Directory funktionen Betinget adgang. Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang Exchange politikken. Du kan finde Exchange om administration af enheder [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
