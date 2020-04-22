---
title: OneDrive for Business Web OneDrive omdirigerer til Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722804"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeret til Delve, når du har klikket på OneDrive

Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

For at løse dette problem skal administratoren give brugerne ret til at oprette webstedet Mine websteder. Det skyldes, at onedrive for business-siden er oprettet på Mine websteder.

Følg disse trin for at give denne rettighed:

1. Klik på **brugerprofiler**i SharePoint Administration.

2. Klik på Administrer **brugertilladelser**i sektionen **Personer** .

3. Tilføj brugere, der har brug for tilladelser til at oprette deres websted Mine websteder. Denne indstilling er som standard angivet til **Alle undtagen eksterne brugere**.

4. Når du har tilføjet brugeren, brugerne eller gruppen, skal du sørge for, at den tilføjede bruger, brugere eller gruppe er markeret, rulle til **afsnittet tilladelser** og derefter markere afkrydsningsfeltet ud for **Opret personligt websted (kræves til personlig lagring, nyhedsopdatering og fulgt indhold).**

5. Klik på **OK**, og få derefter brugeren til at gå til OneDrive-siden for at oprette webstedet.
