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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvågningslogfiler for SharePoint og OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassisk SharePoint-overvågningslogge

SPO Legacy-revision blev overført til Unified revisions log (UAL). Alle SPO Legacy-overvågningsrapporter bliver nu slået fra gennem UAL, og de ældre overvågnings signaler er blevet overført til UAL.

Nøgle ændringer:

* Trimning er ikke tilgængelig som en funktion.
* Valg af bestemte hændelser, der skal overvåges, er ikke tilgængelige. Se [dette dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der er tilgængelige som standard.
* Indstillingen **placering** under **tilpassede rapporter** er ikke tilgængelig.
* Indstillingen **åbner eller henter dokument** hændelser er ikke tilgængelig.

[Konfigurere overvågningsindstillinger for en gruppe af websteder](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderne Unified revisions logfiler for SharePoint og OneDrive fra overholdelse

* [Aktivere/deaktivere Unified Auditing-logføring](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.

Brug søgning i overvågningslog til at kontrollere aktiviteten for filerne, mappe (r), bruger (e), tilladelser:

* [Fil-og side aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappe aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter for anmodninger om deling og adgang](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for Webstedsadministration](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Du kan finde flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningslogfilen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
