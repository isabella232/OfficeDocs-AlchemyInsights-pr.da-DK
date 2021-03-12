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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744606"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Anvend bedste fremgangsmåder for avancerede forespørgselsforespørgsler

For at få resultater hurtigere og undgå timeouts, mens du kører komplekse forespørgsler, skal du anvende disse bedste fremgangsmåder:

- Når du prøver nye forespørgsler, skal du altid bruge en grænse for at undgå at få meget store resultatsæt. Bruges også `count` til at foretage en indledende vurdering af resultatsættets størrelse.
- Brug tidsfiltre først. Ideelt set bør du begrænse dine forespørgsler til syv dage.
- I starten af en forespørgsel lige efter tidsfilteret skal du tilføje de filtre, der forventes at fjerne de fleste af dataene.
- Når du leder efter fulde tokens, skal du bruge `has` operatoren i stedet for `contains` .
- Kør en søgning på en bestemt kolonne i stedet for på tværs af alle kolonner.
- Når du sammenføjer tabeller, skal du først angive tabellen med færre rækker.
- `project` kun de nødvendige kolonner fra de tabeller, du har sammenføjet.

Hvis du vil have mere at vide, skal [du se bedste fremgangsmåder for avanceret forespørgsel.](https://go.microsoft.com/fwlink/?linkid=2144812)
