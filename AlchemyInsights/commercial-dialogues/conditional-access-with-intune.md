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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744540"
---
# <a name="using-conditional-access-with-intune"></a>Brug af Betinget adgang med Intune

Brug af Betinget adgang med Intune kræver tre trin:

- [Opret en politik for overholdelse af regler og standarder for at definere indstillinger, der skal være opfyldt, før enheden betragtes som værende inden for reglerne. En enhed skal f.eks. have en pinkode på mindst 6 cifre, før den betragtes som værende kompatibel.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Opret en politik for betinget adgang, der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal være opfyldt for at få adgang til disse ressourcer. Eksempelvis skal en enhed være kompatibel, før den får adgang til virksomhedens mail.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Sørg for, at både overholdelsespolitikker og betingede adgangspolitikker er rettet mod de ønskede grupper af brugere. Dette kræver muligvis oprettelse af bestemte grupper af brugere i Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Læs mere...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
