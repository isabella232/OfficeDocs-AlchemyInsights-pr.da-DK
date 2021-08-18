---
title: Har du brug for at markere et domæne eller en mailafsender som sikker?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319942"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Har du brug for at markere et domæne eller en mailafsender som sikker?

- Brug af **lister over afsendere,** der er tillid til, anbefales ikke, da det åbner din organisation for spam, phish- og spoofing-angreb.
- Men hvis der er forretningsmæssige krav, anbefaler **vi, at** du **[bruger mail Flow Regler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette. Vores vejledning sikrer, at afsendergodkendelse (bekræfter, at afsendelse af domæne ikke bliver efterlignet). 
    **Bemærk!** Vi anbefaler ikke at administrere falske positive ved hjælp af lister over afsendere, der er tillid til, fordi undtagelser til spamfiltrering kan åbne organisationen for sikkerhedsangreb. Hvis dine brugere modtager meddelelser, der er markeret forkert som spam eller uønsket mail, skal **[du rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Pengeskab Afsendere på Outlook, liste over tilladte afsendere eller tilladte domæner i politikker for uønsket post skal undgås, fordi afsendere tilsidesætter al spam-, spoof- og phish-beskyttelse og sendergodkendelse (SPF, DKIM, DMARC).  Denne metode anbefales kun til midlertidige test.
- Valideringen af, at en bestemt mail omgår antispamevaluering, kan udføres ved at markere "X-Forefront Antispam-Report"-meddelelsesoverskriften (SFV:SFE, SFV:SKA, SFV:SKN) i Brevhoveder for **[uønsket](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** post .
- Da Microsoft ønsker at beskytte vores kunder [som standard, anvendes](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)nogle lejertilsidesættelser ikke for malware og phishing med høj sikkerhed. Disse tilsidesættelser omfatter: o Tilladte afsenderlister eller tilladte domænelister (antispampolitikker) o Outlook Pengeskab Afsendere o IP-tilladelsesliste (filtrering af forbindelse) 
- Den eneste tilsidesættelse, der tillader phishing-meddelelse med høj tillid til at tilsidesætte filtrering, er Exchange regler for mailflow (også kaldet transportregler). Hvis du vil bruge regler for mailflow til at tilsidesætte filtrering, skal du se Brug regler for mailflow til at indstille **[SCL (spam confidence level) i meddelelser.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**