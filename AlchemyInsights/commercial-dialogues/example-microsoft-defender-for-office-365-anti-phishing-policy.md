---
title: Eksempel på Microsoft Defender Office 365 antiphishing-politik
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035000"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Eksempel på Microsoft Defender Office 365 antiphishing-politik

Disse indstillinger aktiverer en politik med navnet *Domæne og administrerende direktør.* Denne politik giver både bruger- og domænebeskyttelse mod efterligning og anvender derefter politikken på alle mails, der modtages af brugere i domænet. Først skal du tilføje følgende oplysninger for at oprette politikken:

- **Navn:** Beskrivelse af domæne **og administrerende** direktør: Sikrer, at den administrerende direktør og dit domæne ikke repræsenteres.
  **Anvendt på:** Vælg **modtagerdomænet er**. Under **Alle disse skal** du vælge **Vælg** og derefter vælge et domæne. Vælg **+ Tilføj.** Markér afkrydsningsfeltet ud for navnet på domænet på listen (f.eks. *contoso.com*), og vælg derefter **Tilføj**. Vælg **Udført**.
- Når politikken er oprettet, kan du finjustere politikken ved hjælp af følgende indstillinger:
  - **Tilføj brugere, der skal beskyttes:** I dette eksempel skal du som minimum tilføje den administrerende direktørs mailadresse.
  - **Tilføj domæner, der skal beskyttes:** Tilføj det organisatoriske domæne, der omfatter den administrerende direktørs kontor.
  - **Vælg handlinger:** **Hvis** mail sendes af en efterligning af en bruger, skal du vælge Omdiriger meddelelse til en anden mailadresse **og** derefter angive mailadressen på sikkerhedsadministratoren (f.eks. *securityadmin@contoso.com).* Hvis **mail sendes af et efterligning af et domæne, skal** du vælge Sæt meddelelsen i **karantæne.**
  - **Postkasseintelligens:** Denne indstilling vælges som standard, når du opretter en ny antiphishingpolitik. Lad denne indstilling være **til for** at opnå de bedste resultater.
  - **Tilføj afsendere og domæner, der er tillid til:** I dette eksempel skal du ikke definere nogen tilsidesættelser.
- Når du har gennemset dine indstillinger, skal du **vælge Opret denne politik** eller **Gem**, efter behov.

Du kan få mere at vide [under Antiphishing-politikker i Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
