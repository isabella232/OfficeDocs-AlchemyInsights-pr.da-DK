---
title: Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658872"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune

Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.
  
Nogle almindelige fejlmeddelelser og løsnings trin:
  
 **Softwaren kan ikke installeres, 0x80cf4017:** Dit konto certifikat er udløbet. Download PC-klientsoftware pakken igen i Intune-administrationskonsollen. Læs denne dokumentation for at få flere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan forekomme i følgende scenarier:
  
-  Brugeren har flere enheder, der er tilmeldt en enheds grænse. Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre enheds grænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Brugerne kan tilmelde sig enheder til Azure AD" er indstillet til "ingen". Sæt det til alle, eller Vælg brugere. Læs [denne dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få flere oplysninger.

-  Enheden er allerede tilmeldt en anden bruger. Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller fjerne registreringen af enheden manuelt, før du prøver igen.

-  Enheden er Windows 10 Home. Kun Windows 10 Pro-, Education-og Enterprise-SKU'er kan deltage i Azure Active Directory.

Yderligere ressourcer, der kan hjælpe med at løse dit problem:
  
-  Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl. Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.

-  Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
