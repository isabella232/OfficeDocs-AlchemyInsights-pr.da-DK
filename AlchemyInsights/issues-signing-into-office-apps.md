---
title: Problemer med at logge på Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709100"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Meddelelse om, at din computers pålidelige platformsmodul ikke fungerer korrekt, i Microsoft 365-apps

Du kan rette fejlen ved at følge disse trin:

- Installér de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Fjern Office-legitimationsoplysninger ved](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) hjælp af Windows Legitimationsstyring.<br/>
    **Bemærk!** Stierne i registreringsdatabasen til Office 2016 er ændret til 16.0. (Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv processen [for brugergendannelse for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) at rette fejl i et platformsmodul (Trusted Platform Module, TPM).
- Angiv EnableADAL = 0 ved at benytte følgende fremgangsmåde:  
    1. Højreklik på knappen Start i Windows, vælg **Kør,** skriv **regedit,** og vælg derefter **OK.**
    2. Vælg **Ja for** at tillade Registreringseditor at foretage ændringer på din enhed.
    3. I Registreringseditor skal du tilføje en DWORD-værdi **af EnableADAL** med en **indstilling på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Du kan finde flere oplysninger under Problemer med forbindelse ved logon efter opdatering til [Office 2016 build 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)