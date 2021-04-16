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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792126"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Har du brug for at markere et domæne eller en mailafsender som sikker?

- Brug af **lister over afsendere,** der er tillid til, anbefales ikke, da det åbner din organisation for spam, phish- og spoofing-angreb.
- Men hvis der er forretningsmæssige krav, anbefaler vi, **at du** bruger regler **[for mailflow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** til dette. Vores vejledning sikrer, at afsendergodkendelse (bekræfter, at afsendelse af domæne ikke bliver efterlignet). **Bemærk!** Vi anbefaler ikke at administrere falske positive ved hjælp af lister over afsendere, der er tillid til, fordi undtagelser til spamfiltrering kan åbne organisationen for sikkerhedsangreb. Hvis dine brugere modtager meddelelser, der er markeret forkert som spam eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Afsendere, der er tillid til i Outlook, liste  over tilladte afsendere eller tilladt domæneliste i antispampolitikker skal undgås, fordi afsendere tilsidesætter al spam-, spoof- og phish-beskyttelse og sendergodkendelse (SPF, DKIM, DMARC). Denne metode anbefales kun til midlertidige test.
