---
title: Konvertere brugerpostkasse til en delt postkasse?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496393"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="85d42-102">Konvertere en postkasse til brugeren til en delt postkasse</span><span class="sxs-lookup"><span data-stu-id="85d42-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="85d42-103">Du kan kun konvertere en brugerpostkasse til en delt postkasse, hvis brugeren har en Exchange-licens.</span><span class="sxs-lookup"><span data-stu-id="85d42-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="85d42-104">Når postkassen er konverteret, vil den fortsat vises i listen over aktive brugere, da listen indeholder delte postkasser.</span><span class="sxs-lookup"><span data-stu-id="85d42-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="85d42-105">Dog vises den konverterede postkasse også i listen over delte postkasser.</span><span class="sxs-lookup"><span data-stu-id="85d42-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="85d42-106">Hvis du forsøger at konvertere en postkasse i Exchange-administrationskonsol, og konverteringen mislykkes, rydde browsercachen, og cookies, og prøv igen.</span><span class="sxs-lookup"><span data-stu-id="85d42-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="85d42-107">Hvis det stadig ikke fungerer, kan du prøve at konvertere postkasse i Exchange Management Shell ved at køre følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="85d42-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="85d42-108">Yderligere oplysninger om konvertering af postkassen er tilgængelig i [konvertere en brugerpostkasse, en delt postkasse](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="85d42-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
