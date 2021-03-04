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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="fe386-102">Synkroniseringsfejl i forbindelse med automatisk Apple-enhedsregistrering</span><span class="sxs-lookup"><span data-stu-id="fe386-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="fe386-103">"Vi har opdaget, at du har en eller flere ADE/DEP-tokens, der er i fejltilstand.</span><span class="sxs-lookup"><span data-stu-id="fe386-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="fe386-104">Indtil fejltilstanden er løst for hvert påvirket token, fungerer ADE-funktionaliteten ikke som forventet."</span><span class="sxs-lookup"><span data-stu-id="fe386-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="fe386-105">Denne fejl kan blive vist på flere forskellige måder, herunder:</span><span class="sxs-lookup"><span data-stu-id="fe386-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="fe386-106">Enheder synkroniseres muligvis ikke fra ABM/ASM til Intune</span><span class="sxs-lookup"><span data-stu-id="fe386-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="fe386-107">Tilmeldingsprofiltildelinger mislykkes muligvis</span><span class="sxs-lookup"><span data-stu-id="fe386-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="fe386-108">Enheder er muligvis ikke færdige med ADE-tilmeldingen</span><span class="sxs-lookup"><span data-stu-id="fe386-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="fe386-109">Kontrollér for den synkroniseringsfejl, der er rapporteret i Intune-konsollen under Enheder> Tilmeld enheder **> Apple-registrering > tilmeldingsprogramtokens.**</span><span class="sxs-lookup"><span data-stu-id="fe386-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="fe386-110">En af de mest almindelige årsager til synkroniseringsfejl er udløb af det aktuelle token.</span><span class="sxs-lookup"><span data-stu-id="fe386-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="fe386-111">I mange tilfælde vil fornyelse af det pågældende token løse problemet.</span><span class="sxs-lookup"><span data-stu-id="fe386-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="fe386-112">Hvis et eller flere af dine tokens er udløbet, kan du se følgende dokumentation, der kan hjælpe dig med at forny dem efter behov:</span><span class="sxs-lookup"><span data-stu-id="fe386-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="fe386-113">Forny et automatiseret enhedsregistreringstoken</span><span class="sxs-lookup"><span data-stu-id="fe386-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="fe386-114">Desuden kan du se følgende dokumentation for at se mulige afhjælpninger for andre fejl, der forårsager tokensynkroniseringsfejl:</span><span class="sxs-lookup"><span data-stu-id="fe386-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="fe386-115">ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS-automatiserede enhedsregistreringstokens</span><span class="sxs-lookup"><span data-stu-id="fe386-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="fe386-116">ABM/ASM-synkroniseringsfejl for iOS/iPadOS og macOS-automatiserede enhedsregistreringstokens</span><span class="sxs-lookup"><span data-stu-id="fe386-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
