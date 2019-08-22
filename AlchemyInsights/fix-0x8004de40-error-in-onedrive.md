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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525053"
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