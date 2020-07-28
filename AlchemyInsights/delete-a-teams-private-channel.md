---
title: Slette en privat Teams-kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438991"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="799d5-102">Slette en privat Teams-kanal</span><span class="sxs-lookup"><span data-stu-id="799d5-102">Delete a Teams private channel</span></span>

<span data-ttu-id="799d5-103">Microsoft er opmærksom på et problem med at slette en privat Teams-kanal, hvis du har aktiveret SharePoint-opbevaringspolitikker for det underliggende SharePoint-websted.</span><span class="sxs-lookup"><span data-stu-id="799d5-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="799d5-104">Microsoft arbejder på en rettelse.</span><span class="sxs-lookup"><span data-stu-id="799d5-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="799d5-105">I mellemtiden kan du bruge følgende løsninger til at slette den private kanal.</span><span class="sxs-lookup"><span data-stu-id="799d5-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="799d5-106">**Ekskluder gruppen/gruppen af websteder fra sharepoint-opbevaringspolitikken.**</span><span class="sxs-lookup"><span data-stu-id="799d5-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="799d5-107">Gå til Office 365-administrationsportalen, og vælg **Vis alle** i venstre navigationsrude.</span><span class="sxs-lookup"><span data-stu-id="799d5-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="799d5-108">Gå **til Sikkerhedskontrol**i **& overvågningspolitik**for  >  **datatab**under  >  **Administration**.</span><span class="sxs-lookup"><span data-stu-id="799d5-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="799d5-109">Identificer en politik, der gælder for Sharepoint-websteder, og rediger politikken, så Sharepoint-webstedet for det team, der indeholder den private kanal, IKKE er inkluderet i opbevaringspolitikken.</span><span class="sxs-lookup"><span data-stu-id="799d5-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="799d5-110">Gem politikken.</span><span class="sxs-lookup"><span data-stu-id="799d5-110">Save the policy.</span></span>
    <span data-ttu-id="799d5-111">Det kan tage op til 24 timer, før politikindstillinger træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="799d5-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="799d5-112">Når webstedet er blevet udeladt, kan du slette den private kanal.</span><span class="sxs-lookup"><span data-stu-id="799d5-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="799d5-113">Du ***kan*** muligvis slette den private kanal ved hjælp af Microsoft Teams på din Android-enhed.</span><span class="sxs-lookup"><span data-stu-id="799d5-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="799d5-114">Du kan finde relaterede SharePoint-oplysninger [under Kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="799d5-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>