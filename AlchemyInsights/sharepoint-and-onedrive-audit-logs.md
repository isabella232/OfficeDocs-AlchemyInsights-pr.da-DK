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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvågningslogfiler for SharePoint og OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassiske SharePoint-overvågningslogfiler

SPO Legacy-overvågning blev overflyttet til Unified audit log (UAL). Alle SPO Legacy revisionsrapporter vil nu blive drevet gennem UAL, og de ældre revisions signaler er blevet migreret til UAL.

Vigtige ændringer:

* Beskæring er ikke tilgængelig som en egenskab.
* Det er ikke muligt at vælge bestemte hændelser til overvågning. Se [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en komplet liste over reviderede hændelser, der er tilgængelige som standard.
* Indstillingen **placering** under **tilpassede rapporter** er ikke tilgængelig.
* Indstillingen **Åbn eller download af dokumenter** er ikke tilgængelig.

[Konfigurere overvågningsindstillinger for en gruppe af websteder](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderne Unified audit-logfiler fra overholdelse af SharePoint og OneDrive

* [Slå logføring af Unified audit til/fra](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.

Brug overvågningslog søgning til at kontrollere aktiviteten for de (t) fil (er), mappe (r), bruger (e), tilladelser:

* [Fil-og side aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappe aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Delings-og adgangs anmodnings aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for Webstedsadministration](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Du finder flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
