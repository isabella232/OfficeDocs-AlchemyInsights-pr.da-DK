---
title: Oversigt over intune-enheder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439158"
---
# <a name="intune-device-inventory"></a>Oversigt over intune-enheder

Bladen Enheder giver administratoren indsigt i enheder under administration i Intune pr. enhed. De viste oplysninger omfatter: Hardware, Fundne programmer, tilstand for overholdelse af enheden og tilstand for enhedskonfiguration.

Lagerdata for hardware og fundne programmer indsamles på en syv-dages cyklus. De programmer og specifikke elementer af hardware rapporteret varierer afhængigt af enhedens operativsystem, og om enheden er personligt eller corporate ejet.

Du kan finde flere oplysninger [under Oplysninger om enheden i Intune](https://docs.microsoft.com/intune/device-inventory).

**Ofte stillede spørgsmål**

Sp: Jeg modtager ikke en komplet oversigt over de programmer, der er til stede på Intune-tilmeldte Windows-enheder. Hvorfor ikke?

A: På nuværende tidspunkt er det kun moderne apps, der er angivet til Windows 10-pc'er, der er identificeret som virksomhedsenheder. Intune indsamler ikke oplysninger om Win32-apps, der er installeret på disse enheder.

Sp: Hvorfor indsamles telefonnumre ikke fra alle enheder?

A: Telefoner kategoriseret som virksomhedsenheder i Intune identificeres ikke med deres fulde telefonnummer, når du f.eks. Bring-you-own-device telefonnumre er altid delvist maskeret med stjerner (****), og viser kun de sidste fire cifre.