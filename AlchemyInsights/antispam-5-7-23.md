---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821405"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="0df7b-102">Løs problemer med levering af mail, fejlkode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="0df7b-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="0df7b-103">Bekræft SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.</span><span class="sxs-lookup"><span data-stu-id="0df7b-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="0df7b-104">Kontrollér, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeres gennem puljen af levering [med høj risiko.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="0df7b-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="0df7b-105">Meddelelser i pulje til levering af høj risiko består ikke SPF-kontroller og accepteres derfor ikke af destinationens mailorganisation.</span><span class="sxs-lookup"><span data-stu-id="0df7b-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="0df7b-106">Hvis problemet fortsætter, skal du muligvis kontakte administratoren for den mailvært, du forsøger at sende mail til.</span><span class="sxs-lookup"><span data-stu-id="0df7b-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="0df7b-107">Læg mærke til de detaljerede eksterne fejl, der er tilgængelige i meddelelsen om ikke-tilgængelig mail.</span><span class="sxs-lookup"><span data-stu-id="0df7b-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="0df7b-108">Microsoft Support kan muligvis ikke hjælpe yderligere.</span><span class="sxs-lookup"><span data-stu-id="0df7b-108">Microsoft support may not be able to assist further.</span></span>
