---
title: Opsætning DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509378"
---
# <a name="setup-dkim"></a>Opsætning DKIM

Den komplette vejledning til konfiguration af DKIM for brugerdefinerede domæner i Microsoft 365 findes [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. For **hvert** brugerdefineret domæne skal du oprette **to** DKIM CNAME-poster hos domænets DNS-hostingtjeneste (typisk domæneregistratoren). for eksempel kræver contoso.com og fourthcoffee.com fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-posterne for **hvert** brugerdefineret domæne bruger følgende formater:

   - **Værtsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Værtsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-post for det brugerdefinerede domæne (f.eks. `contoso-com` for det contoso.com domæne). \<InitialDomain\>er det domæne, du brugte, da du tilmeldte dig Microsoft 365 (f.eks. contoso.onmicrosoft.com).

2. Når du har oprettet CNAME-posterne for dine brugerdefinerede domæner, skal du udfylde følgende instruktioner:

   a. [logge på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med din arbejds- eller skolekonto.

   b. Vælg ikonet for appstarteren øverst til venstre, og vælg **Administrator**.

   c. I navigationen nederst til venstre skal du udvide **Administrator** og vælge **Exchange**.

   D. Gå til **Beskyttelse**  >  **DKIM**.

   E. Vælg domænet, og vælg derefter **Aktivér** for **Signer meddelelser for dette domæne med DKIM-signaturer**. Gentag dette trin for hvert brugerdefineret domæne.
