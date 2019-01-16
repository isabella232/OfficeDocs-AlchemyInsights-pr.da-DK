---
title: Konvertere brugerpostkasse til en delt postkasse?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283328"
---
<span data-ttu-id="b7140-p101">Du kan kun konvertere en brugerpostkasse til en delt postkasse, hvis brugeren har en Exchange-licens. Når postkassen er konverteret, vil den fortsat vises i listen over aktive brugere, da listen indeholder delte postkasser. Dog vises den konverterede postkasse også i listen over delte postkasser.</span><span class="sxs-lookup"><span data-stu-id="b7140-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="b7140-p102">Hvis du forsøger at konvertere en postkasse i Exchange-administrationskonsol, og konverteringen mislykkes, rydde browsercachen, og cookies, og prøv igen. Hvis det stadig ikke fungerer, kan du prøve at konvertere postkasse i Exchange Management Shell ved at køre følgende kommando:</span><span class="sxs-lookup"><span data-stu-id="b7140-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="b7140-107">Yderligere oplysninger om konvertering af postkassen er tilgængelig i [konvertere en brugerpostkasse, en delt postkasse](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="b7140-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
