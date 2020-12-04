---
title: Fejlfinding af PRT-problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573381"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="6e365-102">Fejlfinding af PRT-problem</span><span class="sxs-lookup"><span data-stu-id="6e365-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="6e365-103">For at alle enheder kan fuldføres ved at blive ved med at blive fuldført, skal den være fuldt registeret og i god stand og kunne erhverve et primært PRT-token.</span><span class="sxs-lookup"><span data-stu-id="6e365-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="6e365-104">Hybrid registreringsprocessen for Azure AD join kræver, at enheder er på et virksomhedsnetværk.</span><span class="sxs-lookup"><span data-stu-id="6e365-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="6e365-105">Det fungerer også over VPN, men der er nogle uhensigtsmæssigheder til det.</span><span class="sxs-lookup"><span data-stu-id="6e365-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="6e365-106">Vi har hørt, at kunder har brug for hjælp til at foretage fejlfinding af hybrid Azure AD join-registreringsprocessen under fjernarbejde-omstændigheder.</span><span class="sxs-lookup"><span data-stu-id="6e365-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="6e365-107">Her er en oversigt over, hvad der sker underliggende under processen.</span><span class="sxs-lookup"><span data-stu-id="6e365-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="6e365-108">**Skybaseret kryds godkendelses miljø (ved hjælp af Azure AD adgangskode-hash synkronisering eller pass-through-godkendelse)**</span><span class="sxs-lookup"><span data-stu-id="6e365-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="6e365-109">Dette registrerings forløb kaldes også "synkroniserings joinforbindelse".</span><span class="sxs-lookup"><span data-stu-id="6e365-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="6e365-110">Windows 10 registrerer en SCP-post, når brugeren logger på enheden.</span><span class="sxs-lookup"><span data-stu-id="6e365-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="6e365-111">Enheden forsøger først at hente lejer oplysninger fra klientside-SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="6e365-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="6e365-112">Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="6e365-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="6e365-113">Hvis den mislykkes, kommunikerer enheden med Active Directory lokalt (AD) for at få lejer oplysninger fra SCP (Service Connection Point).</span><span class="sxs-lookup"><span data-stu-id="6e365-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="6e365-114">Hvis du vil bekræfte SCP, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="6e365-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="6e365-115">Vi anbefaler, at du aktiverer SCP i ANNONCEn og kun bruger klient-SCP til indledende validering.</span><span class="sxs-lookup"><span data-stu-id="6e365-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="6e365-116">Windows 10 forsøger at kommunikere med Azure AD undersystem konteksten for at godkende sig selv over for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e365-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="6e365-117">Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer undersystem kontoen ved hjælp af scriptet til registrering af test af enhed.</span><span class="sxs-lookup"><span data-stu-id="6e365-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="6e365-118">Windows 10 genererer et selvsigneret certifikat og gemmer det under computerobjektet i den lokale annonce.</span><span class="sxs-lookup"><span data-stu-id="6e365-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="6e365-119">Dette forudsætter, at du har en oversigt over domænecontrolleren.</span><span class="sxs-lookup"><span data-stu-id="6e365-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="6e365-120">Et enhedsobjekt, der har et certifikat, bliver synkroniseret til Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6e365-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="6e365-121">Synkroniseringscyklus er som standard hver 30 minut, men det afhænger af konfigurationen af Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6e365-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="6e365-122">Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="6e365-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="6e365-123">På dette trin skal du kunne se emne enheden i tilstanden "afventer" under Device blade i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="6e365-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="6e365-124">Næste gang du logger på Windows 10, bliver registreringen fuldført.</span><span class="sxs-lookup"><span data-stu-id="6e365-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="6e365-125">Hvis du bruger en VPN-forbindelse, og en logoff-logon-proces stopper domæne forbindelsen, kan du udløse registreringen manuelt:</span><span class="sxs-lookup"><span data-stu-id="6e365-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="6e365-126">Udsted en dsregcmd/join lokalt på administrator prompt eller eksternt via PSExec til din PC.</span><span class="sxs-lookup"><span data-stu-id="6e365-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="6e365-127">F. eks. PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="6e365-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="6e365-128">Du kan finde flere oplysninger om problemer med hybrid deltagelse under [fejlfinding af problemer med enheder](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="6e365-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
