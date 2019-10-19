---
title: Fejlfinding af problemer med tilmelding af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506917"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding af problemer med tilmelding af iOS-enheder i Microsoft Intune

Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu. 
  
Nogle almindeligt forekommende fejlmeddelelser og løsningstrin:
  
- **Enhedens dæksel er nået** Brugeren har flere enheder tilmeldt end enhedens grænse. Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre enhedens grænse](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjeneste understøttes ikke. Ingen tilmeldings politik:** Apple Push Notification Service (APNS) skal konfigureres eller fornys. Gennemse [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få vejledning i, hvordan du gør det. 
    
- **Brugerlicens typen er ugyldig, eller brugernavnet genkendes ikke:** Brugeren skal tildeles en Intune-eller EMS-licens. Gennemgå disse dokumenter for at tildele en licens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Yderligere ressourcer, som kan hjælpe dig med at løse problemet:
  
1. Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindeligt forekommende registreringsfejl. Læs [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger. 
    
2. Gennemse disse dokumenter for at se en liste over almindeligt forekommende fejl, der forhindrer tilmelding og løsninger på hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Se, hvordan du tilmelder iOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

