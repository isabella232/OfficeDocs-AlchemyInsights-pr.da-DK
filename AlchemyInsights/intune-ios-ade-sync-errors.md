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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="975ea-102">Synkroniseringsfejl for Apple-automatisk enheds tilmelding</span><span class="sxs-lookup"><span data-stu-id="975ea-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="975ea-103">"Vi har registreret, at du har en eller flere ADE/DEP-tokens, som er i en fejltilstand.</span><span class="sxs-lookup"><span data-stu-id="975ea-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="975ea-104">Indtil fejltilstanden er løst for hvert berørt token, fungerer ADE-funktionen ikke for den samme ".</span><span class="sxs-lookup"><span data-stu-id="975ea-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="975ea-105">Denne fejl kan opstå på flere forskellige måder, herunder:</span><span class="sxs-lookup"><span data-stu-id="975ea-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="975ea-106">Enheder synkroniseres muligvis ikke fra ABM/ASM til Intune</span><span class="sxs-lookup"><span data-stu-id="975ea-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="975ea-107">Tildelingen af tilmeldings profilen er muligvis failede</span><span class="sxs-lookup"><span data-stu-id="975ea-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="975ea-108">Enheder har muligvis ikke fuldført ADE-tilmelding</span><span class="sxs-lookup"><span data-stu-id="975ea-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="975ea-109">Søg efter den synkroniseringsfejl, der er rapporteret i Intune-konsollen under **enheder > Registrer enheder > Apple-tilmelding > Tilmeldingsprogram-tokens** og gennemgå følgende dokumentation for at få vist potentielle afhjælpninger:</span><span class="sxs-lookup"><span data-stu-id="975ea-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="975ea-110">ABM/ASM synkroniseringsfejl for iOS/iPadOS og macOS-tokens til registrering af automatisk enhed</span><span class="sxs-lookup"><span data-stu-id="975ea-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
