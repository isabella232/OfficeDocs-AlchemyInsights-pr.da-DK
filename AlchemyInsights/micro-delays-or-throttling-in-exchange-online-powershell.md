---
title: Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868528"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-forsinkelser eller -begrænsning i Exchange Online PowerShell

Du vil muligvis se "Micro-forsinkelse anvendt"-advarsler eller -forsinkelser, når du kører scripts og cmdlets i Exchange Online. Her er nogle forslag til, hvordan du kan løse dette:

- Kør vores diagnosticeringsværktøj for at slappe af din lejers PowerShell-begrænsningspolitikker. Denne løsning løser problemet for de fleste.
- Hvis problemet stadig ikke løses, kan du bruge [Exchange Online v2 PowerShell-modulet,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)som indeholder CMDlet'er, der er baseret på REST-API, og som er væsentligt mere performant. Dette kan være en god løsning til en masse af Get- CMDlets, der ofte anvendes.
- Hvis du skal bruge CMDlet'er, der ikke er dækket af v2-modulet, skal du se Køre [PowerShell-cmdlet'er for](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)et stort antal brugere i Office 365, som handler om, hvordan du kommer uden om Begrænsningsgrænser for PowerShell i Exchange Online.
