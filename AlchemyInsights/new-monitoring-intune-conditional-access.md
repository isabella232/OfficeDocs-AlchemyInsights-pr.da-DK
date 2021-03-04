---
title: Overvåg Betinget adgang i Intune
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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427428"
---
# <a name="monitor-intune-conditional-access"></a>Overvåg Betinget adgang i Intune

Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav. For at løse dette anbefaler vi en eller flere af følgende løsninger:

1. Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til appen Firmaportal og kontrollere, at den vises i firmaportalen. Hvis den ikke gør det, skal brugeren tilmelde enheden.
1. I Azure-portalen skal du gå til **overholdelse af regler og standarder for Intune-enheder.**  >   
1. Hvis du vil have vist rapporten om overholdelse af regler og standarder for enheden for at bekræfte, at brugerens enhed er markeret som kompatibel, **skal** du klikke på Enhedsoverholdelse under **Skærm.**
1. I Azure-portalen skal du gå til **overholdelse af regler og standarder for Intune-enheder.**  >   Klik **på Politikker** under **Administrer.** Kontrollér, at der er tildelt en profil til brugerens enhed på listen over politikker for overholdelse af regler og standarder. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.
1. Rediger brugerens betingede adgangstildeling.
1. I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune,** vælge en politik på listen  >    >  og klikke **på Brugere og grupper.**
1. Hvis du vil målrette en bestemt politik mod en person, skal du føje dem **til listen Medtag.** For at sikre, at en person udelades fra politikken, kan du føje dem til **listen Udelad.**

**Nyttige links:**

- [Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Fejlfindingspolitik](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Overvågning af overholdelse af Intune-enhed](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Disse trin er kun nyttige ved fejlfinding af Funktionen Betinget adgang til Azure Active Directory. Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang med Exchange-politik. Du kan finde flere oplysninger om administration af enheder i Exchange [**her.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
