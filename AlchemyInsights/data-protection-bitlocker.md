---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908704"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivering af BitLocker-kryptering med Intune

 Intune Endpoint Protection Policy kan bruges til at konfigurere BitLocker-krypteringsindstillinger for Windows-enheder. Du finder flere oplysninger under [Indstillinger for Windows 10 (og nyere) for at beskytte enheder ved hjælp af Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politik. Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillinger konfigureres. Se følgende ofte stillede spørgsmål for at få flere oplysninger.
 
Du finder oplysninger om fejlfinding af BitLocker-problemer under [fejlfinding af BitLocker-politikker i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Ofte stillede spørgsmål**

 Sp: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunkts beskyttelsespolitikken?<br>
 A: indstillingerne i Intune Endpoint Protection Policy implementeres ved hjælp af [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ikke alle udgaver eller builds af Windows understøtter BitLocker CSP. <br><br>
      På dette tidspunkt understøttes følgende Windows-udgaver: Enterprise, Education, mobile, mobile Enterprise og Professional (build 1809 og nyere).
 
Q: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS standardindstillinger for krypteringsmetode og cipher styrke (XTS-AES-128), vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?<br>
A: Nej. Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.<br><br>
**Bemærk:** For enheder, der er tilmeldt autopilot, udløses den automatiske kryptering, som ville forekomme under OOBE, ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEM standarderne.
 
Q: Hvis en enhed er krypteret som følge af anvendelsen af Intune politik, vil den blive dekrypteret, når denne politik er fjernet?<br>
A: fjernelse af krypterings relateret politik resulterer ikke i dekryptering af de drev, der blev konfigureret.
 
Spørgsmål: Hvorfor viser Intune-overholdelses politikken, at min enhed ikke har BitLocker aktiveret, selvom den er det?<br>
A: "BitLocker Enabled"-indstillingen i Intune-overholdelses politikken bruger Windows DHA-klienten (Device Health attestering). Denne klient måler kun enheds tilstand på starttidspunktet. Så hvis en enhed ikke er blevet genstartet, siden BitLocker-krypteringen blev fuldført, rapporterer DHA-klienttjenesten ikke BitLocker som værende aktiv.
 
 