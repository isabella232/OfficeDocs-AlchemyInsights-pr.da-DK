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
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- og OneDrive-overvågningslogfiler

## <a name="sharepoint-classic-audit-logs"></a>Klassiske sharePoint-overvågningslogfiler

Den ældre overvågning af SPO blev overført til Unified Audit Log (UAL). Alle spo-ældre revisionsrapporter vil nu blive drevet gennem UAL, og de gamle overvågningssignaler er blevet overført til UAL.

Vigtige ændringer:

* Trimning er IKKE tilgængelig som en kapacitet.
* Det er IKKE muligt at vælge bestemte hændelser, der skal overvåges. Se [dette dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for at få en komplet liste over overvågede hændelser, der er tilgængelige som standard.
* Indstillingen **Placering** under **Tilpassede rapporter** er IKKE tilgængelig.
* Indstillingen **Åbning eller download af dokumenter** er IKKE tilgængelig.

[Konfigurere indstillinger for overvågning for en gruppe af websteder](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- og OneDrive Modern Unified Audit-logfiler fra overholdelse

* [Slå logføring af Unified Audit til/fra](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.

Brug søgning i overvågningslogføring til at kontrollere aktiviteten for filene eller mapperne, brugerne/brugernes tilladelser:

* [Fil- og sideaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappeaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter for deling og adgangsanmodning](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter i administration af byggepladser](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Du kan finde flere oplysninger om, hvordan du henter disse hændelser, [i Søge i overvågningsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
