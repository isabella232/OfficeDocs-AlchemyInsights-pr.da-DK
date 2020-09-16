---
title: Afhjælp fejlen Programmet blev ikke fundet
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666972"
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
