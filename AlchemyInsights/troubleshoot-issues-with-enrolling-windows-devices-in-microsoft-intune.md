---
title: Fejlfinding af problemer med tilmelding af Windows-enheder i Microsoft Intune
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708884"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding af problemer med tilmelding af Windows-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor for at løse problemet nu.
  
Nogle almindelige fejlmeddelelser og løsningstrin:
  
 **Softwaren kan ikke installeres, 0x80cf4017:** Dit kontocertifikat er udløbet. Hent pc-klientsoftwarepakken igen i Intune-administrationskonsollen. Gennemgå denne dokumentation for at få flere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan opstå i følgende scenarier:
  
-  Brugeren har flere enheder tilmeldt end enhedsgrænsen. Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Brugere kan slutte enheder til Azure AD" er indstillet til "ingen". Indstil den til alle eller vælg brugere. Gennemgå [denne dokumentation for](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) at få flere oplysninger.

-  Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller manuelt fjerne tilmeldingen af enheden, før du prøver igen.

-  Enheden er Windows 10 Home. Kun Windows 10 Pro-, Education- og Enterprise SKU'er kan deltage i Azure Active Directory.

Yderligere ressourcer til at løse problemet:
  
-  Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl. Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.

-  Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfindingsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
