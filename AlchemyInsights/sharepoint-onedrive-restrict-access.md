---
title: Adgangsbegrænsning i SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559871"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="4a3eb-102">Adgangsbegrænsning i SharePoint- eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="4a3eb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="4a3eb-103">Der er mange måder at begrænse adgangen til tjenester til SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="4a3eb-104">Disse forskellige adgangsmetoder for begrænsning er beskrevet herunder.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="4a3eb-105">**Begrænsning af tilladelse**</span><span class="sxs-lookup"><span data-stu-id="4a3eb-105">**Permission Restriction**</span></span>

<span data-ttu-id="4a3eb-106">I SharePoint Online og OneDrive til virksomheder kan begrænse vi adgangen til elementer som steder, filer og mapper ved kun at give adgang til de grupper/personer, der skal have adgang.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="4a3eb-107">Tilpasse tilladelser for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="4a3eb-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="4a3eb-108">Tilpasse tilladelser til SharePoint-webstedet</span><span class="sxs-lookup"><span data-stu-id="4a3eb-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="4a3eb-109">Ændre tilladelserne for undermappen</span><span class="sxs-lookup"><span data-stu-id="4a3eb-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="4a3eb-110">Adgangskontrol fra ikke-administreret enheder</span><span class="sxs-lookup"><span data-stu-id="4a3eb-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="4a3eb-111">Som en SharePoint eller global administrator i Office 365, kan du blokere eller begrænse adgang til SharePoint og OneDrive indhold fra ikke-administreret enheder (de pågældende hybrid ikke AD joinforbundne eller kompatibel i Intune).</span><span class="sxs-lookup"><span data-stu-id="4a3eb-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="4a3eb-112">**Netværk placering begrænsning**</span><span class="sxs-lookup"><span data-stu-id="4a3eb-112">**Network Location Restriction**</span></span>

<span data-ttu-id="4a3eb-113">Som IT-administrator, kan du styre adgangen til SharePoint og OneDrive ressourcer, der er baseret på definerede netværksplaceringer, du har tillid til.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="4a3eb-114">Dette er også kendt som placering-baseret politik.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-114">This is also known as location-based policy.</span></span> <span data-ttu-id="4a3eb-115">Yderligere oplysninger finder du [kontrollere adgang til SharePoint Online- og OneDrive-data, der er baseret på placering på netværket](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="4a3eb-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="4a3eb-116">**Webstedsbegrænsningen Lås**</span><span class="sxs-lookup"><span data-stu-id="4a3eb-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="4a3eb-117">I SharePoint Online, har du mulighed for at låse en gruppe af websteder, så du ikke har adgang.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="4a3eb-118">Dette angives via PowerShell og [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) ved hjælp af egenskaben [Sæt SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="4a3eb-119">**Forhindre brugere i at oprette websteder eller underordnede websteder**</span><span class="sxs-lookup"><span data-stu-id="4a3eb-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="4a3eb-120">Som SharePoint Administration eller global administrator af Office 365, kan du lade brugerne oprette og administrere deres egne SharePoint-websteder, skal du bestemme, hvilke websteder de kan oprette, og Angiv placeringen af websteder.</span><span class="sxs-lookup"><span data-stu-id="4a3eb-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="4a3eb-121">Yderligere oplysninger finder du [Administrer websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="4a3eb-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

