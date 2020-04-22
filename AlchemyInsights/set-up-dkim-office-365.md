---
title: DKIM-opsætning
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645666"
---
# <a name="setup-dkim"></a>DKIM-opsætning

Den komplette vejledning til konfiguration af DKIM til brugerdefinerede domæner i Microsoft 365 findes [.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. For **hvert** brugerdefineret domæne skal du oprette **to** DKIM CNAME-poster på domænets DNS-hostingtjeneste (typisk domæneregistratoren). contoso.com og fourthcoffee.com kræve fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-posterne for **hvert** brugerdefineret domæne bruger følgende formater:

   - **Værtsnavn**:`selector1._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Værtsnavn**:`selector2._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> er teksten til `.mail.protection.outlook.com` venstre for i den tilpassede MX-post `contoso-com` for det brugerdefinerede domæne (f.eks. for domænet contoso.com). \<InitialDomain\> er det domæne, du brugte, da du tilmeldte dig Microsoft 365 (f.eks. contoso.onmicrosoft.com).

2. Når du har oprettet CNAME-posterne for dine brugerdefinerede domæner, skal du udføre følgende instruktioner:

   A. [log på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med din arbejds- eller skolekonto.

   B. Vælg ikonet for appstarteren øverst til venstre, og vælg **Administrator**.

   C. Udvid **Administrator** i navigationen nederst til venstre, og vælg **Exchange**.

   D. Gå til **Beskyttelse DKIM** > **DKIM**.

   E. Vælg domænet, og vælg derefter **Aktivér** for **signeringsmeddelelser for dette domæne med DKIM-signaturer**. Gentag dette trin for hvert brugerdefineret domæne.
