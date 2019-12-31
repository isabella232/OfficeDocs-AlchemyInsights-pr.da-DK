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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="59ad3-102">Adgang til BitLocker-genoprettelsesnøgler</span><span class="sxs-lookup"><span data-stu-id="59ad3-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="59ad3-103">Når du konfigurerer BitLocker-indstillinger Intune Endpoint Protection Policy, er det muligt at definere, om BitLocker-genoprettelsesoplysninger skal lagres i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59ad3-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="59ad3-104">Hvis denne indstilling er konfigureret, skal de lagrede genoprettelses data være synlige for en Intune-administrator som en del af enhedens postdata i Intune Devices blade på to måder:</span><span class="sxs-lookup"><span data-stu-id="59ad3-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="59ad3-105">Enheder-Azure AD-enheder-> "enhed" eller enheder-> alle enheder-> "enhed"-> genoprettelsesnøgler</span><span class="sxs-lookup"><span data-stu-id="59ad3-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="59ad3-106">Alternativt, selv om der er administrativ adgang hen til den indretning sig, den opsving nøglen (password) kan set af løb den næste befale af en ophøjet befale lynhurtig:</span><span class="sxs-lookup"><span data-stu-id="59ad3-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="59ad3-107">Hvis enheden blev krypteret, før du tilmeldingen i Intune, kan genoprettelsesnøglen være knyttet til den "Microsoft-konto" (MSA), der bruges til at logge på enheden under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="59ad3-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="59ad3-108">Hvis det var tilfældet, skulle adgang https://onedrive.live.com/recoverykey til og login med denne MSA vise de enheder, for hvilke genoprettelsesnøgler blev gemt.</span><span class="sxs-lookup"><span data-stu-id="59ad3-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="59ad3-109">Hvis enheden blev krypteret som et resultat af konfigurationen via en domænebaseret Gruppepolitik, kan genoprettelsesoplysningerne blive gemt i det lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59ad3-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

