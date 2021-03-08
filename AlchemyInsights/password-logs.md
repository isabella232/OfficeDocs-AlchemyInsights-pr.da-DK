---
title: Adgangskodelogfiler
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524119"
---
# <a name="password-logs"></a>Adgangskodelogfiler

**Jeg har problemer med at få adgang til overvågningslogfiler til nulstilling af adgangskode**

Hvis du vil foretage fejlfinding af problemer med adgang til overvågningslogfiler til nulstilling af adgangskode, skal du udføre følgende trin:

Sørg for, at du er autoriseret til at få vist overvågningslogfiler. 

Kun følgende roller er godkendt:
 - Global administrator
 - Sikkerhedsadministrator
 - Sikkerhedslæser

**Jeg vil se alle overvågningshændelser for nulstilling af adgangskode fra det tidspunkt, jeg oprindeligt installerede**

Op til 120.000 nulstilling af adgangskode/registreringshændelser gemmes i rapporter for de seneste 30 dage. Denne maksimumgrænse gælder for brugergrænsefladen, når du downloader CSV-filen. Der er 1 million begivenheder tilgængelige via PowerShell.
Du kan finde flere oplysninger i nedenstående links:

- [Selvbetjeningshændelser til nulstilling af adgangskode fra Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Sådan downloader du hurtigt registreringshændelser for nulstilling af adgangskode med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Jeg vil gerne vide mere om rapporteringsfunktioner til nulstilling af adgangskode**

Kontrollér, hvem der registrerer eller nulstiller adgangskoder med Overvågningslogfiler til nulstilling af adgangskode i Azure-portalen under **Brugere og grupper.**
Du kan finde flere oplysninger i følgende links:

- [Oversigt over rapporter til nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Sådan får du vist rapporter om nulstilling af adgangskode i Azure-portalen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Selvbetjeningshændelser til nulstilling af adgangskode fra Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Sådan downloader du hurtigt registreringshændelser for nulstilling af adgangskode med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


