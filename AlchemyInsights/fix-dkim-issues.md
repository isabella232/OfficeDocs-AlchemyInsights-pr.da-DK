---
title: Løs problemer med dkim-opsætning
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506768"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="17892-102">Løs problemer med dkim-opsætning</span><span class="sxs-lookup"><span data-stu-id="17892-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="17892-103">Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, skal du følge nedenstående trin:</span><span class="sxs-lookup"><span data-stu-id="17892-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="17892-104">De fleste DKIM-installationsproblemer er relateret til forkerte DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="17892-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="17892-105">Kontroller, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt.</span><span class="sxs-lookup"><span data-stu-id="17892-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="17892-106">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="17892-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="17892-107">Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne (typisk dit domæneregistrator), skal du vente på, at DNS-posterne overføres.</span><span class="sxs-lookup"><span data-stu-id="17892-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="17892-108">Hvis du ikke kan oprette DKIM DNS-posterne i Administration, kan du erstatte \<CustomDomain\> med dit brugerdefinerede domæne (f.eks. contoso.com) og køre denne kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="17892-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
