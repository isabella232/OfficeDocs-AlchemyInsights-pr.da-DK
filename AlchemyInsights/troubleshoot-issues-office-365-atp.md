---
title: Fejlfinding i forbindelse med problemer med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511106"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Fejlfinding i forbindelse med problemer med Office 365 ATP

- **Meddelelse forsinkelser med levering af e-mail-besked?** Prøv at bruge indstillingen Dynamisk levering til dine politikker for safe attachments for ATP. Derved undgås forsinkelser i leveringen af e-mails, samtidig med at modtagerne beskyttes mod skadelige filer.
- **Vil du rapportere falske positiver eller falske negativer?** Brug dette link til at sende filen til analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Vidste du, at du kan aktivere BESKYTTELSE OM ATP Safe Links for mails, der sendes mellem personer i organisationen?** Følg disse trin:
    1. Gå til https://protection.office.com , og log på.
    2. Gå til **Beskyttelseslinks til trusselshåndteringspolitik**  >  **Policy**  >  **Safe Links**.
    3. Under **Politikker, der gælder for bestemte modtagere**, skal du redigere (eller tilføje) en politik.
    4. Vælg **Anvend sikre links på meddelelser, der sendes i organisationen**.
    5. Gem din politik, og giv dig ca. 30 minutter til, at ændringerne kan arbejde sig gennem dit datacenter.
- Hvis du vil have mere hjælp til ATP, skal du se [Avanceret beskyttelse mod trusler i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).