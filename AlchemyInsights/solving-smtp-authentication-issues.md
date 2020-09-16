---
title: Løse problemer med SMTP-godkendelse
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
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737983"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="09d08-102">Løse problemer med SMTP-godkendelse</span><span class="sxs-lookup"><span data-stu-id="09d08-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="09d08-103">Hvis du får fejl 5.7.57 eller 5.7.3, når du forsøger at sende SMTP-mail og godkende med en klient eller et program, er der et par ting, du skal kontrollere:</span><span class="sxs-lookup"><span data-stu-id="09d08-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="09d08-104">Godkendt SMTP-afsendelse kan være deaktiveret i din lejer eller på den postkasse, du forsøger at bruge (Kontrollér begge indstillinger).</span><span class="sxs-lookup"><span data-stu-id="09d08-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="09d08-105">Hvis du vil have mere at vide, skal du se [aktivere eller deaktivere godkendelse af godkendt klient SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="09d08-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="09d08-106">Kontrollér, om [Azure-sikkerhedsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) er aktiveret for din lejer. Hvis den er aktiveret, vil SMTP-godkendelse ved hjælp af basisgodkendelse (også kendt som ældre. dette bruger Brugernavn og adgangskode) mislykkes.</span><span class="sxs-lookup"><span data-stu-id="09d08-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
