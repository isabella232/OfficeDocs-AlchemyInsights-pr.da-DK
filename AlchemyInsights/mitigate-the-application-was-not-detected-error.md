---
title: Afhjælp fejlen Programmet blev ikke fundet
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
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026108"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Afhjælp fejlen "Programmet blev ikke fundet"

Appinstallationsfejlen "Programmet blev ikke registreret efter vellykket installation", som blev blevet rapporteret af Intune, kan forekomme på alle overordnede OS-platforme (Windows, iOS og Android).

De mest almindelige scenarier, der genererer denne fejl, omfatter:

- Appen er blevet opdateret uden for Intune (fra en appstore fra tredjepart) efter den indledende installation. For eksempel kan nogle programmer som f.eks. Google Chrome udføre automatiske opdateringer.
- En bruger har fjernet appen efter den indledende installation.

Hvis du vil løse dette problem, skal du først foretage en gennemgang af de berørte enheder for at fastslå det scenarie, hvor fejlen opstår.

- Hvis appen er blevet opdateret uden for Intune, kan app-installationen indstilles til at ignorere programversionen. Hvis du vil gøre dette, skal du under **Konfiguration af apps > App-oplysninger** indstille **Ignorer app-** version til **Ja**.
- Når du målretter klienten, kan det være relevant at installere programmet som "obligatorisk", og sikre, at den nyeste version installeres.
- Alternativt kan man på iOS-platformen bruge funktionen **Automatiske opdateringer**, der er knyttet til Apple Volume Purchase-programmet, som kan konfigureres til automatisk at opdatere til nye programversioner, når de bliver tilgængelige.

Hvis du vil have mere at vide om fejlfinding af problemer med app-installation, skal du se [Fejlfinding af problemer med app-installation](https://docs.microsoft.com/intune/troubleshoot-app-install).
