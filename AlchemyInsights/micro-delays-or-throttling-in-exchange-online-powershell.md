---
title: Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947835"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell

Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online. Her er to forslag til dette:

- Det kan være en god ide at prøve at bruge [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), som indeholder CMDlets, der er baseret på REST API, og er betydeligt mere produktiv. Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.
- Hvis du skal bruge CMDlets, der endnu ikke er omfattet af v2-modulet, skal du se [Køre PowerShell-cmdlets til et stort antal brugere i Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), som taler om, hvordan du løser forventede PowerShell-begrænsninger i Exchange Online.
