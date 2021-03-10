---
title: Eksempel på politik for microsoft defender til Office 365-antiphishing
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693243"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Eksempel på politik for microsoft defender til Office 365-antiphishing

Disse indstillinger aktiverer en politik med navnet *Domæne og administrerende direktør.* Denne politik giver både bruger- og domænebeskyttelse mod efterligning og anvender derefter politikken på alle mails, der modtages af brugere på domænet. Først skal du tilføje følgende oplysninger for at oprette politikken:

- **Navn:** Beskrivelse af domæne **og administrerende direktør:** Sikrer, at den administrerende direktør og dit domæne ikke bliver efterligning.
  **Anvendt på:** Vælg **modtagerdomænet er.** Under **En af disse** skal du vælge **Vælg** og derefter vælge et domæne. Vælg **+ Tilføj.** Markér afkrydsningsfeltet ud for navnet på domænet på listen (f.eks. *contoso.com),* og vælg derefter **Tilføj.** Vælg **Udført.**
- Når politikken er oprettet, kan du finjustere politikken ved hjælp af følgende indstillinger:
  - **Tilføj brugere, der skal beskyttes:** I dette eksempel skal du som minimum tilføje den administrerende direktørs mailadresse.
  - **Tilføj domæner, der skal beskyttes:** Tilføj det organisatoriske domæne, der omfatter den administrerende direktørs kontor.
  - **Vælg handlinger:** Hvis mail sendes af en efterligning af en **bruger,** skal du vælge Omdiriger meddelelse til en anden mailadresse og derefter angive mailadressen på sikkerhedsadministratoren (f.eks. *securityadmin@contoso.com).*  Hvis **mail sendes af et efterligningsdomæne, skal** du vælge Sæt meddelelsen i **karantæne.**
  - **Postkasseintelligens:** Denne indstilling vælges som standard, når du opretter en ny antiphishingpolitik. Lad denne indstilling være **tændt for at** få de bedste resultater.
  - **Tilføj afsendere og domæner, der er tillid til:** I dette eksempel skal du ikke definere nogen tilsidesættelser.
- Når du har gennemset dine indstillinger, skal du **vælge Opret denne politik** eller **Gem** efter behov.

Du kan få mere at vide [i Politikker for antiphishing i Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
