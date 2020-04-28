---
title: Føje en gruppe til et SharePoint-websted
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912960"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f68d4-102">Problemer ved oprettelse af et gruppeforbundet websted i SharePoint</span><span class="sxs-lookup"><span data-stu-id="f68d4-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f68d4-103">Nogle almindelige problemer, der opstår ved oprettelse eller genoprettelse af et gruppeforbundet websted.</span><span class="sxs-lookup"><span data-stu-id="f68d4-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f68d4-104">Hvis du har slettet en gruppe og dens forbundne websted og ønsker at oprette et andet websted med den samme webadresse, skal du fjerne det forrige websted permanent.</span><span class="sxs-lookup"><span data-stu-id="f68d4-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f68d4-105">Hent [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f68d4-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f68d4-106">Du kan finde flere oplysninger om, hvordan du kommer i gang med Powershell, under [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f68d4-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f68d4-107">Fjern webstedet fra slettede websteder ved hjælp af PowerShell-cmdlet'en [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="f68d4-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f68d4-108">Powershell er forpligtet til permanent at slette gruppewebsteder.</span><span class="sxs-lookup"><span data-stu-id="f68d4-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f68d4-109">Hvis du opretter et gruppeforbundet websted og modtager en advarsel: **Der findes allerede en anden gruppe med det samme alias**, skal du kontrollere de eksisterende grupper fra Microsoft [365 Administration](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f68d4-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f68d4-110">Du kan løse problemet ved at slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.</span><span class="sxs-lookup"><span data-stu-id="f68d4-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f68d4-111">Der er forskellige måder at oprette og bruge moderne grupper med SharePoint på.</span><span class="sxs-lookup"><span data-stu-id="f68d4-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f68d4-112">Du kan forbinde eksisterende websteder med en Microsoft 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="f68d4-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="f68d4-113">Du kan finde flere oplysninger under [Forbinde en Microsoft 365-gruppe ved hjælp af SharePoint-brugergrænsefladen](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f68d4-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f68d4-114">Hvis du vil oprette et microsoft 365-gruppeforbundet websted, skal du oprette et [teamwebsted](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f68d4-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
