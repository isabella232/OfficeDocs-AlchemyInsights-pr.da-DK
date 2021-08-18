---
title: Overvåg betinget adgang i Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327551"
---
# <a name="monitor-intune-conditional-access"></a>Overvåg betinget adgang i Intune

Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav. For at løse problemet anbefaler vi en eller flere af følgende løsninger:

1. Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til Firmaportal-appen og kontrollere, at den vises i Firmaportal. Hvis den ikke gør det, skal brugeren tilmelde enheden.
1. I Azure-portalen skal du gå til Overholdelse af enhed i **Intune**  >  . 
1. Hvis du vil have vist din enheds overholdelsesrapport for at bekræfte, at brugerens enhed er markeret som kompatibel, **skal** du klikke på Enhedsoverholdelse under **Skærm**.
1. I Azure-portalen skal du gå til Overholdelse af enhed i **Intune**  >  . Klik **på Politikker** under **Administrer.** Kontrollér, at en profil er tildelt til brugerens enhed på listen over politikker for overholdelse af regler og standarder. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.
1. Rediger brugerens betingede adgangstildeling.
1. I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune**, vælge en politik på listen  >    >  og klikke **på Brugere og grupper**.
1. Hvis du vil målrette en bestemt politik på en person, skal du føje dem til **listen Medtag.** For at sikre, at en person udelades fra politikken, kan du føje dem til **listen Udelad.**

**Nyttige links:**

- [Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Fejlfindingspolitik](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Overvågning af overholdelse af Intune-enhed](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Bemærk!** Disse trin er kun nyttige i forbindelse med fejlfinding Azure Active Directory funktionen Betinget adgang. Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang Exchange politikken. Du kan finde Exchange om administration af enheder [**her**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
