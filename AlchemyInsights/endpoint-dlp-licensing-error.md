---
title: Fejl i Endpoint-DLP-licens
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564480"
---
# <a name="endpoint-dlp-licensing-error"></a>Fejl i Endpoint-DLP-licens

Når du forsøger at konfigurere Endpoint DLP, hvis du får vist følgende fejlmeddelelse:

`Your organization is missing the licenses required to manage these devices`.

Kontrollér, at du har en af følgende abonnementer eller tilføjelsesprogrammer:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 overholdelse
- Microsoft 365 A5-overholdelse
- Microsoft 365 E5 informations beskyttelse og-styring
- Microsoft 365 A5 information Protection og styreformer

> [!NOTE]
> Dette fungerer ikke for licens kombinationer som: Win E5 + O365 E5 + EMS e5. Du skal have en ren M365 E5-licens for at kunne konfigurere denne funktion.

Du kan finde flere oplysninger om yderligere oplysninger om Endpoint-licenser under [Endpoint-licenser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) til DLP.
