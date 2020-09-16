---
title: Fejlfinding af problemer med Office 365 Advanced Threat Protection (DTT)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758059"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Fejlfinding af problemer med Office 365 DTT

- **Oplever du forsinkelser med levering af mail**? Prøv at bruge indstillingen dynamisk levering for dine ATP-politikker for sikre vedhæftede filer. Dette vil undgå forsinkelser i levering af mails, når du beskytter modtagere fra ondsindede filer.
- **Vil du rapportere falske positive eller falske negativer**? Brug dette link til at sende filen til analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Vidste du, at du kan aktivere beskyttelse med ATP sikre links for mails, der sendes mellem personer i organisationen**? Følg disse trin:
    1. Gå til https://protection.office.com , og log på.
    2. Gå til politik for sikre **trusler administration**  >  **Policy**  >  **Safe Links**.
    3. Under **politikker, der gælder for bestemte modtagere**, skal du redigere (eller tilføje) en politik.
    4. Vælg **Anvend sikre links til meddelelser, der sendes inden for organisationen**.
    5. Gem din politik, og Tillad ca. 30 minutter, før dine ændringer fungerer på deres måde gennem dit datacenter.
- Hvis du vil have mere hjælp til DTT, skal du se [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).