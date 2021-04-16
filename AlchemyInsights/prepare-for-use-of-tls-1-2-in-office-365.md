---
title: Forberedelse til brug af TLS 1.2 i Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085898"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="acb69-102">Forberedelse til brug af TLS 1.2 i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="acb69-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="acb69-103">Pr. 31. oktober 2018 fortsætter Microsoft 365 overgangen til TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="acb69-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="acb69-104">Pr. 15. oktober 2020 begynder udrådningen af TLS 1.0 og 1.1 på tværs af tjenesten.</span><span class="sxs-lookup"><span data-stu-id="acb69-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="acb69-105">Rullen af denne ændring vil fortsætte i løbet af de næste par uger og måneder, men kunder bør antage, at ingen TLS 1.0/1.1-opkald vil fungere, når de interagerer med O365 fra den 15. oktober 2020.</span><span class="sxs-lookup"><span data-stu-id="acb69-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="acb69-106">Som det tidligere er meddelt (MC126199 i dec 2017, MC128929 i februar 2018, MC186827 i juli 2019 og MC218794 i juli 2020) flytter alle vores onlinetjenester til Transport Layer Security (TLS) 1.2+ for at levere førsteklasses kryptering og for at sikre, at vores tjeneste som standard er mere sikker.</span><span class="sxs-lookup"><span data-stu-id="acb69-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="acb69-107">Kunder kan stadig vælge at have TLS 1.0/1.1 på deres servere og ressourcer, men de skal antage, at det kun er TLS 1.2 eller nyere, der fungerer, når de interagerer med O365-ressourcer.</span><span class="sxs-lookup"><span data-stu-id="acb69-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="acb69-108">Du kan få mere at vide om disse ændringer [her](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) og [her.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="acb69-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  