---
title: Hvad du skal gøre, hvis Azure-funktioner ikke fungerer korrekt i Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812864"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Hvad du skal gøre, hvis Azure-funktioner ikke fungerer korrekt i Microsoft Edge

Microsoft Edge har kendte problemer i forbindelse med sikkerhedszoner, der kan påvirke, hvordan Azure-brugere logger på Windows Administration. Du kan få mere at vide [under Kendte problemer i Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Hvis du har problemer med at bruge Azure-funktioner med Microsoft Edge, kan du prøve følgende:

1. På menuen Start i **søgefeltet** skal du **skrive Internetindstillinger** og derefter vælge det.
1. I **Egenskaber for** internet skal du vælge **fanen** Sikkerhed.
1. Vælg **Websteder, der er** tillid til , og vælg derefter **Websteder**.
1. Tilføj din gateway-URL-adresse samt <https://login.microsoftonline.com> og , og vælg <https://login.live.com> **Luk**.
1. I **Egenskaber for internet** skal du vælge fanen Beskyttelse **af** personlige oplysninger.
1. I sektionen Blokering af pop op-vindue skal du vælge **Indstillinger**. Tilføj din gateway-URL-adresse samt <https://login.microsoftonline.com> og , og vælg derefter <https://login.live.com> **Luk**.