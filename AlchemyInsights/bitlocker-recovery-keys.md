---
title: BitLocker-genoprettelsesnøgler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820280"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Adgang til BitLocker-genoprettelsesnøgler

Når du konfigurerer BitLocker-indstillinger beskyttelsespolitik for Intune Endpoint, er det muligt at definere, om BitLocker-genoprettelsesoplysninger skal gemmes i Azure Active Directory.

Hvis denne indstilling er konfigureret, skal de gemte gendannelsesdata være synlige for en Intune-administrator som en del af enhedens postdata i bladet for Intune-enheder på to måder:

Enheder – Azure AD-enheder – > "Enhed" ELLER enheder –> Alle enheder – > "Enhed" – > genoprettelsesnøgler

Hvis der er administrativ adgang til selve enheden, kan genoprettelsesnøglen (Adgangskode) også ses ved at køre følgende kommando fra en kommandoprompt med administrator administratoradgang:

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
Hvis enheden blev krypteret før tilmelding i Intune, kan genoprettelsesnøglen være knyttet til den "Microsoft-konto" (MSA), der blev brugt til at logge på enheden under OOBE-processen. Hvis det er tilfældet, bør adgang til og logge på med den  https://onedrive.live.com/recoverykey pågældende MSA vise de enheder, for hvilke genoprettelsesnøgler blev gemt.
 
Hvis enheden blev krypteret som et resultat af konfiguration via domænebaseret gruppepolitik, kan genoprettelsesoplysningerne gemmes i det lokale Active Directory.

Hvis du har konfigureret en politik for slutpunktsbeskyttelse til at gemme genoprettelsesnøglen i Azure Active Directory, men nøglen til en bestemt enhed ikke er blevet uploadet, kan du udløse overførslen ved at rotere genoprettelsesnøglen for den pågældende enhed fra MEM-konsollen. Du kan få mere at vide [under Roter BitLocker-genoprettelsesnøgler](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

