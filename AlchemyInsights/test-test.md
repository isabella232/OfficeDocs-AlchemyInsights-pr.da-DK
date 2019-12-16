---
title: Vilkår, som mangler i SharePoint Online term store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053507"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="25f37-102">Aktivering af BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="25f37-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="25f37-103">Intune Endpoint Protection Policy kan bruges til at konfigurere Boitlocker krypteringsindstillinger for Windows-enheder som beskrevet i: Windows10 (og nyere) indstillinger for at beskytte enheder ved hjælp af Intune</span><span class="sxs-lookup"><span data-stu-id="25f37-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="25f37-104">Du skal være opmærksom på, at mange nyere enheder, der kører Windows 10, understøtter automatisk BitLocker-kryptering, som udløses uden anvendelse af MDM-politik.</span><span class="sxs-lookup"><span data-stu-id="25f37-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="25f37-105">Dette kan påvirke anvendelsen af politikken, hvis ikke-standardindstillingerne konfigureres.</span><span class="sxs-lookup"><span data-stu-id="25f37-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="25f37-106">Se ofte stillede spørgsmål for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="25f37-106">See FAQ for more detail.</span></span>


<span data-ttu-id="25f37-107">FAQ  Q: hvilke udgaver af Windows understøtter enhedskryptering ved hjælp af slutpunkts beskyttelsespolitikken?</span><span class="sxs-lookup"><span data-stu-id="25f37-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="25f37-108"> A: indstillingerne i Intune Endpoint Protection Policy implementeres ved hjælp af BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="25f37-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="25f37-109">Ikke alle udgaver eller builds af Windows understøtter BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="25f37-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="25f37-110">På dette tidspunkt Windows-udgaver: Enterprise; Uddannelse, mobil, mobil virksomhed og professionel (fra Build 1809 og fremefter) understøttes.</span><span class="sxs-lookup"><span data-stu-id="25f37-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="25f37-111">Q: Hvis en enhed allerede er krypteret med BitLocker ved hjælp af OS standardindstillinger for krypteringsmetode og cipher styrke (XTS-AES-128) vil anvende en politik med forskellige indstillinger automatisk udløse re-kryptering af drevet med de nye indstillinger?</span><span class="sxs-lookup"><span data-stu-id="25f37-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="25f37-112">A: Nej.</span><span class="sxs-lookup"><span data-stu-id="25f37-112">A: No.</span></span> <span data-ttu-id="25f37-113">For at anvende de nye cipher indstillinger drevet skal først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="25f37-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="25f37-114">Bemærkning til enheder, der er tilmeldt med autopilot den automatiske kryptering, der ville opstå under OOBE, udløses ikke, før Intune-politikken evalueres, hvilket gør det muligt at bruge de politikbaserede indstillinger i stedet for OPERATIVSYSTEM standarderne</span><span class="sxs-lookup"><span data-stu-id="25f37-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="25f37-115">Q hvis en enhed er krypteret som følge af anvendelsen af Intune politik vil den blive dekrypteret, når denne politik er fjernet?</span><span class="sxs-lookup"><span data-stu-id="25f37-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="25f37-116">A: fjernelse af krypterings relaterede politik ikke resulterer i dekryptering af de drev, der blev konfigureret.</span><span class="sxs-lookup"><span data-stu-id="25f37-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="25f37-117">Spørgsmål: Hvorfor viser Intune Compliance Policy, at min enhed ikke har "BitLocker Enabled", men det er det?</span><span class="sxs-lookup"><span data-stu-id="25f37-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="25f37-118">A: indstillingen "BitLocker-aktiveret" i Intune-overholdelses politik bruger Windows DHA-klienten (Device Health attestering).</span><span class="sxs-lookup"><span data-stu-id="25f37-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="25f37-119">Denne klient måler kun enheds tilstand på starttidspunktet.</span><span class="sxs-lookup"><span data-stu-id="25f37-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="25f37-120">Så hvis en enhed ikke er blevet genstartet, da BitLocker-kryptering blev fuldført, rapporterer DHA-klienttjenesten ikke BitLocker som værende aktiv.</span><span class="sxs-lookup"><span data-stu-id="25f37-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>