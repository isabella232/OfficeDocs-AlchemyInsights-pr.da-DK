---
title: Fejlfinding af Microsoft Defender for Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: ea05d60d1cdb4079d52e0a317331f7e98845b82bd74429dc8fa63377c2527a74
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900646"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Fejlfinding af Microsoft Defender for Office 365

- **Bemærker du forsinkelser i leveringen af meddelelser?** Brug indstillingen [Dynamisk levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i din Politik for Microsoft Defender til Office 365 Pengeskab vedhæftede filer. Dette hjælper med at undgå forsinkelser i meddelelser, mens modtagerne beskyttes mod skadelige filer.

- **Vil du rapportere falske positive eller falske negativer til Microsoft?** Brug [Indsendelsesstifinder](https://protection.office.com/reportsubmission).

-** Vidste du, at du kan aktivere Pengeskab Links-beskyttelse for interne mails, der sendes mellem modtagere i din organisation?** Følg disse trin:

  1. Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator- eller sikkerhedsadministratorkonto.

  2. I venstre navigationsrude under **Trusselsstyring** skal du **vælge** \> **Pengeskab Links**.

  3. I sektionen **Politikker, der gælder for hele organisationen skal** du markere politikken og klikke på **Rediger.**

  4. Under **Indstillinger** skal du aktivere **Anvend sikre links til meddelelser, der er sendt i organisationen.**
