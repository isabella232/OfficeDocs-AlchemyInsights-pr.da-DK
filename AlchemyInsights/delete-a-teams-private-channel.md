---
title: Slette en privat Teams-kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438991"
---
# <a name="delete-a-teams-private-channel"></a>Slette en privat Teams-kanal

Microsoft er opmærksom på et problem med at slette en privat Teams-kanal, hvis du har aktiveret SharePoint-opbevaringspolitikker for det underliggende SharePoint-websted. Microsoft arbejder på en rettelse. I mellemtiden kan du bruge følgende løsninger til at slette den private kanal.

**Ekskluder gruppen/gruppen af websteder fra sharepoint-opbevaringspolitikken.**

1. Gå til Office 365-administrationsportalen, og vælg **Vis alle** i venstre navigationsrude.
2. Gå **til Sikkerhedskontrol**i **& overvågningspolitik**for  >  **datatab**under  >  **Administration**.
3. Identificer en politik, der gælder for Sharepoint-websteder, og rediger politikken, så Sharepoint-webstedet for det team, der indeholder den private kanal, IKKE er inkluderet i opbevaringspolitikken.
4. Gem politikken.
    Det kan tage op til 24 timer, før politikindstillinger træder i kraft.
    Når webstedet er blevet udeladt, kan du slette den private kanal.  
    
Du ***kan*** muligvis slette den private kanal ved hjælp af Microsoft Teams på din Android-enhed. 

Du kan finde relaterede SharePoint-oplysninger [under Kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).