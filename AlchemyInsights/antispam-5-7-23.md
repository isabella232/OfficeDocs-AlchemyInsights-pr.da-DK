---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676491"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="aabdf-102">Løs problemer med levering af mail, fejlkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="aabdf-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="aabdf-103">Kontroller SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.</span><span class="sxs-lookup"><span data-stu-id="aabdf-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="aabdf-104">Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeret gennem [puljen til levering med høj risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="aabdf-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="aabdf-105">Meddelelser i puljen til levering af høj risiko består ikke SPF-checks og accepteres derfor ikke af destinationsmailorganisationen.</span><span class="sxs-lookup"><span data-stu-id="aabdf-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="aabdf-106">Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mailvært, du forsøger at sende e-mail til.</span><span class="sxs-lookup"><span data-stu-id="aabdf-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="aabdf-107">Noter den detaljerede eksterne fejl, der er tilgængelig i afvisningsmeddelelsen.</span><span class="sxs-lookup"><span data-stu-id="aabdf-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="aabdf-108">Microsoft-support kan muligvis ikke hjælpe yderligere.</span><span class="sxs-lookup"><span data-stu-id="aabdf-108">Microsoft support may not be able to assist further.</span></span>
