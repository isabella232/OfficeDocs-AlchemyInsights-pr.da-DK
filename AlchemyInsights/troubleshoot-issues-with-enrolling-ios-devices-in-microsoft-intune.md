---
title: Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924762"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune

Gennemse ressourcerne nedenfor til at løse dit problem nu. 
  
Nogle almindelige fejlmeddelelser og trin opløsning:
  
- **Enheden Cap er nået** Brugeren har flere enheder, der er tilmeldt end grænsen for enheden. Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Denne Service er ikke understøttet. Ingen registreringspolitik:** Apple Push Notification Service (APN'ER) skal være konfigureret eller fornyes. Gennemse [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få instruktioner om, hvordan du gør det. 
    
- **Bruger licens Type ugyldige eller brugernavn blev ikke genkendt:** Brugeren skal være tildelt en licens til Intune eller EMS. Gennemgå disse dokumenter for at tildele en licens til: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Yderligere ressourcer til at løse problemet:
  
1. Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger. 
    
2. Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lær, hvordan du registrere iOS enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

