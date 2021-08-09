---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934827"
---
# <a name="add-external-users-to-a-distribution-group"></a>Føje eksterne brugere til en distributionsgruppe

Tilføjelse af en ekstern kontakt til en distributionsgruppe (DG) er en proces i to trin:
  
1. Opret en mailkontakt for den eksterne bruger:
    
    1. I Administration skal du gå til **siden**  >  [Brugeres](https://admin.microsoft.com/adminportal/home#/Contact) kontakter. 
    
    2. Vælg **Tilføj en kontakt**.
    
    3. Skriv oplysningerne for din kontakt, og vælg **Tilføj**.
    
2. Føj Mailkontakten til din DG:
    
    1. I Administration skal du gå til **siden**  >  [Grupper.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Find den DG, du vil føje den eksterne bruger til, og vælg den for at åbne dialogboksen Rediger.
    
    3. På fanen **Medlemmer** skal du vælge **Vis alle og administrer medlemmer.** 
    
    4. Vælg **Tilføj medlemmer**.
    
    5. Vælg den Mailkontakt, du oprettede i forrige trin, og vælg derefter **Gem**.
    
Hvis de eksterne brugere ikke kan sende mails til DG eller ikke modtager mails fra den, kan det være fordi, DG er markeret til kun at tillade mails fra interne brugere. Du kan kontrollere denne konfiguration og rette det ved at følge vejledningen [her.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Bemærk!** Denne vejledning gælder ikke, hvis din gruppes type er "Microsoft 365 gruppe" i stedet for "Distributionsgruppe". Hvis det er tilfældet, kan du tilføje den eksterne bruger direkte til gruppen fra Outlook. Detaljerede oplysninger om Microsoft 365 gruppe gæster samt instruktioner til at tilføje eksterne gæster kan findes i [denne artikel.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  