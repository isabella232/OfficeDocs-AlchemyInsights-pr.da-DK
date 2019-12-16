---
title: Fejlfinding af fejl 404, filen blev ikke fundet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 6c23d7c482e3beb900d6e0e2ba596c1ab1db8d7e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050663"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="6b3bd-102">Fejlfinding af fejl 404, filen blev ikke fundet</span><span class="sxs-lookup"><span data-stu-id="6b3bd-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="6b3bd-103">Der modtages en fejl 404, når brugerne forsøger at få adgang til et websted eller en fil i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6b3bd-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="6b3bd-104">Dette skyldes ofte, at et websted eller en fil eller gruppe bliver omdøbt, flyttet eller slettet.</span><span class="sxs-lookup"><span data-stu-id="6b3bd-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="6b3bd-105">For eksempel: brugerne vil opleve en 404-fejl ved forsøget på at få adgang til rodgruppen af websteder, og den er blevet slettet.</span><span class="sxs-lookup"><span data-stu-id="6b3bd-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="6b3bd-106">Sådan løses fejl 404 for et websted, der er omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="6b3bd-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="6b3bd-107">For klassiske websteder, der findes i det klassiske administrations Center, se [Gendan en slettet gruppe af websteder](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="6b3bd-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="6b3bd-108">For moderne websteder (kommunikation, gruppe forbundne eller andre websteder), der findes i det nye SharePoint-Administrationscenter, se [få vist og Gendan slettede websteder i det nye SharePoint-Administrationscenter](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="6b3bd-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="6b3bd-109">Sådan løses fejl 404 for en fil (eller et andet element), der er omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="6b3bd-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="6b3bd-110">Gå til SharePoint-eller OneDrive-webstedet, og få vist papirkurven fra webstedets indhold.</span><span class="sxs-lookup"><span data-stu-id="6b3bd-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="6b3bd-111">Se, [Gendan elementer i papirkurven på et SharePoint-websted](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="6b3bd-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="6b3bd-112">Hvis du stadig ikke kan finde det element, du vil søge i overvågningsloggen, hvis logføring er aktiveret, skal du [søge i overvågningsloggen i Office 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span><span class="sxs-lookup"><span data-stu-id="6b3bd-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
