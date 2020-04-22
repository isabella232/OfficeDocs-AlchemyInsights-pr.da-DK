---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709221"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a77c5-102">Indholdssøgning returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="a77c5-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a77c5-103">Når du kører Indholdssøgninger fra Microsoft 365-sikkerhedskontrollen & Overholdelsescenter, modtager du muligvis uventede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="a77c5-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a77c5-104">Overvej følgende ting, der kan påvirke dine søgeresultater:</span><span class="sxs-lookup"><span data-stu-id="a77c5-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a77c5-105">**Indholdsplaceringer og søgebetingelser**: Sørg for, at du har valgt de korrekte indholdsplaceringer og søgebetingelser.</span><span class="sxs-lookup"><span data-stu-id="a77c5-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a77c5-106">Hvis du har kørt en stor søgning (med mange placeringer), kan du overveje at opdele den i flere søgninger.</span><span class="sxs-lookup"><span data-stu-id="a77c5-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a77c5-107">**Delvist indekserede elementer**: [Delvist indekserede elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postkasser medtages i de estimerede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="a77c5-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a77c5-108">Delvist indekserede elementer fra websteder i SharePoint og OneDrive medtages dog ikke i søgeestimatet.</span><span class="sxs-lookup"><span data-stu-id="a77c5-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a77c5-109">**Søgefejl**: Når du søger i et stort antal postkasser (over 100.000 postkasser), kan du få søgefejl med fejlkoder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="a77c5-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a77c5-110">I dette tilfælde skal du kun prøve at søge efter de fejlbehæftede indholdsplaceringer igen.</span><span class="sxs-lookup"><span data-stu-id="a77c5-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a77c5-111">Se [denne artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="a77c5-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
