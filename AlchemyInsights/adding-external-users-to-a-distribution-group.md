---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737867"
---
# <a name="add-external-users-to-a-distribution-group"></a>Føje eksterne brugere til en distributionsgruppe

Tilføjelse af en ekstern kontakt til en distributionsgruppe (DG) er en proces i to trin:
  
1. Opret en e-mail-kontakt for den eksterne bruger:
    
    1. Gå til siden **brugere** > [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i Admin Center. 
    
    2. Vælg **Tilføj en kontakt**.
    
    3. Skriv oplysningerne for kontakten, og vælg **Tilføj**.
    
2. Føj e-mail-kontakten til dit Generaldirektorat:
    
    1. Gå til siden **grupper** > [grupper](https://admin.microsoft.com/adminportal/home#/groups) i Admin Center. 
    
    2. Find det generaldirektorat, du vil føje den eksterne bruger til, og vælg det for at åbne redigeringsdialogen.
    
    3. Under fanen **medlemmer** skal du vælge **Vis alle og Administrer medlemmer**. 
    
    4. Vælg **Tilføj medlemmer**.
    
    5. Vælg den mail kontakt, du oprettede på det forrige trin, og vælg derefter **Gem**.
    
Hvis efterfølgende trin dine eksterne brugere ikke kan sende e-mails til Generaldirektoratet eller ikke modtager e-mails fra det, kan det være, at Generaldirektoratet er markeret til kun at tillade e-mails fra interne brugere. Du kan kontrollere denne konfiguration og ordne det efter anvisningerne [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Bemærk:** Disse instruktioner gælder ikke, hvis gruppens type er "Office 365 Group" i stedet for "distributionsgruppe". Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook. Detaljerede oplysninger om Office 365-grupper gæster samt instruktioner til tilføjelse af eksterne Gæster kan findes i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  