---
title: Anvend bedste fremgangsmåder for avancerede forespørgselsforespørgsler
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930127"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Anvend bedste fremgangsmåder for avancerede forespørgselsforespørgsler

Du kan få resultater hurtigere og undgå timeouts, mens du kører komplekse forespørgsler, ved at anvende disse bedste fremgangsmåder:

- Når du prøver nye forespørgsler, skal du altid bruge en grænse for at undgå at få meget store resultatsæt. Bruges også `count` til at foretage en indledende vurdering af resultatsættets størrelse.
- Brug tidsfiltre først. Ideelt set bør du begrænse dine forespørgsler til syv dage.
- I starten af en forespørgsel, lige efter tidsfilteret, skal du tilføje de filtre, der forventes, for at fjerne de fleste af dataene.
- Når du leder efter fulde tokens, skal du bruge `has` operatoren i stedet for `contains` .
- Kør en søgning i en bestemt kolonne i stedet for på tværs af alle kolonner.
- Ved sammenføjning af tabeller skal du først angive tabellen med færre rækker.
- `project` kun de nødvendige kolonner fra de tabeller, du har sammenføjet.

Du kan få mere at vide under [Bedste fremgangsmåder for avanceret forespørgselsforespørgsel.](https://go.microsoft.com/fwlink/?linkid=2144812)
