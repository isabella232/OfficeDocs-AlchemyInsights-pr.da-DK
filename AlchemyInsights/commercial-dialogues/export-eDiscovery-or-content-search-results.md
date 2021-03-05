---
title: Eksportere resultater fra eDiscovery/indholdssøgning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481729"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="e9ed3-102">Eksportere resultater fra eDiscovery/indholdssøgning</span><span class="sxs-lookup"><span data-stu-id="e9ed3-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="e9ed3-103">Det kan være nødvendigt at eksportere søgeresultaterne til en PST-fil (fra mail) eller til oprindelige Office-dokumenter (fra SharePoint- og OneDrive for Business-websteder).</span><span class="sxs-lookup"><span data-stu-id="e9ed3-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="e9ed3-104">Hvis det er nødvendigt, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="e9ed3-104">If so, do the following:</span></span>

- <span data-ttu-id="e9ed3-105">Sørg for, at din konto er tildelt de rette tilladelser til at eksportere.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="e9ed3-106">Du kan finde flere oplysninger under [Tildel eDiscovery-tilladelse.](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="e9ed3-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="e9ed3-107">Sørg for, at computeren har opfyldt [alle krav.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="e9ed3-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="e9ed3-108">Ikke alle browsere understøttes, f.eks. Chrome.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="e9ed3-109">Sådan eksporteres fra en indholdssøgning: a.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-109">To export from a Content Search: a.</span></span> <span data-ttu-id="e9ed3-110">Gå til [Sikkerheds- &, og](https://protection.office.com/contentsearch) klik på **Søg,** og vælg derefter **Indholdssøgning.**</span><span class="sxs-lookup"><span data-stu-id="e9ed3-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="e9ed3-111">Vælg en **gemt søgning** på siden Indholdssøgning.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="e9ed3-112">b.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-112">b.</span></span> <span data-ttu-id="e9ed3-113">Vælg **Start** eksport i detaljeruden under **Eksportér resultater** til en computer.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="e9ed3-114">Hvis du eksporterer mere end 100.000 postkasser, skal du bruge PowerShell til at hente eksportresultaterne.</span><span class="sxs-lookup"><span data-stu-id="e9ed3-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="e9ed3-115">Du kan finde flere oplysninger i [Eksportere resultater fra mere end 100.000 postkasser.](https://go.microsoft.com/fwlink/?linkid=2143861)</span><span class="sxs-lookup"><span data-stu-id="e9ed3-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="e9ed3-116">Du kan få mere at vide under [Eksportér søgeresultater for indhold.](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="e9ed3-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>