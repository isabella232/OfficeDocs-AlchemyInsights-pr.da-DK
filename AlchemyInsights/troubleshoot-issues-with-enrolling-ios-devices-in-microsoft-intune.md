---
title: Fejlfinding i forbindelse med problemer med tilmelding af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736152"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med problemer med tilmelding af iOS-enheder i Microsoft Intune

Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu. 
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
- **Enhedshætten er nået** Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjeneste understøttes ikke. Ingen tilmeldingspolitik:** Apns (Apple Push Notification Service) skal konfigureres eller fornys. Gennemse [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få vejledning i, hvordan du gør det. 
    
- **Brugerlicenstypen Ugyldig eller brugernavn et ikke genkendt:** Brugeren skal tildeles en Intune- eller EMS-licens. Gennemse disse dokumenter for at tildele en licens via: [Office Administration](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portal .](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Yderligere ressourcer, der kan hjælpe dig med at løse problemet:
  
1. Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldingsfejl. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger. 
    
2. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsning af hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindingsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Få mere at vide om, hvordan du tilmelder iOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

