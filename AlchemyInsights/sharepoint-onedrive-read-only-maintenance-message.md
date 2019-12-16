---
title: Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051275"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive

Brugere kan modtage en **skrivebeskyttet meddelelse om vedligeholdelse** , når de forsøger at bruge SharePoint eller OneDrive til et af følgende scenarier. 

-   En planlagt eller aktiv vedligeholdelsesaktivitet.  Tjek for dem ved at navigere til [meddelelsescenteret](https://portal.office.com/adminportal/home#/messagecenter).
-   En aktiv tjeneste hændelse med høj prioritet, der kan forekomme. Søg efter meddelelser/hændelser ved at navigere til [tjenestens tilstand](https://portal.office.com/adminportal/home#/servicehealth).
-   En mindre Auto-healing opsving scenario, der kunne ske på grund af uventede begivenheder på serverne, som kan vare mindre end 30 min eller deromkring. 
    
    Der er ingen Message Center eller service Health posts for disse mindre inddrivelser, men du skal være tilbage til normal meget snart.

Ved meget få lejligheder bemærkede vi, at en af de tre scenarier, der er anført ovenfor har været årsag, og tjenesten er blevet genoprettet, men brugerne browser cache er ikke blevet ryddet op.

Forsøg at rydde browserens cache, før du navigerer til webstedet.

1. I din Microsoft Edge-browser skal du vælge **Indstillinger**og derefter vælge **beskyttelse af personlige oplysninger og sikkerhed**.
2. Under **Ryd browsing**skal du vælge **Vælg, hvad du vil rydde**.
3. Vælg **cookies og gemte webstedsdata**, og vælg **Ryd**.

>[!Note] 
> Disse trin kan afvige, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.

>[!Note] 
> En anden mulighed ville være at åbne dit SharePoint-websted eller OneDrive i et nyt InPrivate-vindue.