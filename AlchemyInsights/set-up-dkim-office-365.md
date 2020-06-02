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
# <a name="setup-dkim"></a><span data-ttu-id="b98cb-102">Opsætning DKIM</span><span class="sxs-lookup"><span data-stu-id="b98cb-102">Setup DKIM</span></span>

<span data-ttu-id="b98cb-103">Den komplette vejledning til konfiguration af DKIM for brugerdefinerede domæner i Microsoft 365 findes [her](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="b98cb-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="b98cb-104">For **hvert** brugerdefineret domæne skal du oprette **to** DKIM CNAME-poster hos domænets DNS-hostingtjeneste (typisk domæneregistratoren).</span><span class="sxs-lookup"><span data-stu-id="b98cb-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="b98cb-105">for eksempel kræver contoso.com og fourthcoffee.com fire DKIM CNAME-poster: to for contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="b98cb-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="b98cb-106">DKIM CNAME-posterne for **hvert** brugerdefineret domæne bruger følgende formater:</span><span class="sxs-lookup"><span data-stu-id="b98cb-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="b98cb-107">**Værtsnavn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b98cb-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b98cb-108">**Peger på adresse eller værdi:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b98cb-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b98cb-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b98cb-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="b98cb-110">**Værtsnavn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b98cb-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b98cb-111">**Peger på adresse eller værdi:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b98cb-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b98cb-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b98cb-112">**TTL**: 3600</span></span>

   <span data-ttu-id="b98cb-113">\<DomainGUID\>er teksten til venstre for `.mail.protection.outlook.com` i den tilpassede MX-post for det brugerdefinerede domæne (f.eks. `contoso-com` for det contoso.com domæne).</span><span class="sxs-lookup"><span data-stu-id="b98cb-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="b98cb-114">\<InitialDomain\>er det domæne, du brugte, da du tilmeldte dig Microsoft 365 (f.eks. contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="b98cb-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="b98cb-115">Når du har oprettet CNAME-posterne for dine brugerdefinerede domæner, skal du udfylde følgende instruktioner:</span><span class="sxs-lookup"><span data-stu-id="b98cb-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="b98cb-116">a.</span><span class="sxs-lookup"><span data-stu-id="b98cb-116">a.</span></span> <span data-ttu-id="b98cb-117">[logge på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med din arbejds- eller skolekonto.</span><span class="sxs-lookup"><span data-stu-id="b98cb-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="b98cb-118">b.</span><span class="sxs-lookup"><span data-stu-id="b98cb-118">b.</span></span> <span data-ttu-id="b98cb-119">Vælg ikonet for appstarteren øverst til venstre, og vælg **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="b98cb-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="b98cb-120">c.</span><span class="sxs-lookup"><span data-stu-id="b98cb-120">c.</span></span> <span data-ttu-id="b98cb-121">I navigationen nederst til venstre skal du udvide **Administrator** og vælge **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b98cb-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="b98cb-122">D.</span><span class="sxs-lookup"><span data-stu-id="b98cb-122">d.</span></span> <span data-ttu-id="b98cb-123">Gå til **Beskyttelse**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b98cb-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="b98cb-124">E.</span><span class="sxs-lookup"><span data-stu-id="b98cb-124">e.</span></span> <span data-ttu-id="b98cb-125">Vælg domænet, og vælg derefter **Aktivér** for **Signer meddelelser for dette domæne med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="b98cb-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="b98cb-126">Gentag dette trin for hvert brugerdefineret domæne.</span><span class="sxs-lookup"><span data-stu-id="b98cb-126">Repeat this step for each custom domain.</span></span>
