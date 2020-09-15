---
title: Arbejde med iOS VPP-programmer regel-id 1018
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688940"
---
# <a name="working-with-ios-vpp-applications"></a>Arbejde med iOS VPP-programmer

Læs [, hvordan du administrerer iOS-apps, der er købt via et volumen-købsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , til at få mere at vide om funktioner, begrænsninger og trin, der skal bruges til at udnytte Apple Volume Purchase og support til det i Microsoft Intune.
  
 **Almindelige problemer:** "Jeg har tildelt en iOS VPP-app til mine brugere, men installationen mislykkedes."
  
- Dette kan ske, hvis der bruges et enkelt VPP-token på tværs af flere udbydere af mobilenheder. VPP-tokens fra Apple kan kun bruges med én udbyder. Hvis du har brugt et VPP-token med flere udbydere, skal du overføre tokenet til Intune igen.

- Installationen kan også mislykkes, hvis det samlede antal installationer overskrider antallet af licenser. Hvis du vil have vist en anvendelsesrapport for dine licenser, skal du gå til siden Intune-app-licenser til **Intune** \> **App licenses** . Du kan få mere at vide om, hvordan du gengiver licenser i brug, i [denne artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
