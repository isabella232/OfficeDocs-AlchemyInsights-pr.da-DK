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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068017"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="0fa63-102">Overvågningslogfiler for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="0fa63-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="0fa63-103">**Moderne Unified audit-logfiler fra overholdelse af SharePoint og OneDrive**</span><span class="sxs-lookup"><span data-stu-id="0fa63-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="0fa63-104">Slå logføring af Unified audit til/fra</span><span class="sxs-lookup"><span data-stu-id="0fa63-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="0fa63-105">Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0fa63-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="0fa63-106">Brug overvågningslog søgning til at kontrollere aktiviteten for de (t) fil (er), mappe (r), bruger (e), tilladelser:</span><span class="sxs-lookup"><span data-stu-id="0fa63-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="0fa63-107">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="0fa63-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="0fa63-108">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="0fa63-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="0fa63-109">Delings-og adgangs anmodnings aktiviteter</span><span class="sxs-lookup"><span data-stu-id="0fa63-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="0fa63-110">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="0fa63-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="0fa63-111">Aktiviteter for Webstedsadministration</span><span class="sxs-lookup"><span data-stu-id="0fa63-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="0fa63-112">Du finder flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="0fa63-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="0fa63-113">**Klassiske SharePoint-overvågningslogfiler**</span><span class="sxs-lookup"><span data-stu-id="0fa63-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="0fa63-114">Vi migrerede SPO Legacy-overvågning til Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="0fa63-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="0fa63-115">Dette betyder i det væsentlige, at alle SPO Legacy revisionsrapporter nu vil blive drevet gennem UAL, og de ældre revisions signaler er blevet migreret til UAL.</span><span class="sxs-lookup"><span data-stu-id="0fa63-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="0fa63-116">Vigtige ændringer:</span><span class="sxs-lookup"><span data-stu-id="0fa63-116">Key changes:</span></span>

- <span data-ttu-id="0fa63-117">Beskæring som en egenskab er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="0fa63-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="0fa63-118">Den sektion, hvor du vælger bestemte hændelser til overvågning, er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="0fa63-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="0fa63-119">I [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) kan du se en komplet liste over reviderede hændelser, der er tilgængelige som standard.</span><span class="sxs-lookup"><span data-stu-id="0fa63-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="0fa63-120">Indstillingen "placering" under **tilpassede rapporter** er ikke tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="0fa63-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="0fa63-121">Hændelserne "åbning eller hentning af dokumenter" er ikke tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="0fa63-121">“Opening or downloading documents” events is NOT available.</span></span> 

