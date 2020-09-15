---
title: Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune
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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669242"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune

Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu. 
  
Nogle almindelige fejlmeddelelser og løsnings trin:
  
- **Enheds dæksel er nået** Brugeren har flere enheder, der er tilmeldt en enheds grænse. Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre enheds grænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne tjeneste understøttes ikke. Ingen registreringspolitik:** Apple Push Notification-tjenesten (APNS) skal være konfigureret eller fornyet. Gennemgå [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få oplysninger om, hvordan du gør det. 
    
- **Brugerlicens typen er ugyldig, eller brugernavnet blev ikke genkendt:** Brugeren skal have tildelt en Intune-eller EMS-licens. Gennemgå disse dokumenter for at tildele en licens via: [Office administration](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portalen](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Yderligere ressourcer, der kan hjælpe med at løse dit problem:
  
1. Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl. Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger. 
    
2. Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Få mere at vide om, hvordan du registrerer iOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

