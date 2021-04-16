---
title: Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808965"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu.
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
 **Softwaren kan ikke installeres, 0x80cf4017:** Dit kontocertifikat er udløbet. Download pc-klientsoftwarepakken i Intune-administrationskonsollen igen. Gennemgå denne dokumentation for at få flere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan opstå i følgende scenarier:
  
-  Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Brugere kan slutte enheder til Azure AD" er indstillet til "ingen". Indstil den til alle eller udvalgte brugere. Gennemgå denne [dokumentation for at](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) få flere oplysninger.

-  Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller manuelt fjerne tilmeldingen af enheden, før du prøver igen.

-  Enheden er Windows 10 Home. Kun Windows 10 Pro-, Education- og Enterprise-SKU'er kan deltage i Azure Active Directory.

Yderligere ressourcer, der kan hjælpe med at løse problemet:
  
-  Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.

-  Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt: [Fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [Fejlfinding af dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
