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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506437"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="00ab0-102">Løs problemer med levering af e-mail for fejlkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="00ab0-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="00ab0-103">Kontroller SPF DNS-posten for dit domæne ved en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.</span><span class="sxs-lookup"><span data-stu-id="00ab0-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="00ab0-104">Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeret gennem [high risk-leveringspuljen](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="00ab0-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="00ab0-105">Meddelelser i højrisikoleveringspuljen består ikke SPF-kontroller og accepteres derfor ikke af destinationsmailorganisationen.</span><span class="sxs-lookup"><span data-stu-id="00ab0-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="00ab0-106">Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mailvært, som du forsøger at sende e-mail til.</span><span class="sxs-lookup"><span data-stu-id="00ab0-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="00ab0-107">Gør opmærksom på den detaljerede eksterne fejl, der er tilgængelig i afvisningsmeddelelsen.</span><span class="sxs-lookup"><span data-stu-id="00ab0-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="00ab0-108">Microsoft-support kan muligvis ikke hjælpe yderligere.</span><span class="sxs-lookup"><span data-stu-id="00ab0-108">Microsoft support may not be able to assist further.</span></span>
