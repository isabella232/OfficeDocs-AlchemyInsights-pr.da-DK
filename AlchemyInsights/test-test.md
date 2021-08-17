---
title: Ord, der mangler SharePoint onlinevilkår Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106413"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivering af BitLocker-kryptering med Intune

Intune Endpoint Protection-politik kan bruges til at konfigurere krypteringsindstillinger for Boitlocker til Windows-enheder som beskrevet i: Windows10-indstillinger (og nyere) til at beskytte enheder ved hjælp af Intune

Du skal være opmærksom på, at mange nyere enheder, der Windows 10, understøtter automatisk bitlockerkryptering, som udløses uden anvendelse af MDM-politik. Dette kan påvirke anvendelse af politik, hvis ikke-standardindstillingerne er konfigureret. Se Ofte stillede spørgsmål for at få flere oplysninger.


Ofte stillede spørgsmål: Hvilke versioner af Windows understøtter enhedskryptering ved hjælp Endpoint Protection politik?
A: Indstillingerne i Intune Endpoint Protection politik implementeres ved hjælp af Bitlocker CSP.  Ikke alle versioner eller builds af Windows understøtter Bitlocker CSP. På nuværende tidspunkt Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise og Professional (fra build 1809 og fremefter) understøttes.




SP: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS-standardindstillingerne for krypteringsmetode og krypteringsstyrke (XTS-AES-128), anvendes der automatisk en politik med forskellige indstillinger, som udløser kryptering af drevet igen med de nye indstillinger?

Sv.: Nej. For at anvende de nye krypteringsindstillinger skal drevet først dekrypteres.

Bemærk For enheder, der er tilmeldt Autopilot, udløses den automatiske kryptering, der ville forekomme under OOBE, ikke, før Intune-politikken er evalueret, hvilket tillader, at politikbaserede indstillinger bruges i stedet for OS-standardindstillingerne




Sp Hvis en enhed er krypteret som et resultat af programmet af Intune-politik, bliver den dekrypteret, når denne politik fjernes?

A: Fjernelse af krypteringsrelateret politik medfører IKKE dekryptering af de drev, der blev konfigureret.




Sp: Hvorfor viser intune-overholdelsespolitikken, at min enhed ikke har "BitLocker aktiveret", men det er den?

A: Indstillingen "BitLocker enabled" i intune-overholdelsespolitik benytter Windows Device HealthAtion (AFSER). Denne klient måler kun enhedens tilstand ved start. Så hvis en enhed ikke er blevet genstartet, da bitlocker-krypteringen blev fuldført, rapporterer AFRRØV-klienttjenesten ikke bitlocker som værende aktiv.