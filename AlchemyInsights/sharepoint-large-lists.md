---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720127"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="2e512-102">Arbejde med store lister og biblioteker i SharePoint</span><span class="sxs-lookup"><span data-stu-id="2e512-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="2e512-103">SharePoint-lister og-biblioteker kan indeholde op til 30.000.000 elementer, men når de har mere end 5.000 elementer, får du muligvis vist en grænseværdi for listevisning, når du forsøger at arbejde med dem.</span><span class="sxs-lookup"><span data-stu-id="2e512-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="2e512-104">Denne grænseværdi er der for at opretholde tjenestens ydeevne.</span><span class="sxs-lookup"><span data-stu-id="2e512-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="2e512-105">Den kan ikke ændres.</span><span class="sxs-lookup"><span data-stu-id="2e512-105">It can't be changed.</span></span> <span data-ttu-id="2e512-106">Sådan undgår du at bruge denne grænse:</span><span class="sxs-lookup"><span data-stu-id="2e512-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="2e512-107">**Brug moderne**</span><span class="sxs-lookup"><span data-stu-id="2e512-107">**Use modern**</span></span>

<span data-ttu-id="2e512-108">Visninger, der viser mange elementer, fungerer bedst i den moderne oplevelse.</span><span class="sxs-lookup"><span data-stu-id="2e512-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="2e512-109">[Brug den moderne oplevelse](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til at undgå fejl, du kan se i den klassiske oplevelse.</span><span class="sxs-lookup"><span data-stu-id="2e512-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="2e512-110">**Tilføje indeks**</span><span class="sxs-lookup"><span data-stu-id="2e512-110">**Add indexes**</span></span>

<span data-ttu-id="2e512-111">Når du filtrerer eller sorterer efter en kolonne, der ikke har et indeks, får du muligvis vist en fejlmeddelelse.</span><span class="sxs-lookup"><span data-stu-id="2e512-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="2e512-112">[Tilføje et indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **Listeindstillinger** i menuen Indstillinger og derefter **Indekserede kolonner**.</span><span class="sxs-lookup"><span data-stu-id="2e512-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="2e512-113">**Redigere listevisningen**</span><span class="sxs-lookup"><span data-stu-id="2e512-113">**Edit the list view**</span></span>

<span data-ttu-id="2e512-114">Hvis der opstår en fejl, når du arbejder med en stor liste, skal du [redigere listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="2e512-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="2e512-115">De følgende fire ændringer fjerner fejl i liste visnings tærskelværdien.</span><span class="sxs-lookup"><span data-stu-id="2e512-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="2e512-116">Gør alle fire ændringer for at fjerne alle fejl.</span><span class="sxs-lookup"><span data-stu-id="2e512-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="2e512-117">Hvis du stadig får fejl, skal du kontrollere [Administrer store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="2e512-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="2e512-118">Markér **ingen** fra både **den første sortering efter kolonnen** , og **Sortér derefter efter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="2e512-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="2e512-119">Markér **ingen** af dem **først i den første gruppe efter kolonne** , og **Gruppér efter kolonne**.</span><span class="sxs-lookup"><span data-stu-id="2e512-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="2e512-120">Vælg **ingen** for alle kolonner i sektionen **Totaler** .</span><span class="sxs-lookup"><span data-stu-id="2e512-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="2e512-121">Fjern markeringen af alle kolonnerne undtagen én, der skal vises i sektionen **kolonner** .</span><span class="sxs-lookup"><span data-stu-id="2e512-121">Deselect all but one column for display from the **Columns** section.</span></span>

