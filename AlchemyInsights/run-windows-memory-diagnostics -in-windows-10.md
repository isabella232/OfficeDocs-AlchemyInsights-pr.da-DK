---
title: Kør Windows Hukommelsesdiagnosticering i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720784"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Kør Windows Hukommelsesdiagnosticering i Windows 10

Hvis Windows og apps på din PC går ned, fryser eller reagerer på en ustabil måde, kan der være et problem med pc'ens hukommelse (RAM). Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.

Skriv **hukommelsesdiagnosticering**i søgefeltet på proceslinjen, og vælg derefter **Windows Hukommelsesdiagnosticering**. 

Hvis du vil køre diagnosticeringen, skal du genstarte computeren. Du har mulighed for at genstarte med det samme (Gem dit arbejde, og Luk åbne dokumenter og mails først), eller Planlæg diagnosticeringen til at køre automatisk, næste gang PC genstartes:

![Windows Hukommelsesdiagnosticering](media/windows-memory-diagnostic.png)

Når pc'en genstartes, kører **værktøjet Windows Hukommelsesdiagnosticering** automatisk. Status og status vises, når diagnosticeringen kører, og du har mulighed for at annullere diagnosticeringen ved at trykke på **ESC** -tasten på tastaturet.

Når diagnosticeringen er fuldført, vil Windows starte normalt.
Når skrivebordet vises umiddelbart efter genstart, vises der en meddelelse (ved siden af **handlings Center** -ikonet på proceslinjen) for at angive, om der er fundet hukommelsesfejl. Det kan f.eks. være:

Her er ikonet for løsnings Centeret: ![Handlingscenter-ikon](media/action-center-icon.png) 

Og et eksempel på en meddelelse: ![Ingen hukommelsesfejl](media/no-memory-errors.png)

Hvis du ikke har mistet beskeden, kan du vælge ikonet for **handlingscenter** på proceslinjen for at få vist **Løsningscenter** og få vist en liste over meddelelser, der kan rulles i.

Hvis du vil gennemgå detaljerede oplysninger, skal du skrive **begivenhed** i søgefeltet på proceslinjen og derefter vælge **Logbog**. I **logbogens**venstre rude skal du gå til **Windows Logs > system**. I højre rude skal du scanne ned på listen, mens du kigger på **kilde** kolonnen, indtil du ser begivenheder med kildeværdien **MemoryDiagnostics-resultater**. Fremhæv hver enkelt begivenhed, og se resultat oplysningerne i feltet under fanen **Generelt** under listen.
