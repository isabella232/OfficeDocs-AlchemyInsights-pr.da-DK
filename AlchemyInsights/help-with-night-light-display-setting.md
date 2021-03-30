---
title: Hjælp til skærmindstillingen nattelys
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404397"
---
# <a name="help-with-the-night-light-display-setting"></a>Hjælp til skærmindstillingen nattelys

Hvis du vil have mere at vide om indstillinger for nattid, skal du se Angive [din skærm til nattid i Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Hvis indstillingerne for nattelys er nedtonet i Indstillinger, skal du kontrollere din skærmdriver: 

1. Klik på søgefeltet på proceslinjen, og **skriv Enhedshåndtering,** og vælg **derefter Enhedshåndtering** i søgeresultaterne.
1. Udvid **skærmkort.** 

Funktionen nattelys er desværre ikke tilgængelig, hvis enheden bruger en DisplayLink-driver eller en Basic Display-driver.

Funktionen nattelys gør brug af den nyeste grafikteknologi, så det kan være nødvendigt at opdatere skærmdriveren:  

- Søg efter opdateringer ved at gå til **Opdatering**  >  **af**  >  **startindstillinger &**  >  **Sikkerhedsopdatering til Windows Update** for at søge efter  >  **opdateringer.**  

ELLER

- Besøg hardwareproducentens supportwebsted for manuelt at downloade og installere de nyeste skærmdrivere.

## <a name="reset-night-light-in-the-registry"></a>Nulstil nattelys i registreringsdatabasen

Hvis det ikke virker at opdatere din skærmdriver, skal du muligvis nulstille nattelys i registreringsdatabasen.  

**Advarsel!** Dette fejlfindingstrin anbefales kun til erfarne brugere. Der kan forekomme alvorlige problemer, hvis du redigerer registreringsdatabasen forkert. For yderligere beskyttelse skal du sikkerhedskopiering af registreringsdatabasen, før du redigerer den, så du kan gendanne den, hvis der opstår problemer.

1. Skriv **regedit i søgefeltet,** og vælg derefter **Registreringseditor** i søgeresultaterne.

1. Gå til følgende registreringsdatabasenøgle: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksportér og slet derefter følgende undernøgle:$$windows.data.bluelightreangivelse.bluelightrestate

1. Eksportér og slet derefter følgende undernøgle:$$windows.data.bluelightrerettelse.settings

1. Genstart Windows, og kontrollér, om indstillingerne for nattelys er tilgængelige.


