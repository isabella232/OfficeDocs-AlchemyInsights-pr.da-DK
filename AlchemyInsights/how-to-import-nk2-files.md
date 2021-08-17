---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043200"
---
# <a name="how-to-import-nk2-files"></a>Sådan importerer du .nk2-filer 

Når du starter Microsoft Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365 for første gang, importeres din kaldenavnscache (gemt i .nk2-filen med profilnavnet) til en skjult meddelelse i dit standardmeddelelseslager.

Hvis du vil importere .nk2-filer til Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365, skal du sørge for, at .nk2-filen er i følgende mappe: %appdata%\Microsoft\Outlook

**Bemærk!**.nk2-filen skal have samme navn som den aktuelle Outlook 2013 eller Outlook 2016 profil. Profilnavnet er som standard "Outlook". Hvis du vil kontrollere profilnavnet, skal du følge disse trin: 
1. Klik **på Start**, og klik derefter på **Kontrolpanel.**
2. Dobbeltklik på **Mail**.
3. I dialogboksen Konfiguration af mail skal du vælge **Vis profiler**.
4. Vælg **Start**  >  **Kør.**
5. I feltet **Åbn** skal du skrive *outlook.exe /importnk2* og derefter vælge **OK.** 

Når du har importeret .nk2-filen, flettes indholdet af filen ind i den eksisterende kaldenavnscache, der er gemt i din postkasse.

**Bemærk!**.nk2-filen omdøbes med filtypenavnet .old, næste gang du starter Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook til Microsoft 365. Hvis du vil importere .nk2-filen igen, skal du først fjerne filtypenavnet .old.

Du kan finde flere oplysninger [i Importere eller kopiere listen til autofuldfør til en anden computer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)