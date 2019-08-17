---
title: Opbevaringspolitikker i Exchange Admin Center virker ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444802"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="deac5-102">Opbevaringspolitikker i Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="deac5-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="deac5-103">**Problem:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Admin Center anvender ikke på postkasser eller elementer ikke er flyttet til arkivet postkassen eller slettet.</span><span class="sxs-lookup"><span data-stu-id="deac5-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="deac5-104">**Grundlæggende årsager:**</span><span class="sxs-lookup"><span data-stu-id="deac5-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="deac5-105">Dette kan skyldes, at den **Styrede mappe assistenten** ikke er behandlet i brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="deac5-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="deac5-106">Den administrerede mappe assistenten prøver at behandle hver postkasse i din skybaserede organisation en gang hver syvende dag.</span><span class="sxs-lookup"><span data-stu-id="deac5-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="deac5-107">Hvis du ændrer et mærke til opbevaring eller anvende en anden opbevaringspolitik på en postkasse, kan du vente, indtil den administrerede mappe bistå behandler postkassen, eller du kan køre cmdlet Start-ManagedFolderAssistant for at starte en administreret Mappeassistent for at behandle en bestemt postkasse.</span><span class="sxs-lookup"><span data-stu-id="deac5-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="deac5-108">Køre denne cmdlet er nyttigt til test eller fejlfinding en opbevaringspolitik eller tilbageholdelse mærke indstillinger.</span><span class="sxs-lookup"><span data-stu-id="deac5-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="deac5-109">Yderligere oplysninger finder du på [Kør en administreret Mappeassistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="deac5-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="deac5-110">**Løsning:** Kør følgende kommando for at starte en administreret Mappeassistent for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="deac5-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="deac5-111">Dette kan også opstå, hvis **RetentionHold** er **aktiveret** for postkassen.</span><span class="sxs-lookup"><span data-stu-id="deac5-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="deac5-112">Hvis postkassen er placeret i en RetentionHold, behandles opbevaringspolitik på postkassen ikke i samme periode.</span><span class="sxs-lookup"><span data-stu-id="deac5-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="deac5-113">For yderligere oplysninger om skal vælge indstillingen RetentionHold se: [Postkasse tilbageholdelse Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="deac5-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="deac5-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="deac5-114">**Solution:**</span></span>
    
  - <span data-ttu-id="deac5-115">Kontroller status for RetentionHold-indstilling på en bestemt postkasse i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="deac5-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="deac5-116">Kør følgende kommando for at **deaktivere** RetentionHold for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="deac5-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="deac5-117">Nu køre igen mappen administreret assistenten:</span><span class="sxs-lookup"><span data-stu-id="deac5-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="deac5-118">**Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler en administreret Mappeassistent ikke automatisk postkassen.</span><span class="sxs-lookup"><span data-stu-id="deac5-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="deac5-119">Se yderligere oplysninger på opbevaringspolitikker i Exchange Admin Center:</span><span class="sxs-lookup"><span data-stu-id="deac5-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="deac5-120">Tilbageholdelse af mærker og opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="deac5-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="deac5-121">Anvende en opbevaringspolitik til postkasser</span><span class="sxs-lookup"><span data-stu-id="deac5-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="deac5-122">Tilføje eller fjerne koder for tilbageholdelse</span><span class="sxs-lookup"><span data-stu-id="deac5-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="deac5-123">Sådan identificeres spærringstype, der er placeret på en postkasse</span><span class="sxs-lookup"><span data-stu-id="deac5-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
