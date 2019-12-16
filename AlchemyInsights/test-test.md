---
title: Vilkår, som mangler i SharePoint Online term store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053507"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivering af BitLocker-kryptering med Intune

Intune Endpoint Protection Policy kan bruges til at konfigurere Boitlocker krypteringsindstillinger for Windows-enheder som beskrevet i: Windows10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune

Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politik. Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillingerne konfigureres. Se ofte stillede spørgsmål for at få flere oplysninger.


FAQ  Q: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunkts beskyttelsespolitikken?
 A: indstillingerne i Intune Endpoint Protection Policy implementeres ved hjælp af BitLocker CSP.Ikke alle udgaver eller builds af Windows understøtter BitLocker CSP. 
      På dette tidspunkt Windows-udgaver: Enterprise; Uddannelse, mobil, mobil virksomhed og professionel (fra Build 1809 og fremefter) understøttes.




Q: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS standardindstillinger for krypteringsmetode og cipher styrke (XTS-AES-128) vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?

A: Nej. For at anvende de nye cipher indstillinger drevet skal først dekrypteres.

Bemærkning til enheder, der er tilmeldt med autopilot den automatiske kryptering, der ville opstå under OOBE, udløses ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEM standarderne




Q hvis en enhed er krypteret som følge af anvendelsen af Intune politik vil den blive dekrypteret, når denne politik er fjernet?

A: fjernelse af krypterings relaterede politik ikke resulterer i dekryptering af de drev, der blev konfigureret.




Spørgsmål: Hvorfor viser Intune Compliance Policy, at min enhed ikke har "BitLocker Enabled", men det er det?

A: indstillingen "BitLocker-aktiveret" i Intune-overholdelses politik bruger Windows DHA-klienten (Device Health attestering). Denne klient måler kun enheds tilstand på starttidspunktet. Så hvis en enhed ikke er blevet genstartet, da BitLocker-kryptering blev fuldført, rapporterer DHA-klienttjenesten ikke BitLocker som værende aktiv.