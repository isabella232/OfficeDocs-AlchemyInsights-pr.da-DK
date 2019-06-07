---
title: Opsætning af DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764967"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="288a0-102">Opsætning af DKIM i Office 365</span><span class="sxs-lookup"><span data-stu-id="288a0-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="288a0-103">Komplet vejledning til konfiguration af DKIM til brugerdefinerede domæner i Office 365 er [her](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="288a0-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="288a0-104">For **hver** brugerdefineret domæne skal du oprette **to** DKIM CNAME-post i domænets DNS-værtstjeneste (typisk domæneregistrator).</span><span class="sxs-lookup"><span data-stu-id="288a0-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="288a0-105">For eksempel contoso.com og fourthcoffee.com kræver fire DKIM CNAME-poster: to til contoso.com og to for fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="288a0-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="288a0-106">DKIM CNAME-poster for **hver** brugerdefineret domæne kan bruge følgende formater:</span><span class="sxs-lookup"><span data-stu-id="288a0-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="288a0-107">**Host-navn**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="288a0-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="288a0-108">**Peger på adresse eller værdi**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="288a0-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="288a0-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="288a0-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="288a0-110">**Host-navn**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="288a0-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="288a0-111">**Peger på adresse eller værdi**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="288a0-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="288a0-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="288a0-112">**TTL**: 3600</span></span>

   <span data-ttu-id="288a0-113">\<DomainGUID\> tekst til venstre for `.mail.protection.outlook.com` i tilpassede MX-posten for custom Domains (for eksempel `contoso-com` med domænet Contoso.com).</span><span class="sxs-lookup"><span data-stu-id="288a0-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="288a0-114">\<InitialDomain\> , er det domæne, du brugte, da du tilmeldte dig Office 365 (for eksempel contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="288a0-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="288a0-115">Når du har oprettet CNAME-poster til dine brugerdefinerede domæner, kan du udføre følgende instruktioner:</span><span class="sxs-lookup"><span data-stu-id="288a0-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="288a0-116">en.</span><span class="sxs-lookup"><span data-stu-id="288a0-116">a.</span></span> <span data-ttu-id="288a0-117">[Log på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med kontoen arbejdet eller skolen.</span><span class="sxs-lookup"><span data-stu-id="288a0-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="288a0-118">b.</span><span class="sxs-lookup"><span data-stu-id="288a0-118">b.</span></span> <span data-ttu-id="288a0-119">Vælg ikonet app Opgavestarter øverst til venstre, og vælg **Admin**.</span><span class="sxs-lookup"><span data-stu-id="288a0-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="288a0-120">c.</span><span class="sxs-lookup"><span data-stu-id="288a0-120">c.</span></span> <span data-ttu-id="288a0-121">Udvid **Admin** i det nederste venstre navigationspanel, og vælg **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="288a0-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="288a0-122">d.</span><span class="sxs-lookup"><span data-stu-id="288a0-122">d.</span></span> <span data-ttu-id="288a0-123">Gå til **beskyttelse af** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="288a0-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="288a0-124">e.</span><span class="sxs-lookup"><span data-stu-id="288a0-124">e.</span></span> <span data-ttu-id="288a0-125">Vælg domænet, og vælg derefter **Aktiver** for **Log-meddelelser til dette domæne med DKIM-signaturer**.</span><span class="sxs-lookup"><span data-stu-id="288a0-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="288a0-126">Gentag dette trin for hvert brugerdefinerede domæne.</span><span class="sxs-lookup"><span data-stu-id="288a0-126">Repeat this step for each custom domain.</span></span>
