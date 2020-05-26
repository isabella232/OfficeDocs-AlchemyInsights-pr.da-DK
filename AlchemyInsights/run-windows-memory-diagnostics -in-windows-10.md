---
title: Køre Windows Hukommelsesdiagnosticering i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357378"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Køre Windows Hukommelsesdiagnosticering i Windows 10

Hvis Windows og apps på din pc går ned, fryser eller handler ustabilt, kan du have et problem med pc'ens hukommelse (RAM). Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.

Skriv **hukommelsesdiagnosticering**i søgefeltet på proceslinjen, og vælg derefter **Windows Hukommelsesdiagnosticering**. 

Hvis du vil køre diagnosticeringen, skal pc'en genstartes. Du har mulighed for at genstarte med det samme (gem dit arbejde og luk åbne dokumenter og e-mails først), eller planlæg, at diagnosticeringen skal køre automatisk, næste gang pc'en genstarter:

![Diagnosticering af Windows-hukommelse](media/windows-memory-diagnostic.png)

Når pc'en genstartes, kører **Windows Hukommelsesdiagnosticering** automatisk. Status og status vises, mens diagnosticeringen kører, og du har mulighed for at annullere diagnosticeringen ved at trykke på **ESC-tasten** på tastaturet.

Når diagnosticeringen er fuldført, starter Windows normalt.
Umiddelbart efter genstartvises der en meddelelse (ud for ikonet **Løsningscenter** på proceslinjen) umiddelbart efter genstarten for at angive, om der er fundet hukommelsesfejl. Det kan f.eks. være:

Her er ikonet Løsningscenter: ![Ikon for Handlingscenter](media/action-center-icon.png) 

Og en prøve anmeldelse: ![Ingen hukommelsesfejl](media/no-memory-errors.png)

Hvis du ikke har modtaget meddelelsen, kan du vælge ikonet **Løsningscenter** på proceslinjen for at få vist **Løsningscenter** og se en liste over meddelelser, der kan rulles igennem.

Hvis du vil gennemse detaljerede oplysninger, skal du skrive **hændelse** i søgefeltet på proceslinjen og derefter vælge **Logbog**. Gå til **Windows Logs > System**i **logbogs**venstre rude . Skan ned på listen i højre rude, mens du ser på kolonnen **Kilde,** indtil du ser hændelser med Kildeværdien **MemoryDiagnostics-Results**. Fremhæv hver af disse hændelser, og se resultatoplysningerne i feltet under fanen **Generelt** under listen.
