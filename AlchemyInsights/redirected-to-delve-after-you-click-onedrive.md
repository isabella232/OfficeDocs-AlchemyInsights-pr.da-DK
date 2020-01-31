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
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571194"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Omdirigeret til Delve, når du har klikket på OneDrive

Se vores detaljerede [fejlfindingsvejledning](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Hvis du vil løse problemet, skal Office 365-administratoren give brugerne ret til at oprette deres websted Mine websteder. Det skyldes, at siden OneDrive for Business er oprettet på Mine websteder.

Følg disse trin for at give denne ret:

1. Klik på **brugerprofiler**i SharePoint Administration.

2. Klik på Administrer **brugertilladelser**i sektionen **Personer** .

3. Tilføj brugere, der har brug for tilladelser til at oprette deres websted Mine websteder. Denne indstilling er som standard angivet til **Alle undtagen eksterne brugere**.

4. Når du har tilføjet brugeren, brugerne eller gruppen, skal du kontrollere, at den tilføjede bruger, brugere eller gruppe er markeret, rulle til afsnittet **Tilladelser** og derefter markere afkrydsningsfeltet ud **for Opret personligt websted (kræves til personliglagring, nyhedsopdatering og fulgt indhold).**

5. Klik på **OK**, og få derefter brugeren til at gå til OneDrive-siden for at oprette webstedet.
