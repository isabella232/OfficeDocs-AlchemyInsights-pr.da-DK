---
title: Problemer, der logger på Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938176"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fastsættelse af Office-meddelelsen "din computer du har tillid til Platform-modulet ikke virker korrekt" apps

Du kan rette denne fejl, kan du prøve følgende:

- Installere de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Fjern Office legitimationsoplysninger](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af styring af legitimationsoplysninger i Windows.<br/>
    **Bemærk:** Stier i registreringsdatabasen for Office 2016 er ændret til 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv at [processen til genoprettelse af brugeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at rette fejl til TPM (Trusted Platform Module).
- Angiv EnableADAL = 0 ved hjælp af følgende trin:  
    1. Skal du højreklikke på knappen Start i Windows, Vælg **Kør**, Skriv **regedit**, og klik derefter på **OK**.
    2. Vælg **Ja** for at gøre det muligt for Registreringseditor til at foretage ændringer til din enhed.
    3. I Registreringseditor, føje en DWORD-værdi på **EnableADAL** med en indstilling på **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Yderligere oplysninger finder du under [forbindelsen problemer i logon efter opdatering til Office 2016 build 16.0.7967 på Windows-10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).