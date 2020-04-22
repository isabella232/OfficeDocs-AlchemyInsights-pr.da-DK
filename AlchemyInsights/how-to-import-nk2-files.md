---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759326"
---
# <a name="how-to-import-nk2-files"></a>Sådan importeres .nk2-filer 

Når du starter Microsoft Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365 for første gang, importeres din cache med kaldenavnet (gemt i *filen profilename*.nk2) til en skjult meddelelse i standardmeddelelseslageret.

Hvis du vil importere .nk2-filer til Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365, skal du kontrollere, at .nk2-filen findes i følgende mappe: %appdata%\Microsoft\Outlook

**Bemærk:** Filen .nk2 skal have samme navn som din aktuelle Outlook 2013- eller Outlook 2016-profil. Profilnavnet er som standard "Outlook". FÃ ̧lg disse trin for at kontrollere profilnavnet: 
1. Klik på **Start**, og klik derefter på **Kontrolpanel**.
2. Dobbeltklik på **Mail**.
3. Vælg **Vis profiler**i dialogboksen Mailopsætning .
4. Vælg **Start** > **kørsel**.
5. Skriv *outlook.exe /importnk2*i feltet **Åbn** , og vælg derefter **OK**. 

Når du har importeret .nk2-filen, flettes indholdet af filen til den eksisterende cache med kaldenavne, der er gemt i postkassen.

**Bemærk:** Filen .nk2 omdøbes med filtypenavnet .old, næste gang du starter Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365. Hvis du vil importere .nk2-filen igen, skal du først fjerne filtypenavnet .old.

Yderligere oplysninger finder du i [Importér eller kopiér listen til automatisk fuldførelse til en anden computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).