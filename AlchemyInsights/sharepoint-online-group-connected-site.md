---
title: Føje en gruppe til et SharePoint-websted
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507841"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="bb71e-102">Problemer, når du opretter eller gruppe tilsluttet websteder i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bb71e-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="bb71e-103">Der er et par almindelige problemer, der opstår, når forbundet websted, oprette eller genoprette en gruppe.</span><span class="sxs-lookup"><span data-stu-id="bb71e-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="bb71e-104">Hvis du har slettet en gruppe og dets forbundne websted og ønsker at oprette et andet websted med samme URL-adresse, skal du fjerne det forrige websted permanent.</span><span class="sxs-lookup"><span data-stu-id="bb71e-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="bb71e-105">Hent [Simuleret administrationsshell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="bb71e-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="bb71e-106">Se [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) for at få flere oplysninger på Introduktion til powershell</span><span class="sxs-lookup"><span data-stu-id="bb71e-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="bb71e-107">Fjern webstedet fra slettet websteder ved hjælp af [Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="bb71e-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="bb71e-108">Hvis du opretter en gruppe forbundne websted, og du modtager en advarsel, der findes allerede en anden gruppe med det samme alias, kan du se de eksisterende grupper fra [Office 365 Admin-Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="bb71e-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="bb71e-109">Tildelt til at løse problemet, Slet den eksisterende gruppe, hvis det ikke længere er nødvendigt eller oprette webstedet med et andet alias.</span><span class="sxs-lookup"><span data-stu-id="bb71e-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="bb71e-110">Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bb71e-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="bb71e-111">Du kan oprette forbindelse til eksisterende websteder til Office 365-gruppen.</span><span class="sxs-lookup"><span data-stu-id="bb71e-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="bb71e-112">Du kan finde flere oplysninger, skal [Tilslut en Office 365-gruppe, ved hjælp af SharePoint bruger ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="bb71e-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="bb71e-113">Hvis du vil oprette et Office 365 gruppe forbundne websted, skal du oprette et websted for Team.</span><span class="sxs-lookup"><span data-stu-id="bb71e-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="bb71e-114">For yderligere oplysninger se [oprette et websted for team i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="bb71e-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

