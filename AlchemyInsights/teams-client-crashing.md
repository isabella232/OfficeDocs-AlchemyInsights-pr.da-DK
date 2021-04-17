---
title: Går Teams-klient ned?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826265"
---
# <a name="teams-client-crashing"></a>Går Teams-klient ned?

Hvis din Teams-klient går ned, kan du prøve følgende:

- Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Sørg for, at alle [URL-adresser og adresseintervaller for Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.

- Log på med din lejeradministratorkonto, og kontrollér dit Dashboard for [tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen forringelse af tjenesten eller strømsvigt.

- Fjern og geninstaller Teams-programmet (link)
    - Gå til mappen %appdata%\Microsoft\teams\ på computeren, og slet alle filer i mappen.
    - [Download og installér Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), og hvis det er muligt, skal du installere Teams som administrator (højreklik på Teams-installationsprogrammet, og vælg "Kør som administrator", hvis det er tilgængeligt).

Hvis din Teams-klient stadig går ned, kan du så genskabe problemet? Hvis det er sådan:

1. Brug Trinoptager til at registrere dine trin.
    - Luk ALLE unødvendige eller fortrolige programmer.
    - Start Trinoptager, og genskab problemet, mens du er logget på med den pågældende brugerkonto.
    - [Indsaml de teamlogfiler, der registrerer de registrerede genpropro trin](https://docs.microsoft.com/microsoftteams/log-files). **Bemærk!** Sørg for at registrere logonadressen på den pådrede bruger.
    - Indsaml oplysninger om dumpet og/eller Bucket (Windows). Start Windows Powershell på den computer, hvor nedbruddet sker, og kør følgende kommandoer:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Vedhæft filen til din supportsag.
