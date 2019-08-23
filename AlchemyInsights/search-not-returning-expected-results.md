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
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551409"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="eee69-102">Indhold søgning returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="eee69-102">Content Search not returning expected results</span></span>

<span data-ttu-id="eee69-103">Når du kører søgninger indhold fra Office 365-sikkerhed & Overholdelsescenter, vises der muligvis uventet søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="eee69-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="eee69-104">Overvej følgende ting, der kan påvirke dine søgeresultater:</span><span class="sxs-lookup"><span data-stu-id="eee69-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="eee69-105">**Indholdssteder og søgebetingelser**: Kontroller, at du har valgt de korrekte indhold placeringer og søgebetingelser.</span><span class="sxs-lookup"><span data-stu-id="eee69-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="eee69-106">Hvis du har kørt en stor søgning (med mange steder), kan du overveje at opdele det i flere søgninger.</span><span class="sxs-lookup"><span data-stu-id="eee69-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="eee69-107">**Delvist indekserede elementer**: [delvist indekserede elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postkasser er inkluderet i de anslåede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="eee69-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="eee69-108">Delvist indekserede elementer fra websteder i SharePoint- og OneDrive medtages dog ikke i estimatet søgning.</span><span class="sxs-lookup"><span data-stu-id="eee69-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="eee69-109">**Søg fejl**: Når du søger efter et stort antal postkasser (mere end 100.000 postkasser), kan du få search-fejl med fejlkoderne som CS008-009- og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="eee69-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="eee69-110">Prøv i så fald Søg kun efter de mislykkede indholdssteder.</span><span class="sxs-lookup"><span data-stu-id="eee69-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="eee69-111">Se [denne artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="eee69-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
