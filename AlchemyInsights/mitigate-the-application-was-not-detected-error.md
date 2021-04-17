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
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836345"
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
