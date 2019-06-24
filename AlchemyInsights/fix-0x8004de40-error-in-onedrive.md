---
title: Rette fejl i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133971"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Rette fejl i 0x8004de40 i OneDrive

Hvis du modtager fejlmeddelelsen 0x8004de40 med OneDrive:

- Genstart computeren, mens du har forbindelse til din atkiv Directory-domæne.
- Hvis en genstart ikke løser problemet, ophæve dit medlemskab og slutte enheden fra Azure AD. 

**Bemærk**: Du skal være på virksomhedens netværk, mens du udfører disse trin. Ikke udføre disse trin, når du ikke kan oprette forbindelse til din virksomheds infrastruktur (for eksempel, mens du rejser). 

- Åbn en kommandoprompt. 
- For at åbne en kommandoprompt, klik på - **Start**, højreklik på **kommandoprompt**og derefter klikke på **Kør som administrator**.
- Skriv *dsregcmd /leave* , og tryk på **Enter**.
- Når du er færdig, kan du skrive *dsregcmd /join* og tryk på **Enter**.
- Når du er færdig, kan du lukke kommandoprompten.
- Genstart computeren, og log ind OneDrive.