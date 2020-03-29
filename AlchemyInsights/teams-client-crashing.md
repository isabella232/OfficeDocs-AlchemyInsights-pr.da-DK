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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030537"
---
# <a name="teams-client-crashing"></a>Går Teams-klient ned?

Hvis din Teams-klient går ned, kan du prøve følgende:

- Hvis du bruger Teams-skrivebordsapp, [skal du sørge for, at appen er helt opdateret](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Sørg for, at alle [Office 365-webadresser og -adresseområder](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgængelige.

- Log på med din administratorkonto, og kontroller dit [Dashboard for tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for at bekræfte, at der ikke er nogen afbrydelse eller forringelse af tjenesten.

 - Som sidste trin kan du forsøge at rydde Teams-klientcachen:

    1.  Afslut Microsoft Teams-skrivebordsklienten helt. Du kan højreklikke på **Teams** fra ikonbakken, og klikke på **Afslut**, eller køre Jobliste og afslutte processen helt.

    2.  Gå til Stifinder, og skriv %appdata%\Microsoft\teams.

    3.  Når du er i kataloget, får du vist nogle af følgende mapper:

         - I **Programcache** skal du gå til Cache og slette alle filer på cacheplaceringen: %appdata%\Microsoft\teams\application cache\cache.

        - Inde fra **Blob_storage** skal du slette alle filer: %appdata%\Microsoft\teams\blob_storage.

        - Inde fra **Cache** skal du slette alle filer: %appdata%\Microsoft\teams\Cache.

        - Inde fra **databaser** skal du slette alle filer: %appdata%\Microsoft\teams\databases.

        - Inde fra **GPUCache** skal du slette alle filer: %appdata%\Microsoft\teams\GPUcache.

        - Inde fra **IndexedDB** skal du slette .db-filen: %appdata%\Microsoft\teams\IndexedDB.

        - Inde fra **Lokalt lager** skal du slette alle filer: %appdata%\Microsoft\teams\Local Storage.

        - Til sidst skal du inde fra **tmp** slette en hvilken som helst fil: %appdata%\Microsoft\teams\tmp.

    4. Genstart din Teams-klient.
