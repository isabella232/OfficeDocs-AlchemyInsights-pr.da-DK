---
title: Arbejde med iOS VPP programmer regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364840"
---
# <a name="working-with-ios-vpp-applications"></a>Arbejde med iOS VPP-programmer

Læs, [hvordan du administrerer iOS-apps, der er købt via en diskenhed køb program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) at vide om funktioner, betingelser og trin til at gøre brug af Apple volumen købe programmet og understøttelse af den i Microsoft Intune.
  
 **Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til brugerne, men installationen mislykkedes".
  
- Dette kan ske, hvis der bruges et enkelt VPP-token på tværs af flere udbydere af mobile device management. VPP tokens fra Apple kan kun bruges sammen med én udbyder. Hvis du har brugt et VPP-token med flere leverandører, skal du igen overføre token til Intune.

- Installationen kan mislykkes også, hvis det samlede antal anlæg overstiger antallet af licenser. For at få vist en anvendelsesrapport for dine licenser, gå til **Intune Mobile apps** \> siden **App licenser** . Hvis du vil vide mere om at frigøre licenser i brug, se [i denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
