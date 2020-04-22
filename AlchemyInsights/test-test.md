---
title: Vilkår, der mangler i SharePoint Online-ordlagring
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766847"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivering af Bitlocker-kryptering med Intune

Intune Endpoint Protection Policy kan bruges til at konfigurere Boitlocker-krypteringsindstillinger for Windows-enheder som beskrevet i : Windows10-indstillinger (og nyere) for at beskytte enheder, der bruger Intune

Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10 understøtter automatisk bitlocker kryptering, som udløses uden anvendelse af MDM politik. Dette kan påvirke anvendelsen af politikken, hvis der ikke er konfigureret standardindstillinger. Se ofte stillede spørgsmål for at få flere oplysninger.


Ofte  stillede spørgsmål Q: Hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunktsbeskyttelsespolitikken?
 Sv.: Intune-slutpunktsbeskyttelsespolitikken implementeres ved hjælp af Bitlocker CSP.Ikke alle udgaver eller builds af Windows understøtter Bitlocker CSP. 
      På dette tidspunkt Windows Editions: Enterprise; Uddannelse, mobil, mobil virksomhed og professionel (fra build 1809 og fremefter) understøttes.




Sp: Hvis en enhed allerede er krypteret med Bitlocker ved hjælp af OS-standardindstillingerne for krypteringsmetode og krypteringsstyrke (XTS-AES-128) vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?

A: Nej. For at anvende de nye cipher indstillinger drevet skal først dekrypteres.

Bemærk For enheder, der er tilmeldt Autopilot, udløses den automatiske kryptering, der ville opstå under OOBE, ikke, før Intune-politikken er evalueret, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for os-standardindstillingerne




Q Hvis en enhed er krypteret som følge af anvendelsen af Intune politik vil det blive dekrypteret, når denne politik er fjernet?

A: Fjernelse af kryptering relateret politik ikke resulterer i dekryptering af de drev, der blev konfigureret.




Sp: Hvorfor viser intune Compliance-politikken, at min enhed ikke har "Bitlocker aktiveret", men det er den?

Sv. Indstillingen "Bitlocker enabled" i intune compliance policy anvender DHA-klienten (Windows Device Health Attestation). Denne klient måler kun enhedens tilstand på starttidspunktet. Så hvis en enhed ikke er blevet genstartet, da bitlocker kryptering blev afsluttet DHA klienttjeneste vil ikke rapportere bitlocker som værende aktiv.