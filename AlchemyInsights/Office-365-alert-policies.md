---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312681"
---
# <a name="alert-policies"></a>Beskedpolitikker

Microsoft 365 indeholder standardbeskedpolitikker, der udløser beskeder for organisationer med et Microsoft 365 Enterprise- eller Microsoft 365 us Government E1/G1-, E3/G3- eller E5/G5-abonnement. [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) Derfor kan administratorer modtage en besked via mail fra Office365Alerts@microsoft.com med en emnelinje som f.eks. "En besked med lav alvorsgrad: navn på *beskedpolitik".* Der sendes beskeder, når der udløses beskeder for almindelige aktiviteter, f.eks. når brugere:

- Opret indbakkeregler, der videresender mail.
- Tildel tilladelser til deres postkasse.
- Del eller slet et stort antal filer i SharePoint fildeling.
- Opret eDiscovery-søgninger, og eksportér søgeresultater.

Sådan gennemser og reagerer du på en besked:

1. Gør et af følgende:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Beskeder**. Eller du kan bruge til at gå **direkte til siden** Vigtige <https://compliance.microsoft.com/compliancealerts> beskeder.
   - I Microsoft 365 Defender på skal <https://security.microsoft.com> du gå **til & beskeder om** \> **beskeder**. Eller du kan bruge til at gå **direkte til siden** Vigtige <https://security.microsoft.com/alerts> beskeder.
2. Klik på en besked for at få vist en pop op-side med oplysninger om beskeden.

Du kan handle på en besked, f.eks. fjerne [en mistænkelig indbakkeregel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Eller du kan blot lukke beskeden ved at klikke **på Løs** på pop op-siden med beskeden.

Du kan finde flere oplysninger om konfiguration og administration af beskedpolitikker i [denne artikel.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Vigtigt:** Beskeder via mail fra Microsoft beder dig aldrig om at gøre følgende:

- Angiv en adgangskode
- Bekræft sikkerhedsoplysningerne for din konto
- Godkend dig selv igen

Hvis du modtager en mail med disse typer anmodninger, blev den ikke sendt af Microsoft og bør betragtes som forsøg på phishing. Hvis du modtager en meddelelse med disse typer anmodninger, [skal du rapportere meddelelsen til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
