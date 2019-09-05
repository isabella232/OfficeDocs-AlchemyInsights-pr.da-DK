---
title: Begrænse adgangen i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750658"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="eeb6b-102">Begrænse adgangen i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="eeb6b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="eeb6b-103">Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester på.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="eeb6b-104">Disse forskellige adgangsbegrænsnings metoder er skitseret nedenfor.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="eeb6b-105">**Begrænsning af tilladelse**</span><span class="sxs-lookup"><span data-stu-id="eeb6b-105">**Permission Restriction**</span></span>

<span data-ttu-id="eeb6b-106">I SharePoint Online og OneDrive for Business begrænser vi adgangen til elementer som websteder, filer og mapper ved kun at give adgang til de grupper/personer, der skal have adgang.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="eeb6b-107">Tilpasse tilladelser for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="eeb6b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="eeb6b-108">Tilpas tilladelser til SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="eeb6b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="eeb6b-109">Ændre tilladelserne for en undermappe</span><span class="sxs-lookup"><span data-stu-id="eeb6b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="eeb6b-110">Styre adgang fra ikke-administrerede enheder</span><span class="sxs-lookup"><span data-stu-id="eeb6b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="eeb6b-111">Som SharePoint-eller Global administrator i Office 365 kan du blokere eller begrænse adgangen til SharePoint-og OneDrive-indhold fra ikke-administrerede enheder (dem, der ikke er hybrid annoncer, som er joinforbundne eller kompatible i Intune).</span><span class="sxs-lookup"><span data-stu-id="eeb6b-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="eeb6b-112">**Begrænsning af netværksplacering**</span><span class="sxs-lookup"><span data-stu-id="eeb6b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="eeb6b-113">Som IT-administrator kan du styre adgangen til SharePoint-og OneDrive-ressourcer baseret på definerede netværksplaceringer, som du har tillid til.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="eeb6b-114">Dette kaldes også lokationsbaseret politik.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="eeb6b-115">Du kan finde flere oplysninger under [kontrollere adgang til SharePoint Online-og OneDrive-data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="eeb6b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="eeb6b-116">**Begrænsning af websteds låsning**</span><span class="sxs-lookup"><span data-stu-id="eeb6b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="eeb6b-117">I SharePoint Online har du mulighed for at låse en gruppe af websteder op, så ingen har adgang.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="eeb6b-118">Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="eeb6b-119">**Begrænse brugere i at oprette websteder eller underordnede websteder**</span><span class="sxs-lookup"><span data-stu-id="eeb6b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="eeb6b-120">Som SharePoint-administrator eller global Office 365-administrator kan du lade dine brugere oprette og administrere deres egne SharePoint-websteder, bestemme, hvilke typer websteder de kan oprette, og angive placeringen af webstederne.</span><span class="sxs-lookup"><span data-stu-id="eeb6b-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="eeb6b-121">Du kan finde flere oplysninger under [administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="eeb6b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

