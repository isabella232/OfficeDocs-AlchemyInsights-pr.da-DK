---
title: Problemer med at logge på Microsoft 365 apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744630"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemer med at logge på Microsoft 365 Apps

Bemærk! Hvis du bruger en ældre version af Windows (f.eks. Windows 7 SP1, Windows Server 2008 R2), skal du bruge den nemme løsning til at aktivere TLS 1.2 som standard. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Få mere at vide under Opdater for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP Windows .

Du kan løse logonproblemer med Microsoft 365 ved at prøve følgende indstillinger på den pågældende computer:  

- Du Windows oplysninger [Anbefalinger oplysninger om løsning af almindelige problemer med logon](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Til Mac skal du [se Kan du ikke logge på en Office 2016 til Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tip** På Windows-computere kan vi diagnosticere og automatisk løse Office almindelige problemer med logon for dig. Download og kør **[Microsoft-Support- og genoprettelsesassistent at](https://aka.ms/SaRA-OfficeSignInScenario)** bruge vores automatiserede værktøj.

**Bemærk!** Deaktivering af moderne godkendelse (ADAL) eller WAM (Web Account Management) til løsning af problemer med logon eller aktivering **anbefales ikke.** Hvis fejlene opstår, når du opretter forbindelse til en Microsoft 365 bruger Office 2013, skal du sikre dig, at du aktiverer moderne godkendelse [for](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Office klient.

Du kan finde specifikke fejlfindingshandlinger i:

[Forbindelsesproblemer ved logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Du kan ikke logge på din organisationskonto, f.eks. Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Sådan foretager du fejlfinding af ikke-browserapps, der ikke kan logge på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Gentagne gange bedt om legitimationsoplysninger i Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)