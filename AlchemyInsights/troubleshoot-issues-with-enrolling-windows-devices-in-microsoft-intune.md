---
title: Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665826"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor til at løse dit problem nu.
  
Nogle almindelige fejlmeddelelser og trin opløsning:
  
 **Kan ikke installeres softwaren, 0x80cf4017:** Din konto er udløbet. Hent igen PC-klient softwarepakke i administrationskonsollen Intune. Gennemse dokumentationen for at få yderligere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan opstå i følgende situationer:
  
-  Brugeren har flere enheder, der er tilmeldt end grænsen for enheden. Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Brugere kan tilslutte enheder til Azure AD" er indstillet til "ingen". Sæt den til alle, eller Vælg brugere. Gennemse [dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få yderligere oplysninger.

-  Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, kan du fjerne enheden fra konsollen Azure Intune eller manuelt unenroll enheden, før du prøver igen.

-  Enheden er Windows Home 10. Kun Windows 10 Pro, uddannelse og Enterprise lagervarer kan deltage i Azure Active Directory.

Yderligere ressourcer til at løse problemet:
  
-  Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.

-  Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lær at registrere Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
