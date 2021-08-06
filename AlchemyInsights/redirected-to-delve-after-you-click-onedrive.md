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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922981"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeret til en Delve, når du klikker på OneDrive

Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

For at løse dette problem skal administratoren give brugerne ret til at oprette deres Mit websted-websted. Dette skyldes, at OneDrive for Business oprettes på Mine websteder.

Hvis du vil tildele denne ret, skal du følge disse trin:

1. Klik SharePoint brugerprofiler i **Administration.**

2. I sektionen **Personer** skal du klikke **på Administrer brugertilladelser**.

3. Tilføj brugere, der skal have tilladelse til at oprette deres Mit websted-websted. Denne indstilling er som standard indstillet til **Alle undtagen eksterne brugere.**

4. Når du har tilføjet brugeren, brugerne eller gruppen, skal du kontrollere, at den tilføjede bruger, brugere eller gruppe er markeret, rulle ned til **tilladelsessektionen** og derefter markere afkrydsningsfeltet ud for Opret personligt websted (påkrævet til personligt **lager, nyhedsstrøm** og fulgte indhold).

5. Klik **på OK,** og få derefter brugeren til at gå til OneDrive for at oprette webstedet.
