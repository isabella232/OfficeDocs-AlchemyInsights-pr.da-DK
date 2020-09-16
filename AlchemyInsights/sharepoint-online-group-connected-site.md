---
title: Føje en gruppe til et SharePoint-websted
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771193"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="db02a-102">Problemer ved oprettelse af et gruppe forbundet websted i SharePoint</span><span class="sxs-lookup"><span data-stu-id="db02a-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="db02a-103">Der opstod nogle almindelige problemer med at oprette eller genoprette en gruppes forbundne websted.</span><span class="sxs-lookup"><span data-stu-id="db02a-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="db02a-104">Hvis du har slettet en gruppe og den tilknyttede websted og vil oprette et andet websted med den samme URL-adresse, skal du fjerne det tidligere websted permanent.</span><span class="sxs-lookup"><span data-stu-id="db02a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="db02a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="db02a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="db02a-106">Du kan finde flere oplysninger om at komme i gang med PowerShell i [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="db02a-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="db02a-107">Fjernwebstedet fra slettede websteder ved hjælp af PowerShell [-cmdlet'en Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="db02a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="db02a-108">PowerShell kræves for at slette gruppe websteder permanent.</span><span class="sxs-lookup"><span data-stu-id="db02a-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="db02a-109">Hvis du opretter en gruppe forbundet websted og modtager en advarsel: der **findes allerede en gruppe med det samme alias**, skal du kontrollere de eksisterende grupper fra [Microsoft 365 administration](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="db02a-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="db02a-110">For at løse problemet skal du slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.</span><span class="sxs-lookup"><span data-stu-id="db02a-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="db02a-111">Der er forskellige måder at oprette og bruge moderne grupper på i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="db02a-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="db02a-112">Du kan forbinde eksisterende websteder til en Microsoft 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="db02a-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="db02a-113">Du kan finde flere oplysninger i [Opret forbindelse til en Microsoft 365-gruppe ved hjælp af SharePoint-brugergrænsefladen](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="db02a-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="db02a-114">Hvis du vil oprette et Microsoft 365-gruppens forbundne websted, skal du oprette et [team websted](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="db02a-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
