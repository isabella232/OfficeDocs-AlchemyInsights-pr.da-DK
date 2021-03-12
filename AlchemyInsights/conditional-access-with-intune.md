---
title: Betinget adgang med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704780"
---
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug  **af Betinget adgang**  med Intune kræver tre trin:

- Opret en  **politik for overholdelse**  af regler og standarder [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)for at definere indstillinger, der skal opfyldes, før enheden betragtes som værende kompatibel. En enhed skal f.eks. have en pinkode på mindst 6 cifre, før den betragtes som værende kompatibel.
- Opret en **politik for betinget adgang,**  der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer.  [Eksempelvis skal en enhed](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  være kompatibel, før den får adgang til virksomhedens mail.
- Sørg **for, at både overholdelsespolitikker**  **og betingede**  adgangspolitikker er rettet mod de ønskede grupper af brugere. Dette kræver muligvis oprettelse af bestemte grupper af brugere i Azure Active Directory.

**Nyttige links:**

[Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindingspolitik](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

For at beskytte mail (Exchange Online) mod adgang fra enheder, der ikke er lige så relevante, skal begge dokumenter følges:

1. [Beskyt mailadgang fra enheder, der bruger EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskyt mailadgang fra enheder, der bruger moderne godkendelsesklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)