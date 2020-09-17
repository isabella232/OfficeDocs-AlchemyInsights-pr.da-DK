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
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="d7bd2-102">Har du brug for at markere et domæne eller en mail afsender som sikker?</span><span class="sxs-lookup"><span data-stu-id="d7bd2-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="d7bd2-103">Det **anbefales ikke at bruge listen over sikre afsendere** , da det åbner din organisation for spam, Phish og spoofing-angreb.</span><span class="sxs-lookup"><span data-stu-id="d7bd2-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="d7bd2-104">Men hvis der er et virksomheds krav, anbefaler vi, **at** du bruger **[regler for mail flow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette.</span><span class="sxs-lookup"><span data-stu-id="d7bd2-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="d7bd2-105">Vores vejledning sikrer, at afsender-godkendelsen (bekræfter, at domæne ikke bliver spoofet).</span><span class="sxs-lookup"><span data-stu-id="d7bd2-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="d7bd2-106">**Bemærk**! vi anbefaler ikke at administrere falske positive tal ved hjælp af lister over sikre afsendere, da undtagelser for spam filtrering kan åbne din organisation for sikkerhedsangreb.</span><span class="sxs-lookup"><span data-stu-id="d7bd2-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="d7bd2-107">Hvis dine brugere modtager meddelelser, der er markeret forkert som spam eller uønsket mail, skal du **[rapportere meddelelser og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="d7bd2-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="d7bd2-108">Sikre afsendere i Outlook, listen over tilladte afsendere eller en tilladt domæne liste i politikker for spam-spam **bør undgås** , fordi afsenderen tilsidesætter alle spam-, spoofing-og Phish-beskyttelse og afsender godkendelse (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="d7bd2-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="d7bd2-109">Denne metode bruges bedst til midlertidig test.</span><span class="sxs-lookup"><span data-stu-id="d7bd2-109">This method is best used for temporary testing only.</span></span>
