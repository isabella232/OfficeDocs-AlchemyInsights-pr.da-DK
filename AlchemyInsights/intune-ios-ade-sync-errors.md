---
title: Synkroniseringsfejl i forbindelse med automatisk Apple-enhedsregistrering
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448916"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfejl i forbindelse med automatisk Apple-enhedsregistrering

"Vi har opdaget, at du har en eller flere ADE/DEP-tokens, der er i fejltilstand. Indtil fejltilstanden er løst for hvert påvirket token, fungerer ADE-funktionaliteten ikke som forventet."

Denne fejl kan blive vist på flere forskellige måder, herunder:

1. Enheder synkroniseres muligvis ikke fra ABM/ASM til Intune
2. Tilmeldingsprofiltildelinger mislykkes muligvis
3. Enheder er muligvis ikke færdige med ADE-tilmeldingen

Kontrollér for den synkroniseringsfejl, der er rapporteret i Intune-konsollen under Enheder> Tilmeld enheder **> Apple-registrering > tilmeldingsprogramtokens.**

En af de mest almindelige årsager til synkroniseringsfejl er udløb af det aktuelle token. I mange tilfælde vil fornyelse af det pågældende token løse problemet.

Hvis et eller flere af dine tokens er udløbet, kan du se følgende dokumentation, der kan hjælpe dig med at forny dem efter behov:

[Forny et automatiseret enhedsregistreringstoken](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Desuden kan du se følgende dokumentation for at se mulige afhjælpninger for andre fejl, der forårsager tokensynkroniseringsfejl:

[ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS-automatiserede enhedsregistreringstokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS-automatiserede enhedsregistreringstokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
