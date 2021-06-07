---
title: Problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793756"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux

Denne artikel vejleder dig gennem trinnene til at identificere problemer med ydeevnen for Microsoft Defender til slutpunkt på Linux.

Det er vigtigt først at kontrollere, at det problem, du oplever, er løst med den [nyeste version.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Hvis du vil starte undersøgelsen, skal [du se Fejlfinding af problemer med ydeevnen for Microsoft Defender til Slutpunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Udeladelse

Udeladelse kan være med til at reducere problemer med ydeevnen. Gennemse dine undtagelser, før du begynder, så yderligere risici kendes og dokumenteres.

Få mere at vide under [Konfigurer og valider udeladelse af Microsoft Defender til Slutpunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Når du har flere filer & mapper, der skal udelades, og de alle er på det samme mountpoint, kan det være nemmere at udelukke mountpointen. Fra og med udgivelsen fra februar 101.22.80 kan du udelade et helt mountpoint.

Hvis /mnt/backup f.eks. er et mountpoint, kan du tilføje /mnt/backup til listen exclude ved at køre denne kommando:

`$ mdatp exclusion folder add –path /mnt/backup`

**Bemærk!** Hvis du tilføjer udeladelse, øges risikoen for, at malware ikke registreres, og de skal håndteres og implementeres med omhu.

## <a name="need-help"></a>Har du brug for hjælp?

For at hjælpe dig på den mest effektive måde skal du indsamle de diagnostiske data, før du åbner en supportsag.
