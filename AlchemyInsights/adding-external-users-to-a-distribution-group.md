---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910926"
---
# <a name="add-external-users-to-a-distribution-group"></a>Føje eksterne brugere til en distributionsgruppe

Tilføjelse af en ekstern kontakt til en distributionsgruppe (DG) er en totrinsproces:
  
1. Opret en mailkontaktperson for den eksterne bruger:
    
    1. Gå til siden **Brugere** > [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i Administration. 
    
    2. Vælg **Tilføj en kontakt**.
    
    3. Skriv oplysningerne til kontaktpersonen, og vælg **Tilføj**.
    
2. Føj mailkontakten til dit generaldirektorat:
    
    1. Gå til siden Grupper **i** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) Administration. 
    
    2. Find det Dg, du vil føje den eksterne bruger til, og vælg det for at åbne dialogboksen Rediger.
    
    3. Vælg Vis alle **og administrer medlemmer**under fanen **Medlemmer** . 
    
    4. Vælg **Tilføj medlemmer**.
    
    5. Vælg den mailkontakt, du oprettede i forrige trin, og vælg derefter **Gem**.
    
Hvis dine eksterne brugere efter at have fulgt disse trin ikke kan sende e-mails til generaldirektoratet eller ikke modtager e-mails fra det, kan det skyldes, at gD'et er markeret, så de kun tillader e-mails fra interne brugere. Du kan kontrollere denne konfiguration og rette den efter anvisningerne [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Bemærk:** Disse instruktioner gælder ikke, hvis gruppens type er "Microsoft 365-gruppe" i stedet for "Distributionsgruppe". Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook. Detaljerede oplysninger om gæster i Microsoft 365 Grupper samt instruktioner til tilføjelse af eksterne gæster findes i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  