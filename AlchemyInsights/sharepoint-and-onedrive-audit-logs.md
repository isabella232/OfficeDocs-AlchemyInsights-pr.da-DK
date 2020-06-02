---
title: Klassiske SharePoint-overvågningslograpporter
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509594"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="86a0b-102">SharePoint- og OneDrive-overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="86a0b-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="86a0b-103">Klassiske sharePoint-overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="86a0b-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="86a0b-104">Den ældre overvågning af SPO blev overført til Unified Audit Log (UAL).</span><span class="sxs-lookup"><span data-stu-id="86a0b-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="86a0b-105">Alle spo-ældre revisionsrapporter vil nu blive drevet gennem UAL, og de gamle overvågningssignaler er blevet overført til UAL.</span><span class="sxs-lookup"><span data-stu-id="86a0b-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="86a0b-106">Vigtige ændringer:</span><span class="sxs-lookup"><span data-stu-id="86a0b-106">Key changes:</span></span>

* <span data-ttu-id="86a0b-107">Trimning er IKKE tilgængelig som en kapacitet.</span><span class="sxs-lookup"><span data-stu-id="86a0b-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="86a0b-108">Det er IKKE muligt at vælge bestemte hændelser, der skal overvåges.</span><span class="sxs-lookup"><span data-stu-id="86a0b-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="86a0b-109">Se [dette dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der er tilgængelige som standard.</span><span class="sxs-lookup"><span data-stu-id="86a0b-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="86a0b-110">Indstillingen **Placering** under **Tilpassede rapporter** er IKKE tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="86a0b-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="86a0b-111">Indstillingen **Åbning eller download af dokumenter** er IKKE tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="86a0b-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="86a0b-112">Konfigurere indstillinger for overvågning for en gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="86a0b-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="86a0b-113">SharePoint- og OneDrive Modern Unified Audit-logfiler fra overholdelse</span><span class="sxs-lookup"><span data-stu-id="86a0b-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="86a0b-114">Slå logføring af Unified Audit til/fra</span><span class="sxs-lookup"><span data-stu-id="86a0b-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="86a0b-115">Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="86a0b-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="86a0b-116">Brug søgning i overvågningslogføring til at kontrollere aktiviteten for filene eller mapperne, brugerne/brugernes tilladelser:</span><span class="sxs-lookup"><span data-stu-id="86a0b-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="86a0b-117">Fil- og sideaktiviteter</span><span class="sxs-lookup"><span data-stu-id="86a0b-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="86a0b-118">Mappeaktiviteter</span><span class="sxs-lookup"><span data-stu-id="86a0b-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="86a0b-119">Aktiviteter for deling og adgangsanmodning</span><span class="sxs-lookup"><span data-stu-id="86a0b-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="86a0b-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="86a0b-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="86a0b-121">Aktiviteter i administration af byggepladser</span><span class="sxs-lookup"><span data-stu-id="86a0b-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="86a0b-122">Du kan finde flere oplysninger om, hvordan du henter disse hændelser, [i Søge i overvågningsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="86a0b-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
