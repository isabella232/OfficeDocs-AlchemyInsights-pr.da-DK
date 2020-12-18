---
title: Synkroniseringsfejl for Apple-automatisk enheds tilmelding
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714739"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfejl for Apple-automatisk enheds tilmelding

"Vi har registreret, at du har en eller flere ADE/DEP-tokens, som er i en fejltilstand. Indtil fejltilstanden er løst for hvert berørt token, fungerer ADE-funktionen ikke for den samme ".

Denne fejl kan opstå på flere forskellige måder, herunder:

1. Enheder synkroniseres muligvis ikke fra ABM/ASM til Intune
2. Tildelingen af tilmeldings profilen er muligvis failede
3. Enheder har muligvis ikke fuldført ADE-tilmelding

Søg efter den synkroniseringsfejl, der er rapporteret i Intune-konsollen under **enheder > Registrer enheder > Apple-tilmelding > Tilmeldingsprogram-tokens** og gennemgå følgende dokumentation for at få vist potentielle afhjælpninger:

[ABM/ASM synkroniseringsfejl for iOS/iPadOS og macOS-tokens til registrering af automatisk enhed](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
