---
title: Indstil autosvar for en postkasse
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820928"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="b332f-102">Indstil autosvar for en brugers postkasse</span><span class="sxs-lookup"><span data-stu-id="b332f-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="b332f-103">**Metode 1**</span><span class="sxs-lookup"><span data-stu-id="b332f-103">**Method 1**</span></span>

1. <span data-ttu-id="b332f-104">Log på Microsoft 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="b332f-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="b332f-105">Gå til **Brugere > Aktive brugere** (eller **Grupper > Delte postkasser**, hvis du indstiller dette for en delt postkasse).</span><span class="sxs-lookup"><span data-stu-id="b332f-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="b332f-106">Vælg en bruger, der har en Microsoft Exchange-postkasse.</span><span class="sxs-lookup"><span data-stu-id="b332f-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="b332f-107">I menuen, der kommer frem i højre side, skal du gå til **Mailindstillinger > Autosvar** (hvis det er en delt postkasse, skal du blot klikke på **Autosvar** i menuen).</span><span class="sxs-lookup"><span data-stu-id="b332f-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="b332f-108">**Metode 2**</span><span class="sxs-lookup"><span data-stu-id="b332f-108">**Method 2**</span></span>

1. <span data-ttu-id="b332f-109">Log på Microsoft 365-administratorportalen ved hjælp af administratorens legitimationsoplysninger.</span><span class="sxs-lookup"><span data-stu-id="b332f-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="b332f-110">Udvid **Administration**, og klik derefter på **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b332f-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="b332f-111">Klik på billedet i øverste højre hjørne, klik på **En anden bruger**, og vælg derefter den brugerpostkasse, du vil ændre.</span><span class="sxs-lookup"><span data-stu-id="b332f-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="b332f-112">I venstre side skal du vælge **Indstillinger**, klikke på **Organiser mails** og derefter klikke på **Autosvar.**</span><span class="sxs-lookup"><span data-stu-id="b332f-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="b332f-113">**Metode 3**</span><span class="sxs-lookup"><span data-stu-id="b332f-113">**Method 3**</span></span>

<span data-ttu-id="b332f-114">Kør følgende cmdlet i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b332f-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b332f-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b332f-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="b332f-116">Du kan finde flere oplysninger om denne cmdlet under [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="b332f-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
