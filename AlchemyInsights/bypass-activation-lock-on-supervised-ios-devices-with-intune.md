---
title: Omgå aktiveringslås på overvågede iOS-enheder med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423491"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Omgå aktiveringslås på overvågede iOS-enheder med Intune

Muligheden for at omgå aktiveringslåsen på iOS-enheder gør det nemmere at komme sig efter det scenario, hvor en bruger aktiverer aktiveringslås på en virksomhedsenhed, og forlader derefter virksomheden.

Forudsætninger for at omgå en aktiveringslås omfatter:

- En enhed er, der er "overvåget".
- Aktiveringslåsen er aktiveret ved hjælp af begrænsningspolitikken for iOS-enheder i Intune.

Når du omgår en aktiveringslås, skal du desuden:

- Fysisk besidder enheden bliver udslettet.
- Kopier koden, før du udsteder sletningen.

**Bemærk:** Der er ikke store og små bogstaver i tørrekoden, så "-" tegnene er ikke påkrævet.

Yderligere oplysninger finder du [i Bypass Activation Lock on Supervised iOS-enheder med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Ofte stillede spørgsmål**

Sp: **Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder den fast i en ventende tilstand.**

A: For en ekstern handling for at fuldføre, den målrettede enhed skal være online og sund. I følgende situationer forbliver fjernhandlingen i ventende tilstand i 30 dage, eller indtil enheden anerkender kommandoen, når enheden:

- Har ikke forbindelse.
- Mister sin ledelsesstatus med Intune.

Hvis du mener, at en enhed ikke længere tjekker ind, og at den ikke fjerner firmadata, skal du vælge Slet. Hvis du sletter enheden, fjernes enhedsposten, så den ikke længere vises på listen Intune over enheder. Hvis enheden skal være aktiv igen, skal brugeren tilmelde enheden igen.

Sp: **Hvorfor er visse fjernhandlinger ikke tilgængelige for mig at bruge?**

A: Ikke alle platforme understøtter alle eksterne enhedshandlinger. Følgende fjernhandlinger er platformsspecifikke.

- Omgå aktiveringslås (kun iOS)
- Ny start (kun Windows)
- Tilstanden Mistet (kun iOS)
- Find enhed (kun iOS)
- Genstart (kun Windows)

Du kan finde flere oplysninger om hver handling under [Tilgængelige enhedshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).