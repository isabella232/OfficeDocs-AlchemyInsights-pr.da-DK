---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118568"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivering af BitLocker-kryptering med Intune

Intune Endpoint Protection-politik kan bruges til at konfigurere Bitlocker-krypteringsindstillinger for Windows enheder. Du kan finde flere oplysninger [Windows 10 indstillinger (og nyere) for at beskytte enheder ved hjælp af Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Ud over politikken Endpoint Protection findes der også en krypteringsrapport, som giver en mere detaljeret visning af krypteringsstatus for enheder. Denne rapport kan tilgås via MEM-portalen under **Enheder > Skærm** og derefter under Konfiguration **vælge** [Krypteringsrapport](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Hvis du finder ud af, at BitLocker ikke er aktiveret som forventet, eller at den profil, der bruges til at aktivere BitLocker, er i en fejltilstand, skal du gennemse krypteringsrapporten for at få en bedre forståelse af, hvorfor funktionsmåden opstår.

Du kan finde oplysninger om, hvordan du fortolker rapporten, herunder de forskellige krypteringsstatusværdier, under [Overvåge enhedskryptering med Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Du skal være opmærksom på, at mange nyere enheder, der Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politik. Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillingerne er konfigureret. Se de følgende ofte stillede spørgsmål for at få flere oplysninger.

Du kan finde oplysninger om fejlfinding af bitlockerproblemer [under Fejlfinding af BitLocker-politikker Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Ofte stillede spørgsmål**

Sp: Hvilke versioner af Windows understøtter enhedskryptering ved hjælp Endpoint Protection politik?<br>
A: Indstillingerne i Intune Endpoint Protection politik implementeres ved hjælp af [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ikke alle versioner eller builds af Windows understøtter Bitlocker CSP. <br><br>

Sp: Hvordan kan BitLocker aktiveres på enheder uden at kræve brugerinteraktion?<br>
A: Så længe de nødvendige forudsætninger er opfyldt, er det muligt at aktivere BitLocker "Silent Encryption" via Intune. Se oplysningerne om krav til enheden, og se politikindstillinger for at aktivere automatisk kryptering i følgende dokument: [Aktivér automatisk BitLocker-kryptering.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

SP: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS-standardindstillingerne for krypteringsmetode og krypteringsstyrke (XTS-AES-128), vil anvendelse af en politik med forskellige indstillinger automatisk udløse kryptering af drevet med de nye indstillinger?<br>
Sv.: Nej. Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.<br><br>
**Bemærk!** For enheder, der er tilmeldt Autopilot, udløses den automatiske kryptering, der ville forekomme under OOBE, ikke, før Intune-politikken evalueres, hvilket tillader, at de politikbaserede indstillinger kan bruges i stedet for OS-standardindstillingerne.
 
Sp: Hvis en enhed er krypteret som et resultat af programmet for Intune-politik, bliver den så dekrypteret, når denne politik fjernes?<br>
A: Fjernelse af krypteringsrelateret politik medfører IKKE dekryptering af de drev, der blev konfigureret.
 
Sp: Hvorfor viser Intune-overholdelsespolitikken, at min enhed ikke har BitLocker aktiveret, selvom den er?<br>
A: Indstillingen "BitLocker aktiveret" i Intune-overholdelsespolitikken anvender Windows device healthation (AFSER). Denne klient måler kun enhedens tilstand ved start. Så hvis en enhed ikke er blevet genstartet, da bitlocker-krypteringen blev fuldført, rapporterer DEN AMERIKANSKE CLIENT Client Service ikke BitLocker som værende aktiv.
 
 