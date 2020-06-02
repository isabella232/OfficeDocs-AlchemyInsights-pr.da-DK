---
title: Fejlfinding i forbindelse med fejl 404, filen blev ikke fundet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: c860b9db63e8d341cbe5e6d8d1d420b4c9d01c9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505337"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="4b64d-102">Fejlfinding i forbindelse med fejl 404, filen blev ikke fundet</span><span class="sxs-lookup"><span data-stu-id="4b64d-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="4b64d-103">Der modtages en fejl 404, når brugerne forsøger at få adgang til et websted eller en fil i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4b64d-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="4b64d-104">Dette skyldes ofte, at et websted eller en fil eller gruppe omdøbes, flyttes eller slettes.</span><span class="sxs-lookup"><span data-stu-id="4b64d-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="4b64d-105">Eksempel: Brugerne vil opleve en 404-fejl, der forsøger at få adgang til rodgruppe for websteder, og den er blevet slettet.</span><span class="sxs-lookup"><span data-stu-id="4b64d-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="4b64d-106">Sådan løses fejl 404 for et websted, der er blevet omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="4b64d-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="4b64d-107">Du kan se klassiske websteder, der findes i Classic Administration, under [Gendanne en slettet gruppe af websteder](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="4b64d-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="4b64d-108">For moderne websteder (kommunikation, gruppeforbundet eller andre websteder), der findes i den nye SharePoint Administration, skal du se [Få vist og gendanne slettede websteder i den nye SharePoint Administration](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="4b64d-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="4b64d-109">Sådan løses fejl 404 for en fil (eller et andet element), der er blevet omdøbt, flyttet eller slettet:</span><span class="sxs-lookup"><span data-stu-id="4b64d-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="4b64d-110">Gå til SharePoint- eller OneDrive-webstedet, og få vist papirkurven fra webstedets indhold.</span><span class="sxs-lookup"><span data-stu-id="4b64d-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="4b64d-111">Se [Gendanne elementer i papirkurven på et SharePoint-websted](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="4b64d-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="4b64d-112">Hvis du stadig ikke kan finde elementet, kan du søge i overvågningsloggen, hvis logføring er aktiveret, [skal du søge i overvågningsloggen i Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="4b64d-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
