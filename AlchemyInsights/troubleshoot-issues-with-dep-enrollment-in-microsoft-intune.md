---
title: Fejlfinding af problemer med DEP-registrering i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: e77295f0395919a723dcec1a313ca03154ae59b1bea22bf791f3a0f923cab60d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008252"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Fejlfinding af problemer med DEP-registrering i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu.
  
1. Hvis DEP-enheden ikke kan tilmeldes, og MFA (Multi-Factor Authentication) er aktiveret, skal du deaktivere MFA. MFA understøttes i øjeblikket ikke for DEP-registrering

2. Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.

3. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [Fejlfinding af dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

4. [Få mere at vide om tilmeldingsprogram til enheder](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
