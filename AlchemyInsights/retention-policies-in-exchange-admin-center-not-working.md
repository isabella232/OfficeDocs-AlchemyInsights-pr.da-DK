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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="03e11-102">Opbevaringspolitikker i Exchange administration</span><span class="sxs-lookup"><span data-stu-id="03e11-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="03e11-103">Hvis du vil have os til at køre automatiske tjek af de indstillinger, der er nævnt nedenfor, skal du vælge knappen tilbage <-øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med opbevaringspolitikker.</span><span class="sxs-lookup"><span data-stu-id="03e11-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="03e11-104">**Problem:** Nyligt oprettede eller opdaterede opbevaringspolitikker i Exchange Admin Center gælder ikke for postkasser eller elementer flyttes ikke til arkiv postkassen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="03e11-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="03e11-105">**Rod-årsager:**</span><span class="sxs-lookup"><span data-stu-id="03e11-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="03e11-106">Dette kan skyldes, at **assistenten til administrerede mapper** ikke har behandlet brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="03e11-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="03e11-107">Assistent til administrerede mapper forsøger at behandle hver postkasse i din skybaserede organisation én gang hver syvende dag.</span><span class="sxs-lookup"><span data-stu-id="03e11-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="03e11-108">Hvis du ændrer et opbevarings mærke eller anvender en anden opbevaringspolitik til en postkasse, kan du vente, indtil den administrerede mappe hjælper med at behandle postkassen, eller du kan køre Start-ManagedFolderAssistant-cmdlet'en for at starte en bestemt postkasse.</span><span class="sxs-lookup"><span data-stu-id="03e11-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="03e11-109">Det er nyttigt at køre denne cmdlet for at teste eller foretage fejlfinding af en opbevaringspolitik eller indstillinger for opbevarings mærker.</span><span class="sxs-lookup"><span data-stu-id="03e11-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="03e11-110">Hvis du vil have mere at vide, skal du gå til [Kør administreret mappe assistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="03e11-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="03e11-111">**Løsning:** Kør følgende kommando for at starte assistenten administreret mappe for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="03e11-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="03e11-112">Dette kan også ske, hvis **RetentionHold** er blevet **aktiveret** på postkassen.</span><span class="sxs-lookup"><span data-stu-id="03e11-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="03e11-113">Hvis postkassen er blevet placeret på en RetentionHold, bliver opbevaringspolitikken på postkassen ikke behandlet i det pågældende tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="03e11-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="03e11-114">Du kan finde flere oplysninger på RetentionHold-indstillingen under: [bevarelse af postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="03e11-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="03e11-115">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="03e11-115">**Solution:**</span></span>
    
  - <span data-ttu-id="03e11-116">Kontrollér status for indstillingen RetentionHold i den specifikke postkasse i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="03e11-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="03e11-117">Kør følgende kommando for at **deaktivere** RetentionHold på en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="03e11-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="03e11-118">Kør nu den administrerede mappe assistent igen:</span><span class="sxs-lookup"><span data-stu-id="03e11-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="03e11-119">**Bemærk:** Hvis en postkasse er mindre end 10 MB, vil den administrerede mappe assistent ikke automatisk behandle postkassen.</span><span class="sxs-lookup"><span data-stu-id="03e11-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="03e11-120">Du kan finde flere oplysninger om opbevaringspolitikker i Exchange administration ved at gå til:</span><span class="sxs-lookup"><span data-stu-id="03e11-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="03e11-121">Opbevarings mærker og opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="03e11-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="03e11-122">Anvende en opbevaringspolitik til postkasser</span><span class="sxs-lookup"><span data-stu-id="03e11-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="03e11-123">Tilføje eller fjerne opbevarings mærker</span><span class="sxs-lookup"><span data-stu-id="03e11-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="03e11-124">Sådan identificerer du den type venteposition, der er placeret i en postkasse</span><span class="sxs-lookup"><span data-stu-id="03e11-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
