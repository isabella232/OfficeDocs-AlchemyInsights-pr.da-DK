---
title: Opbevaringspolitikker i Exchange Administration fungerer ikke
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952222"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Opbevaringspolitikker i Exchange Administration

Hvis du vil have os til at køre automatiserede kontroller af de indstillinger, der er nævnt nedenfor, skal du vælge knappen Tilbage < – øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med opbevaringspolitikkerne.

Hvis du har problemer med opbevaringspolitikker i Exchange Administration, der ikke gælder for postkasser eller elementer, der ikke flyttes til arkivpostkassen, skal du kontrollere følgende:

**Rodårsagen:**

- **Administreret mappeassistent** har ikke behandlet brugerens postkasse. Den administrerede mappeassistent forsøger at behandle hver postkasse i din skybaserede organisation én gang hver syv dage.

  **Løsning:** Kør assistenten til administrerede mapper.

- **Opbevaringshold** er **aktiveret** på postkassen. Hvis postkassen er placeret på en Opbevaringshold, behandles opbevaringspolitikken for postkassen ikke i dette tidsrum.

  **Løsning:** Kontrollér status for indstilling og opdatering af Opbevaringsposition efter behov. Du kan få mere at vide under [Opbevaringsposition for postkasse](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Bemærk!** Hvis en postkasse er mindre end 10 MB, behandler den administrerede mappeassistent ikke automatisk postkassen.
 
Du kan finde flere oplysninger om opbevaringspolitikker i Exchange Administration i:

- [Opbevaringstags og opbevaringspolitikker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Anvend en opbevaringspolitik på postkasser eller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Tilføj [eller fjern opbevaringsmærker](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Sådan identificeres den type venteposition, der er sat i en postkasse](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
