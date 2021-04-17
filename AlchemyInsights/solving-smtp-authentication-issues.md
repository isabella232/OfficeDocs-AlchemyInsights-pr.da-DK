---
title: Løsning af problemer med SMTP-godkendelse
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826409"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="de038-102">Løsning af problemer med SMTP-godkendelse</span><span class="sxs-lookup"><span data-stu-id="de038-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="de038-103">Hvis du får fejl 5.7.57 eller 5.7.3, når du forsøger at sende SMTP-mail og godkende med en klient eller et program, er der et par ting, du skal kontrollere:</span><span class="sxs-lookup"><span data-stu-id="de038-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="de038-104">Godkendt SMTP-indsendelse kan være deaktiveret i din lejer eller på den postkasse, du forsøger at bruge (markér begge indstillinger).</span><span class="sxs-lookup"><span data-stu-id="de038-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="de038-105">Se Aktivér eller deaktiver [godkendt SMTP-klientindsendelse](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)for at få mere at vide.</span><span class="sxs-lookup"><span data-stu-id="de038-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="de038-106">Kontrollér, om [Azure Security-standardindstillinger](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) er aktiveret for din lejer. Hvis det er aktiveret, vil SMTP-godkendelse ved hjælp af grundlæggende godkendelse (også kaldet "ældre" ).brug af brugernavn og adgangskode) mislykkes.</span><span class="sxs-lookup"><span data-stu-id="de038-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
