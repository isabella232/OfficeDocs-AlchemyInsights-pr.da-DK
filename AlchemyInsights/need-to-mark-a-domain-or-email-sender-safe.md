---
title: Har du brug for at markere et domæne eller en mail afsender som sikker?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803239"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Har du brug for at markere et domæne eller en mail afsender som sikker?

- Det **anbefales ikke at bruge listen over sikre afsendere** , da det åbner din organisation for spam, Phish og spoofing-angreb.
- Men hvis der er et virksomheds krav, anbefaler vi, **at** du bruger **[regler for mail flow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette. Vores vejledning sikrer, at afsender-godkendelsen (bekræfter, at domæne ikke bliver spoofet). **Bemærk**! vi anbefaler ikke at administrere falske positive tal ved hjælp af lister over sikre afsendere, da undtagelser for spam filtrering kan åbne din organisation for sikkerhedsangreb. Hvis dine brugere modtager meddelelser, der er markeret forkert som spam eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.
- Sikre afsendere i Outlook, listen over tilladte afsendere eller en tilladt domæne liste i politikker for spam-spam **bør undgås** , fordi afsenderen tilsidesætter alle spam-, spoofing-og Phish-beskyttelse og afsender godkendelse (SPF, DKIM, DMARC). Denne metode bruges bedst til midlertidig test.
