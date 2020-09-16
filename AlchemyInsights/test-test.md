---
title: Manglende termer fra SharePoint Online-ordbank
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750445"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivere BitLocker-kryptering med Intune

Intune Endpoint Protection-politikken kan bruges til at konfigurere Boitlocker-krypteringsindstillinger for Windows-enheder som beskrevet i: Windows10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune

Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, der udløses uden anvendelse af MDM-politikken. Dette kan påvirke anvendelsen af politik, hvis ikke-standardindstillingerne er konfigureret. Du kan finde flere oplysninger under ofte stillede spørgsmål.


Ofte stillede spørgsmål   : hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af Endpoint Protection-politikken?
 A: indstillingerne i politikken for Intune Endpoint Protection implementeres ved hjælp af BitLocker-CSP.Ikke alle udgaver eller builds af Windows understøtter BitLocker-program til kryptografiske tjenester. 
      På nuværende tidspunkt Windows-udgaver: Enterprise; Education, mobile, mobil virksomhed og Professional (fra Build 1809) understøttes.




Sp: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af standardindstillingerne for krypteringsmetode og krypteringsgrad (XTS-AES-128), anvender en politik med andre indstillinger automatisk kryptering af drevet med de nye indstillinger?

Sv.: Nej. Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.

Bemærk! de enheder, der tilmeldes med autopilot, automatisk kryptering, der skulle forekomme under OOBE, udløses ikke, før Intune-politikken evalueres, hvilket gør det muligt for de politikbaserede indstillinger, der skal bruges i stedet for OPERATIVSYSTEMETS standarder




SP hvis en enhed krypteres som et resultat af anvendelsen af Intune-politikken, dekrypteres den, når politikken fjernes?

A: fjernelse af krypterings relateret politik medfører ikke dekryptering af de drev, der er konfigureret.




Sp: Hvorfor viser politikken for kompatibilitets overholdelse, at min enhed ikke har "BitLocker aktiveret", men det er?

A: indstillingen "BitLocker-aktiveret" i overholdelses politik for Intune anvender Windows-DHA (Device Health attestation). Denne klient måler kun enhedstilstanden på starttidspunktet. Hvis en enhed ikke er blevet genstartet, siden BitLocker-kryptering blev fuldført, vil DHA-klienttjenesten ikke rapportere BitLocker som aktiv.