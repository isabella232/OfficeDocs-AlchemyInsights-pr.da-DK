---
title: Read-Only meddelelse om vedligeholdelse, når du forsøger at bruge SharePoint eller OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910540"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only meddelelse om vedligeholdelse, når du forsøger at bruge SharePoint eller OneDrive

Brugere modtager muligvis en **meddelelse om skrivebeskyttet** vedligeholdelse, når de forsøger at bruge SharePoint eller OneDrive til et af følgende scenarier. 

-   En planlagt eller aktiv vedligeholdelsesaktivitet.  Søg efter dem ved at navigere til [Meddelelsescenter](https://portal.office.com/adminportal/home#/messagecenter).
-   En aktiv tjenestehændelse med høj prioritet, der kan forekomme. Se efter eventuelle råd/hændelser ved at gå til [Tjeneste sundhed](https://portal.office.com/adminportal/home#/servicehealth).
-   Et mindre scenarie med automatisk genoprettelse, der kan forekomme pga. uventede hændelser på serverne, som kan vare mindre end 30 min. 
    
    Der er ingen indlæg til Meddelelsescenter eller Tjenestestilstand for disse mindre gendannelser, men du bør meget snart vende tilbage til normal.

Meget få gange har vi observeret, at et af de tre scenarier, der er nævnt ovenfor, har været årsagen, og tjenesten er blevet gendannet, men brugernes browsercache er ikke blevet ryddet.

Forsøg at rydde browsercachen, før du navigerer til webstedet.

1. I din Microsoft Edge skal du **vælge** Indstillinger og derefter vælge Beskyttelse af **personlige oplysninger og sikkerhed**.
2. Under **Ryd browser skal** du vælge Vælg, hvad der skal **ryddes**.
3. Vælg **Cookies og gemte webstedsdata,** og vælg **Ryd**.

>[!Note] 
> Disse trin kan variere, når du bruger andre browsere, f.eks Mozilla Firefox eller Google Chrome.

>[!Note] 
> En anden mulighed ville være at åbne SharePoint websted eller OneDrive i et nyt InPrivate-vindue.