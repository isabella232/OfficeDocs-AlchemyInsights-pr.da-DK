---
title: Kør Windows Hukommelsesdiagnosticering i Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826661"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Kør Windows Hukommelsesdiagnosticering i Windows 10

Hvis Windows og apps på din pc går ned, fryser eller fungerer ustabilt, kan der være problemer med pc'ens hukommelse (RAM). Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.

Skriv hukommelsesdiagnosticering i **søgefeltet på proceslinjen,** og vælg derefter **Windows Hukommelsesdiagnosticering.** 

Pc'en skal genstartes for at køre diagnosticeringen. Du har mulighed for at genstarte med det samme (gem dit arbejde, og luk åbne dokumenter og mails først), eller planlæg diagnosticeringen til at køre automatisk, næste gang pc'en genstarter:

![Windows Hukommelsesdiagnosticering](media/windows-memory-diagnostic.png)

Når pc'en genstarter, **kører Windows Hukommelsesdiagnosticering** automatisk. Status og status vises i diagnosticeringsværktøjet, og du kan annullere diagnosticeringen ved at trykke på **Esc** på tastaturet.

Når diagnosticeringen er fuldført, starter Windows normalt.
Straks efter genstart, når skrivebordet vises, vises der  en meddelelse (ud for ikonet Handlingscenter på proceslinjen) for at angive, om der blev fundet hukommelsesfejl. Eksempel:

Her er ikonet Handlingscenter: ![Ikonet Handlingscenter](media/action-center-icon.png) 

Og en eksempelmeddelelse: ![Ingen hukommelsesfejl](media/no-memory-errors.png)

Hvis du ikke når at  se meddelelsen, kan du  vælge ikonet handlingscenter på proceslinjen for at få vist Handlingscenter og få vist en liste over meddelelser, der kan rulles i.

Hvis du vil gennemse detaljerede oplysninger, **skal** du skrive begivenhed i søgefeltet på proceslinjen og derefter vælge **Log på**. I **ruden til** venstre for Logbog skal du gå til **Windows-logge > System.** I højre rude skal du rulle ned på  listen, mens du kigger på kolonnen Kilde, indtil du ser hændelser med kildeværdien **MemoryDiagnostics-Results.** Fremhæv hver enkelt begivenhed, og få vist resultatoplysningerne i feltet under **fanen** Generelt under listen.
