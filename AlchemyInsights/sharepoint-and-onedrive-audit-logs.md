---
title: Klassiske rapporter i SharePoint-overvågningslog
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992612"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="9a40a-102">Overvågningslogfiler for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="9a40a-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="9a40a-103">Klassiske SharePoint-overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="9a40a-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="9a40a-104">SPO Legacy-overvågning blev overflyttet til Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="9a40a-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="9a40a-105">Alle SPO Legacy revisionsrapporter vil nu blive drevet gennem UAL, og de ældre revisions signaler er blevet migreret til UAL.</span><span class="sxs-lookup"><span data-stu-id="9a40a-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="9a40a-106">Vigtige ændringer:</span><span class="sxs-lookup"><span data-stu-id="9a40a-106">Key changes:</span></span>

* <span data-ttu-id="9a40a-107">Beskæring er ikke tilgængelig som en egenskab.</span><span class="sxs-lookup"><span data-stu-id="9a40a-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="9a40a-108">Det er ikke muligt at vælge bestemte hændelser til overvågning.</span><span class="sxs-lookup"><span data-stu-id="9a40a-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="9a40a-109">Se [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en komplet liste over reviderede hændelser, der er tilgængelige som standard.</span><span class="sxs-lookup"><span data-stu-id="9a40a-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="9a40a-110">Indstillingen **placering** under **tilpassede rapporter** er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="9a40a-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="9a40a-111">Indstillingen **Åbn eller download af dokumenter** er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="9a40a-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="9a40a-112">Konfigurere overvågningsindstillinger for en gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="9a40a-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="9a40a-113">Moderne Unified audit-logfiler fra overholdelse af SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="9a40a-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="9a40a-114">Slå logføring af Unified audit til/fra</span><span class="sxs-lookup"><span data-stu-id="9a40a-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="9a40a-115">Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a40a-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="9a40a-116">Brug overvågningslog søgning til at kontrollere aktiviteten for de (t) fil (er), mappe (r), bruger (e), tilladelser:</span><span class="sxs-lookup"><span data-stu-id="9a40a-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="9a40a-117">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9a40a-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="9a40a-118">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9a40a-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="9a40a-119">Delings-og adgangs anmodnings aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9a40a-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="9a40a-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="9a40a-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="9a40a-121">Aktiviteter for Webstedsadministration</span><span class="sxs-lookup"><span data-stu-id="9a40a-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="9a40a-122">Du finder flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="9a40a-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
