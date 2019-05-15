---
title: Moderne sted som rodwebstedet
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057691"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="d3f02-102">Moderne sted som rodwebstedet</span><span class="sxs-lookup"><span data-stu-id="d3f02-102">Modern site as root site</span></span>

<span data-ttu-id="d3f02-103">[Frigivelse af målet](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) kunder kan nu aktivere moderne kommunikation indtryk på classic-rodwebstedet for deres lejer i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d3f02-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="d3f02-104">Denne funktion kan aktiveres ved at køre en simpel PowerShell-cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d3f02-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="d3f02-105">Rodwebstedet har på vellykket udførelse af PowerShell-command(s), en ny hjemmeside til kommunikation-websted.</span><span class="sxs-lookup"><span data-stu-id="d3f02-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="d3f02-106">Oplysninger om krav til PowerShell-cmdlet og funktion er tilgængelige i artiklen [Aktivere SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="d3f02-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="d3f02-107">Vi skal gradvis rullende ud, slået fra som standard til målrettet Release kunderne i tidlig maj-2019 og rulle ud vil være tilgængelige i hele verden ved udgangen af juni 2019.</span><span class="sxs-lookup"><span data-stu-id="d3f02-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="d3f02-108">Fortsætte med at henvise til [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for andre nye funktioner med moderne.</span><span class="sxs-lookup"><span data-stu-id="d3f02-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="d3f02-109">**Vigtigt**: Slet ikke klassiske rod-webstedet for at oprette et websted til et moderne kommunikation.</span><span class="sxs-lookup"><span data-stu-id="d3f02-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="d3f02-110">Dette understøttes ikke af Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3f02-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="d3f02-111">Slette rodwebstedet, bliver alle SharePoint-websteder i din organisation utilgængelige for alle brugere, før du gendanne webstedet eller oprette et nyt websted med samme URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="d3f02-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 