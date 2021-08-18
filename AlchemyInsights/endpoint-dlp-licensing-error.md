---
title: DLP-licensfejl i slutpunkt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090127"
---
# <a name="endpoint-dlp-licensing-error"></a>DLP-licensfejl i slutpunkt

Hvis du får vist følgende fejl, når du forsøger at konfigurere Slutpunkt DLP:

`Your organization is missing the licenses required to manage these devices`.

Sørg for, at du har et af følgende abonnementer eller tilføjelser:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 overholdelse af regler og standarder
- Microsoft 365 A5 overholdelse af regler og standarder
- Microsoft 365 E5 beskyttelse og styring af oplysninger
- Microsoft 365 A5 beskyttelse og styring af oplysninger

> [!NOTE]
> Dette fungerer ikke for licenskombinationer som: Win E5 + O365 E5 + EMS E5. Du skal have en ren M365 E5-licens for at konfigurere denne funktion.

Du kan finde flere oplysninger om DLP-licensering for [slutpunkter i Endpoint DLP-licensering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
