---
title: Opbevaringspolitikker i Exchange Administration fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742427"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker i Exchange Administration

 **Spørgsmål:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Administration gælder ikke for postkasser, eller elementer flyttes ikke til arkivpostkassen eller slettes. 
  
 **Grundlæggende årsager:**
  
- Det kan skyldes, **at assistenten til administrerede mapper** ikke har behandlet brugerens postkasse. Assistenten til administrerede mapper forsøger at behandle alle postkasser i din skybaserede organisation én gang hver syvende dag. Hvis du ændrer en opbevaringskode eller anvender en anden opbevaringspolitik på en postkasse, kan du vente, indtil Assist en administreret mappe behandler postkassen, eller du kan køre cmdlet'en StartManagedFolderAssistant for at starte assistenten til administrerede mapper for at behandle en bestemt postkasse. Kørsel af denne cmdlet er nyttig til test eller fejlfinding af en opbevaringspolitik eller indstillinger for opbevaringskode. Yderligere oplysninger finder du under [Kør assistenten til administrerede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kør følgende kommando for at starte assistenten til administrerede mapper for en bestemt postkasse:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også ske, hvis **RetentionHold** **er** aktiveret i postkassen. Hvis postkassen er placeret på et RetentionHold, behandles opbevaringspolitikken på postkassen ikke i dette tidsrum. Du kan finde flere oplysninger om indstillingen RetentionHold under: [Tilbageholdelse af postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontroller status for indstillingen RetentionHold på den specifikke postkasse i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kør følgende kommando for at **deaktivere** RetentionHold i en bestemt postkasse:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kør nu assistenten til administrerede mapper igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler assistenten for administrerede mapper ikke automatisk postkassen.
 
Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration under:
- [Opbevaringskoder og opbevaringspolitikker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Anvende en opbevaringspolitik på postkasser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Tilføje eller fjerne fastholdelseskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Sådan identificeres den type venteposition, der er placeret i en postkasse](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
