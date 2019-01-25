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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29463912"
---
Du kan kun konvertere en brugerpostkasse til en delt postkasse, hvis brugeren har en Exchange-licens. Når postkassen er konverteret, vil den fortsat vises i listen over aktive brugere, da listen indeholder delte postkasser. Dog vises den konverterede postkasse også i listen over delte postkasser. 
  
Hvis du forsøger at konvertere en postkasse i Exchange-administrationskonsol, og konverteringen mislykkes, rydde browsercachen, og cookies, og prøv igen. Hvis det stadig ikke fungerer, kan du prøve at konvertere postkasse i Exchange Management Shell ved at køre følgende kommando:
  
```
Set-Mailbox -Type Shared
```

Yderligere oplysninger om konvertering af postkassen er tilgængelig i [konvertere en brugerpostkasse, en delt postkasse](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
