---
title: Fejlfinding af problemer med Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766739"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Fejlfinding af problemer med Office 365 ATP

- **Bemærk forsinkelser med levering af e-mail-meddelelser?** Prøv at bruge indstillingen Dynamisk levering til politikkerne for vedhæftede filer, der er sikkert for ATP. Dette vil undgå forsinkelser i leveringen af e-mails, samtidig med at modtagerne beskyttes mod skadelige filer.
- **Vil du rapportere falske positiver eller falske negativer?** Brug dette link til at sende filen til analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Vidste du, at du kan aktivere ATP Safe Links beskyttelse for e-mail sendt mellem personer i din organisation?** Følg disse trin:
    1. Gå https://protection.office.comtil , og log på.
    2. Gå til **Politik for trusselsstyring,** > **Policy** > **Sikre links**.
    3. Rediger (eller tilføj) en politik **under Politikker, der gælder for bestemte modtagere.**
    4. Vælg **Anvend sikre links til meddelelser, der sendes i organisationen**.
    5. Gem din politik, og giv dine ændringer ca. 30 minutter til at fungere gennem datacenteret.
- Du kan få mere hjælp til ATP under [Avanceret trusselsbeskyttelse i Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).