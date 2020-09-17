---
title: Konfigurer DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808701"
---
# <a name="setup-dkim"></a>Konfigurer DKIM

Den komplette vejledning til konfiguration af DKIM til brugerdefinerede domæner i Microsoft 365 er [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. For **hvert** brugerdefineret domæne skal du oprette **to** DKIM CNAME-poster hos dit domænes DNS-værtstjeneste (typisk domæneregistrator). For eksempel kræver contoso.com og fourthcoffee.com fire DKIM CNAME-poster: to for contoso.com og to til fourthcoffee.com.

   DKIM CNAME-posterne for **hvert** brugerdefineret domænebruger følgende formater:

   - **Værtsnavn**: `selector1._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Værtsnavn**: `selector2._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-post for det brugerdefinerede domæne (f. eks. `contoso-com` for domænet contoso.com). \<InitialDomain\> det domæne, du brugte, da du tilmeldte dig Microsoft 365 (f. eks. contoso.onmicrosoft.com).

2. Når du har oprettet CNAME-posterne for dine brugerdefinerede domæner, skal du udføre følgende instruktioner:

   a. [Log på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med din arbejds-eller skolekonto.

   b. Vælg ikonet for app-starteren øverst til venstre, og vælg **administrator**.

   c. Udvid **administrator** i nederste venstre navigationsrude, og vælg **Exchange**.

   d. Gå til **beskyttelses**  >  **DKIM**.

   e. Vælg domænet, og vælg derefter **Aktivér** for **signering af meddelelser for dette domæne med DKIM-signaturer**. Gentag dette trin for hvert brugerdefinerede domæne.
