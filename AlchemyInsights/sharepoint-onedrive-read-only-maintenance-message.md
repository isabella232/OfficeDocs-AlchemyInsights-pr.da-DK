---
title: Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670826"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivebeskyttet for vedligeholdelses meddelelse, når du forsøger at bruge SharePoint eller OneDrive

Brugere kan modtage en **skrivebeskyttet til vedligeholdelses** meddelelse, når de forsøger at bruge SharePoint eller OneDrive til en af følgende scenarier. 

-   En planlagt eller aktiv vedligeholdelses aktivitet.  Du kan søge efter dem ved at gå til [meddelelses Center](https://portal.office.com/adminportal/home#/messagecenter).
-   En høj prioritet, aktiv tjeneste hændelse, der kan forekomme. Kontrollér, om der er rådgivere/Incidents ved at navigere til [tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).
-   Et mindre automatisk reparerende genoprettelses scenarie, der kan ske på grund af eventuelle uventede begivenheder på de servere, der muligvis er på under 30 min. 
    
    Der er ingen meddelelses Center-eller tjeneste Tilstandsposter for disse mindre regress, men du bør snart være tilbage til normal.

I ganske få tilfælde observerede vi, at et af de tre scenarier, der er nævnt ovenfor, har været årsag til, at tjenesten er blevet gendannet, men browserens browsercache er ikke blevet ryddet op.

Prøv at rydde browsercachen, før du navigerer til webstedet.

1. Vælg **Indstillinger**i din Microsoft Edge-browser, og vælg derefter **beskyttelse af personlige oplysninger og sikkerhed**.
2. Under **Ryd browsing**skal du vælge **Vælg det, der skal ryddes**.
3. Vælg **cookies og gemte webstedsdata**, og vælg **Ryd**.

>[!Note] 
> Disse trin kan være forskellige, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.

>[!Note] 
> En anden mulighed er at åbne dit SharePoint-websted eller OneDrive i et nyt InPrivate-vindue.