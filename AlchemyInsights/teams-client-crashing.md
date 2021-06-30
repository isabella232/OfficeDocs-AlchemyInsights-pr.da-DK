---
title: Teams klient går ned
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187715"
---
# <a name="teams-client-crashing"></a>Teams klient går ned

Hvis din Teams-klient går ned, kan du prøve følgende:

- Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Sørg for, at [alle Microsoft 365 og adresseintervaller er](/microsoftteams/connectivity-issues) tilgængelige.

- Log på med din lejeradministratorkonto, og kontrollér dit Dashboard for [tjenestetilstand](/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen forringelse af tjenesten eller strømsvigt.

- Fjern og geninstaller Teams programmet
    - Gå til mappen %appdata%\Microsoft\Teams\ på computeren, og slet alle filer i mappen.
    - [Download og installér Teams-appen](https://www.microsoft.com/microsoft-teams/download-app), og hvis det er muligt, skal du installere Teams som administrator (højreklik på installationsprogrammet til Teams, og vælg Kør som **administrator,** hvis det er tilgængeligt).

Hvis klienten Teams, der stadig går ned, kan du prøve at genskabe problemet. Hvis du kan:

1. Brug Trinoptager til at registrere dine trin.
    - Luk ALLE unødvendige eller fortrolige programmer.
    - Start Trinoptager, og genskab problemet, mens du er logget på med den pågældende brugerkonto.
    - [Indsaml de teamlogfiler, der registrerer de registrerede genpropro trin](/microsoftteams/log-files). **Bemærk!** Sørg for at registrere logonadressen på den pådrede bruger.
    - Indsaml oplysninger om dump og/eller fejl bucket (Windows). Start Windows Powershell på den computer, hvor nedbruddet sker, og kør følgende kommandoer (tryk på Enter efter hver kommando):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Når tekstfilen er oprettet og vises på skærmen, skal du gemme filen og vedhæfte den til serviceanmodningen. 
