---
title: Konfigurer DKIM med brugerdefinerede domæner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744091"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="2dc64-102">Konfigurer DKIM med brugerdefinerede domæner</span><span class="sxs-lookup"><span data-stu-id="2dc64-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="2dc64-103">Du skal publicere to CNAME-poster for hvert brugerdefineret domæne i DNS.</span><span class="sxs-lookup"><span data-stu-id="2dc64-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="2dc64-104">Det gør du ved at bruge følgende format:</span><span class="sxs-lookup"><span data-stu-id="2dc64-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="2dc64-105">**DomainGUID** er teksten til venstre for **.mail.protection.outlook.com** i den brugerdefinerede MX-post for det brugerdefinerede domæne (f.eks. contoso-com for **domænet contoso.com).**</span><span class="sxs-lookup"><span data-stu-id="2dc64-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="2dc64-106">**InitialDomain er** det domæne, du brugte, da du tilmeldte dig Office 365 (f.eks. **contoso.onmicrosoft.com).**</span><span class="sxs-lookup"><span data-stu-id="2dc64-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="2dc64-107">Du kan finde flere oplysninger om DNS-poster [under Opret DNS-poster for Office 365 hos enhver DNS-udbyder.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="2dc64-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>