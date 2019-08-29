---
title: Opsætning af DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666258"
---
# <a name="setup-dkim-in-office-365"></a>Opsætning af DKIM i Office 365

Komplet vejledning til konfiguration af DKIM til brugerdefinerede domæner i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. For **hver** brugerdefineret domæne skal du oprette **to** DKIM CNAME-post i domænets DNS-værtstjeneste (typisk domæneregistrator). For eksempel contoso.com og fourthcoffee.com kræver fire DKIM CNAME-poster: to til contoso.com og to for fourthcoffee.com.

   DKIM CNAME-poster for **hver** brugerdefineret domæne kan bruge følgende formater:

   - **Host-navn**:`selector1._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Host-navn**:`selector2._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> tekst til venstre for `.mail.protection.outlook.com` i tilpassede MX-posten for custom Domains (for eksempel `contoso-com` med domænet Contoso.com). \<InitialDomain\> , er det domæne, du brugte, da du tilmeldte dig Office 365 (for eksempel contoso.onmicrosoft.com).

2. Når du har oprettet CNAME-poster til dine brugerdefinerede domæner, kan du udføre følgende instruktioner:

   en. [Log på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med kontoen arbejdet eller skolen.

   b. Vælg ikonet app Opgavestarter øverst til venstre, og vælg **Admin**.

   c. Udvid **Admin** i det nederste venstre navigationspanel, og vælg **Exchange**.

   d. Gå til **beskyttelse af** > **DKIM**.

   e. Vælg domænet, og vælg derefter **Aktiver** for **Log-meddelelser til dette domæne med DKIM-signaturer**. Gentag dette trin for hvert brugerdefinerede domæne.
