---
title: 1491 – søgning-ikke-returnerede – forventede-resultater
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740468"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e2bc1-102">Indholdssøgning returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="e2bc1-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e2bc1-103">Når du kører indholds søgninger fra Microsoft 365 Security & Compliance Center, får du muligvis uventede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e2bc1-104">Overvej følgende ting, der kan påvirke søgeresultaterne:</span><span class="sxs-lookup"><span data-stu-id="e2bc1-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e2bc1-105">**Indholds placeringer og søgebetingelser**: Sørg for, at du har valgt de korrekte indholds placeringer og søgebetingelserne.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e2bc1-106">Hvis du har kørt en stor søgning (med mange placeringer), kan du overveje at opdele den i flere søgninger.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e2bc1-107">**Delvist indekserede elementer**:  [delvist indekserede elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postkasser medtages i de anslåede søgeresultater.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e2bc1-108">Delvist indekserede elementer fra websteder i SharePoint og OneDrive medtages dog ikke i søge estimatet.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e2bc1-109">**Søgefejl**: når du søger i et stort antal postkasser (over 100.000-postkasser), kan du få søgefejl med fejlkoder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="e2bc1-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e2bc1-110">I dette tilfælde kan du prøve kun at søge efter de mislykkede indholds placeringer.</span><span class="sxs-lookup"><span data-stu-id="e2bc1-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e2bc1-111">Du kan finde flere oplysninger i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="e2bc1-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
