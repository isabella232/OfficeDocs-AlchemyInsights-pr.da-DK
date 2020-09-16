---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731233"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

 Intune Endpoint Protection-politikken kan bruges til at konfigurere BitLocker-krypteringsindstillinger for Windows-enheder. Hvis du vil have mere at vide, skal du se [Windows 10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politikken. Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillingerne er konfigureret. Du kan finde flere oplysninger i følgende ofte stillede spørgsmål.
 
Du kan finde oplysninger om fejlfinding af problemer [med BitLocker under fejlfinding af BitLocker-politikker i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Ofte stillede spørgsmål**

 Sp: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af Endpoint Protection-politikken?<br>
 A: indstillingerne i politikken for Intune Endpoint Protection implementeres ved hjælp af [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ikke alle udgaver eller builds til Windows understøtter BitLocker-program til kryptografiske tjenester. <br><br>
      På nuværende tidspunkt understøttes følgende versioner af Windows: Enterprise, Education, mobile, mobil virksomhed og Professional (build 1809 og nyere).
 
Sp: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af standardindstillingerne for krypteringsmetode og krypteringsgrad (XTS-AES-128), vil en politik med andre indstillinger automatisk udløse genkryptering af drevet med de nye indstillinger?<br>
Sv.: Nej. Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.<br><br>
**Bemærk:** For enheder, der er tilmeldt autopilot, udløses den automatiske kryptering, der skulle forekomme under OOBE, ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEMETS standardindstillinger.
 
Sp: Hvis en enhed krypteres som et resultat af anvendelsen af Intune-politikken, dekrypteres den, når politikken fjernes?<br>
A: fjernelse af krypterings relateret politik medfører ikke dekryptering af de drev, der er konfigureret.
 
Sp: Hvorfor viser det, at min enhed ikke har BitLocker aktiveret, selvom min enhed ikke har BitLocker aktiveret, selvom det er?<br>
A: indstillingen "BitLocker-aktiveret" i aftale overholdelses politik anvender Windows-DHA (Device Health attestation-klient). Denne klient måler kun enhedstilstanden på starttidspunktet. Hvis en enhed ikke er blevet genstartet, siden BitLocker-kryptering blev fuldført, vil DHA-klienttjenesten ikke rapportere BitLocker som aktiv.
 
 