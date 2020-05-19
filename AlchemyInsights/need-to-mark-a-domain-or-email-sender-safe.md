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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="2dec0-102">Har du brug for at markere et domæne eller en e-mail-afsender sikker?</span><span class="sxs-lookup"><span data-stu-id="2dec0-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="2dec0-103">Det anbefales ikke at bruge **lister over sikre afsendere,** da det åbner din organisation for spam-, phish- og spoofing-angreb.</span><span class="sxs-lookup"><span data-stu-id="2dec0-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="2dec0-104">Men hvis der er et forretningskrav, anbefaler vi, **at** du bruger **[mailflowregler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** til dette formål.</span><span class="sxs-lookup"><span data-stu-id="2dec0-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="2dec0-105">Vores vejledning sikrer afsendergodkendelse (kontrollerer, at afsendelsesdomænet ikke bliver forfalsket).</span><span class="sxs-lookup"><span data-stu-id="2dec0-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="2dec0-106">**Bemærk:** Vi anbefaler ikke, at du administrerer falske positiver ved hjælp af lister over sikre afsendere, da undtagelser til spamfiltrering kan åbne din organisation for sikkerhedsangreb.</span><span class="sxs-lookup"><span data-stu-id="2dec0-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="2dec0-107">Hvis dine brugere modtager meddelelser, der er forkert markeret som spam- eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="2dec0-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="2dec0-108">Afsendere, der er tillid til i Outlook, listen over tilladte afsendere eller tilladte domænelister i politikker mod **spam, bør undgås,** fordi afsendere går uden om al spam-, spoof- og phish-beskyttelse og afsendergodkendelse (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="2dec0-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="2dec0-109">Denne metode bruges bedst til midlertidig testning.</span><span class="sxs-lookup"><span data-stu-id="2dec0-109">This method is best used for temporary testing only.</span></span>
