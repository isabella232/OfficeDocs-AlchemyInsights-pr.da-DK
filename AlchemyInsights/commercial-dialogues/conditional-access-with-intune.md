---
title: Brug af Betinget adgang med Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005768"
---
# <a name="using-conditional-access-with-intune"></a>Brug af Betinget adgang med Intune

Brug af Betinget adgang med Intune kræver tre trin:

- [Opret en Politik for overholdelse af regler og standarder for at definere indstillinger, der skal opfyldes, før enheden betragtes som værende inden for reglerne. En enhed skal f.eks. have en pinkode på mindst seks cifre, før den betragtes som værende inden for reglerne.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Opret en Betinget adgangspolitik, der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer. Eksempelvis skal en enhed være kompatibel, før der tilgås virksomhedens mail.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Sørg for, at både Politikker for overholdelse af regler og standarder og Betingede adgangspolitikker er målrettet de ønskede grupper af brugere. Dette kræver muligvis oprettelse af bestemte grupper af brugere Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Læs mere...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
