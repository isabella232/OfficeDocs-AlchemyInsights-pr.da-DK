---
title: Betinget adgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931424"
---
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug af **betinget adgang** med Intune kræver 3 trin:

- Opret en **overholdelsespolitik** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for at definere indstillinger, der skal være opfyldt, før enheden anses for at være kompatibel. For eksempel skal en enhed have en nål på mindst 6 cifre, før den anses for at være kompatibel.
- Opret en **politik for betinget adgang,** der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.  For eksempel skal en enhed være [kompatibel,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) før du får adgang til virksomhedens e-mail.
- Sørg **for,** at både overholdelsespolitikker og **politikker for betinget adgang** målrettes mod de ønskede brugergrupper. Dette kan kræve, at der oprettes bestemte grupper af brugere i Azure Active Directory.

**Nyttige links:**

[Oversigt over overholdelse af enhed](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfinding i forbindelse med nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindingspolitik](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

For at beskytte e-mail (Exchange online) mod adgang for ikke-koverensstemmelsesenheder skal begge dokumenter følges:

1. [Beskyt e-mailadgang mod enheder, der bruger EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskyt mailadgang fra enheder ved hjælp af moderne godkendelsesklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)