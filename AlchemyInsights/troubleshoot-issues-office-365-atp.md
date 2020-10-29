---
title: Fejlfinding af problemer med Microsoft Defender til Office 365 (DTT)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801401"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Fejlfinding af problemer med Office 365 DTT

- **Oplever du forsinkelser med levering af mail** ? Prøv at bruge indstillingen dynamisk levering for dine ATP-politikker for sikre vedhæftede filer. Dette vil undgå forsinkelser i levering af mails, når du beskytter modtagere fra ondsindede filer.
- **Vil du rapportere falske positive eller falske negativer** ? Brug dette link til at sende filen til analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Vidste du, at du kan aktivere beskyttelse med ATP sikre links for mails, der sendes mellem personer i organisationen** ? Følg disse trin:
    1. Gå til https://protection.office.com , og log på.
    2. Gå til politik for sikre **trusler administration**  >  **Policy**  >  **Safe Links** .
    3. Under **politikker, der gælder for bestemte modtagere** , skal du redigere (eller tilføje) en politik.
    4. Vælg **Anvend sikre links til meddelelser, der sendes inden for organisationen** .
    5. Gem din politik, og Tillad ca. 30 minutter, før dine ændringer fungerer på deres måde gennem dit datacenter.
- Du kan få mere hjælp til DTT i [Microsoft Defender til Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).