---
title: Fejlfinding af Microsoft Defender til Office 365
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801437"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Fejlfinding af Microsoft Defender til Office 365

- Bemærker du forsinkelser i meddelelseslevering? Brug indstillingen [dynamisk levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i din politik for sikker sikkerhedstilknytning af DTT. Det hjælper med at undgå forsinkelser i meddelelser, mens du beskytter modtagere fra ondsindede filer.

- Vil du rapportere falske positive eller falske negativer til Microsoft? Brug dette [link](https://www.microsoft.com/wdsi/filesubmission/) til at sende filer til analyse.

- Vidste du, at du kan aktivere beskyttelse af sikre links for interne mails, der sendes mellem modtagere i din organisation? Følg disse trin:

  1. Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator-eller sikkerhedsadministrator konto.

  2. I venstre navigationsrude under **trussels styring** skal du **Policy** vælge \> **sikre links** til politik.

  3. I de **politikker, der gælder for hele sektionen organisation** , skal du vælge politikken og klikke på **Rediger** .

  4. Under **Indstillinger** skal du aktivere **Anvend sikre links til meddelelser, der sendes inden for organisationen** .
