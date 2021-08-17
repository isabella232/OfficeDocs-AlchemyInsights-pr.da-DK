---
title: Arbejde med iOS VPP-programmers regel-id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083008"
---
# <a name="working-with-ios-vpp-applications"></a>Arbejde med iOS VPP-programmer

Læs Sådan administrerer du [iOS-apps,](https://docs.microsoft.com/intune/vpp-apps-ios) der er købt via et volumenkøbsprogram med Microsoft Intune, for at få mere at vide om funktioner, begrænsninger og trin til at gøre brug af Apple Volume Purchase Program og supporten til det i Microsoft Intune.
  
 **Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til mine brugere, men installationen mislykkedes."
  
- Dette kan ske, hvis der bruges et enkelt VPP-token på tværs af flere udbydere af administration af mobilenheder. VPP-tokens fra Apple kan kun bruges med én udbyder. Hvis du har brugt et VPP-token sammen med flere udbydere, skal du overføre tokenet til Intune igen.

- Installationen kan også mislykkes, hvis det samlede antal installationer overstiger antallet af licenser. Hvis du vil have vist en anvendelsesrapport for dine licenser, skal du gå **til siden Licenser til Intune-mobilapps.** \>  Se denne artikel for at få mere at vide om, hvordan du [friskriver licenser i brug.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
