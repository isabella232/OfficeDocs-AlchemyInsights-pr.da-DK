---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488511"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="c0022-102">Arbejde med store lister og biblioteker i SharePoint</span><span class="sxs-lookup"><span data-stu-id="c0022-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="c0022-103">SharePoint-lister og-biblioteker kan indeholde op til 30.000.000 elementer, men når de har mere end 5.000 elementer, får du muligvis vist en tærskel fejl for listevisning, når du forsøger at arbejde med dem.</span><span class="sxs-lookup"><span data-stu-id="c0022-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="c0022-104">Denne tærskel er på plads for at opretholde ydelsen af tjenesten.</span><span class="sxs-lookup"><span data-stu-id="c0022-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="c0022-105">Det kan ikke ændres.</span><span class="sxs-lookup"><span data-stu-id="c0022-105">It can't be changed.</span></span> <span data-ttu-id="c0022-106">For at undgå at ramme denne tærskel:</span><span class="sxs-lookup"><span data-stu-id="c0022-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="c0022-107">**Bruge moderne**</span><span class="sxs-lookup"><span data-stu-id="c0022-107">**Use modern**</span></span>

<span data-ttu-id="c0022-108">Visninger, der viser mange elementer, fungerer bedst i den moderne oplevelse.</span><span class="sxs-lookup"><span data-stu-id="c0022-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="c0022-109">[Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) for at undgå fejl, du kan se i den klassiske oplevelse.</span><span class="sxs-lookup"><span data-stu-id="c0022-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="c0022-110">**Tilføje indekser**</span><span class="sxs-lookup"><span data-stu-id="c0022-110">**Add indexes**</span></span>

<span data-ttu-id="c0022-111">Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, vises der muligvis en fejlmeddelelse.</span><span class="sxs-lookup"><span data-stu-id="c0022-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="c0022-112">[Tilføj et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i menuen Indstillinger og derefter **Indekserede kolonner**.</span><span class="sxs-lookup"><span data-stu-id="c0022-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="c0022-113">**Redigere listevisningen**</span><span class="sxs-lookup"><span data-stu-id="c0022-113">**Edit the list view**</span></span>

<span data-ttu-id="c0022-114">Hvis der opstår en fejl, når du arbejder med en stor liste, bør du [redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="c0022-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="c0022-115">De følgende fire ændringer vil fjerne tærskel fejl for listevisning.</span><span class="sxs-lookup"><span data-stu-id="c0022-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="c0022-116">Foretag alle fire ændringer for at fjerne alle fejl.</span><span class="sxs-lookup"><span data-stu-id="c0022-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="c0022-117">Hvis du stadig får fejl, skal du kontrollere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="c0022-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="c0022-118">Vælg **ingen** fra begge **første sorter efter kolonnen** , og **Sortér derefter efter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="c0022-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="c0022-119">Vælg **ingen** fra begge **første grupper efter kolonnen** , og **Gruppér derefter efter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="c0022-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="c0022-120">Vælg **ingen** for alle kolonner i afsnittet **Totaler** .</span><span class="sxs-lookup"><span data-stu-id="c0022-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="c0022-121">Fravælg alle, men én kolonne til visning fra sektionen **kolonner** .</span><span class="sxs-lookup"><span data-stu-id="c0022-121">Deselect all but one column for display from the **Columns** section.</span></span>

