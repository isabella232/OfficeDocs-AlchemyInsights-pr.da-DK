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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663507"
---
# <a name="add-external-users-to-a-distribution-group"></a>Føje eksterne brugere til en distributionsgruppe

Tilføjelse af en ekstern kontakt til en distributionsgruppe er en proces i to trin:
  
1. Opret en mail kontakt for den eksterne bruger:
    
    1. I administration skal du gå til siden med **Users**  >  [Kontaktpersoner](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Vælg **Tilføj en kontaktperson**.
    
    3. Skriv oplysningerne for kontakten, og vælg **Tilføj**.
    
2. Føj mail kontakten til din DG:
    
    1. I administration skal du gå til siden **grupper**-  >  [grupper](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Find den DG, du vil føje den eksterne bruger til, og vælg den for at åbne dialogboksen Rediger.
    
    3. På fanen **medlemmer** skal du vælge **Vis alle og Administrer medlemmer**. 
    
    4. Vælg **Tilføj medlemmer**.
    
    5. Vælg den mail kontakt, du oprettede på det forrige trin, og vælg derefter **Gem**.
    
Hvis dine eksterne brugere efter at have fulgt disse trin ikke kan sende mails til DG eller ikke modtager mails fra den, kan det være, at DG er markeret til kun at tillade mails fra interne brugere. Du kan kontrollere denne konfiguration og rette den ved at følge vejledningen [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Bemærk:** Disse instruktioner gælder ikke, hvis din gruppes type er "Microsoft 365-gruppe" i stedet for "distributionsgruppe". Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook. Du kan finde detaljerede oplysninger om Microsoft 365-grupper gæster samt instruktioner til at tilføje eksterne gæster i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  