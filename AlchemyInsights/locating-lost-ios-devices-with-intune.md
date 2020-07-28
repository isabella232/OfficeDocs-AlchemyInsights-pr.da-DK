---
title: Lokalisering af mistede iOS-enheder med Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439142"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Lokalisering af mistede iOS-enheder med Intune

Aktivering af mistet tilstand på en iOS-enhed gør det muligt for en administrator at få vist en besked og et telefonnummer på låseskærmen.

Når tilstanden er gået tabt, kan administratoren bruge handlingen Find enhed til at identificere enhedens fysiske placering.

Handlingen Find enhed i Intune fungerer sammen med iOS-enheder for at vise placeringen af en bestemt enhed på et kort.

Brug af denne handling kræver, at iOS-enheden er i:

- Overvåget tilstand
- Tilstanden Mistet

Du kan finde flere oplysninger under [Aktivere mistet tilstand på iOS/iPadOS-enheder med Intune-](https://docs.microsoft.com/intune/device-lost-mode) og Find mistede eller stjålne [iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-locate).

**Ofte stillede spørgsmål**

Sp: Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder den fast i en ventende tilstand.

A: For en ekstern handling for at fuldføre, den målrettede enhed skal være online og sund. I følgende situationer forbliver fjernhandlingen i ventende tilstand i 30 dage, eller indtil enheden anerkender kommandoen:

- Når enheden ikke har forbindelse
- Når enheden mister sin administrationsstatus med Intune

Hvis du mener, at en enhed ikke længere tjekker ind, og at den ikke kan fjerne firmadata, skal du vælge Slet. Hvis du sletter enheden, fjernes enhedsposten, så den ikke længere vises på listen Intune over enheder. Hvis enheden bliver aktiv igen, skal brugeren tilmelde den igen.

Sp: Hvorfor er visse fjernhandlinger ikke tilgængelige for mig at bruge?

A: Ikke alle platforme understøtter alle eksterne enhedshandlinger. Følgende fjernhandlinger er platformsspecifikke, så de er kun tilgængelige for de anbe bemærkede platforme.

- Omgå aktiveringslås (kun iOS)
- Ny start (kun Windows)
- Tilstanden Mistet (kun iOS)
- Find enhed (kun iOS)
- Genstart (kun Windows)

Du kan finde flere oplysninger om hver handling under [Tilgængelige enhedshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).