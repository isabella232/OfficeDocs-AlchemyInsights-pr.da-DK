---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014066"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

Enheds bladet giver administratoren indsigt i enheder under administration i Intune pr. enhed. De viste oplysninger omfatter: Hardware, programmer, der opdages, tilstanden Enhedsoverholdelsestilstand og Enhedskonfigurationstilstand.

Lagerdata for hardware og opdagede programmer indsamles i en cyklus på syv dage. De programmer og specifikke elementer af hardware, der rapporteres, varierer afhængigt af enhedens operativsystem, og om enheden er personligt eller virksomhedsejet.

Få mere at vide under [Se enhedsdetaljer i Intune](https://docs.microsoft.com/intune/device-inventory).

**Ofte stillede spørgsmål**

Sp: Jeg modtager ikke en komplet lagerliste over programmer, der findes på Intune-tilmeldte Windows enheder. Hvorfor ikke?

A: På nuværende tidspunkt er det kun moderne apps, der er angivet for Windows 10 pc'er, der er identificeret som virksomhedens enheder. Intune indsamler ikke oplysninger om Win32-apps, der er installeret på disse enheder.

Sp: Hvorfor indsamles telefonnumre ikke fra alle enheder?

A: Telefoner, der er kategoriseret som virksomhedens enheder i Intune, identificeres ikke med deres fulde telefonnummer, når du f.eks. kører en lagerrapport for mobilenheder. Bring-you-own-device-telefonnumre er altid delvist maskeret med stjerner (****) og viser kun de sidste fire cifre.