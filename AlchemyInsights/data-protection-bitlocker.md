---
title: DataProtection-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768811"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="c7204-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="c7204-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="c7204-103">Intune Endpoint Protection-politikken kan bruges til at konfigurere BitLocker-krypteringsindstillinger for Windows-enheder.</span><span class="sxs-lookup"><span data-stu-id="c7204-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="c7204-104">Hvis du vil have mere at vide, skal du se [Windows 10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="c7204-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="c7204-105">Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politikken.</span><span class="sxs-lookup"><span data-stu-id="c7204-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="c7204-106">Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillingerne er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="c7204-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="c7204-107">Du kan finde flere oplysninger i følgende ofte stillede spørgsmål.</span><span class="sxs-lookup"><span data-stu-id="c7204-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="c7204-108">Du kan finde oplysninger om fejlfinding af problemer [med BitLocker under fejlfinding af BitLocker-politikker i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="c7204-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="c7204-109">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="c7204-109">**FAQ**</span></span>

<span data-ttu-id="c7204-110">Sp: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af Endpoint Protection-politikken?</span><span class="sxs-lookup"><span data-stu-id="c7204-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="c7204-111">A: indstillingerne i politikken for Intune Endpoint Protection implementeres ved hjælp af [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="c7204-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="c7204-112">Ikke alle udgaver eller builds til Windows understøtter BitLocker-program til kryptografiske tjenester.</span><span class="sxs-lookup"><span data-stu-id="c7204-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="c7204-113">Sp: Hvordan kan BitLocker aktiveres på enheder uden at kræve slutbruger interaktion?</span><span class="sxs-lookup"><span data-stu-id="c7204-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="c7204-114">A: så længe de nødvendige forudsætninger er opfyldt, er det muligt at aktivere BitLocker "uovervåget kryptering" via Intune.</span><span class="sxs-lookup"><span data-stu-id="c7204-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="c7204-115">Se detaljerne om enheds kravene og eksempel politikindstillinger for at aktivere uovervåget kryptering i følgende dokument: [aktivere BitLocker-kryptering automatisk](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="c7204-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="c7204-116">Sp: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af standardindstillingerne for krypteringsmetode og krypteringsgrad (XTS-AES-128), vil en politik med andre indstillinger automatisk udløse genkryptering af drevet med de nye indstillinger?</span><span class="sxs-lookup"><span data-stu-id="c7204-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="c7204-117">Sv.: Nej.</span><span class="sxs-lookup"><span data-stu-id="c7204-117">A: No.</span></span> <span data-ttu-id="c7204-118">Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="c7204-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="c7204-119">**Bemærk:** For enheder, der er tilmeldt autopilot, udløses den automatiske kryptering, der skulle forekomme under OOBE, ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEMETS standardindstillinger.</span><span class="sxs-lookup"><span data-stu-id="c7204-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="c7204-120">Sp: Hvis en enhed krypteres som et resultat af anvendelsen af Intune-politikken, dekrypteres den, når politikken fjernes?</span><span class="sxs-lookup"><span data-stu-id="c7204-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="c7204-121">A: fjernelse af krypterings relateret politik medfører ikke dekryptering af de drev, der er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="c7204-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="c7204-122">Sp: Hvorfor viser det, at min enhed ikke har BitLocker aktiveret, selvom min enhed ikke har BitLocker aktiveret, selvom det er?</span><span class="sxs-lookup"><span data-stu-id="c7204-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="c7204-123">A: indstillingen "BitLocker-aktiveret" i aftale overholdelses politik anvender Windows-DHA (Device Health attestation-klient).</span><span class="sxs-lookup"><span data-stu-id="c7204-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="c7204-124">Denne klient måler kun enhedstilstanden på starttidspunktet.</span><span class="sxs-lookup"><span data-stu-id="c7204-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="c7204-125">Hvis en enhed ikke er blevet genstartet, siden BitLocker-kryptering blev fuldført, vil DHA-klienttjenesten ikke rapportere BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="c7204-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 