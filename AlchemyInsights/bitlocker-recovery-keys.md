---
title: BitLocker-genoprettelsesnøgler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505062"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Adgang til BitLocker-genoprettelsesnøgler

Når du konfigurerer Indstillinger for BitLocker, er det muligt at definere, om BitLocker-genoprettelsesoplysninger skal gemmes i Azure Active Directory.

Hvis denne indstilling er konfigureret, skal de gemte gendannelsesdata være synlige for en Intune-administrator som en del af enhedens postdata i bladet for Intune-enheder på to måder:

Enheder – Azure AD-enheder – > "Enhed" ELLER enheder –> Alle enheder – > "Enhed" – > genoprettelsesnøgler

Hvis der er administrativ adgang til selve enheden, kan genoprettelsesnøglen (adgangskode) også ses ved at køre følgende kommando fra en kommandoprompt med administrator administrator:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Hvis enheden blev krypteret før tilmelding i Intune, kan genoprettelsesnøglen være knyttet til den "Microsoft-konto" (MSA), der blev brugt til at logge på enheden under OOBE-processen. Hvis det var tilfældet, skulle adgang til og logge på med den pågældende MSA vise de  https://onedrive.live.com/recoverykey enheder, som genoprettelsesnøgler blev gemt på.
 
Hvis enheden blev krypteret som et resultat af konfiguration via domænebaseret gruppepolitik, kan genoprettelsesoplysningerne blive gemt i det lokale Active Directory.

Hvis du har konfigureret en politik for slutpunktsbeskyttelse til at gemme genoprettelsesnøglen i Azure Active Directory, men nøglen til en bestemt enhed ikke er blevet overført, kan du udløse overførslen ved at rotere genoprettelsesnøglen for den pågældende enhed fra MEM-konsollen. Du kan få mere at vide [under Roter BitLocker-genoprettelsesnøgler.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

