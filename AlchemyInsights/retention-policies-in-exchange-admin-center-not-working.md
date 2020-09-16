---
title: Opbevaringspolitikker i Exchange Admin Center virker ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740504"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker i Exchange administration

Hvis du vil have os til at køre automatiske tjek af de indstillinger, der er nævnt nedenfor, skal du vælge knappen tilbage <-øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med opbevaringspolitikker.

 **Problem:** Nyligt oprettede eller opdaterede opbevaringspolitikker i Exchange Admin Center gælder ikke for postkasser eller elementer flyttes ikke til arkiv postkassen eller slettes. 
  
 **Rod-årsager:**
  
- Dette kan skyldes, at **assistenten til administrerede mapper** ikke har behandlet brugerens postkasse. Assistent til administrerede mapper forsøger at behandle hver postkasse i din skybaserede organisation én gang hver syvende dag. Hvis du ændrer et opbevarings mærke eller anvender en anden opbevaringspolitik til en postkasse, kan du vente, indtil den administrerede mappe hjælper med at behandle postkassen, eller du kan køre Start-ManagedFolderAssistant-cmdlet'en for at starte en bestemt postkasse. Det er nyttigt at køre denne cmdlet for at teste eller foretage fejlfinding af en opbevaringspolitik eller indstillinger for opbevarings mærker. Hvis du vil have mere at vide, skal du gå til [Kør administreret mappe assistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kør følgende kommando for at starte assistenten administreret mappe for en bestemt postkasse:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også ske, hvis **RetentionHold** er blevet **aktiveret** på postkassen. Hvis postkassen er blevet placeret på en RetentionHold, bliver opbevaringspolitikken på postkassen ikke behandlet i det pågældende tidspunkt. Du kan finde flere oplysninger på RetentionHold-indstillingen under: [bevarelse af postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Løsning**
    
  - Kontrollér status for indstillingen RetentionHold i den specifikke postkasse i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kør følgende kommando for at **deaktivere** RetentionHold på en bestemt postkasse:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kør nu den administrerede mappe assistent igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Bemærk:** Hvis en postkasse er mindre end 10 MB, vil den administrerede mappe assistent ikke automatisk behandle postkassen.
 
Du kan finde flere oplysninger om opbevaringspolitikker i Exchange administration ved at gå til:
- [Opbevarings mærker og opbevaringspolitikker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Anvende en opbevaringspolitik til postkasser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Tilføje eller fjerne opbevarings mærker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Sådan identificerer du den type venteposition, der er placeret i en postkasse](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
