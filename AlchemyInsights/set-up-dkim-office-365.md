---
title: Setup DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108550"
---
# <a name="setup-dkim"></a>Setup DKIM

De komplette instruktioner til konfiguration af DKIM for brugerdefinerede domæner i Microsoft 365 er [her.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. For **hvert** brugerdefineret domæne skal du oprette to **DKIM** CNAME-poster hos domænets DNS-værtstjeneste (typisk domæneregistratoren). Eksempelvis kræver contoso.com og fourthcoffee.com DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.

   DKIM CNAME-posterne for **hvert** brugerdefinerede domæne bruger følgende formater:

   - **Værtsnavn:**`selector1._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Værtsnavn:**`selector2._domainkey.<CustomDomain>`

     **Peger på adresse eller værdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> er teksten til venstre for den brugerdefinerede MX-post for det brugerdefinerede domæne `.mail.protection.outlook.com` `contoso-com` (f.eks. for contoso.com). \<InitialDomain\>er det domæne, du brugte, da du tilmeldte dig Microsoft 365 (f.eks. contoso.onmicrosoft.com).

2. Når du har oprettet CNAME-posterne for dine brugerdefinerede domæner, skal du følge disse instruktioner:

   a. [logge på Microsoft 365 med](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) din arbejds- eller skolekonto.

   b. Vælg ikonet for appstarteren øverst til venstre, og vælg **Administrator**.

   c. I navigationen nederst til venstre skal du **udvide Administrator** og **vælge Exchange**.

   d. Gå til **Beskyttelse**  >  **DKIM.**

   e. Vælg domænet, og vælg derefter **Aktivér** for **Signer meddelelser for dette domæne med DKIM-signaturer.** Gentag dette trin for hvert brugerdefinerede domæne.
