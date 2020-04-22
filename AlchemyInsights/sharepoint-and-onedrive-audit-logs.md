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
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- og OneDrive-overvågningslogfiler

## <a name="sharepoint-classic-audit-logs"></a>Klassiske Overvågningslogfiler til SharePoint

SPO-ældre overvågning blev overført til UAL (Unified Audit Log). Alle SPO-ældre overvågningsrapporter vil nu blive drevet gennem UAL, og de ældre overvågningssignaler er blevet overført til UAL.

Vigtige ændringer:

* Beskæring er IKKE tilgængelig som en funktion.
* Det er IKKE muligt at vælge bestemte hændelser, der skal overvåges. Se [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der som standard er tilgængelige.
* Indstillingen **Placering** under **Tilpassede rapporter** er IKKE tilgængelig.
* Indstillingen **Åbning eller hentning af dokumenter** er IKKE tilgængelig.

[Konfigurere overvågningsindstillinger for en gruppe af websteder](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- og OneDrive Modern Unified Audit-logfiler fra overholdelse af regler og standarder

* [Slå Unified Audit Logging til/fra](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.

Brug overvågningslogsøgning til at kontrollere aktiviteten af filen eller de filer, mapper, brugere, tilladelser, der er:

* [Fil- og sideaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappeaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dele og få adgang til anmodningsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter i forbindelse med webstedsadministration](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Yderligere oplysninger om, hvordan du henter disse hændelser, finder [du i Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
