---
title: Fejlfinding af OneDrive går ned
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826193"
---
# <a name="troubleshoot-onedrive-crashes"></a>Fejlfinding af OneDrive går ned

Hvis OneDrive går ned gentagne gange, kan du prøve disse fejlfindingstrin:

**Sørg for, at registreringsdatabasenøgler ikke er angivet:**

1. Brug registreringseditoren til at navigere til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC er til stede og angivet til 1, skal du åbne nøglen og ændre værdien til 0.
3. Start OneDrive manuelt ved at gå til Start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i søgefeltet, og klik derefter på OneDrive-skrivebordsappen.

**Nulstil OneDrive:**

Bemærkninger:

- Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder din personlige OneDrive, hvis konfigureret).
- Du mister ikke filer eller data ved at nulstille OneDrive på computeren.

**Sådan nulstiller du OneDrive:**

1. Åbn dialogboksen Kør ved at trykke på Windows-tasten og R.
2. Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og tryk på OK. Et kommandovindue vises muligvis kort.
3. Start OneDrive manuelt ved at gå til Start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i søgefeltet, og klik derefter på OneDrive-skrivebordsappen.

Bemærkninger:

- Hvis du havde valgt kun at synkronisere nogle mapper før nulstillingen, er du nødt til at gøre dette igen, når synkroniseringen er fuldført. Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres til din computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)for at få flere   oplysninger.
- Du skal gennemføre dette for dit personlige OneDrive og OneDrive for Business.