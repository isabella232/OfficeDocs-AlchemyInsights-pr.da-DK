---
title: Klassiske rapporter om SharePoint-overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662202"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="28c21-102">Overvågningslogfiler for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="28c21-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="28c21-103">Klassisk SharePoint-overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="28c21-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="28c21-104">SPO Legacy-revision blev overført til Unified revisions log (UAL).</span><span class="sxs-lookup"><span data-stu-id="28c21-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="28c21-105">Alle SPO Legacy-overvågningsrapporter bliver nu slået fra gennem UAL, og de ældre overvågnings signaler er blevet overført til UAL.</span><span class="sxs-lookup"><span data-stu-id="28c21-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="28c21-106">Nøgle ændringer:</span><span class="sxs-lookup"><span data-stu-id="28c21-106">Key changes:</span></span>

* <span data-ttu-id="28c21-107">Trimning er ikke tilgængelig som en funktion.</span><span class="sxs-lookup"><span data-stu-id="28c21-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="28c21-108">Valg af bestemte hændelser, der skal overvåges, er ikke tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="28c21-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="28c21-109">Se [dette dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der er tilgængelige som standard.</span><span class="sxs-lookup"><span data-stu-id="28c21-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="28c21-110">Indstillingen **placering** under **tilpassede rapporter** er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="28c21-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="28c21-111">Indstillingen **åbner eller henter dokument** hændelser er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="28c21-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="28c21-112">Konfigurere overvågningsindstillinger for en gruppe af websteder</span><span class="sxs-lookup"><span data-stu-id="28c21-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="28c21-113">Moderne Unified revisions logfiler for SharePoint og OneDrive fra overholdelse</span><span class="sxs-lookup"><span data-stu-id="28c21-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="28c21-114">Aktivere/deaktivere Unified Auditing-logføring</span><span class="sxs-lookup"><span data-stu-id="28c21-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="28c21-115">Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="28c21-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="28c21-116">Brug søgning i overvågningslog til at kontrollere aktiviteten for filerne, mappe (r), bruger (e), tilladelser:</span><span class="sxs-lookup"><span data-stu-id="28c21-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="28c21-117">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="28c21-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="28c21-118">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="28c21-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="28c21-119">Aktiviteter for anmodninger om deling og adgang</span><span class="sxs-lookup"><span data-stu-id="28c21-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="28c21-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="28c21-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="28c21-121">Aktiviteter for Webstedsadministration</span><span class="sxs-lookup"><span data-stu-id="28c21-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="28c21-122">Du kan finde flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningslogfilen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="28c21-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
