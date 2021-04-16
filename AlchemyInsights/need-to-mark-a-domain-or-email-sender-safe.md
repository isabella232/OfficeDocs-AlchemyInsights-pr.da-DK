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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="ad427-102">Har du brug for at markere et domæne eller en mailafsender som sikker?</span><span class="sxs-lookup"><span data-stu-id="ad427-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="ad427-103">Brug af **lister over afsendere,** der er tillid til, anbefales ikke, da det åbner din organisation for spam, phish- og spoofing-angreb.</span><span class="sxs-lookup"><span data-stu-id="ad427-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="ad427-104">Men hvis der er forretningsmæssige krav, anbefaler vi, **at du** bruger regler **[for mailflow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** til dette.</span><span class="sxs-lookup"><span data-stu-id="ad427-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="ad427-105">Vores vejledning sikrer, at afsendergodkendelse (bekræfter, at afsendelse af domæne ikke bliver efterlignet).</span><span class="sxs-lookup"><span data-stu-id="ad427-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="ad427-106">**Bemærk!** Vi anbefaler ikke at administrere falske positive ved hjælp af lister over afsendere, der er tillid til, fordi undtagelser til spamfiltrering kan åbne organisationen for sikkerhedsangreb.</span><span class="sxs-lookup"><span data-stu-id="ad427-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="ad427-107">Hvis dine brugere modtager meddelelser, der er markeret forkert som spam eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="ad427-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="ad427-108">Afsendere, der er tillid til i Outlook, liste  over tilladte afsendere eller tilladt domæneliste i antispampolitikker skal undgås, fordi afsendere tilsidesætter al spam-, spoof- og phish-beskyttelse og sendergodkendelse (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="ad427-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="ad427-109">Denne metode anbefales kun til midlertidige test.</span><span class="sxs-lookup"><span data-stu-id="ad427-109">This method is best used for temporary testing only.</span></span>
