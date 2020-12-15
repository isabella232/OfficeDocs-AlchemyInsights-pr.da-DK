---
title: Enhed i afventende tilstand
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677569"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="82178-102">Enhed i afventende tilstand</span><span class="sxs-lookup"><span data-stu-id="82178-102">Device in pending state</span></span>

<span data-ttu-id="82178-103">**Forudsætninger**</span><span class="sxs-lookup"><span data-stu-id="82178-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="82178-104">Hvis du konfigurerer enheds registreringer for første gang, skal du sørge for, at du har gennemgået [Introduktion til Enhedsadministration i Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , der hjælper dig med at få enheder under kontrol af Azure ad.</span><span class="sxs-lookup"><span data-stu-id="82178-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="82178-105">Hvis du registrerer enheder i Azure AD direkte og tilmelder dem til Intune, skal du sikre dig, at du har [konfigureret Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , og at [licensen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) er placeret først.</span><span class="sxs-lookup"><span data-stu-id="82178-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="82178-106">Sørg for, at du har tilladelse til at udføre handlinger i Azure AD og i det lokale-annonce.</span><span class="sxs-lookup"><span data-stu-id="82178-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="82178-107">Kun en global administrator i Azure AD kan administrere indstillinger for enheds registreringer.</span><span class="sxs-lookup"><span data-stu-id="82178-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="82178-108">Hvis du er ved at konfigurere automatisk registrering i dit lokale Active Directory, skal du desuden være administrator af Active Directory og AD FS (hvis relevant).</span><span class="sxs-lookup"><span data-stu-id="82178-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="82178-109">Den hybride tilmelding til Azure AD join kræver, at der er enheder i virksomhedens netværk.</span><span class="sxs-lookup"><span data-stu-id="82178-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="82178-110">Det fungerer også over VPN, men der er nogle uhensigtsmæssigheder til det.</span><span class="sxs-lookup"><span data-stu-id="82178-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="82178-111">Vi har hørt, at kunder har brug for hjælp til fejlfinding i forbindelse med den hybride tilmelding til Azure AD join under fjernarbejde-omstændigheder.</span><span class="sxs-lookup"><span data-stu-id="82178-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="82178-112">**Skybaseret kryds godkendelses miljø (ved hjælp af Azure AD adgangskode-hash synkronisering eller pass-through-godkendelse)**</span><span class="sxs-lookup"><span data-stu-id="82178-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="82178-113">Dette registrerings forløb kaldes også "synkroniserings joinforbindelse".</span><span class="sxs-lookup"><span data-stu-id="82178-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="82178-114">Her er en oversigt over, hvad der sker under registreringsprocessen:</span><span class="sxs-lookup"><span data-stu-id="82178-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="82178-115">Windows 10 registrerer Service Connection Point-posten (SCP), når brugeren logger på enheden.</span><span class="sxs-lookup"><span data-stu-id="82178-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="82178-116">Enheden forsøger først at hente lejer oplysninger fra klientside-SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="82178-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="82178-117">Du kan finde flere oplysninger i afsnittet [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="82178-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="82178-118">Hvis den mislykkes, kommunikerer enheden med Active Directory lokalt for at få lejer oplysninger fra SCP.</span><span class="sxs-lookup"><span data-stu-id="82178-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="82178-119">Hvis du vil bekræfte SCP, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="82178-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="82178-120">Vi anbefaler, at du aktiverer SCP i Active Directory og kun bruger klient-SCP til indledende validering.</span><span class="sxs-lookup"><span data-stu-id="82178-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="82178-121">Windows 10 forsøger at kommunikere med Azure AD undersystem konteksten for at godkende sig selv over for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82178-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="82178-122">Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer undersystem kontoen ved hjælp af [scriptet til registrering af test af enhed](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="82178-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="82178-123">Windows 10 genererer selvsigneret certifikat og gemmer det under computerobjektet i Active Directory lokalt.</span><span class="sxs-lookup"><span data-stu-id="82178-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="82178-124">Dette forudsætter, at du har en oversigt over domænecontrolleren.</span><span class="sxs-lookup"><span data-stu-id="82178-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="82178-125">Enhedsobjekt, der har certifikatet, synkroniseret til Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="82178-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="82178-126">Synkroniseringscyklus er som standard hver 30 minut, men det afhænger af konfigurationen af Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="82178-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="82178-127">Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="82178-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="82178-128">På dette trin skal du kunne se emne enheden i tilstanden "**afventer**" under Device blade i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="82178-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="82178-129">Næste gang du logger på Windows 10, bliver registreringen fuldført.</span><span class="sxs-lookup"><span data-stu-id="82178-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="82178-130">Hvis du er på VPN og logger af/logger på og afslutter domæne forbindelsen, kan du udløse registreringen manuelt.</span><span class="sxs-lookup"><span data-stu-id="82178-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="82178-131">Sådan gør du:</span><span class="sxs-lookup"><span data-stu-id="82178-131">To do that:</span></span>
    >
    > <span data-ttu-id="82178-132">Udsted en `dsregcmd /join` lokal administrator prompt eller fjern via PsExec til din pc.</span><span class="sxs-lookup"><span data-stu-id="82178-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="82178-133">F. eks.: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="82178-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="82178-134">Du kan finde almindelige problemer med registrering af Azure Active Directory-enhed under [ofte stillede spørgsmål om enheder](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="82178-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
