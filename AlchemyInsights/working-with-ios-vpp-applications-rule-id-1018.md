---
title: Arbejde med iOS VPP-programregel-id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719951"
---
# <a name="working-with-ios-vpp-applications"></a>Arbejde med iOS VPP-programmer

Læs [Hvordan du administrerer iOS-apps, der er købt via et volumenkøbsprogram med Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) for at få mere at vide om funktioner, begrænsninger og trin til at gøre brug af Apple Volume Purchase Program og support til det i Microsoft Intune.
  
 **Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til mine brugere, men installationen mislykkedes."
  
- Dette kan ske, hvis et enkelt VPP-token bruges på tværs af flere udbydere af administration af mobilenheder. VPP-tokens fra Apple må kun bruges hos én udbyder. Hvis du har brugt et VPP-token med flere udbydere, skal du uploade tokenet til Intune igen.

- Installationen kan også mislykkes, hvis det samlede antal installationer overstiger antallet af licenser. Hvis du vil se en brugsrapport for dine licenser, skal du gå til siden **Intune Mobile Apps** \> **App-licenser.** Du kan få mere at vide om, hvordan du tilbagegør licenser i brug, i [denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
