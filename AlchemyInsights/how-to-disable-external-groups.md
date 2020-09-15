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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704122"
---
# <a name="how-to-disable-external-groups"></a>Sådan deaktiveres eksterne grupper

Yammer-ekstern kommunikation anvender regler for Exchange-transport (Etr'er), et sæt proaktive kontrolelementer til at forhindre, at firmaoplysninger deles. Hvis du vil begrænse brugerne i at oprette eksterne grupper, skal du konfigurere en Exchange-transportregel (ETR) og derefter konfigurere Yammer til at blokere for eksterne meddelelser.
  
Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at angive ETR, der skal anvendes i Yammer:
  
- Log på Yammer som en bekræftet administrator, og gå til **yammer-Administrationscenter**og gå til C **indhold og sikkerhedsindstillinger for sikkerhed \> .**

- Gå til **eksterne meddelelser**, og vælg **Gennemtving dine Exchange Online Exchange-transport regler (Etr'er) i Yammer.**

- Vælg **Gem**.

Hvis du vil have mere at vide, skal du se [Deaktiver eksterne beskeder i et Yammer-netværk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  