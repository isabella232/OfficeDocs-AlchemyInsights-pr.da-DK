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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konvertere en postkasse til brugeren til en delt postkasse

Du kan kun konvertere en brugerpostkasse til en delt postkasse, hvis brugeren har en Exchange-licens. Når postkassen er konverteret, vil den fortsat vises i listen over aktive brugere, da listen indeholder delte postkasser. Dog vises den konverterede postkasse også i listen over delte postkasser. 
  
Hvis du forsøger at konvertere en postkasse i Exchange-administrationskonsol, og konverteringen mislykkes, rydde browsercachen, og cookies, og prøv igen. Hvis det stadig ikke fungerer, kan du prøve at konvertere postkasse i Exchange Management Shell ved at køre følgende kommando:
  
```
Set-Mailbox -Type Shared
```

Yderligere oplysninger om konvertering af postkassen er tilgængelig i [konvertere en brugerpostkasse, en delt postkasse](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
