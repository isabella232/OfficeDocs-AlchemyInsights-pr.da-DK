---
title: Opbevaringspolitikker i Exchange Admin Center virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786764"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6bea2-102">Opbevaringspolitikker i Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="6bea2-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="6bea2-103">**Problem:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Admin Center anvender ikke på postkasser eller elementer ikke er flyttet til arkivet postkassen eller slettet.</span><span class="sxs-lookup"><span data-stu-id="6bea2-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6bea2-104">**Grundlæggende årsager:**</span><span class="sxs-lookup"><span data-stu-id="6bea2-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="6bea2-p101">Dette kan skyldes, at den **Styrede mappe assistenten** ikke er behandlet i brugerens postkasse. Den administrerede mappe assistenten prøver at behandle hver postkasse i din skybaserede organisation en gang hver syvende dag. Hvis du ændrer et mærke til opbevaring eller anvende en anden opbevaringspolitik på en postkasse, kan du vente, indtil den administrerede mappe bistå behandler postkassen, eller du kan køre cmdlet Start-ManagedFolderAssistant for at starte en administreret Mappeassistent for at behandle en bestemt postkasse. Køre denne cmdlet er nyttigt til test eller fejlfinding en opbevaringspolitik eller tilbageholdelse mærke indstillinger. Yderligere oplysninger finder du på [Kør en administreret Mappeassistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="6bea2-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6bea2-110">**Løsning:** Kør følgende kommando for at starte en administreret Mappeassistent for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="6bea2-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6bea2-p102">Dette kan også opstå, hvis **RetentionHold** er **aktiveret** for postkassen. Hvis postkassen er placeret i en RetentionHold, behandles opbevaringspolitik på postkassen ikke i samme periode. For yderligere oplysninger om skal vælge indstillingen RetentionHold se: [Postkasse tilbageholdelse Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6bea2-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6bea2-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="6bea2-114">**Solution:**</span></span>
    
  - <span data-ttu-id="6bea2-115">Kontroller status for RetentionHold-indstilling på en bestemt postkasse i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="6bea2-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6bea2-116">Kør følgende kommando for at **deaktivere** RetentionHold for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="6bea2-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6bea2-117">Nu køre igen mappen administreret assistenten:</span><span class="sxs-lookup"><span data-stu-id="6bea2-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6bea2-118">**Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler en administreret Mappeassistent ikke automatisk postkassen.</span><span class="sxs-lookup"><span data-stu-id="6bea2-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

