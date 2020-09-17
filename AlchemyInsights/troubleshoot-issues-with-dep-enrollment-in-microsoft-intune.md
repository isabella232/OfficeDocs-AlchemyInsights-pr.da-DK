---
title: Fejlfinding af problemer med DEP-tilmelding i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797290"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Fejlfinding af problemer med DEP-tilmelding i Microsoft Intune

Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.
  
1. Hvis DEP-enheden ikke kan registrere og MFA (multi-Factor Authentication) er aktiveret, skal du deaktivere MFA. Aktuelt MFA understøttes ikke for registrering af forhindring af datakørsel

2. Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl. Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.

3. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [Få mere at vide om tilmeldings programmet til enheder](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
