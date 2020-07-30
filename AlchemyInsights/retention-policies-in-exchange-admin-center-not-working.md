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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522801"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="086c9-102">Opbevaringspolitikker i Exchange Administration</span><span class="sxs-lookup"><span data-stu-id="086c9-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="086c9-103">Hvis du vil have os til at køre automatiske kontroller for de indstillinger, der er nævnt nedenfor, skal du vælge tilbage-knappen < - øverst på denne side, og derefter indtaste e-mail-adressen på den bruger, der har problemer med opbevaring politikker.</span><span class="sxs-lookup"><span data-stu-id="086c9-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="086c9-104">**Udstedelse:** Nyligt oprettede eller opdaterede opbevaringspolitikker i Exchange Administration gælder ikke for postkasser, eller elementer flyttes ikke til arkivpostkassen eller slettes.</span><span class="sxs-lookup"><span data-stu-id="086c9-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="086c9-105">**Grundlæggende årsager:**</span><span class="sxs-lookup"><span data-stu-id="086c9-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="086c9-106">Det kan skyldes, **at assistenten for administrerede** mapper ikke har behandlet brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="086c9-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="086c9-107">Assistenten for administrerede mapper forsøger at behandle alle postkasser i din skybaserede organisation én gang hver syvende dag.</span><span class="sxs-lookup"><span data-stu-id="086c9-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="086c9-108">Hvis du ændrer en opbevaringskode eller anvender en anden opbevaringspolitik på en postkasse, kan du vente, indtil Assisten Til administreret mappe behandler postkassen, eller du kan køre cmdlet'en Start-ManagedFolderAssistant for at starte assistenten For administreret mappe for at behandle en bestemt postkasse.</span><span class="sxs-lookup"><span data-stu-id="086c9-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="086c9-109">Kørsel af denne cmdlet er nyttig til test eller fejlfinding af en opbevaringspolitik eller indstillinger for opbevaringskode.</span><span class="sxs-lookup"><span data-stu-id="086c9-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="086c9-110">Du kan finde flere oplysninger under [Kør assistent for administrerede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="086c9-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="086c9-111">**Løsning:** Kør følgende kommando for at starte assistenten for administrerede mapper for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="086c9-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="086c9-112">Dette kan også ske, hvis **RetentionHold** er **aktiveret** i postkassen.</span><span class="sxs-lookup"><span data-stu-id="086c9-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="086c9-113">Hvis postkassen er placeret på et RetentionHold, behandles opbevaringspolitikken i postkassen ikke i dette tidsrum.</span><span class="sxs-lookup"><span data-stu-id="086c9-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="086c9-114">Du kan finde flere oplysninger om indstillingen RetentionHold under: Opbevaring [af postkasse.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="086c9-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="086c9-115">**Løsning:**</span><span class="sxs-lookup"><span data-stu-id="086c9-115">**Solution:**</span></span>
    
  - <span data-ttu-id="086c9-116">Kontroller status for RetentionHold-indstillingen for den specifikke postkasse i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="086c9-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="086c9-117">Kør følgende kommando for at **deaktivere** RetentionHold på en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="086c9-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="086c9-118">Kør nu assistenten til mappen Administreret igen:</span><span class="sxs-lookup"><span data-stu-id="086c9-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="086c9-119">**Bemærk:** Hvis en postkasse er mindre end 10 MB, behandler assistenten For administreret mappe ikke automatisk postkassen.</span><span class="sxs-lookup"><span data-stu-id="086c9-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="086c9-120">Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration under:</span><span class="sxs-lookup"><span data-stu-id="086c9-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="086c9-121">Opbevaringskoder og opbevaringspolitikker</span><span class="sxs-lookup"><span data-stu-id="086c9-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="086c9-122">Anvende en opbevaringspolitik på postkasser</span><span class="sxs-lookup"><span data-stu-id="086c9-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="086c9-123">Tilføje eller fjerne opbevaringskoder</span><span class="sxs-lookup"><span data-stu-id="086c9-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="086c9-124">Sådan identificeres den type venteposition, der er placeret i en postkasse</span><span class="sxs-lookup"><span data-stu-id="086c9-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
