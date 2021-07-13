---
title: Udgående relaypulje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381631"
---
# <a name="outbound-relay-pool"></a>Udgående relaypulje

Microsoft foretager nogle ændringer i konfigurationen til videresendelse eller videresendelse af mail via Microsoft 365. Meddelelser i visse scenarier videresendes eller videresendes via Microsoft 365 ved hjælp af en særlig relæpulje. Meddelelser, der sendes ved hjælp af relaygruppen, kan ende i modtagerens mappe med uønsket mail. Få mere at vide under [Udgående leveringspuljer](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

For at undgå et scenarie med brug af relæpuljen skal du kontrollere, at videresendte/videresendte meddelelser opfylder et af følgende kriterier:

- Den udgående afsender er et accepteret domæne for lejeren.
- SPF (Sender Policy Framework) overføres, når meddelelsen kommer til at Microsoft 365.
- DomainKeys Identified Mail (DKIM) på P2-afsenderdomænet passerer, når meddelelsen kommer Microsoft 365.
 
Meddelelser, der opfylder ovenstående kriterier, videresendes ikke gennem relæpuljen.

Hvis MX-posten for dit domæne peges på en tredjepartsserver eller en lokal server, skal du bruge udvidet filtrering for at sikre, at SPF-valideringen er korrekt for indgående mails, og for at undgå at sende mails via relæpuljen.

**Hvordan kan vi se, om vi er påvirket af relæpuljen?**

Hvis dine videresendte eller videresendte mails bruger et af ovenstående kriterier, videresendes meddelelser ikke gennem relæpuljen. Men hvis en meddelelse sendes gennem en relæpulje, er udgående server-IP i området 40.95.0.0/16, og navnet på den udgående server inkluderer **rly** i navnet.

