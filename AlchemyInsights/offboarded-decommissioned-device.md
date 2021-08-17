---
title: Problemer med at fjerne en ikke-tavlet eller udkøret enhed fra Enhedens lager
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076637"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemer med at fjerne en ikke-tavlet eller udkøret enhed fra Enhedens lager

Microsoft Defender til Slutpunkt tillader i øjeblikket ikke manuelt at fjerne enhedsposten for en offboardet eller ud afviklet enhed fra Lager over enheder.

Af sikkerhedsmæssige årsager forbliver enheden i portalen som en historisk post i op til 180 dage. Men enhedens data slettes i henhold til din konfigurerede opbevaringsperiode.

**Bemærk!** En offboarded eller udkomponeret enhed skifter automatisk til **Inaktiv tilstand** efter syv dage. Desuden tages enheder, der ikke er aktive inden for de seneste 30 dage, ikke med i de data, der afspejler din organisation Håndtering af trusler og sikkerhedsrisici eksponeringsscore eller Microsoft Secure Score for enheder.
 
Hvis du stadig ikke vil se visse enheder i visningen Lagerenhed, kan du prøve at placere et enhedsmærke for at filtrere den udkomne enhed fra visningen Lagerenhed.

Du kan finde flere oplysninger under:

[Offboard-enheder fra Microsoft Defender for Endpoint-tjenesten](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Eksponeringsscore i Håndtering af trusler og sikkerhedsrisici](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Ret usunde sensorerne i Microsoft Defender til Slutpunkt](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Sådan bruges mærkning effektivt (del 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Sådan bruges mærkning effektivt (del 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Sådan bruges mærkning effektivt (del 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




