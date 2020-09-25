---
title: 1490 – fejlfinding – eDiscovery-fejl
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277813"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="06aab-102">Fejlfinding af indholds søgefejl</span><span class="sxs-lookup"><span data-stu-id="06aab-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="06aab-103">Oplever du problemer med at søge efter indhold eller få fejl, når du eksporterer søgeresultater?</span><span class="sxs-lookup"><span data-stu-id="06aab-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="06aab-104">For eksempel modtager du følgende, når du kører søgninger?</span><span class="sxs-lookup"><span data-stu-id="06aab-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="06aab-105">CS008-eller CS012-fejl</span><span class="sxs-lookup"><span data-stu-id="06aab-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="06aab-106">Fejl på serveren er optaget/timeout</span><span class="sxs-lookup"><span data-stu-id="06aab-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="06aab-107">Der opstod en programfejl</span><span class="sxs-lookup"><span data-stu-id="06aab-107">Application error occurred</span></span>

<span data-ttu-id="06aab-108">Eller når du søger efter eller eksporterer resultater fra et stort antal postkasser (over 100.000-postkasser), får du eksport fejl?</span><span class="sxs-lookup"><span data-stu-id="06aab-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="06aab-109">For disse fejltyper kan du prøve at søge efter de indholdssteder, der er mislykket.</span><span class="sxs-lookup"><span data-stu-id="06aab-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="06aab-110">Du kan finde flere oplysninger i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="06aab-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="06aab-111">Hvis du eksporterer mere end 100K-postkasser, skal du bruge følgende PowerShell til at downloade eksportresultaterne:  [eksportere resultater fra mere end 100K postkasser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="06aab-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
