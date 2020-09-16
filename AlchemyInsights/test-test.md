---
title: Manglende termer fra SharePoint Online-ordbank
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750445"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="8c72b-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="8c72b-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="8c72b-103">Intune Endpoint Protection-politikken kan bruges til at konfigurere Boitlocker-krypteringsindstillinger for Windows-enheder som beskrevet i: Windows10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune</span><span class="sxs-lookup"><span data-stu-id="8c72b-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="8c72b-104">Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, der udløses uden anvendelse af MDM-politikken.</span><span class="sxs-lookup"><span data-stu-id="8c72b-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="8c72b-105">Dette kan påvirke anvendelsen af politik, hvis ikke-standardindstillingerne er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="8c72b-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="8c72b-106">Du kan finde flere oplysninger under ofte stillede spørgsmål.</span><span class="sxs-lookup"><span data-stu-id="8c72b-106">See FAQ for more detail.</span></span>


<span data-ttu-id="8c72b-107">Ofte stillede spørgsmål   : hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af Endpoint Protection-politikken?</span><span class="sxs-lookup"><span data-stu-id="8c72b-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="8c72b-108"> A: indstillingerne i politikken for Intune Endpoint Protection implementeres ved hjælp af BitLocker-CSP.</span><span class="sxs-lookup"><span data-stu-id="8c72b-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="8c72b-109">Ikke alle udgaver eller builds af Windows understøtter BitLocker-program til kryptografiske tjenester. 
     </span><span class="sxs-lookup"><span data-stu-id="8c72b-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="8c72b-110">På nuværende tidspunkt Windows-udgaver: Enterprise; Education, mobile, mobil virksomhed og Professional (fra Build 1809) understøttes.</span><span class="sxs-lookup"><span data-stu-id="8c72b-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="8c72b-111">Sp: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af standardindstillingerne for krypteringsmetode og krypteringsgrad (XTS-AES-128), anvender en politik med andre indstillinger automatisk kryptering af drevet med de nye indstillinger?</span><span class="sxs-lookup"><span data-stu-id="8c72b-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="8c72b-112">Sv.: Nej.</span><span class="sxs-lookup"><span data-stu-id="8c72b-112">A: No.</span></span> <span data-ttu-id="8c72b-113">Hvis du vil anvende de nye krypteringsindstillinger, skal drevet først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="8c72b-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="8c72b-114">Bemærk! de enheder, der tilmeldes med autopilot, automatisk kryptering, der skulle forekomme under OOBE, udløses ikke, før Intune-politikken evalueres, hvilket gør det muligt for de politikbaserede indstillinger, der skal bruges i stedet for OPERATIVSYSTEMETS standarder</span><span class="sxs-lookup"><span data-stu-id="8c72b-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="8c72b-115">SP hvis en enhed krypteres som et resultat af anvendelsen af Intune-politikken, dekrypteres den, når politikken fjernes?</span><span class="sxs-lookup"><span data-stu-id="8c72b-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="8c72b-116">A: fjernelse af krypterings relateret politik medfører ikke dekryptering af de drev, der er konfigureret.</span><span class="sxs-lookup"><span data-stu-id="8c72b-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="8c72b-117">Sp: Hvorfor viser politikken for kompatibilitets overholdelse, at min enhed ikke har "BitLocker aktiveret", men det er?</span><span class="sxs-lookup"><span data-stu-id="8c72b-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="8c72b-118">A: indstillingen "BitLocker-aktiveret" i overholdelses politik for Intune anvender Windows-DHA (Device Health attestation).</span><span class="sxs-lookup"><span data-stu-id="8c72b-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="8c72b-119">Denne klient måler kun enhedstilstanden på starttidspunktet.</span><span class="sxs-lookup"><span data-stu-id="8c72b-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="8c72b-120">Hvis en enhed ikke er blevet genstartet, siden BitLocker-kryptering blev fuldført, vil DHA-klienttjenesten ikke rapportere BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="8c72b-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>