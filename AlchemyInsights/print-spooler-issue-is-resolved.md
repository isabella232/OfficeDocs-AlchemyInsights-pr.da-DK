---
title: Problemet med udskriftskøen er blevet rettet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801835"
---
# <a name="print-spooler-issue-is-resolved"></a>Problemet med udskriftskøen er blevet rettet

Hvis din enhed blev opdateret med Windows 10  **os Build 19041,329**, kan du have observeret et problem, hvor visse printere ikke kan udskrive. Printspooleren kan udløse en fejl eller lukke uventet ved forsøg på at udskrive, og der kommer ingen output fra den pågældende printer. Dette problem er løst i operativsystemet Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Vedvarende undersøgelse**

Den lokale sikkerheds myndigheds undersystem (LSASS)-fil (**Isass.exe**) lykkes muligvis ikke på nogle enheder med fejlmeddelelsen "en kritisk systemproces, C:\WINDOWS\system32\Isass.exe, mislykkedes med statuskoden c0000008. Computeren skal genstartes nu.  **Microsoft arbejder på en løsning og giver dig en opdatering i en kommende udgivelse.**

Hvis du vil have mere at vide, skal du se  [kendte problemer med Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).