---
title: Opbevaringspolitikker Exchange Administration fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074926"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker Exchange Administration

Hvis du vil have os til at køre automatiserede kontroller af de indstillinger, der er nævnt nedenfor, skal du vælge knappen Tilbage < – øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med opbevaringspolitikkerne.

Hvis du har problemer med opbevaringspolitikker i Exchange Administration, der ikke gælder for postkasser eller elementer, der ikke flyttes til arkivpostkassen, skal du kontrollere følgende:

**Rodårsagen:**

- **Administreret mappeassistent** har ikke behandlet brugerens postkasse. Den administrerede mappeassistent forsøger at behandle hver postkasse i din skybaserede organisation én gang hver syv dage.

  **Løsning:** Kør assistenten til administrerede mapper.

- **Opbevaringshold** er **aktiveret** på postkassen. Hvis postkassen er placeret på en Opbevaringshold, behandles opbevaringspolitikken for postkassen ikke i dette tidsrum.

  **Løsning:** Kontrollér status for indstilling og opdatering af Opbevaringsposition efter behov. Du kan få mere at vide under [Opbevaringsposition for postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Bemærk!** Hvis en postkasse er mindre end 10 MB, behandler den administrerede mappeassistent ikke automatisk postkassen.
 
Du kan finde flere oplysninger om opbevaringspolitikker Exchange Administration i:

- [Opbevaringstags og opbevaringspolitikker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Anvend en opbevaringspolitik på postkasser eller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Tilføj [eller fjern opbevaringsmærker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Sådan identificeres den type venteposition, der er sat i en postkasse](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
