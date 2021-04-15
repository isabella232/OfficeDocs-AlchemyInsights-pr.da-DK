---
title: Bekræfte dit domæne
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770985"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a9858-102">Bekræfte dit domæne</span><span class="sxs-lookup"><span data-stu-id="a9858-102">Verify your domain</span></span>

 <span data-ttu-id="a9858-103">**Posten er sandsynligvis ikke opdateret på hele internettet.**</span><span class="sxs-lookup"><span data-stu-id="a9858-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a9858-104">Det tager typisk et par minutter for os at få vist den nye post, men nogle gange kan det tage op til et par timer.</span><span class="sxs-lookup"><span data-stu-id="a9858-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a9858-105">Hvis du allerede har ventet i lang tid, skal du kontrollere, at du har kopieret og indsat den nøjagtige værdi i TXT-bekræftelsesposten hos din DNS-vært.</span><span class="sxs-lookup"><span data-stu-id="a9858-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a9858-106">Ét almindelige problem er ikke omfatter "MS = " delen af posten.</span><span class="sxs-lookup"><span data-stu-id="a9858-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a9858-107">Vi har også brug for den!</span><span class="sxs-lookup"><span data-stu-id="a9858-107">We need that too!</span></span>

- <span data-ttu-id="a9858-108">Hos nogle DNS-værter skal du gemme zonefilen (hvor DNS-posten er gemt), så den bliver opdateret på hele internettet.</span><span class="sxs-lookup"><span data-stu-id="a9858-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a9858-109">Sørg for, at du har gemt dine ændringer, så Microsoft kan se og bekræfte posten.</span><span class="sxs-lookup"><span data-stu-id="a9858-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
