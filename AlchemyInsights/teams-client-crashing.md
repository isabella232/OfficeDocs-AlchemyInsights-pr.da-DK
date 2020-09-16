---
title: Går Teams-klient ned?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691101"
---
# <a name="teams-client-crashing"></a>Går Teams-klient ned?

Hvis din Teams-klient går ned, kan du prøve følgende:

- Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Sørg for, at alle [Microsoft 365-URL-adresser og adresseområder](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.

- Log på med din lejeradministrator konto, og Kontrollér dit [tjeneste tilstands Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen afbrydelse eller tjeneste forringelse.

- Fjern og geninstaller teams-programmet (link)
    - Gå til mappen%appdata%\Microsoft\teams\ på computeren, og slet alle filer i den pågældende mappe.
    - [Download og installér teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og hvis det er muligt, skal du installere teams som administrator (Højreklik på teams Installer, og vælg "Kør som administrator", hvis det er muligt).

Hvis dine teams-klient stadig går ned, kan du genskabe problemet? Hvis det er tilfældet:

1. Brug Trinoptager til at registrere dine trin.
    - Luk alle unødvendige eller fortrolige programmer.
    - Start Trinoptager, og Genskab problemet, mens du er logget på med den pågældende brugerkonto.
    - [Indsaml de team logfiler, der henter de registrerede repro-trin](https://docs.microsoft.com/microsoftteams/log-files). **Bemærk**: Sørg for, at du registrerer logonnavnet for den påvirkede bruger.
    - Indsaml oplysninger om lagring og/eller fejl-buckets (Windows). Start Windows PowerShell på den computer, hvor crashet opstår, og Kør følgende kommandoer:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Vedhæft filen til din support-sag.
