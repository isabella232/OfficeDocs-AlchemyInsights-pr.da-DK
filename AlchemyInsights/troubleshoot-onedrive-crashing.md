---
title: Fejlfinding af OneDrive-nedbrud
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664992"
---
# <a name="troubleshoot-onedrive-crashes"></a>Fejlfinding af OneDrive-nedbrud

Hvis OneDrive gentagne gange går ned, kan du prøve disse trin til fejlfinding:

**Kontrollér, at registreringsdatabasenøgler ikke er angivet:**

1. Ved hjælp af registrerings Editor skal du gå til HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC er angivet og indstillet til 1, skal du åbne nøglen og ændre værdien til 0.
3. Start OneDrive manuelt ved at gå til start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), Skriv OneDrive i søgefeltet, og klik derefter på OneDrive-programmet på computeren.

**Nulstil OneDrive:**

Vejledningen

- Nulstilling af OneDrive afbryder forbindelsen til alle dine eksisterende synkroniseringsforbindelser (herunder dit personlige OneDrive, hvis det er konfigureret).
- Du mister ikke filer eller data ved at nulstille OneDrive på computeren.

**Sådan nulstilles OneDrive:**

1. Åbn en kørsels dialogboks ved at trykke på Windows-tasten og R.
2. Skriv% localappdata% \Microsoft\OneDrive\onedrive.exe/reset, og tryk på OK. Et kommandovindue vises muligvis kortvarigt.
3. Start OneDrive manuelt ved at gå til start ![Tryk på Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), Skriv OneDrive i søgefeltet, og klik derefter på OneDrive-programmet på computeren.

Vejledningen

- Hvis du har valgt kun at synkronisere nogle mapper før nulstillingen, skal du gøre det igen, når synkroniseringen er fuldført. Læs [Vælg, hvilke OneDrive-mapper der skal synkroniseres med din computer for at](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   få flere oplysninger.
- Du skal fuldføre dette for dit personlige OneDrive og OneDrive for Business.