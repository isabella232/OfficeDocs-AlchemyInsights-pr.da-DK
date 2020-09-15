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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="fa6cb-102">Få adgang til BitLocker-genoprettelses nøgler</span><span class="sxs-lookup"><span data-stu-id="fa6cb-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="fa6cb-103">Når du konfigurerer BitLocker-indstillinger Intune Endpoint Protection-politik, er det muligt at angive, om BitLocker-genoprettelsesoplysninger skal gemmes i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fa6cb-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="fa6cb-104">Hvis denne indstilling er konfigureret, skal de gemte genoprettelses data være synlige for en Intune-administrator som en del af enhedens postdata i Intune Devices blade på to måder:</span><span class="sxs-lookup"><span data-stu-id="fa6cb-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="fa6cb-105">Enheder-Azure AD-enheder – > "enhed" eller enheder-> alle enheder-> "enhed"-> genoprettelses nøgler</span><span class="sxs-lookup"><span data-stu-id="fa6cb-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="fa6cb-106">Hvis der er administratoradgang til selve enheden, kan du se genoprettelsesnøglen (adgangskode) ved at køre følgende kommando fra en kommandoprompt med administratorrettigheder:</span><span class="sxs-lookup"><span data-stu-id="fa6cb-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="fa6cb-107">Hvis enheden blev krypteret før enrolment i Intune, kan genoprettelsesnøglen være blevet knyttet til "Microsoft-kontoen" (MSA), der bruges til at logge på enheden under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="fa6cb-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="fa6cb-108">Hvis det var tilfældet, skal du få adgang til  https://onedrive.live.com/recoverykey og logge på med den pågældende MSA for at vise de enheder, som genoprettelses nøgler blev gemt for.</span><span class="sxs-lookup"><span data-stu-id="fa6cb-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="fa6cb-109">Hvis enheden blev krypteret som et resultat af konfigurationen via domænebaseret Gruppepolitik, bliver genoprettelses oplysningerne muligvis gemt i det lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fa6cb-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

