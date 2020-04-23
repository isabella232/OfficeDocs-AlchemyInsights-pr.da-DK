---
title: Løs problemer med Konfiguration af DKIM
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717556"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="ce3b4-102">Løs problemer med Konfiguration af DKIM</span><span class="sxs-lookup"><span data-stu-id="ce3b4-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="ce3b4-103">Hvis du oplever problemer med at aktivere DKIM for dit brugerdefinerede domæne, skal du følge følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="ce3b4-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="ce3b4-104">De fleste DKIM-installationsproblemer er relateret til forkerte DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="ce3b4-105">Kontroller, at DKIM CNAME-posten **(ikke** en TXT-post) er formateret korrekt.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="ce3b4-106">Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="ce3b4-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="ce3b4-107">Når du har oprettet eller opdateret dine DKIM DNS-poster på DNS-hostingtjenesten for dit domæne (typisk din domæneregistrator), skal du vente på, at DNS-posterne overføres.</span><span class="sxs-lookup"><span data-stu-id="ce3b4-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="ce3b4-108">Hvis du ikke kan oprette DKIM DNS-posterne i \<Administration, kan du erstatte CustomDomain\> med dit brugerdefinerede domæne `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`(f.eks. contoso.com) og køre denne kommando i Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .</span><span class="sxs-lookup"><span data-stu-id="ce3b4-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
