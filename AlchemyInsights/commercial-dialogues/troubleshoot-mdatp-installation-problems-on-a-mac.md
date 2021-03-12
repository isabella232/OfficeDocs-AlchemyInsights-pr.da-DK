---
title: Fejlfinding af MDATP-installationsproblemer på en Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744659"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Fejlfinding af MDATP-installationsproblemer på en Mac

Hvis manuel installation mislykkes, **viser** installationsguiden oversigtssiden følgende fejl:

"Der opstod en fejl under installationen. Installationsprogrammet stødte på en fejl, der forårsagede, at installationen mislykkedes. Kontakt softwareproducenten for at få hjælp."

I MDM-installationer viser siden også en generisk installationsfejl.

Selvom vi ikke viser nøjagtige fejl til slutbrugere, beholder vi en logfil med installationsprocessen i **/Library/Logs/Microsoft/mdatp/install.log.** Hver installationssession føjes til denne logfil. Hvis du kun vil have output fra den seneste installationssession, skal du bruge `sed` .

Du kan få mere at vide [under Fejlfinding af installationsproblemer for Microsoft Defender ATP til Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
