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
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069706"
---
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug  **af Betinget adgang**  med Intune kræver tre trin:

- Opret en **Politik for overholdelse** af regler og standarder [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)for at definere indstillinger, der skal opfyldes, før enheden betragtes som værende inden for reglerne. En enhed skal f.eks. have en pinkode på mindst seks cifre, før den betragtes som værende inden for reglerne.
- Opret en **Betinget adgangspolitik,**  der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer.  [Eksempelvis skal en enhed](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  være kompatibel, før der tilgås virksomhedens mail.
- Sørg **for, at både Politikker**  for  **overholdelse af regler og standarder og**  Betingede adgangspolitikker er målrettet de ønskede grupper af brugere. Dette kræver muligvis oprettelse af bestemte grupper af brugere Azure Active Directory.

**Nyttige links:**

[Oversigt over enhedsoverholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings-nøglecenter](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindingspolitik](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

For at beskytte mail (Exchange online) mod adgang fra enheder, der ikke er lige så relevante, skal begge dokumenter følges:

1. [Beskyt mailadgang fra enheder med EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskyt mailadgang fra enheder, der bruger moderne godkendelsesklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)