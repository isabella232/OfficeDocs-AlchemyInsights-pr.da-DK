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
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741959"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="46784-102">SharePoint- og OneDrive-overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="46784-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="46784-103">Klassiske Overvågningslogfiler til SharePoint</span><span class="sxs-lookup"><span data-stu-id="46784-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="46784-104">SPO-ældre overvågning blev overført til UAL (Unified Audit Log).</span><span class="sxs-lookup"><span data-stu-id="46784-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="46784-105">Alle SPO-ældre overvågningsrapporter vil nu blive drevet gennem UAL, og de ældre overvågningssignaler er blevet overført til UAL.</span><span class="sxs-lookup"><span data-stu-id="46784-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="46784-106">Vigtige ændringer:</span><span class="sxs-lookup"><span data-stu-id="46784-106">Key changes:</span></span>

* <span data-ttu-id="46784-107">Beskæring er IKKE tilgængelig som en funktion.</span><span class="sxs-lookup"><span data-stu-id="46784-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="46784-108">Det er IKKE muligt at vælge bestemte hændelser, der skal overvåges.</span><span class="sxs-lookup"><span data-stu-id="46784-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="46784-109">Se [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der som standard er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="46784-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="46784-110">Indstillingen **Placering** under **Tilpassede rapporter** er IKKE tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="46784-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="46784-111">Indstillingen **Åbning eller hentning af dokumenter** er IKKE tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="46784-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="46784-112">Konfigurere overvågningsindstillinger for en gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="46784-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="46784-113">SharePoint- og OneDrive Modern Unified Audit-logfiler fra overholdelse af regler og standarder</span><span class="sxs-lookup"><span data-stu-id="46784-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="46784-114">Slå Unified Audit Logging til/fra</span><span class="sxs-lookup"><span data-stu-id="46784-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="46784-115">Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="46784-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="46784-116">Brug overvågningslogsøgning til at kontrollere aktiviteten af filen eller de filer, mapper, brugere, tilladelser, der er:</span><span class="sxs-lookup"><span data-stu-id="46784-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="46784-117">Fil- og sideaktiviteter</span><span class="sxs-lookup"><span data-stu-id="46784-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="46784-118">Mappeaktiviteter</span><span class="sxs-lookup"><span data-stu-id="46784-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="46784-119">Dele og få adgang til anmodningsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="46784-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="46784-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="46784-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="46784-121">Aktiviteter i forbindelse med webstedsadministration</span><span class="sxs-lookup"><span data-stu-id="46784-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="46784-122">Yderligere oplysninger om, hvordan du henter disse hændelser, finder [du i Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="46784-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
