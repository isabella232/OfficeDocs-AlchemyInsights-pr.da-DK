---
title: Fejlfinding af problemer med tilmelding af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708956"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding af problemer med tilmelding af iOS-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu. 
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
- **Enhedsgrænse nået** Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Denne tjeneste understøttes ikke. Ingen registreringspolitik:** Apple Push Notification Service (APNS) skal konfigureres eller fornyes. Gennemgå [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få en vejledning i, hvordan du gør det. 
    
- **Ugyldig brugerlicenstype eller brugernavnet blev ikke genkendt:** Brugeren skal have tildelt en Intune- eller EMS-licens. Gennemse disse dokumenter for at tildele en licens [via: Office Administration eller](https://docs.microsoft.com/intune/licenses-assign) [Azure-portalen.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Yderligere ressourcer til at løse problemet:
  
1. Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger. 
    
2. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindingsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Få mere at vide om, hvordan du tilmelder iOS-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

