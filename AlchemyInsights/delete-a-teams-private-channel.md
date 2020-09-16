---
title: Slette en privat kanal i teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730909"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="e8837-102">Slette en privat kanal i teams</span><span class="sxs-lookup"><span data-stu-id="e8837-102">Delete a Teams private channel</span></span>

<span data-ttu-id="e8837-103">Microsoft er opmærksom på et problem, der sletter en privat kanal for teams, hvis du har aktiveret SharePoint-opbevaringspolitikker for det underliggende SharePoint-websted.</span><span class="sxs-lookup"><span data-stu-id="e8837-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="e8837-104">Microsoft arbejder på en rettelse.</span><span class="sxs-lookup"><span data-stu-id="e8837-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="e8837-105">I mellemtiden kan du bruge følgende løsninger til at slette den private kanal.</span><span class="sxs-lookup"><span data-stu-id="e8837-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="e8837-106">**Udelad gruppe-eller gruppe af websteder fra SharePoint-opbevaringspolitikken.**</span><span class="sxs-lookup"><span data-stu-id="e8837-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="e8837-107">Gå til Office 365 administrations portalen, og vælg **Vis alle** i venstre navigationsrude.</span><span class="sxs-lookup"><span data-stu-id="e8837-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="e8837-108">Gå **Admin centers**til **Security &**  >  politik for**forebyggelse af datatab**under administration  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="e8837-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="e8837-109">Identificer alle politikker, der gælder for SharePoint-websteder, og Rediger politikken, så SharePoint-webstedet for det team, der indeholder den private kanal, ikke er omfattet af opbevaringspolitikken.</span><span class="sxs-lookup"><span data-stu-id="e8837-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="e8837-110">Gem politikken.</span><span class="sxs-lookup"><span data-stu-id="e8837-110">Save the policy.</span></span>
    <span data-ttu-id="e8837-111">Det kan tage op til 24 timer, før politikindstillingerne træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="e8837-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="e8837-112">Når webstedet er blevet udeladt, kan du slette den private kanal.</span><span class="sxs-lookup"><span data-stu-id="e8837-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="e8837-113">Du vil  ***muligvis*** kunne slette den private kanal ved hjælp af Microsoft teams på din Android-enhed.</span><span class="sxs-lookup"><span data-stu-id="e8837-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="e8837-114">Hvis du vil have relaterede SharePoint-oplysninger, skal du se [kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="e8837-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>