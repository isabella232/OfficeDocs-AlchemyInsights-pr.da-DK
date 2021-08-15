---
title: Synkroniseringsfejl ved automatisk tilmelding til Apple-enhed
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013742"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfejl ved automatisk tilmelding til Apple-enhed

"Vi har opdaget, at du har en eller flere ADE/DEP-tokens, der er i fejltilstand. Indtil fejltilstanden er løst for hvert påvirket token, vil ADE-funktionaliteten ikke fungere som forventet.".

Denne fejl kan blive vist på flere forskellige måder, herunder:

1. Enheder synkroniseres muligvis ikke fra ABM/ASM til Intune
2. Registreringsprofiltildelinger mislykkes muligvis
3. Enheder fuldfører muligvis ikke ADE-tilmeldingen

Kontrollér for den synkroniseringsfejl, der er rapporteret i Intune-konsollen under Enheder > Tilmeld **enheder > Apple-> Tilmeldingsprogramtokens**.

En af de mest almindelige årsager til synkroniseringsfejl er udløb af det aktuelle token. I mange tilfælde kan fornyelse af det pågældende token løse problemet.

Hvis et eller flere af dine tokens er udløbet, skal du se følgende dokumentation, der kan hjælpe dig med at forny dem efter behov:

[Forny et automatiseret enhedsregistreringstoken](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Desuden kan du se følgende dokumentation for at se mulige afhjælpninger for andre fejl, der forårsager tokensynkroniseringsfejl:

[ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS Automatiserede enhedsregistreringstokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS Automatiserede enhedsregistreringstokens](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
