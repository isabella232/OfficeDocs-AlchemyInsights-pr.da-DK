---
title: Jeg bliver blokeret af Betinget adgang med domæne forbundet enhed
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035721"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="f6c83-102">Jeg bliver blokeret af Betinget adgang med domæne forbundet enhed</span><span class="sxs-lookup"><span data-stu-id="f6c83-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="f6c83-103">**Stærkt anbefalede værktøjer**</span><span class="sxs-lookup"><span data-stu-id="f6c83-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="f6c83-104">[Fejlfindingsværktøjet til registrering af enheder](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – det værktøj, der hjælper med at foretage fejlfinding af de mest almindelige problemer med enhedsregistrering.</span><span class="sxs-lookup"><span data-stu-id="f6c83-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="f6c83-105">[Test enhedsregistreringsforbindelsesscript](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – det script, der hjælper med at sikre, at en enhed kan få adgang til enhedsregistreringsslutpunkterne under systemkontoen.</span><span class="sxs-lookup"><span data-stu-id="f6c83-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="f6c83-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – det script, der giver dig mulighed for at søge efter og administrere forældede enheder i dit miljø.</span><span class="sxs-lookup"><span data-stu-id="f6c83-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="f6c83-107">Her er nogle almindelige årsager til, at betinget adgang mislykkes på en enhed, der har tilsluttet sig et domæne (Hybrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f6c83-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="f6c83-108">**Der er ingen Azure AD PRT** på enheden – Du skal sikre dig, at enheden har azure AD Primary Refresh Token (PRT).</span><span class="sxs-lookup"><span data-stu-id="f6c83-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="f6c83-109">Du kan finde flere oplysninger om PRT i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="f6c83-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="f6c83-110">Hvis du vil bekræfte, om du har Azure AD PRT, kan du køre kommandoen på enheden og kontrollere, om `dsregcmd/status` "AzureAdPrt" er lig med "JA".</span><span class="sxs-lookup"><span data-stu-id="f6c83-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="f6c83-111">Hvis "AzureAdPrt" er "NEJ", skal du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="f6c83-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="f6c83-112">Uanset om du har et organisationsnetværk med **AD FS,** og det ikke er tilgængeligt fra dine brugeres hjemmenetværk: I dette tilfælde skal du sikre, at dine "brugernavnmixede" slutpunkter er tilgængelige fra ekstranet.</span><span class="sxs-lookup"><span data-stu-id="f6c83-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="f6c83-113">Hvis din AD FS er bag et VPN, skal du sikre dig, at brugerne opretter forbindelse til VPN og logger på enheden igen.</span><span class="sxs-lookup"><span data-stu-id="f6c83-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="f6c83-114">Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="f6c83-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="f6c83-115">**Om enhedens TPM** er fejlagtig og derfor ikke kan godkende enheden: Kontrollér "tpm.msc" for at se, om tilstanden af TPM er "Klar".</span><span class="sxs-lookup"><span data-stu-id="f6c83-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="f6c83-116">Hvis ikke, skal `dsregcmd/leave` du køre og lade enheden slutte sig til Azure AD igen.</span><span class="sxs-lookup"><span data-stu-id="f6c83-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="f6c83-117">Prøv derefter igen.</span><span class="sxs-lookup"><span data-stu-id="f6c83-117">Then, try again.</span></span> <span data-ttu-id="f6c83-118">Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="f6c83-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="f6c83-119">**Du bruger en tredjepartsidentitetsudbyder, som ikke understøtter WS-Trust protokol.**</span><span class="sxs-lookup"><span data-stu-id="f6c83-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="f6c83-120">Som beskrevet i vores dokumenter kan hybride Azure AD-enheder ikke fungere i dette tilfælde.</span><span class="sxs-lookup"><span data-stu-id="f6c83-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="f6c83-121">Arbejd sammen med din identitetsudbyder for at få support.</span><span class="sxs-lookup"><span data-stu-id="f6c83-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="f6c83-122">Brugere bruger **Chrome-browseren uden Windows 10-konti** eller Office-udvidelsen Chrome bruger ikke automatisk PRT på AAD-enheder, der er forbundet med eller **hybrid-AAD-enheder:** Dette fører til fejl i enhedsbaserede betingede adgangspolitikker, hvor fejlmeddelelsen "Ikke-registreret enhed" vises.</span><span class="sxs-lookup"><span data-stu-id="f6c83-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="f6c83-123">Hvis du vil bruge Chrome-browseren korrekt, skal du installere "Windows 10-konti" eller "Office-udvidelsen til brugernes Chrome-browser" via SCCM eller Intune.</span><span class="sxs-lookup"><span data-stu-id="f6c83-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="f6c83-124">Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="f6c83-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="f6c83-125">Hvis det ikke er muligt at skubbe udvidelsen eksternt, skal du give brugerne besked om, at de manuelt skal installere en af ovennævnte udvidelser for at få adgang til programmer bag enhedsbaseret betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="f6c83-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="f6c83-126">Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="f6c83-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="f6c83-127">Enheden var korrekt hybrid i Azure AD, men den blev ved et uheld slettet eller deaktiveret, enten på grund af synkroniseringsændringer i Azure AD Connect eller fra **Azure-portalen:** Hvis dette sker, genkendes enhedsobjektet ikke længere som en fuldt forbundet enhed, selvom statussen "AzureAdJoined" og "PRT" vises som gyldig på enheden.</span><span class="sxs-lookup"><span data-stu-id="f6c83-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="f6c83-128">Du kan løse dette problem ved at `dsregcmd/leave` køre på de berørte enheder og lade dem slutte sig til Azure AD igen.</span><span class="sxs-lookup"><span data-stu-id="f6c83-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="f6c83-129">Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="f6c83-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="f6c83-130">Hvis dine enheder bruger Windows 10-opdateringen 1809 med VPN/skyproxy og ser problemer med tilstanden "AzureAdPrt" eller en app med SSO-problemer (outlook opretter ikke forbindelse til postkassen, selvom du havde PRT), skal du sikre dig, at du har denne programrettelse [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller den kumulative aprilopdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) for at forhindre PRT-fejl på disse computere.</span><span class="sxs-lookup"><span data-stu-id="f6c83-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















