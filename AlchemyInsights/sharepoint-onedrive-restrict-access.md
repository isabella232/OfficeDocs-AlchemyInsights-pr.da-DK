---
title: Begræns adgang i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700449"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="039f2-102">Begræns adgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="039f2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="039f2-103">Der er mange måder at begrænse adgangen til SharePoint Online/OneDrive-tjenester på.</span><span class="sxs-lookup"><span data-stu-id="039f2-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="039f2-104">Disse forskellige adgangs begrænsnings metoder er skitseret nedenfor.</span><span class="sxs-lookup"><span data-stu-id="039f2-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="039f2-105">**Tilladelses begrænsning**</span><span class="sxs-lookup"><span data-stu-id="039f2-105">**Permission Restriction**</span></span>

<span data-ttu-id="039f2-106">I SharePoint Online og OneDrive for Business kan vi begrænse adgangen til elementer som websteder, filer og mapper ved kun at give adgang til de grupper/enkeltpersoner, der skal have adgang.</span><span class="sxs-lookup"><span data-stu-id="039f2-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="039f2-107">Tilpasse tilladelser for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="039f2-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="039f2-108">Tilpas tilladelser til SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="039f2-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="039f2-109">Ændre tilladelserne for en undermappe</span><span class="sxs-lookup"><span data-stu-id="039f2-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="039f2-110">Kontrollér adgang fra ikke-administrerede enheder</span><span class="sxs-lookup"><span data-stu-id="039f2-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="039f2-111">Som SharePoint-eller Global administrator kan du blokere eller begrænse adgangen til SharePoint-og OneDrive-indhold fra ikke-administrerede enheder (dem, der ikke er hybride AD gangen eller kompatibel i Intune).</span><span class="sxs-lookup"><span data-stu-id="039f2-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="039f2-112">**Netværks placerings begrænsning**</span><span class="sxs-lookup"><span data-stu-id="039f2-112">**Network Location Restriction**</span></span>

<span data-ttu-id="039f2-113">Som IT-administrator kan du kontrollere adgangen til SharePoint-og OneDrive-ressourcer baseret på definerede netværksplaceringer, du har tillid til.</span><span class="sxs-lookup"><span data-stu-id="039f2-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="039f2-114">Dette kaldes også en placerings baseret politik.</span><span class="sxs-lookup"><span data-stu-id="039f2-114">This is also known as location-based policy.</span></span> <span data-ttu-id="039f2-115">Hvis du vil have mere at vide, skal du se [kontrollere adgang til SharePoint Online og OneDrive-data baseret på netværksplacering](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="039f2-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="039f2-116">**Begrænsning af websteds låse**</span><span class="sxs-lookup"><span data-stu-id="039f2-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="039f2-117">I SharePoint Online har du mulighed for at låse en gruppe af websteder, så ingen har adgang.</span><span class="sxs-lookup"><span data-stu-id="039f2-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="039f2-118">Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -Lock.</span><span class="sxs-lookup"><span data-stu-id="039f2-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="039f2-119">**Begræns brugere fra at oprette websteder eller underordnede websteder**</span><span class="sxs-lookup"><span data-stu-id="039f2-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="039f2-120">Som SharePoint-administrator eller Global administrator kan du give brugerne mulighed for at oprette og administrere deres egne SharePoint-websteder, angive, hvilken slags websteder de kan oprette, og angive placeringen af webstederne.</span><span class="sxs-lookup"><span data-stu-id="039f2-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="039f2-121">Hvis du vil have mere at vide, skal du se [administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="039f2-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

