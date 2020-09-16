---
title: Oversigt over Intune-enheder
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667872"
---
# <a name="intune-device-inventory"></a>Oversigt over Intune-enheder

Device-bladet giver administrator indsigt i enheder under administration i Intune på et enkelt enheds grundlag. De oplysninger, der vises, omfatter: hardware, registrerede programmer, enheds kompatibilitetstilstand og enheds konfigurationstilstand.

Lagerdata for hardware og opdagede programmer indsamles på en 7-dages cyklus. Programmer og specifikke elementer af hardware, der rapporteres, varierer afhængigt af enhedens operativsystem, og om enheden er personligt eller firma ejet.

Hvis du vil have mere at vide, skal du se [få vist enhedsoplysninger i Intune](https://docs.microsoft.com/intune/device-inventory).

**Ofte stillede spørgsmål**

Sp: Jeg modtager ikke en komplet oversigt over programmer, der er tilgængelige på de Intune-registrerede Windows-enheder. Hvorfor ikke?

A: på nuværende tidspunkt vises kun moderne apps til Windows 10-pc'er, der er identificeret som virksomhedens enheder. Intune indsamler ikke oplysninger om de Win32-apps, der er installeret på disse enheder.

Sp: Hvorfor indsamles der ikke telefonnumre fra alle enheder?

En: telefoner, der er kategoriseret som virksomhedsenheder i Intune, identificeres ikke med deres fulde telefonnummer, når du for eksempel kører en lager rapport fra en mobil enhed. Sæt telefonnumre til telefonenheder er altid delvist afmasket med asterisk (* * * *), og kun de sidste fire cifre vises.