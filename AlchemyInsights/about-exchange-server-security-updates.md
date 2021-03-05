---
title: Om Exchange Server sikkerhedsopdateringer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481118"
---
# <a name="about-exchange-server-security-updates"></a>Om Exchange Server sikkerhedsopdateringer

Microsoft har udgivet en række vigtige sikkerhedsopdateringer til Exchange Server lokale miljø. De påvirkede serverversioner er alle opdateringsniveauer i Exchange Server 2010, 2013, 2016 og 2019. Exchange Online påvirkes IKKE, men hvis du har nogle lokale Exchange-servere på grund af hybridkonfiguration, er de potentielt sårbar.

Hvis du vil opdatere dine lokale servere, skal der som minimum køres følgende versioner af Exchange:

- Exchange 2010 Service Pack 3
- Exchange Server 23 CU 2013
- Exchange Server 2016 CU 19 eller CU 18
- Exchange Server 2019 CU 8 eller CU 7

Se følgende meddelelse om placering af rettelser: [Udgivet: Marts 2021 Exchange Server sikkerhedsopdateringer](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Vigtige bemærkninger:**

Installation af opdateringer fungerer ikke, hvis dine lokale servere ikke kører nødvendige Exchange-versioner, som vist på listen ovenfor.

Hvis du installerer opdateringer manuelt, skal du læse afsnittet "Kendte problemer" i artiklerne om opdatering af KB for at få vigtige oplysninger. Sikkerhedsopdateringer SKAL køres fra administratorerede CMD/PowerShell-prompts!
