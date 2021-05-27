---
title: Regler for reduktion af angrebsoverfladen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676126"
---
# <a name="attack-surface-reduction-rules"></a>Regler for reduktion af angrebsoverfladen

Udelukkelse af filer eller mapper kan reducere beskyttelsen, der leveres af regler for reduktion af angrebsoverfladen, alvorligt. Filer, der ville være blevet blokeret af en regel, har tilladelse til at køre, og ingen rapport eller hændelse registreres. En udeladelse gælder for alle regler, der tillader udeladelse.

I ASR-udeladelse bruges den samme syntaks som Microsoft Defender Antivirus udeladelser. Du kan få mere at [vide under Konfigurere og validere udeladelse for Microsoft Defender Antivirus scanninger.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Du kan undgå problemer ved at [gennemse Almindelige fejl, der skal undgås, når du definerer udeladelse.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Ikke alle asr-regler understøtter udeladelse. Hvis du vil validere, om din regel understøtter udeladelse, skal du se tabellen [Regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Regler for reduktion af angrebsoverfladen

Din organisations angrebsoverflade indeholder alle de steder, hvor en hacker kan kompromittere organisationens enheder eller netværk. At reducere angrebsoverfladen betyder, at du beskytter organisationens enheder og netværket, hvilket efterlader hackere med færre måder at udføre angreb på. Konfiguration af regler for reduktion af angrebsoverfladen i Microsoft Defender til slutpunkt kan hjælpe.

Du kan finde flere oplysninger under:

- [Knyt ASR-regel-GUID til navn](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Krav til ASR-regler:
    - [Windows 10 Pro, version 1709 eller nyere](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, version 1709 eller nyere](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, version 1803 (halvårlige kanal) eller nyere](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificer den korrekte udeladelse, der skal anvendes

1. Se efter eventID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operational Log.

1. Vurder blokscenariet og konteksten, og bekræft, at blokeringen af dette scenarie skal være fjernet.

1. Læs værdien Sti i oplysninger om begivenheden, som er den værdi, der definerer udeladelse.
    - Gør udelukkelsen så streng som mulig.
    - Anvend et jokertegn, hvor det er nødvendigt (du kan f.eks. erstatte variablen Bruger).

1. Anvend udelukkelsen i henhold til dine installationsbehov. Du kan få mere at vide [under Tilpas regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Udeladelse er ikke tilladt

1. Afgør, om reglen understøtter udeladelse. Du kan få mere at vide [under Regler for reduktion af angrebsoverfladen.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Gennemse de undtagelser, der er anvendt, og bekræft med hændelsesdataene for slåfejl eller fejlfortolke jokertegn. Du kan få mere at vide under [Understøttede udeladelsestyper](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Hvis effekten af reglen er for stor, skal du overveje at flytte reglen (tilbage) til overvågningstilstand for at udføre yderligere validering. Du kan få mere at [vide under Test, hvordan microsoft Defender for Endpoint-funktioner fungerer i overvågningstilstand.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Indsaml supportdata for at åbne en supportsag ved hjælp af denne kommando:
    
   ** MDEClientAnalyzer.cmd -v**

    Du kan få mere at [vide under Problemer med onboardingmaskine til Microsoft Defender til slutpunkter.](issues-with-onboarding-machines.md)
