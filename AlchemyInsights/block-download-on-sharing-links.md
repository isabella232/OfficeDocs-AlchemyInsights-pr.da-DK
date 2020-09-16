---
title: Bloker hentning af delingslinks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685736"
---
# <a name="block-download-on-sharing-links"></a>Bloker hentning af delingslinks

**Bloker hentning** er tilgængelig for **skrivebeskyttede links** til Office-dokumenter. Når du vælger denne indstilling, kan personer, der får adgang til filen via det link, du har oprettet, ikke se muligheder for at hente, udskrive eller kopiere filen.

Administratorer kan kontrollere, om indstillingen "Bloker hentning af filer" kun vises for Office-filer eller ej ved at ændre `BlockDownloadLinksFileType` indstillingen i PowerShell [-cmdlet'en Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) eller [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .
