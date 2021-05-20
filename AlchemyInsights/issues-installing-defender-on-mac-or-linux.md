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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539674"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemer med installation af Microsoft Defender på Mac eller Linux

**Mac**

- Sørg for, at systemkravene er opfyldt, før du Microsoft Defender ATP til Mac. Du kan finde flere oplysninger [under Sådan installerer du Microsoft Defender ATP til Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Gennemse oplysningerne i filen: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Sørg for, at systemkravene er opfyldt, før du Microsoft Defender ATP til Linux. Du kan finde flere oplysninger [under Sådan installerer du MDATP til Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Hvis du vil bekræfte, MDATP tjeneste kører, skal du se [Installation mislykkedes.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hvis du vil foretage fejlfinding og løse problemer, hvis tjenesten ikke kører, skal du se Trin til fejlfinding, [hvis mdatp-tjenesten ikke kører.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Du kan finde trin til at kontrollere klientkonfigurationen, som bekræfter produktets tilstand, og for at køre en registreringstest på EICAR-tekstfilen, under [Klientkonfiguration.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Bemærk!** Du kan finde en liste over understøttede filsystemer til aktivitet under [Microsoft Defender ATP til Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)