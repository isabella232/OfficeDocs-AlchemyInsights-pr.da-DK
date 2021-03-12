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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713389"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemer med installation af Microsoft Defender på Mac eller Linux

**Mac**

- Sørg for, at systemkravene er opfyldt, før du installerer Microsoft Defender ATP til Mac. Du kan få mere at vide [under Sådan installerer du Microsoft Defender ATP til Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Gennemse oplysningerne i filen: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Sørg for, at systemkravene er opfyldt, før du installerer Microsoft Defender ATP til Linux. Du kan få mere at vide [under Sådan installerer du Microsoft Defender ATP til Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Hvis du vil bekræfte, at MDATP-tjenesten kører, skal du se [Installation mislykkedes.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Hvis du vil foretage fejlfinding og løse problemer, hvis tjenesten ikke kører, skal du se Trin til fejlfinding, [hvis mdatp-tjenesten ikke kører.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Du kan finde trin til at kontrollere klientkonfigurationen, som bekræfter produktets tilstand, og til at køre en registreringstest på tekstfilen EICAR under [Klientkonfiguration.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Bemærk!** Du kan finde en liste over understøttede filsystemer til aktivitet ved adgang under [Microsoft Defender ATP til Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)