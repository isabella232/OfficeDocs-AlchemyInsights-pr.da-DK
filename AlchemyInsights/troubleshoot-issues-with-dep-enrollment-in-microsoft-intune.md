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
ms.openlocfilehash: 27abeafba5588ca74569ba6bebc5d940b767ea3f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824501"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Fejlfinding af problemer med DEP-registrering i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu.
  
1. Hvis DEP-enheden ikke kan tilmeldes, og MFA (Multi-Factor Authentication) er aktiveret, skal du deaktivere MFA. MFA understøttes i øjeblikket ikke for DEP-registrering

2. Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.

3. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [Fejlfinding af dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

4. [Få mere at vide om tilmeldingsprogram til enheder](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
