---
title: Problemer med at logge på Microsoft 365-apps
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579859"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Rettelse af Microsoft 365-apps "Computerens platformsmodul, der er tillid til, fungerer ikke korrekt"

Du kan rette fejlen ved at følge disse trin:

- Installer de nyeste opdateringer til [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Ryd Office-legitimationsoplysninger](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjælp af Windows Legitimationsstyring.<br/>
    **Bemærk:** Registreringsdatabasen stier for Office 2016 er ændret til 16.0. (Eks.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prøv [brugergenoprettelsesprocessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for at rette TPM-fejl (Trusted Platform Module).
- Angiv EnableADAL = 0 ved hjælp af følgende trin:  
    1. Højreklik på knappen Start i Windows, vælg **Kør**, skriv **regedit**, og vælg derefter **OK**.
    2. Vælg **Ja** for at tillade, at Registreringseditor foretager ændringer på enheden.
    3. Tilføj en DWORD-værdi i **EnableADAL** i Registreringseditor med en indstilling **på 0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Du kan finde flere oplysninger [under Forbindelsesproblemer ved logon efter opdatering til Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).