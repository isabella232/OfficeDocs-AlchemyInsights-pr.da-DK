---
title: Skrivebeskyttet for vedligeholdelse, når du forsøger at bruge SharePoint- eller OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620717"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivebeskyttet for vedligeholdelse, når du forsøger at bruge SharePoint- eller OneDrive

Brugere kan modtager meddelelsen **Skrivebeskyttet for vedligeholdelse** , når du forsøger at bruge SharePoint- eller OneDrive til en af følgende situationer. 

-   En planlagt eller aktiv vedligeholdelse aktivitet.  Søge efter dem ved at gå til [Message Center](https://portal.office.com/adminportal/home#/messagecenter).
-   En høj prioritet, aktiv tjeneste hændelse, der kan forekomme. Kontrollere, om eventuelle råd om hændelser ved at navigere til [Service sundhed](https://portal.office.com/adminportal/home#/servicehealth).
-   En mindre automatisk reparationspenselværktøjet nedbrud, der kunne ske noget på grund af uventede hændelser på de servere, som måske sidste for mindre end 30 min. eller så. 
    
    Der er ingen meddelelse Center eller Service sundhed bogføres for disse mindre tilbagebetalinger, men du skal være tilbage til normal snart.

I meget få tilfælde konstaterede vi, at et af de tre scenarier, der er anført ovenfor, er årsagen, og service er blevet gendannet, men browsercachen brugerne endnu ikke ryddet.

Du bør forsøge at rydde browsercachen før navigere til webstedet.

1. Vælg **Indstillinger**i browseren Microsoft Edge, og vælg derefter **personlige oplysninger og sikkerhed**.
2. Vælg **vælge Ryd**under **Ryd søgning**.
3. Vælg **Cookies og gemt webstedet data**, og vælg **Slet**.

>[!Note] 
> Disse trin kan variere, når du bruger andre browsere som Mozilla Firefox eller Google Chrome.

>[!Note] 
> En anden mulighed ville være at åbne SharePoint-webstedet eller OneDrive i et nyt InPrivate-vindue.