---
title: Finde mistede iOS-enheder med Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675150"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Finde mistede iOS-enheder med Intune

Hvis du aktiverer tilstanden Hittegods på en iOS-enhed, kan en administrator have en meddelelse og et telefonnummer, der vises på låseskærmen.

Når tilstanden tabt er aktiveret, kan administratoren bruge handlingen Find enhed til at identificere enhedens fysiske placering.

Handlingen Find enhed i Intune fungerer med iOS-enheder for at vise placeringen af en bestemt enhed på et kort.

Hvis du bruger denne handling, skal iOS-enheden være i:

- Overvåget tilstand
- Mistet tilstand

Hvis du vil have mere at vide, skal du se [aktivere tilstanden tabt på iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-lost-mode) og [finde mistede eller stjålne iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-locate).

**Ofte stillede spørgsmål**

Sp: Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder det fast i en afventende tilstand.

A: for at en fjernhandling kan fuldføres, skal den målrettede enhed være online og sunde. I følgende situationer forbliver Fjernhandlingen i en afventende tilstand i 30 dage, eller indtil enheden godkender kommandoen:

- Når enheden ikke har forbindelse
- Når enheden mister sin administrations status med Intune

Hvis du tror, at en enhed ikke længere tjekkes ind, og at den ikke kan fjerne firmadata, skal du vælge Slet. Sletning fjerner enhedsposten, så den ikke længere vises på listen over enheder i Intune. Hvis enheden igen bliver aktiv, skal brugeren tilmelde den igen.

Sp: Hvorfor kan jeg ikke bruge visse fjernhandlinger?

En: ikke alle platforme understøtter alle handlinger med Fjern enheder. Følgende fjernhandlinger er platformspecifikke, så de er kun tilgængelige for de platforme, der er angivet.

- Tilsidesæt aktiverings låse (kun iOS)
- Ny start dato (kun Windows)
- Tilstanden mistede (kun iOS)
- Find enhed (kun iOS)
- Genstart (kun Windows)

Du kan finde flere oplysninger om hver handling under [tilgængelige enheds handlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).