---
title: OneDrive for Business Web OneDrive omdirigerer til Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799983"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeret til Delve, når du har klikket på OneDrive

Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

For at løse dette problem skal administratoren give brugerne ret til at oprette deres Mit websted-websted. Dette skyldes, at siden OneDrive for Business oprettes på Mine websteder.

Hvis du vil tildele denne ret, skal du følge disse trin:

1. Klik på brugerprofiler i SharePoint **Administration.**

2. I sektionen **Personer** skal du klikke **på Administrer brugertilladelser**.

3. Tilføj brugere, der skal have tilladelse til at oprette deres Mit websted-websted. Denne indstilling er som standard indstillet til **Alle undtagen eksterne brugere.**

4. Når du har tilføjet brugeren, brugerne eller gruppen, skal du kontrollere, at den tilføjede bruger, brugere eller gruppe er markeret, rulle ned til **tilladelsessektionen** og derefter markere afkrydsningsfeltet ud for Opret personligt websted (påkrævet til personligt **lager, nyhedsstrøm** og fulgte indhold).

5. Klik **på OK,** og få derefter brugeren til at gå til OneDrive-siden for at oprette webstedet.
