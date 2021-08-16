---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015614"
---
# <a name="how-to-disable-external-groups"></a>Sådan deaktiveres eksterne grupper

Yammer eksterne meddelelser gælder Exchange Transportregler (ETR'er), som er en gruppe proaktive kontrolelementer, der skal forhindre, at virksomhedens oplysninger deles. For at forhindre brugere i at oprette eksterne grupper skal du konfigurere en Exchange-transportregel (ETR) og derefter konfigurere Yammer til at bruge Exchange-transportreglen til at blokere eksterne meddelelser.
  
Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at indstille EtR til at gælde i Yammer:
  
- Log på Yammer som bekræftet administrator, og **i Yammer Administration** skal du gå til C Indhold og sikkerhed **\> Indstillinger.**

- Under **Eksterne meddelelser** skal du vælge **Gennemtving Exchange Online Exchange Transportregler (ETR'er) Yammer.**

- Vælg **Gem**.

Du kan få mere at vide [under Deaktiver eksterne beskeder i Yammer netværk.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  