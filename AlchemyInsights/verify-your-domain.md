---
title: Bekræfte dit domæne
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734300"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4f9cd-102">Bekræfte dit domæne</span><span class="sxs-lookup"><span data-stu-id="4f9cd-102">Verify your domain</span></span>

 <span data-ttu-id="4f9cd-103">**Posten er sandsynligvis ikke blevet opdateret på internettet.**</span><span class="sxs-lookup"><span data-stu-id="4f9cd-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4f9cd-104">Det tager normalt kun et par minutter, før vi kan se den nye post, men nogle gange kan det tage op til et par timer.</span><span class="sxs-lookup"><span data-stu-id="4f9cd-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4f9cd-105">Hvis du har ventet på, at du allerede har gjort det, skal du dobbelttjekke, at du har kopieret og indsat den nøjagtige værdi i TXT-bekræftelses posten hos din DNS-vært.</span><span class="sxs-lookup"><span data-stu-id="4f9cd-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4f9cd-106">Et almindeligt problem omfatter ikke "MS ="-delen af posten.</span><span class="sxs-lookup"><span data-stu-id="4f9cd-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4f9cd-107">Vi har brug for!</span><span class="sxs-lookup"><span data-stu-id="4f9cd-107">We need that too!</span></span>

- <span data-ttu-id="4f9cd-108">På nogle DNS-værter skal du udføre et ekstra trin for at gemme zone filen (hvor DNS-posten er gemt), så den bliver opdateret på internettet.</span><span class="sxs-lookup"><span data-stu-id="4f9cd-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4f9cd-109">Sørg for, at du har gemt dine ændringer, så Microsoft kan se og bekræfte posten.</span><span class="sxs-lookup"><span data-stu-id="4f9cd-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
