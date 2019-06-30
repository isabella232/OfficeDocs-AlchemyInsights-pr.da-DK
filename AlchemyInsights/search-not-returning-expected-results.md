---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355871"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="82a29-102">Indhold søgning returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="82a29-102">Content Search not returning expected results</span></span>

<span data-ttu-id="82a29-103">Når du kører søgninger indhold fra Office 365-sikkerhed & Overholdelsescenter, vises der muligvis uventet søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="82a29-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="82a29-104">Overvej følgende ting, der kan påvirke dine søgeresultater:</span><span class="sxs-lookup"><span data-stu-id="82a29-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="82a29-105">**Indholdssteder og søgebetingelser**: Kontroller, at du har valgt de korrekte indhold placeringer og søgebetingelser.</span><span class="sxs-lookup"><span data-stu-id="82a29-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="82a29-106">Hvis du har kørt en stor søgning (med mange steder), kan du overveje at opdele det i flere søgninger.</span><span class="sxs-lookup"><span data-stu-id="82a29-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="82a29-107">**Delvist indekserede elementer**: [delvist indekserede elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postkasser er inkluderet i de anslåede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="82a29-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="82a29-108">Delvist indekserede elementer fra websteder i SharePoint- og OneDrive medtages dog ikke i estimatet søgning.</span><span class="sxs-lookup"><span data-stu-id="82a29-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="82a29-109">**Søg fejl**: Når du søger efter et stort antal postkasser (mere end 100.000 postkasser), kan du få search-fejl med fejlkoderne som CS008-009- og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="82a29-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="82a29-110">Prøv i så fald Søg kun efter de mislykkede indholdssteder.</span><span class="sxs-lookup"><span data-stu-id="82a29-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="82a29-111">Se [denne artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="82a29-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
