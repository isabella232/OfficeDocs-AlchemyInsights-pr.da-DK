---
title: Bekræfte dit domæne
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710437"
---
# <a name="verify-your-domain"></a><span data-ttu-id="e04c0-102">Bekræfte dit domæne</span><span class="sxs-lookup"><span data-stu-id="e04c0-102">Verify your domain</span></span>

 <span data-ttu-id="e04c0-103">**Posten har sandsynligvis ikke opdateret på internettet.**</span><span class="sxs-lookup"><span data-stu-id="e04c0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="e04c0-104">Det tager typisk kun et par minutter for os at kunne se den nye rekord, men lejlighedsvis kan det tage så lang tid som et par timer.</span><span class="sxs-lookup"><span data-stu-id="e04c0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="e04c0-105">Hvis du allerede har ventet så længe, skal du dobbelttjekke, at du har kopieret og indsat den nøjagtige værdi i TXT-bekræftelsesposten hos din DNS-vært.</span><span class="sxs-lookup"><span data-stu-id="e04c0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="e04c0-106">Et almindeligt problem er ikke at medtage delen "MS=" af posten.</span><span class="sxs-lookup"><span data-stu-id="e04c0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="e04c0-107">Det har vi også brug for!</span><span class="sxs-lookup"><span data-stu-id="e04c0-107">We need that too!</span></span>

- <span data-ttu-id="e04c0-108">På nogle DNS-værter skal du tage et ekstra skridt for at gemme zonefilen (hvor DNS-posten er gemt), så den opdateres via internettet.</span><span class="sxs-lookup"><span data-stu-id="e04c0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="e04c0-109">Sørg for, at du har gemt ændringerne, så Microsoft kan se og bekræfte posten.</span><span class="sxs-lookup"><span data-stu-id="e04c0-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
