---
title: Problemer med installation af Microsoft Defender på Mac eller Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325243"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemer med installation af Microsoft Defender på Mac eller Linux

**Mac**

- Sørg for, at systemkravene er opfyldt, før du installerer Microsoft Defender ATP til Mac. Du kan få mere at vide [under Sådan installerer du Microsoft Defender ATP til Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Gennemse oplysningerne i filen: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Sørg for, at systemkravene er opfyldt, før du installerer Microsoft Defender ATP til Linux. Du kan få mere at vide [under Sådan installerer du MDATP til Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Se Installation mislykkedes for at bekræfte, at [MDATP-tjenesten kører.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hvis du vil foretage fejlfinding og løse problemer, hvis tjenesten ikke kører, skal du se Trin til fejlfinding, [hvis mdatp-tjenesten ikke kører.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Du kan finde trin til at kontrollere klientkonfigurationen, som bekræfter produktets tilstand, og for at køre en registreringstest på EICAR-tekstfilen, under [Klientkonfiguration.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Bemærk!** Du kan finde en liste over understøttede filsystemer til aktivitet ved adgang under [Microsoft Defender ATP til Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)