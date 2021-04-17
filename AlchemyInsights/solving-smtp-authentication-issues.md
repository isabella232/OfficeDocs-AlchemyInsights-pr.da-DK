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
# <a name="solving-smtp-authentication-issues"></a>Løsning af problemer med SMTP-godkendelse

Hvis du får fejl 5.7.57 eller 5.7.3, når du forsøger at sende SMTP-mail og godkende med en klient eller et program, er der et par ting, du skal kontrollere:

- Godkendt SMTP-indsendelse kan være deaktiveret i din lejer eller på den postkasse, du forsøger at bruge (markér begge indstillinger). Se Aktivér eller deaktiver [godkendt SMTP-klientindsendelse](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)for at få mere at vide.

- Kontrollér, om [Azure Security-standardindstillinger](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) er aktiveret for din lejer. Hvis det er aktiveret, vil SMTP-godkendelse ved hjælp af grundlæggende godkendelse (også kaldet "ældre" ).brug af brugernavn og adgangskode) mislykkes.
