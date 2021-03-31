---
title: 126 Fejlen "Henter en postkasse" i OWA blev ikke fundet?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426656"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Får du en postkassefejl, som ikke blev fundet i Outlook på internettet?

Hvis du bruger Outlook på internettet, og du får en postkasse, der ikke blev fundet **som** fejl, har den konto, du brugte til at oprette forbindelse til Outlook på internettet, ikke en Exchange Online-licens, og derfor er der ikke knyttet nogen postkasse til kontoen. Din administrator kan tildele en licens til din konto ved at følge disse trin:

1. Åbn [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) Administration, og gå  til **Aktive** brugere under sektionen Brugere, og vælg den bruger, der får vist fejlen.

2. På brugersiden, der åbnes, skal du gå til  sektionen Licenser og **apps,** vælge den relevante placeringsværdi og tildele en licens, der indeholder Exchange Online (udvid licensen for at få vist dens detaljer). Klik på Gem ændringer, når du **er færdig.**

I nogle tilfælde, hvis licensen allerede er tildelt en brugerkonto, hjælper fjernelse og gentildeling af licensen med at løse problemet og få den klargjort korrekt i systemet: 

- Kontrollér, om dine M365 Exchange Online-abonnementer (og andre, hvis du har nogen) er aktuelle og ikke er udløbet for nylig.

Når du har kontrolleret, at dit abonnement ikke er udløbet, og der er tildelt en gyldig licens til brugerkontoen, kan der gå op til 24 timer, før licensen er klargjort, så det kan være en god ide at vente på, at problemet bliver løst. Du kan få mere at vide [under Tildel og administrer licenser.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)