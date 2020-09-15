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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695173"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Rettelse af Microsoft 365-apps "din computers Trusted Platform-modul fungerer ikke korrekt"-meddelelse

Du kan rette fejlen ved at følge disse trin:

- Installer de seneste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows credential Manager.<br/>
    **Bemærk:** Registreringsdatabase stierne til Office 2016 er blevet ændret til 16,0. (F. eks.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [genoprettelsesprocessen for brugeren](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at løse TPM-fejl (Trusted Platform Module).
- Angiv EnableADAL = 0 ved hjælp af følgende trin:  
    1. Højreklik på knappen Start i Windows, Vælg **Kør**, Skriv **regedit**, og vælg derefter **OK**.
    2. Vælg **Ja** for at tillade, at registrerings Editor foretager ændringer på din enhed.
    3. I registrerings Editor skal du tilføje en DWORD-værdi for **EnableADAL** med en indstilling på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Hvis du vil have mere at vide, skal du se [forbindelsesproblemer i logon efter opdatering til Office 2016 Build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).