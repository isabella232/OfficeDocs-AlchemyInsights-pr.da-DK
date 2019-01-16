---
title: Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283454"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune

Gennemse ressourcerne nedenfor til at løse dit problem nu. 
  
Nogle almindelige fejlmeddelelser og trin opløsning:
  
- **Enheden Cap er nået** Brugeren har flere enheder, der er tilmeldt end grænsen for enheden. Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/en-us/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne Service er ikke understøttet. Ingen registreringspolitik:** Apple Push Notification Service (APN'ER) skal være konfigureret eller fornyes. Gennemse [dette dokument](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for at få instruktioner om, hvordan du gør det. 
    
- **Bruger licens Type ugyldige eller brugernavn blev ikke genkendt:** Brugeren skal være tildelt en licens til Intune eller EMS. Gennemgå disse dokumenter for at tildele en licens til: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Yderligere ressourcer til at løse problemet:
  
1. Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) for at få yderligere oplysninger. 
    
2. Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfinding doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lær, hvordan du registrere iOS enheder i Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

