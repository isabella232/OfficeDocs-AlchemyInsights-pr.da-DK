---
title: Placering af mistede iOS-enheder med Intune
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
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042300"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Placering af mistede iOS-enheder med Intune

Hvis du aktiverer mistet tilstand på en iOS-enhed, kan administratoren få vist et telefonnummer til en meddelelse og kontakt på låseskærmen.

Når den mistede tilstand er aktiveret, kan administratoren bruge handlingen Find enhed til at identificere enhedens fysiske placering.

Handlingen Find enhed i Intune fungerer sammen med iOS-enheder for at vise placeringen af en bestemt enhed på et kort.

Hvis du bruger denne handling, skal iOS-enheden være i:

- Overvåget tilstand
- Mistet tilstand

Du kan få mere at vide under Aktivér mistet tilstand på [iOS-/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-lost-mode) og Find mistede eller stjålne [iOS-/iPadOS-enheder med Intune.](https://docs.microsoft.com/intune/device-locate)

**Ofte stillede spørgsmål**

Sp: Jeg udstedte en fjernhandling for at fjerne virksomhedsdata fra en enhed, og nu sidder de fast i en afventende tilstand.

A: Hvis en fjernhandling skal kunne fuldføres, skal den målrettede enhed være online og sund. I følgende situationer forbliver fjernhandlingen i en afventende tilstand i 30 dage, eller indtil enheden anerkender kommandoen:

- Når enheden ikke har forbindelse
- Når enheden mister administrationsstatus med Intune

Hvis du mener, at en enhed ikke længere tjekker ind, og at den ikke vil kunne fjerne virksomhedsdata, skal du vælge Slet. Når du sletter, fjernes enhedsposten, så den ikke længere vises på Intune-listen over enheder. Hvis enheden bliver aktiv igen, skal brugeren tilmelde den igen.

Sp: Hvorfor er visse fjernhandlinger ikke tilgængelige for mig at bruge?

A: Ikke alle platforme understøtter alle fjernenhedshandlinger. Følgende fjernhandlinger er platformspecifikke, så de er kun tilgængelige for de platforme, der er angivet.

- Tilgå aktiveringslås (kun iOS)
- Frisk start (kun Windows)
- Mistet tilstand (kun iOS)
- Find enhed (kun iOS)
- Genstart (kun Windows)

Hvis du vil have mere at vide om hver enkelt handling, skal [du se Tilgængelige enhedshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).