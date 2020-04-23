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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="2b627-102">Opbevaringspolitikker i Exchange Administration</span><span class="sxs-lookup"><span data-stu-id="2b627-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="2b627-103">**Spørgsmål:** Nyoprettede eller opdaterede opbevaringspolitikker i Exchange Administration gælder ikke for postkasser, eller elementer flyttes ikke til arkivpostkassen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="2b627-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="2b627-104">**Grundlæggende årsager:**</span><span class="sxs-lookup"><span data-stu-id="2b627-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="2b627-105">Det kan skyldes, **at assistenten til administrerede mapper** ikke har behandlet brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="2b627-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="2b627-106">Assistenten til administrerede mapper forsøger at behandle alle postkasser i din skybaserede organisation én gang hver syvende dag.</span><span class="sxs-lookup"><span data-stu-id="2b627-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="2b627-107">Hvis du ændrer en opbevaringskode eller anvender en anden opbevaringspolitik på en postkasse, kan du vente, indtil Assist en administreret mappe behandler postkassen, eller du kan køre cmdlet'en StartManagedFolderAssistant for at starte assistenten til administrerede mapper for at behandle en bestemt postkasse.</span><span class="sxs-lookup"><span data-stu-id="2b627-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="2b627-108">Kørsel af denne cmdlet er nyttig til test eller fejlfinding af en opbevaringspolitik eller indstillinger for opbevaringskode.</span><span class="sxs-lookup"><span data-stu-id="2b627-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="2b627-109">Yderligere oplysninger finder du under [Kør assistenten til administrerede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="2b627-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="2b627-110">**Løsning:** Kør følgende kommando for at starte assistenten til administrerede mapper for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="2b627-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="2b627-111">Dette kan også ske, hvis **RetentionHold** **er** aktiveret i postkassen.</span><span class="sxs-lookup"><span data-stu-id="2b627-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="2b627-112">Hvis postkassen er placeret på et RetentionHold, behandles opbevaringspolitikken på postkassen ikke i dette tidsrum.</span><span class="sxs-lookup"><span data-stu-id="2b627-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="2b627-113">Du kan finde flere oplysninger om indstillingen RetentionHold under: [Tilbageholdelse af postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="2b627-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="2b627-114">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="2b627-114">**Solution:**</span></span>
    
  - <span data-ttu-id="2b627-115">Kontroller status for indstillingen RetentionHold på den specifikke postkasse i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="2b627-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="2b627-116">Kør følgende kommando for at **deaktivere** RetentionHold i en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="2b627-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="2b627-117">Kør nu assistenten til administrerede mapper igen:</span><span class="sxs-lookup"><span data-stu-id="2b627-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="2b627-118">**Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler assistenten for administrerede mapper ikke automatisk postkassen.</span><span class="sxs-lookup"><span data-stu-id="2b627-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="2b627-119">Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration under:</span><span class="sxs-lookup"><span data-stu-id="2b627-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="2b627-120">Opbevaringskoder og opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="2b627-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="2b627-121">Anvende en opbevaringspolitik på postkasser</span><span class="sxs-lookup"><span data-stu-id="2b627-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="2b627-122">Tilføje eller fjerne fastholdelseskoder</span><span class="sxs-lookup"><span data-stu-id="2b627-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="2b627-123">Sådan identificeres den type venteposition, der er placeret i en postkasse</span><span class="sxs-lookup"><span data-stu-id="2b627-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
