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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvågningslogfiler for SharePoint og OneDrive

**Moderne Unified audit-logfiler fra overholdelse af SharePoint og OneDrive**

- [Slå logføring af Unified audit til/fra](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Der kræves ingen yderligere konfiguration i SharePoint eller OneDrive.

- Brug overvågningslog søgning til at kontrollere aktiviteten for de (t) fil (er), mappe (r), bruger (e), tilladelser:

    - [Fil-og side aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Mappe aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Delings-og adgangs anmodnings aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Aktiviteter for Webstedsadministration](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Du finder flere oplysninger om, hvordan du henter disse hændelser, i [søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Klassiske SharePoint-overvågningslogfiler**

Vi migrerede SPO Legacy-overvågning til Unified audit log (UAL). Dette betyder i det væsentlige, at alle SPO Legacy revisionsrapporter nu vil blive drevet gennem UAL, og de ældre revisions signaler er blevet migreret til UAL.

Vigtige ændringer:

- Beskæring som en egenskab er ikke tilgængelig.
- Den sektion, hvor du vælger bestemte hændelser til overvågning, er ikke tilgængelig. I [dette dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) kan du se en komplet liste over reviderede hændelser, der er tilgængelige som standard.
- Indstillingen "placering" under **tilpassede rapporter** er ikke tilgængelig. 
- Hændelserne "åbning eller hentning af dokumenter" er ikke tilgængelige. 

