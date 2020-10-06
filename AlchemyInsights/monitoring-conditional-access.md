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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366422"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Overvågning af betinget adgang for Exchange

Brugere, der er målrettet med betinget adgang, modtager en mailbesked, hvis de ikke opfylder din organisations adgangs krav. Vi anbefaler en eller flere af følgende løsninger for at løse problemet:

- Hvis enheden anses for at være tilmeldt, skal du bede brugeren om at gå til appen Firmaportal og bekræfte, at den vises på Firmaportalen. Hvis det ikke er den, skal brugeren tilmelde enheden.
- I Azure-portalen skal du gå til Intune > enhedskompatibilitet. Klik på enheds overholdelse under overvågning. Se din enheds kompatibilitetsrapport for at bekræfte, at brugerens enhed er markeret som kompatibel.
- I Azure-portalen skal du gå til Intune > enhedskompatibilitet. Under Administrer skal du klikke på politikker. På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed. Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens overholdelses status.
- Redigere brugerens betingede adgangs tildeling.

1. Gå til politikker for **Intune**  >  **betinget adgang**til Intune i Azure-portalen  >  **Policies**.
2. Vælg en politik på listen.
3. Klik på brugere og grupper.
4. Hvis du vil målrette en bestemt politik til en anden, skal du føje dem til listen Medtag. Hvis du vil sikre dig, at en person udelades fra politikken, skal du føje dem til listen Udelad.

Nyttige links:

[Oversigt over enheds overholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings NØGLECENTER](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindings politik](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Overvåge Intune-enhedskompatibilitet](https://docs.microsoft.com/intune/compliance-policy-monitor)

Bemærk! disse trin er kun nyttige til fejlfinding af betinget adgang til Azure Active Directory-funktionen. Det er også muligt at sætte en enheds blokering for en enhed, at det er en mail adgang med Exchange-politik. Du kan finde flere oplysninger om administration af Exchange-enheder [her](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
