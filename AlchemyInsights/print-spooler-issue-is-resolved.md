---
title: Print Spooler-problemet er løst
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911332"
---
# <a name="print-spooler-issue-is-resolved"></a>Print Spooler-problemet er løst

Hvis din enhed er opdateret med Windows 10 **OS Build 19041.329,** har du muligvis observeret et problem, hvor visse printere ikke kan udskrives.   Print Spooleren kan give en fejl eller lukke uventet, når du forsøger at udskrive, og der kommer ingen output fra den pågældende printer. Dette problem er løst i os Build **19041.331,** [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Løbende undersøgelse**

LSASS-filen (Local Security Authority Subsystem Service) (**Isass.exe**) kan mislykkes på visse enheder med fejlmeddelelsen "En kritisk systemproces, C:\WINDOWS\system32\Isass.exe, mislykkedes med statuskoden c0000008. Computeren skal nu genstartes".  **Microsoft arbejder på en løsning og leverer en opdatering i en kommende version.**

Du kan finde flere oplysninger i Windows 10, der er kendt [med version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).