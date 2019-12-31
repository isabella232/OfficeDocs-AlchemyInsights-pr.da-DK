---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908704"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bd395-102">Aktivering af BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="bd395-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="bd395-103">Intune Endpoint Protection Policy kan bruges til at konfigurere BitLocker-krypteringsindstillinger for Windows-enheder.</span><span class="sxs-lookup"><span data-stu-id="bd395-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="bd395-104">Du finder flere oplysninger under [Indstillinger for Windows 10 (og nyere) for at beskytte enheder ved hjælp af Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="bd395-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="bd395-105">Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politik.</span><span class="sxs-lookup"><span data-stu-id="bd395-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bd395-106">Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillinger konfigureres.</span><span class="sxs-lookup"><span data-stu-id="bd395-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="bd395-107">Se følgende ofte stillede spørgsmål for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="bd395-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="bd395-108">Du finder oplysninger om fejlfinding af BitLocker-problemer under [fejlfinding af BitLocker-politikker i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="bd395-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="bd395-109">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="bd395-109">**FAQ**</span></span>

 <span data-ttu-id="bd395-110">Sp: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunkts beskyttelsespolitikken?</span><span class="sxs-lookup"><span data-stu-id="bd395-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="bd395-111">A: indstillingerne i Intune Endpoint Protection Policy implementeres ved hjælp af [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="bd395-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="bd395-112">Ikke alle udgaver eller builds af Windows understøtter BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="bd395-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="bd395-113">På dette tidspunkt understøttes følgende Windows-udgaver: Enterprise, Education, mobile, mobile Enterprise og Professional (build 1809 og nyere).</span><span class="sxs-lookup"><span data-stu-id="bd395-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="bd395-114">Q: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS standardindstillinger for krypteringsmetode og cipher styrke (XTS-AES-128), vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?</span><span class="sxs-lookup"><span data-stu-id="bd395-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="bd395-115">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="bd395-115">A: No.</span></span> <span data-ttu-id="bd395-116">Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="bd395-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="bd395-117">**Bemærk:** For enheder, der er tilmeldt autopilot, udløses den automatiske kryptering, som ville forekomme under OOBE, ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEM standarderne.</span><span class="sxs-lookup"><span data-stu-id="bd395-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="bd395-118">Q: Hvis en enhed er krypteret som følge af anvendelsen af Intune politik, vil den blive dekrypteret, når denne politik er fjernet?</span><span class="sxs-lookup"><span data-stu-id="bd395-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="bd395-119">A: fjernelse af krypterings relateret politik resulterer ikke i dekryptering af de drev, der blev konfigureret.</span><span class="sxs-lookup"><span data-stu-id="bd395-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="bd395-120">Spørgsmål: Hvorfor viser Intune-overholdelses politikken, at min enhed ikke har BitLocker aktiveret, selvom den er det?</span><span class="sxs-lookup"><span data-stu-id="bd395-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="bd395-121">A: "BitLocker Enabled"-indstillingen i Intune-overholdelses politikken bruger Windows DHA-klienten (Device Health attestering).</span><span class="sxs-lookup"><span data-stu-id="bd395-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bd395-122">Denne klient måler kun enheds tilstand på starttidspunktet.</span><span class="sxs-lookup"><span data-stu-id="bd395-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="bd395-123">Så hvis en enhed ikke er blevet genstartet, siden BitLocker-krypteringen blev fuldført, rapporterer DHA-klienttjenesten ikke BitLocker som værende aktiv.</span><span class="sxs-lookup"><span data-stu-id="bd395-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 