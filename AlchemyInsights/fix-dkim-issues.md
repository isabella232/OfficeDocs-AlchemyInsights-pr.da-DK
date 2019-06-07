---
title: Løse problemer med installationen af DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764955"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="3eade-102">Løse problemer med installationen af DKIM</span><span class="sxs-lookup"><span data-stu-id="3eade-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="3eade-103">Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, kan du bruge følgende trin:</span><span class="sxs-lookup"><span data-stu-id="3eade-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="3eade-104">De fleste problemer med installationen af DKIM er relateret til forkert DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="3eade-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="3eade-105">Kontroller, at DKIM CNAME-posten (**ikke** en TXT-post) er formateret korrekt.</span><span class="sxs-lookup"><span data-stu-id="3eade-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="3eade-106">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="3eade-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="3eade-107">Når du opretter eller opdaterer din DKIM DNS-poster på DNS-værtstjeneste for dit domæne (typisk din domæneregistrator), venter på DNS-poster til at sprede.</span><span class="sxs-lookup"><span data-stu-id="3eade-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="3eade-108">Hvis du ikke kan oprette DKIM DNS poster i admin center, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (for eksempel contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="3eade-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
