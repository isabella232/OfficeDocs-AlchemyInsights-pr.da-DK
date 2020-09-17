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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807653"
---
# <a name="conditional-access-with-intune"></a>Betinget adgang med Intune

Brug af  **betinget adgang**  med Intune kræver 3 trin:

- Opret en  **overholdelses politik**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) for at definere indstillinger, der skal opfyldes, før enheden anses for at være kompatibel. For eksempel skal en enhed have en pinkode på mindst 6 cifre, før den anses for at være kompatibel.
- Opret en **politik for betinget adgang**  , der definerer, hvilke ressourcer der beskyttes, og hvilke betingelser der skal opfyldes for at få adgang til disse ressourcer.  [For eksempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  skal en enhed være kompatibel, før du kan få adgang til virksomhedens mail.
- Sørg for, at både **overholdelsespolitikker**  og  **politikker for betinget adgang**  er målrettet til de ønskede grupper af brugere. Dette kan kræve, at du opretter bestemte grupper af brugere i Azure Active Directory.

**Nyttige links:**

[Oversigt over enheds overholdelse](https://docs.microsoft.com/intune/device-compliance-get-started)

[Fejlfindings NØGLECENTER](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fejlfindings politik](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Hvis du vil beskytte mail (Exchange Online) fra Access fra ikke-kompatible enheder, skal begge dokumenter følges:

1. [Beskytte mail adgang fra enheder ved hjælp af EA](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Beskytte mail adgang fra enheder, der bruger moderne godkendelses klienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)