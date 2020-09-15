---
title: Spam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717319"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="783c5-102">Løs problemer med levering af mail for fejlkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="783c5-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="783c5-103">Kontrollér SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF-eller DNS-post kontrol på internettet.</span><span class="sxs-lookup"><span data-stu-id="783c5-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="783c5-104">Kontrollér, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og sendt via [puljen til stor risiko levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="783c5-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="783c5-105">Meddelelser i puljen til levering af høj risiko opfylder ikke SPF checks, og de accepteres derfor ikke af organisationens destinations-e-mail.</span><span class="sxs-lookup"><span data-stu-id="783c5-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="783c5-106">Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mail vært, du forsøger at sende mail til.</span><span class="sxs-lookup"><span data-stu-id="783c5-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="783c5-107">Vær opmærksom på den detaljerede eksterne fejl, der er tilgængelig i meddelelsen bold.</span><span class="sxs-lookup"><span data-stu-id="783c5-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="783c5-108">Microsoft Support kan muligvis ikke hjælpe yderligere.</span><span class="sxs-lookup"><span data-stu-id="783c5-108">Microsoft support may not be able to assist further.</span></span>
