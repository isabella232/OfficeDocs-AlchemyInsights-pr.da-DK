---
title: Fix 0x8004de40 fejl i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052031"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 fejl i OneDrive

Hvis du får en 0x8004de40-fejl med OneDrive:

- Genstart den berørte computer, mens du har forbindelse til dit Acitve Directory-domæne.
- Hvis en genstart ikke løser problemet, kan du fjerne joinforbindelse og tilslutte din enhed igen fra Azure AD. 

**Bemærk**: du bør være på virksomhedens netværk, mens du udfører disse trin. Udfør ikke disse trin, når du ikke kan oprette forbindelse til virksomhedens infrastruktur (f. eks. under rejser). 

- Åbn en kommandoprompt med administratorrettigheder. 
- Hvis du vil åbne en kommandoprompt med administratorrettigheder, skal du klikke på- **Start**, højreklikke på **kommandoprompt**og derefter klikke på **Kør som administrator**.
- Skriv *dsregcmd/Leave* , og tryk på **Enter**.
- Skriv *dsregcmd/join* , når du er færdig, og tryk på **Enter**.
- Luk kommandoprompten, når du er færdig.
- Genstart computeren, og log på OneDrive.