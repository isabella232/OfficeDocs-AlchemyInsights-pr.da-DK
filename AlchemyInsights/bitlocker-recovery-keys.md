---
title: BitLocker-genoprettelses nøgler
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685880"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Få adgang til BitLocker-genoprettelses nøgler

Når du konfigurerer BitLocker-indstillinger Intune Endpoint Protection-politik, er det muligt at angive, om BitLocker-genoprettelsesoplysninger skal gemmes i Azure Active Directory.

Hvis denne indstilling er konfigureret, skal de gemte genoprettelses data være synlige for en Intune-administrator som en del af enhedens postdata i Intune Devices blade på to måder:

Enheder-Azure AD-enheder – > "enhed" eller enheder-> alle enheder-> "enhed"-> genoprettelses nøgler

Hvis der er administratoradgang til selve enheden, kan du se genoprettelsesnøglen (adgangskode) ved at køre følgende kommando fra en kommandoprompt med administratorrettigheder:

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
Hvis enheden blev krypteret før enrolment i Intune, kan genoprettelsesnøglen være blevet knyttet til "Microsoft-kontoen" (MSA), der bruges til at logge på enheden under OOBE-processen. Hvis det var tilfældet, skal du få adgang til  https://onedrive.live.com/recoverykey og logge på med den pågældende MSA for at vise de enheder, som genoprettelses nøgler blev gemt for.
 
Hvis enheden blev krypteret som et resultat af konfigurationen via domænebaseret Gruppepolitik, bliver genoprettelses oplysningerne muligvis gemt i det lokale Active Directory.
 

