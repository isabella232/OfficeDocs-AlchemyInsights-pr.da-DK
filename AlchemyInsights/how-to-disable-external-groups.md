---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720762"
---
# <a name="how-to-disable-external-groups"></a>Sådan deaktiveres eksterne grupper

Yammers eksterne meddelelser anvender Exchange Transport Rules (ETR'er), som er et sæt proaktive kontrolelementer, der forhindrer, at virksomhedsoplysninger deles. Hvis du vil begrænse brugeres mulighed for at oprette eksterne grupper, skal du konfigurere en Exchange-transportregel (ETR) og derefter konfigurere Yammer til at bruge Exchange Transport-reglen til at blokere eksterne meddelelser.
  
Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at indstille ETR til at gælde i Yammer:
  
- Log på Yammer som en bekræftet administrator, og gå til **C-indstillinger \> for indholds- og sikkerhedssikkerhed i** **Yammer Administration.**

- Vælg **Gennemtving dine Exchange Online Exchange Transport-regler (ETR'er) i Yammer under** **Eksterne meddelelser.**

- Vælg **Gem**.

Yderligere oplysninger finder du i [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  