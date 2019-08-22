---
title: Tilføje eksterne brugere til en distributionsgruppe
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494521"
---
# <a name="add-external-users-to-a-distribution-group"></a>Du kan tilføje eksterne brugere til en distributionsgruppe?

Tilføjer en ekstern kontaktperson til en Distribution gruppe (GD) er en proces i 2 trin:
  
1. Oprette en E-mail-kontaktperson til den eksterne bruger:
    
    1. Gå til **brugere**i centeret administration > side med[kontaktpersoner](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Vælg **Tilføj en kontaktperson**.
    
    3. Skriv oplysningerne om kontaktpersonen, og vælg **Tilføj**.
    
2. Føj E-mail-kontaktpersonen til din GD:
    
    1. Gå til **grupper**i centeret administration > [grupper](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Find den GD, du vil tilføje den eksterne bruger, og vælg den for at åbne dialogboksen Rediger.
    
    3. Vælg **Vis alle og administrer medlemmer**under fanen **medlemmer** . 
    
    4. Vælg **Tilføj medlemmer**.
    
    5. Marker den E-mail-kontakt, du oprettede i forrige trin, og vælg derefter **Gem**.
    
Hvis efter følgende eksterne brugere kan ikke sende e-mails til GD eller ikke modtage e-mails fra den, kan det skyldes, at GD er markeret for at tillade kun e-mails fra interne brugere. Du kan kontrollere denne konfiguration og løse problemet efter anvisningerne [her](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Bemærk:** Disse instruktioner gælder ikke, hvis din gruppe er "Office 365 group" i stedet for "Distributionsgruppe." Hvis det er tilfældet, kan du tilføje den eksterne bruger direkte til gruppen fra Outlook. Yderligere oplysninger om Office 365 grupper gæster samt instruktioner til tilføjelse af eksterne gæster kan findes i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  