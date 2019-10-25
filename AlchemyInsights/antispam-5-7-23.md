---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682086"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="32b2b-102">Løs problemer med levering af e-mail for fejlkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="32b2b-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="32b2b-103">Bekræft SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF-eller DNS-post kontrol på internettet.</span><span class="sxs-lookup"><span data-stu-id="32b2b-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="32b2b-104">Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Office 365, og at den blev distribueret via [puljen med høj risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="32b2b-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="32b2b-105">Meddelelser i den høje risiko leverings pulje vil ikke passere SPF-checks og vil derfor ikke blive accepteret af destinations-e-mail-organisationen.</span><span class="sxs-lookup"><span data-stu-id="32b2b-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="32b2b-106">Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mail vært, som du forsøger at sende mails til.</span><span class="sxs-lookup"><span data-stu-id="32b2b-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="32b2b-107">Notér den detaljerede eksterne fejl, der er tilgængelig i meddelelsen Bounce.</span><span class="sxs-lookup"><span data-stu-id="32b2b-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="32b2b-108">Support til Office 365 kan muligvis ikke hjælpe yderligere.</span><span class="sxs-lookup"><span data-stu-id="32b2b-108">Office 365 support may not be able to assist further.</span></span>