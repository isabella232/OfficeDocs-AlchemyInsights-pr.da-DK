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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051095"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="bf6d5-102">Problemer ved oprettelse eller gruppe af tilknyttede websteder i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bf6d5-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="bf6d5-103">Der er et par almindeligt forekommende problemer, når du opretter eller genopretter en gruppe forbundet websted.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="bf6d5-104">Hvis du har slettet en gruppe og dens tilsluttede websted og ønsker at oprette et andet websted med den samme webadresse, skal du fjerne det forrige websted permanent.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="bf6d5-105">Hent [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="bf6d5-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="bf6d5-106">Du kan finde flere oplysninger om, hvordan du kommer i gang med PowerShell, under [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="bf6d5-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="bf6d5-107">Fjernwebstedet fra slettede websteder ved hjælp af [Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="bf6d5-108">Hvis du opretter et websted med tilknyttede websteder og modtager en advarsel om, at der allerede findes en anden gruppe med det samme alias, skal du kontrollere de eksisterende grupper fra [Office 365 fra administrationscenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="bf6d5-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="bf6d5-109">Du kan løse problemet ved at slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="bf6d5-110">Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="bf6d5-111">Du kan oprette forbindelse mellem eksisterende websteder og en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="bf6d5-112">Du kan finde flere oplysninger under [oprette forbindelse fra en Office 365-gruppe ved hjælp af SharePoint-bruger ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="bf6d5-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="bf6d5-113">Hvis du vil oprette et Office 365-gruppe tilsluttet websted, skal du oprette et team websted.</span><span class="sxs-lookup"><span data-stu-id="bf6d5-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="bf6d5-114">Du kan finde flere oplysninger under [oprette et teamwebsted i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="bf6d5-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

