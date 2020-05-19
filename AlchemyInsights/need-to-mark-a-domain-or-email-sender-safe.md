---
title: Har du brug for at markere et domæne eller en e-mail-afsender sikker?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281130"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Har du brug for at markere et domæne eller en e-mail-afsender sikker?

- Det anbefales ikke at bruge **lister over sikre afsendere,** da det åbner din organisation for spam-, phish- og spoofing-angreb.
- Men hvis der er et forretningskrav, anbefaler vi, **at** du bruger **[mailflowregler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** til dette formål. Vores vejledning sikrer afsendergodkendelse (kontrollerer, at afsendelsesdomænet ikke bliver forfalsket). **Bemærk:** Vi anbefaler ikke, at du administrerer falske positiver ved hjælp af lister over sikre afsendere, da undtagelser til spamfiltrering kan åbne din organisation for sikkerhedsangreb. Hvis dine brugere modtager meddelelser, der er forkert markeret som spam- eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Afsendere, der er tillid til i Outlook, listen over tilladte afsendere eller tilladte domænelister i politikker mod **spam, bør undgås,** fordi afsendere går uden om al spam-, spoof- og phish-beskyttelse og afsendergodkendelse (SPF, DKIM, DMARC). Denne metode bruges bedst til midlertidig testning.
