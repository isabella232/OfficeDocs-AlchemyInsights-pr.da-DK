---
title: Slet en Teams privat kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 33bf8a5cdc3a8e8da78c9d02e11387a778a7acce483e4485f595d9e05b344433
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948265"
---
# <a name="delete-a-teams-private-channel"></a>Slet en Teams privat kanal

Microsoft har kendskab til et problem med at slette en Teams privat kanal, hvis du har SharePoint Opbevaringspolitikker aktiveret for den underliggende SharePoint websted. Microsoft arbejder på at finde en løsning. I mellemtiden kan du bruge følgende løsninger til at slette den private kanal.

**Udelad gruppen af team/websteder fra SharePoint-opbevaringspolitikken.**

1. Gå til Office 365, og vælg **Vis alle i** venstre navigationsrude.
2. Under **Administration skal du** gå til Security & Compliance **Data** Loss  >  **Prevention**  >  **Policy**.
3. Identificer enhver politik, der gælder for Sharepoint-websteder, og rediger politikken, så Sharepoint-webstedet for teamet, der indeholder den private kanal IKKE er inkluderet i opbevaringspolitikken.
4. Gem politikken.
    Det kan tage op til 24 timer, før politikindstillingerne træder i kraft.
    Når webstedet er blevet udelukket, kan du slette den private kanal.  
    
Du ***kan*** muligvis slette den private kanal ved hjælp af Microsoft Teams på din Android-enhed. 

Du kan SharePoint oplysninger i [Kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).