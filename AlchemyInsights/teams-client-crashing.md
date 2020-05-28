---
title: Går Teams-klient ned?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354046"
---
# <a name="teams-client-crashing"></a>Går Teams-klient ned?

Hvis din Teams-klient går ned, kan du prøve følgende:

- Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Sørg for, at alle [Microsoft 365-url'er og adresseområder](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.

- Log på med din lejeradministratorkonto, og tjek [dashboardet for tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at kontrollere, at der ikke er nogen nedbrud eller forringelse af tjenesten.

- Fjerne og geninstallere programmet Teams (link)
    - Gå til mappen %appdata%\Microsoft\teams\ på computeren, og slet alle filer i den pågældende mappe.
    - [Download og installer Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og installer, hvis det er muligt, Teams som administrator (højreklik på installationsprogrammet Teams, og vælg "Kør som administrator", hvis det er muligt).

Hvis din Teams-klient stadig går ned, kan du så genskabe problemet? Hvis ja:

1. Brug Trinoptageren til at hente dine trin.
    - Luk ALLE unødvendige eller fortrolige ansøgninger.
    - Start Trinoptageren, og gengiv problemet, mens du er logget på med den berørte brugerkonto.
    - [Saml de holdlogfiler, der registrerer de registrerede reprotrin](https://docs.microsoft.com/microsoftteams/log-files). **Bemærk:** Sørg for at registrere logonadressen for den påvirkede bruger.
    - Indsaml oplysningerne om dump og/eller fejlbucket (Windows). Start Windows Powershell på den maskine, hvor nedbruddet sker, og kør følgende kommandoer:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Vedhæft filen til supportsagen.
