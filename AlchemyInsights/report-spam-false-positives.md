---
title: Vil du rapportere en falsk spam positiv til Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396609"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Er der legitime meddelelser, der markeres som spam?

Det er frustrerende, når en legitim mail ender i mappen Uønsket mail eller i karantæne. Overvej disse mest almindelige årsager til falske positive:

**Lejer tilsidesætter (mest almindeligt)** Dette er helt inden for din kontrol for at afhjælpe problemet.

Sende meddelelsen på en Microsoft 365 Defender analyse af de på gældende politikker og regler; oplysninger om kant er tilgængelige inden for få minutter.
Gennemse eller rediger politikkerne eller reglerne, alt efter hvad der er relevant. 

**Slutbrugerens tilsidesættelser (almindeligt)** Dette er helt inden for din kontrol for at afhjælpe problemet. 

Sende meddelelsen på en Microsoft 365 Defender analyse af de på gældende politikker og regler; oplysninger om kant er tilgængelige inden for få minutter. 

Hvis en meddelelse blev blokeret, fordi den blev sendt fra en adresse på en brugers liste over blokerede afsendere, indeholder brevhovederne vurdering af spamfiltrering "SFV:BLK".

**Afsenders mailgodkendelse** Dette er delvist inden for din kontrol for at afhjælpe problemet.

Send meddelelsen for at analysere fejl i afsenderens mailgodkendelse på leveringstidspunktet. resultater er tilgængelige inden for en dag. 

Hvis du ejer afsendende infrastruktur, skal du se, hvordan du justerer den med SPF, DKIM og DMARC for at sikre, at destinationsmailsystemerne har tillid til meddelelser, der sendes fra dit domæne. Alternativt kan du kontakte afsenderne for at adressere deres DNS-konfigurationer.

**Microsoft-filtreringskriterier** Dette er delvist inden for din kontrol for at afhjælpe problemet.

Sende meddelelsen og rapportere meddelelsen som sikker; Genscanne resultater er tilgængelige inden for en dag. Brug lejerens tilladelse/blokeringsliste, når du er uenig i filtreringskriterier i bestemte situationer. Du bør dog ikke tilsidesætte Microsofts filtreringskriterie permanent. 

Du kan finde flere oplysninger under:

- Gør det muligt for dine slutbrugere at sende meddelelser til Microsoft. Microsoft bruger disse indsendelser til at forbedre effektiviteten af teknologier til mailbeskyttelse, og de vises i indsendelsesrapporter, som du kan bruge som en indikation i at opdatere politikker. 

- Hvis du vil se en kort video om at sende meddelelser til analyse, skal [du se Sende meddelelser til analyse](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Brug administratorindsendelse til at sende mistænkeligt spam, phish, URL-adresser og filer til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Administrer lejerens tilladelses-/blokeringsliste](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Antispam-brevhoveder i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Beskyttelse mod udgående spam i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)