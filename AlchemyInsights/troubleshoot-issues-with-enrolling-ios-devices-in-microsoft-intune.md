---
title: Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047970"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu. 
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
- **Caps til enhed er nået** Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Denne tjeneste understøttes ikke. Ingen registreringspolitik:** Apple Push Notification Service (APNS) skal konfigureres eller fornyes. Gennemgå [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få vejledning i, hvordan du gør dette. 
    
- **Brugerlicenstype Ugyldig eller Brugernavn blev ikke genkendt:** Brugeren skal have tildelt en Intune- eller EMS-licens. Gennemse disse dokumenter for at tildele en licens [via: Office Administration eller](https://docs.microsoft.com/intune/licenses-assign) [Azure-portalen.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Yderligere ressourcer, der kan hjælpe med at løse problemet:
  
1. Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger. 
    
2. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [Fejlfinding af dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Få mere at vide om, hvordan du tilmelder iOS-enheder Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

