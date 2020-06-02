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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502601"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker i Exchange Administration

 **Udgave:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Administration gælder ikke for postkasser, eller elementer flyttes ikke til arkivpostkassen eller slettes. 
  
 **Grundlæggende årsager:**
  
- Det kan skyldes, **at assistenten for administrerede mapper** ikke har behandlet brugerens postkasse. Assistenten for administrerede mapper forsøger at behandle alle postkasser i din skybaserede organisation én gang hver syvende dag. Hvis du ændrer en opbevaringskode eller anvender en anden opbevaringspolitik på en postkasse, kan du vente, indtil Den administrerede mappeassistent behandler postkassen, eller du kan køre cmdlet'en Start-ManagedFolderAssistant for at starte assistenten for administrerede mapper for at behandle en bestemt postkasse. Kørsel af denne cmdlet er nyttig til test eller fejlfinding af en opbevaringspolitik eller indstillinger for opbevaringstag. Yderligere oplysninger finder du ved at besøge [Kør assistent for administrerede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kør følgende kommando for at starte assistenten for administrerede mapper for en bestemt postkasse:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også ske, hvis **RetentionHold** er **aktiveret** i postkassen. Hvis postkassen er placeret på et RetentionHold, behandles opbevaringspolitikken på postkassen ikke i det pågældende tidsrum. Du kan finde flere oplysninger om indstillingen RetentionHold under: [Opbevaringsposition i postkassen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontroller status for indstillingen RetentionHold på den specifikke postkasse i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kør følgende kommando for at **deaktivere** RetentionHold på en bestemt postkasse:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kør nu assistenten for administrerede mapper igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler assistenten for administrerede mapper ikke automatisk postkassen.
 
Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration under:
- [Opbevaringskoder og opbevaringspolitikker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Anvende en opbevaringspolitik på postkasser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Tilføje eller fjerne opbevaringskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Sådan identificeres den type venteposition, der er placeret i en postkasse](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
