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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="95283-102">Adgang til BitLocker-genoprettelsesnøgler</span><span class="sxs-lookup"><span data-stu-id="95283-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="95283-103">Når du konfigurerer BitLocker-indstillinger beskyttelsespolitik for Intune Endpoint, er det muligt at definere, om BitLocker-genoprettelsesoplysninger skal gemmes i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="95283-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="95283-104">Hvis denne indstilling er konfigureret, skal de gemte gendannelsesdata være synlige for en Intune-administrator som en del af enhedens postdata i bladet for Intune-enheder på to måder:</span><span class="sxs-lookup"><span data-stu-id="95283-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="95283-105">Enheder – Azure AD-enheder – > "Enhed" ELLER enheder –> Alle enheder – > "Enhed" – > genoprettelsesnøgler</span><span class="sxs-lookup"><span data-stu-id="95283-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="95283-106">Hvis der er administrativ adgang til selve enheden, kan genoprettelsesnøglen (Adgangskode) også ses ved at køre følgende kommando fra en kommandoprompt med administrator administratoradgang:</span><span class="sxs-lookup"><span data-stu-id="95283-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="95283-107">Hvis enheden blev krypteret før tilmelding i Intune, kan genoprettelsesnøglen være knyttet til den "Microsoft-konto" (MSA), der blev brugt til at logge på enheden under OOBE-processen.</span><span class="sxs-lookup"><span data-stu-id="95283-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="95283-108">Hvis det er tilfældet, bør adgang til og logge på med den  https://onedrive.live.com/recoverykey pågældende MSA vise de enheder, for hvilke genoprettelsesnøgler blev gemt.</span><span class="sxs-lookup"><span data-stu-id="95283-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="95283-109">Hvis enheden blev krypteret som et resultat af konfiguration via domænebaseret gruppepolitik, kan genoprettelsesoplysningerne gemmes i det lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="95283-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="95283-110">Hvis du har konfigureret en politik for slutpunktsbeskyttelse til at gemme genoprettelsesnøglen i Azure Active Directory, men nøglen til en bestemt enhed ikke er blevet uploadet, kan du udløse overførslen ved at rotere genoprettelsesnøglen for den pågældende enhed fra MEM-konsollen.</span><span class="sxs-lookup"><span data-stu-id="95283-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="95283-111">Du kan få mere at vide [under Roter BitLocker-genoprettelsesnøgler](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="95283-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

