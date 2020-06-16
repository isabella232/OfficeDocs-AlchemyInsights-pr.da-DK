---
title: Fejlfinding i forbindelse med nedbrud i OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748796"
---
# <a name="troubleshoot-onedrive-crashes"></a>Fejlfinding i forbindelse med nedbrud i OneDrive

Hvis OneDrive gentagne gange går ned, kan du prøve disse fejlfindingstrin:

**Kontroller, at registreringsdatabasenøgler ikke er angivet:**

1. Brug Registreringseditor til at navigere til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC er til stede og indstillet til 1, skal du åbne nøglen og ændre værdien til 0.
3. Start OneDrive manuelt ved at gå til Start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skal du skrive OneDrive i søgefeltet og derefter klikke på OneDrive-skrivebordsappen.

**Nulstil OneDrive:**

Noter:

- Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder dit personlige OneDrive, hvis konfigureret).
- Du mister ikke filer eller data ved at nulstille OneDrive på din computer.

**Sådan nulstilles OneDrive:**

1. Åbn dialogboksen Kør ved at trykke på Windows-tasten og R.
2. Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og tryk på OK. Der vises muligvis et kommandovindue kortvarigt.
3. Start OneDrive manuelt ved at gå til Start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skal du skrive OneDrive i søgefeltet og derefter klikke på OneDrive-skrivebordsappen.

Noter:

- Hvis du havde valgt kun at synkronisere nogle mapper før nulstillingen, skal du gøre det igen, når synkroniseringen er fuldført. Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres til computeren](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)for at få flere   oplysninger.
- Du skal udfylde dette for dit personlige OneDrive og OneDrive for Business.