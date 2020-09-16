---
title: Ret DKIM-konfigurationsproblemer
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744944"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="82081-102">Ret DKIM-konfigurationsproblemer</span><span class="sxs-lookup"><span data-stu-id="82081-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="82081-103">Hvis du oplever problemer med at aktivere DKIM til dit brugerdefinerede domæne, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="82081-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="82081-104">De fleste DKIM-konfigurationsproblemer er relateret til forkerte DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="82081-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="82081-105">Kontrollér, at posten DKIM CNAME (**ikke** en TXT-post) er formateret korrekt.</span><span class="sxs-lookup"><span data-stu-id="82081-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="82081-106">Du kan finde flere oplysninger i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="82081-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="82081-107">Når du har oprettet eller opdateret dine DKIM DNS-poster hos DNS-værtstjenesten for dit domæne (typisk en domæneregistrator), skal du vente på, at DNS-posterne skal overføres.</span><span class="sxs-lookup"><span data-stu-id="82081-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="82081-108">Hvis du ikke kan oprette DKIM DNS-poster i administration, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (f. eks contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="82081-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
