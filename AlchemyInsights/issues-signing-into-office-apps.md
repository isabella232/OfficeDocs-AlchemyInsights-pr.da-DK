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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986885"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Du får Microsoft 365 fejlmeddelelsen "Computerens platforms modul, der er tillid til, fungerer ikke korrekt"

Du kan rette fejlen ved at følge disse trin:

- Installér de seneste opdateringer [til Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Ryd Office legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Legitimationsstyring.<br/>
    **Bemærk!** Stierne i registreringsdatabasen Office 2016 ændret til 16.0. (Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv processen [for brugergendannelse for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) at løse problemer med fejl i et platformsmodul (Trusted Platform Module).
- Angiv EnableADAL = 0 ved at benytte følgende fremgangsmåde:  
    1. Højreklik på knappen Windows Start, vælg **Kør**, skriv **regedit**, og vælg derefter **OK**.
    2. Vælg **Ja for** at tillade registreringseditor at foretage ændringer på din enhed.
    3. I Registreringseditor skal du tilføje en **DWORD-værdi af EnableADAL** med en **indstilling på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Du kan få mere at vide under Forbindelsesproblemer ved logon efter opdatering til [Office 2016 build 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)