---
title: Tilbageførsel af adgangskode virker ikke
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243288"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="7aafe-102">Tilbageførsel af adgangskode virker ikke</span><span class="sxs-lookup"><span data-stu-id="7aafe-102">Password Writeback is not working</span></span>

<span data-ttu-id="7aafe-103">**Jeg har problemer med at konfigurere tilbageførsel af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="7aafe-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="7aafe-104">Tilbageførsel af adgangskode er en premium-funktion.</span><span class="sxs-lookup"><span data-stu-id="7aafe-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="7aafe-105">Sørg for, at du forstår licenskravene:</span><span class="sxs-lookup"><span data-stu-id="7aafe-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="7aafe-106">Du skal have mindst én licens tildelt i organisationen</span><span class="sxs-lookup"><span data-stu-id="7aafe-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="7aafe-107">**Kun brugere i skyen** – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="7aafe-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="7aafe-108">**Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="7aafe-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="7aafe-109">Du kan få mere at vide om licenskrav under [Licenskrav til nulstilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) af adgangskode til Azure AD via selvbetjening</span><span class="sxs-lookup"><span data-stu-id="7aafe-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="7aafe-110">Du har mindst én administratorkonto og én testbrugerkonto med en af de relevante licenser.</span><span class="sxs-lookup"><span data-stu-id="7aafe-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="7aafe-111">Du skal oprette forbindelse mellem Azure AD Connect og Den primære domænecontroller-emulator, for at tilbageførsel af adgangskode kan fungere.</span><span class="sxs-lookup"><span data-stu-id="7aafe-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="7aafe-112">Du kan konfigurere Azure AD Connect til at bruge en  primær domænecontroller ved at højreklikke på egenskaberne for Active Directory-synkroniseringsforbindelse og derefter vælge **konfigurer katalogpartitioner.**</span><span class="sxs-lookup"><span data-stu-id="7aafe-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="7aafe-113">Derfra skal du kigge efter **sektionen forbindelsesindstillinger** for domænecontrolleren og markere afkrydsningsfeltet med titlen brug **kun foretrukne domænecontrollere.**</span><span class="sxs-lookup"><span data-stu-id="7aafe-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="7aafe-114">Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Connect stadig nå ud til PDC for at få tilbageførsel af adgangskode.</span><span class="sxs-lookup"><span data-stu-id="7aafe-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="7aafe-115">Nulstilling af adgangskode er konfigureret og aktiveret i din lejer.</span><span class="sxs-lookup"><span data-stu-id="7aafe-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="7aafe-116">Du kan finde flere oplysninger i [Aktivere brugere til at nulstille deres Azure AD-adgangskoder.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="7aafe-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="7aafe-117">Sørg for, at den administratorkonto, der bruges til at aktivere tilbageførsel af adgangskode, er en skybaseret administratorkonto (oprettet i Azure AD ikke i det lokale AD)</span><span class="sxs-lookup"><span data-stu-id="7aafe-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="7aafe-118">Du har en lokal enkelt- eller flerskovs-AD-installation, der kører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de nyeste servicepakker installeret</span><span class="sxs-lookup"><span data-stu-id="7aafe-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="7aafe-119">Du har Azure AD Connect-værktøjet installeret, og du har forberedt dit AD-miljø til synkronisering med skyen.</span><span class="sxs-lookup"><span data-stu-id="7aafe-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="7aafe-120">Før du tester tilbageførsel af adgangskode, skal du først fuldføre en fuld import og fuld synkronisering fra både AD og Azure AD i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7aafe-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="7aafe-121">Du kan få mere at vide ved at se, hvordan [du kan udføre en fuld synkronisering og fuld import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="7aafe-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="7aafe-122">**Jeg har et problem med forbindelse til tilbageførsel af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="7aafe-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="7aafe-123">Download og aktivér den nyeste version af [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="7aafe-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="7aafe-124">Firewallkonfiguration: Azure AD Connect-værktøjet (1.1.443 og derover) skal have **udgående HTTPS-adgang** for at:</span><span class="sxs-lookup"><span data-stu-id="7aafe-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="7aafe-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7aafe-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="7aafe-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="7aafe-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="7aafe-127">Tillad, at inaktive forbindelser bevares i mindst 2-3 minutter</span><span class="sxs-lookup"><span data-stu-id="7aafe-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="7aafe-128">**Jeg har stadig problemer med tilbageførsel af adgangskode**</span><span class="sxs-lookup"><span data-stu-id="7aafe-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="7aafe-129">Hvis du stadig har problemer, kan du prøve at deaktivere og genaktivere tjenesten til tilbageførsel af adgangskode i Azure AD Connect-værktøjet</span><span class="sxs-lookup"><span data-stu-id="7aafe-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="7aafe-130">Du kan få mere at vide ved at [se, hvordan du deaktiverer og genaktiverer tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="7aafe-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
