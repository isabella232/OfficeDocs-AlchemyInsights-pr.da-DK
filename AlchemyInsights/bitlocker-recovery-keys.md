---
title: BitLocker-genoprettelsesnøgler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908809"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Adgang til BitLocker-genoprettelsesnøgler

Når du konfigurerer BitLocker-indstillinger Intune Endpoint Protection Policy, er det muligt at definere, om BitLocker-genoprettelsesoplysninger skal lagres i Azure Active Directory.

Hvis denne indstilling er konfigureret, skal de lagrede genoprettelses data være synlige for en Intune-administrator som en del af enhedens postdata i Intune Devices blade på to måder:

Enheder-Azure AD-enheder-> "enhed" eller enheder-> alle enheder-> "enhed"-> genoprettelsesnøgler

Alternativt, selv om der er administrativ adgang hen til den indretning sig, den opsving nøglen (password) kan set af løb den næste befale af en ophøjet befale lynhurtig:

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
Hvis enheden blev krypteret, før du tilmeldingen i Intune, kan genoprettelsesnøglen være knyttet til den "Microsoft-konto" (MSA), der bruges til at logge på enheden under OOBE-processen. Hvis det var tilfældet, skulle adgang https://onedrive.live.com/recoverykey til og login med denne MSA vise de enheder, for hvilke genoprettelsesnøgler blev gemt.
 
Hvis enheden blev krypteret som et resultat af konfigurationen via en domænebaseret Gruppepolitik, kan genoprettelsesoplysningerne blive gemt i det lokale Active Directory.
 

