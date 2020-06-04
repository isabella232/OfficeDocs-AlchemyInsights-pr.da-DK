---
title: Fejlfinding i forbindelse med registrering af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665826"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registrering af Windows-enheder i Microsoft Intune

Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
 **Softwaren kan ikke installeres, 0x80cf4017:** Dit kontocertifikat er udløbet. Download pc-klientens softwarepakke igen i Intune Admin Console. Læs denne dokumentation for at få flere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan opstå i følgende scenarier:
  
-  Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Brugere kan slutte sig til azure AD" er indstillet til "ingen". Indstil den til alle eller vælg brugere. Læs [denne dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få flere oplysninger.

-  Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller manuelt frigøre enheden, før du prøver igen.

-  Enheden er Windows 10 Home. Det er kun Windows 10 Pro- og Education- og Enterprise-SKU'er, der kan deltage i Azure Active Directory.

Yderligere ressourcer, der kan hjælpe dig med at løse problemet:
  
-  Brug [Intune-fejlfindingsportal til](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) at diagnosticere og løse almindelige tilmeldingsfejl. Læs [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.

-  Gennemse disse dokumenter for at få vist en liste over almindelige fejl, der forhindrer tilmelding og løsninger på de enkelte: [Fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [Fejlfinding af dokumenter](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
