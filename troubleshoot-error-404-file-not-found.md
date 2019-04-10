---
title: Fejlfinding i forbindelse med fejl 404 fil ikke fundet
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 467feb3cb436a2e0135162657876e5c45d8d56bd
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747233"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="b98d6-102">Fejlfinding i forbindelse med fejl 404 fil ikke fundet</span><span class="sxs-lookup"><span data-stu-id="b98d6-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="b98d6-103">En fejl 404 modtages, når brugere forsøger at få adgang til et websted eller en fil i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b98d6-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="b98d6-104">Dette skyldes ofte et websted eller en fil eller en gruppe få omdøbt, flyttet eller slettet.</span><span class="sxs-lookup"><span data-stu-id="b98d6-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="b98d6-105">For eksempel: brugere vil opleve en 404 fejl ved forsøg på at få adgang til roden af websteder og er blevet slettet.</span><span class="sxs-lookup"><span data-stu-id="b98d6-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="b98d6-106">Sådan løses fejl 404 for et websted, der er blevet omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="b98d6-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="b98d6-107">Klassiske websteder, der findes i den klassiske Admin Center, finder du [gendanner en slettet gruppe af websteder](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="b98d6-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="b98d6-108">Moderne websteder (kommunikation, gruppe-forbindelse, eller andre steder), som findes i det nye SharePoint Administration center, finder du i [View og gendanne slettet websteder i det nye SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="b98d6-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/en-us/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="b98d6-109">Sådan løses fejl 404 til en fil (eller et andet element), der er blevet omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="b98d6-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="b98d6-110">Gå til webstedet SharePoint- eller OneDrive, og få vist papirkurven fra webstedets indhold.</span><span class="sxs-lookup"><span data-stu-id="b98d6-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="b98d6-111">Se [gendanne elementer i papirkurven på SharePoint-webstedet](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="b98d6-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="b98d6-112">Hvis du stadig ikke kan finde det element, du kan søge overvågningsloggen, hvis logføring er aktiveret, se [søgning audit logge på Office 365 sikkerhed & Overholdelsescenter](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span><span class="sxs-lookup"><span data-stu-id="b98d6-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
