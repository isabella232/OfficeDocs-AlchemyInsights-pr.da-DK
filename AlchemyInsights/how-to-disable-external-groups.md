---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739487"
---
# <a name="how-to-disable-external-groups"></a>Sådan deaktiveres eksterne grupper

Yammer External messaging anvender Exchange transport Rules (ETRs), et sæt proaktive kontrolelementer for at forhindre, at virksomhedsoplysninger deles. Hvis du vil begrænse brugere i at oprette eksterne grupper, skal du konfigurere en Exchange transport Rule (ETR) og derefter konfigurere Yammer til at bruge Exchange-transportreglen til at blokere eksterne meddelelser.
  
Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at indstille ETR til at gælde i Yammer:
  
- Log på Yammer som en bekræftet administrator, og gå til indstillinger for C- **indhold og sikkerheds \> sikkerhed** i **yammer administration**.

- Under **eksterne meddelelser**skal du vælge gennem **Tving dine Exchange Online Exchange transport Rules (ETRS) i Yammer.**

- Vælg **Gem**.

Du finder flere oplysninger under [deaktivere eksterne meddelelser i et Yammer-netværk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  