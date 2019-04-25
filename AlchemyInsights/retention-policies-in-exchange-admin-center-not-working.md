---
title: Opbevaringspolitikker i Exchange Admin Center virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371292"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker i Exchange Admin Center

 **Problem:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Admin Center anvender ikke på postkasser eller elementer ikke er flyttet til arkivet postkassen eller slettet. 
  
 **Grundlæggende årsager:**
  
- Dette kan skyldes, at den **Styrede mappe assistenten** ikke er behandlet i brugerens postkasse. Den administrerede mappe assistenten prøver at behandle hver postkasse i din skybaserede organisation en gang hver syvende dag. Hvis du ændrer et mærke til opbevaring eller anvende en anden opbevaringspolitik på en postkasse, kan du vente, indtil den administrerede mappe bistå behandler postkassen, eller du kan køre cmdlet Start-ManagedFolderAssistant for at starte en administreret Mappeassistent for at behandle en bestemt postkasse. Køre denne cmdlet er nyttigt til test eller fejlfinding en opbevaringspolitik eller tilbageholdelse mærke indstillinger. Yderligere oplysninger finder du på [Kør en administreret Mappeassistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kør følgende kommando for at starte en administreret Mappeassistent for en bestemt postkasse: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også opstå, hvis **RetentionHold** er **aktiveret** for postkassen. Hvis postkassen er placeret i en RetentionHold, behandles opbevaringspolitik på postkassen ikke i samme periode. For yderligere oplysninger om skal vælge indstillingen RetentionHold se: [Postkasse tilbageholdelse Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontroller status for RetentionHold-indstilling på en bestemt postkasse i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kør følgende kommando for at **deaktivere** RetentionHold for en bestemt postkasse: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nu køre igen mappen administreret assistenten:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler en administreret Mappeassistent ikke automatisk postkassen. 
  

