---
title: Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420586"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor til at løse dit problem nu.
  
Nogle almindelige problemer og trin til løsning:
  
 **Enhed ikke krypteret fejl i firmaets Portal:** Nyere versioner af Android, især fra og med v7.0, kræver en start-adgangskode til at sikre, at enheden bliver fuldt krypteret. Almindelige løsninger er at aktivere pinkoden start eller fuldt krypterer enheden. Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få yderligere oplysninger. 
  
 **Enheder ikke kan kontrollere med tjenesten Intune eller vises som "Unhealthy" i administrationskonsollen Intune:** Nogle Samsung 4.4 og 5.5 enheder kan ikke kontrollere på tjenesten. Der er 3 mulige løsninger på dette problem: 
  
1. Åbn app Intune firmaets Portal, som automatisk starter en enhedssynkronisering manuelt.
    
2. Opdatere enheden Android 6.0 eller nyere.
    
3. Du kan deaktivere Samsung Smart Manager fra administration af portalen Intune virksomhed. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få yderligere oplysninger om disse problemer og løsninger. 
    
 **Bruger licens Type ugyldige** eller **bruger navn blev ikke genkendt fejl:** brugeren skal være tildelt en licens til Intune eller EMS. Gennemgå disse dokumenter for at tildele en licens til: Office Admin Center eller Azure portal. 
  
Yderligere ressourcer til at løse problemet:
  
1. Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger. 
    
2. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver. 
    
3. [Lær at tilmelde Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

