---
title: Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559655"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune

Gennemse ressourcerne nedenfor til at løse dit problem nu.
  
Nogle almindelige fejlmeddelelser og trin opløsning:
  
 **Kan ikke installeres softwaren, 0x80cf4017:** Din konto er udløbet. Hent igen PC-klient softwarepakke i administrationskonsollen Intune. Gennemse dokumentationen for at få yderligere oplysninger.
  
 **Fejlkode 0x801c0003:** Fejlen kan opstå i følgende situationer:
  
1. Brugeren har flere enheder, der er tilmeldt end grænsen for enheden. Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Brugere kan tilslutte enheder til Azure AD" er indstillet til "ingen". Sæt den til alle, eller Vælg brugere. Gennemse [dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få yderligere oplysninger.

3. Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, kan du fjerne enheden fra konsollen Azure Intune eller manuelt unenroll enheden, før du prøver igen.

4. Enheden er Windows Home 10. Kun Windows 10 Pro, uddannelse og Enterprise lagervarer kan deltage i Azure Active Directory.

Yderligere ressourcer til at løse problemet:
  
1. Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.

2. Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lær at registrere Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
