---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767279"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="18040-102">Arbejde med store lister og biblioteker i SharePoint</span><span class="sxs-lookup"><span data-stu-id="18040-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="18040-103">SharePoint-lister og -biblioteker kan indeholde op til 30 millioner elementer, men når de har mere end 5.000 elementer, får du muligvis vist en listevisningstærskelfejl, når du forsøger at arbejde med dem.</span><span class="sxs-lookup"><span data-stu-id="18040-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="18040-104">Denne grænseværdi er der for at opretholde tjenestens ydeevne.</span><span class="sxs-lookup"><span data-stu-id="18040-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="18040-105">Den kan ikke ændres.</span><span class="sxs-lookup"><span data-stu-id="18040-105">It can't be changed.</span></span> <span data-ttu-id="18040-106">Sådan undgår du at ramme denne grænse:</span><span class="sxs-lookup"><span data-stu-id="18040-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="18040-107">**Brug moderne**</span><span class="sxs-lookup"><span data-stu-id="18040-107">**Use modern**</span></span>

<span data-ttu-id="18040-108">Visninger, der viser mange ting fungerer bedst i den moderne oplevelse.</span><span class="sxs-lookup"><span data-stu-id="18040-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="18040-109">[Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til at undgå fejl, du kan se i den klassiske oplevelse.</span><span class="sxs-lookup"><span data-stu-id="18040-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="18040-110">**Tilføje indeks**</span><span class="sxs-lookup"><span data-stu-id="18040-110">**Add indexes**</span></span>

<span data-ttu-id="18040-111">Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, vises der muligvis en fejlmeddelelse.</span><span class="sxs-lookup"><span data-stu-id="18040-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="18040-112">[Tilføj et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i indstillingsmenuen og derefter **indekserede kolonner**.</span><span class="sxs-lookup"><span data-stu-id="18040-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="18040-113">**Redigere listevisningen**</span><span class="sxs-lookup"><span data-stu-id="18040-113">**Edit the list view**</span></span>

<span data-ttu-id="18040-114">Hvis der opstår en fejl, når du arbejder med en stor liste, skal [du redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="18040-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="18040-115">Følgende fire ændringer fjerner listevisningstærskelfejl.</span><span class="sxs-lookup"><span data-stu-id="18040-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="18040-116">Foretag alle fire ændringer for at fjerne alle fejl.</span><span class="sxs-lookup"><span data-stu-id="18040-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="18040-117">Hvis du stadig får fejl, skal du markere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="18040-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="18040-118">Vælg **Ingen** fra både **Første sortering efter kolonne** og Sorter derefter efter **kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="18040-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="18040-119">Vælg **Ingen** fra både **første gruppe efter kolonne** og derefter **grupperefter kolonne**.</span><span class="sxs-lookup"><span data-stu-id="18040-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="18040-120">Vælg **Ingen** for alle kolonner i sektionen **Totaler.**</span><span class="sxs-lookup"><span data-stu-id="18040-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="18040-121">Fravælg alle kolonner undtagen én, der skal vises, i sektionen **Kolonner.**</span><span class="sxs-lookup"><span data-stu-id="18040-121">Deselect all but one column for display from the **Columns** section.</span></span>

