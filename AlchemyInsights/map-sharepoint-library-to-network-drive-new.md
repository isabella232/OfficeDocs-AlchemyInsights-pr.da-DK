---
title: Knytte et SharePoint til et netværksdrev
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315542"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Knytte et SharePoint til et netværksdrev

I stedet for at tilknytte et netværksdrev skal SharePoint filer med den OneDrive-synkronisering klient, som leverer Files On-Demand. Få adgang til alle dine filer OneDrive uden brug af lokal lagerplads. Få mere at vide under [Synkroniser SharePoint- Teams](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) filer med din computer og Gem [diskplads med OneDrive Files On-Demand til Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

Hvis du vælger at tilknytte et drev i stedet for at bruge [den nye OneDrive-synkronisering klient,](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)skal du sørge for at følge disse trin:

- [Fejlfinding af tilknyttede netværksdrev, der opretter forbindelse til SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Godkendelsesfejl opstår, når klienten ikke har understøttelse af TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**BEMÆRK!** Hvis du bruger Internet Explorer 10 med Windows 8 eller Windows 7 og modtager Access  nægtet, eller **Sti** ikke er tilgængelig, når du tilknytter et drev, kan du løse dette problem ved at installere dette [hotfix.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)