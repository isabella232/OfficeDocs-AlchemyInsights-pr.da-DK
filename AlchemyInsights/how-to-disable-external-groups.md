---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399585"
---
# <a name="how-to-disable-external-groups"></a>Sådan deaktiveres eksterne grupper

Yammer eksterne meddelelser gælder Transport udvekslingsregler (ETRs), en række proaktive kontrol for at forhindre, at virksomhedens oplysninger deles. Hvis du vil forhindre brugere i at oprette eksterne grupper, skal du konfigurere en Exchange-transport regel (ETR), og konfigurer derefter Yammer for at bruge reglen Exchange Transport til at blokere eksterne meddelelser. 
  
Når du har oprettet en regel i Exchange Online admin center, skal du følge disse trin for at angive ETR til anvendelse i Yammer:
  
- Logge på Yammer som en kontrolleret admin, og i den **Yammer admin center**, skal du gå til C **Kræv og sikkerhed \> sikkerhedsindstillinger.**
    
- Vælg under **Eksterne meddelelser**, **gennemtvinge din Exchange Online Transport udvekslingsregler (ETRs) i Yammer.**
    
- Vælg **Gem**. 
    
Yderligere oplysninger finder du under [kontrol, der er eksterne meddelelser i et Yammer-netværk med regler for Transport af Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  

