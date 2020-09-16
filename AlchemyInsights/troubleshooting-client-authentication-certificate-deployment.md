---
title: Fejlfinding af installation af klientgodkendelsescertifikat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658980"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="785f7-102">Fejlfinding af installation af klientgodkendelsescertifikat</span><span class="sxs-lookup"><span data-stu-id="785f7-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="785f7-103">Intune-certifikater til NDES/SCEP-og PKCS/PFX-klientcertifikater bruges normalt sammen med andre profiltyper som WiFi, VPN og mail, så brugerne kan godkende virksomhedens ressourcer.</span><span class="sxs-lookup"><span data-stu-id="785f7-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="785f7-104">Når disse profiltyper er sammenkædet med en klients certifikatprofil, afhænger af den vellykkede installation af profilen.</span><span class="sxs-lookup"><span data-stu-id="785f7-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="785f7-105">Startkonfigurationen af infrastrukturen og den tilknyttede konfiguration af klientcertifikat profilen kræver ofte fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="785f7-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="785f7-106">Hvis du vil have en trinvis vejledning til, hvordan du kan konfigurere NDES Connector og fejlfindingsvejledning til at isolere problemer med certifikat installation, skal du se:</span><span class="sxs-lookup"><span data-stu-id="785f7-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="785f7-107">Konfigurere infrastruktur til at understøtte SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="785f7-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="785f7-108">Oversigt over fejlfinding af SCEP-certifikat profiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="785f7-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="785f7-109">Brug de henvisende PowerShell-scripts til at bekræfte konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="785f7-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="785f7-110">Du kan få mere at vide under [bekræftelses scripts til Intune-certifikat forbindelser](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="785f7-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="785f7-111">**Andre almindelige problemer**</span><span class="sxs-lookup"><span data-stu-id="785f7-111">**Other common issues**</span></span>

<span data-ttu-id="785f7-112">**Når jeg forsøger at installere Intune Certificate Connector på NDES Connector-serveren, får jeg meddelelsen "adgangskoden i certifikatanmodningen kan ikke bekræftes. Det er muligvis allerede blevet brugt. Få en ny adgangskode, der skal sendes med denne anmodning.**</span><span class="sxs-lookup"><span data-stu-id="785f7-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="785f7-113">Denne meddelelse betyder, at du skal køre installationen af certifikat forbindelse som administrator.</span><span class="sxs-lookup"><span data-stu-id="785f7-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="785f7-114">I nogle miljøer skal de servere, hvor Intune-certifikatet kører, bruge en proxyserver til at oprette forbindelse til Intune, og certifikat forbindelsen skal derfor bruge en proxy.</span><span class="sxs-lookup"><span data-stu-id="785f7-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="785f7-115">Under visse omstændigheder ignorerer NDES-connectoren de konfigurerede proxyindstillinger, og det kan være nødvendigt at konfigurere proxyindstillingerne, mens du kører i sikkerhedskonteksten for LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="785f7-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="785f7-116">Løsningen er at køre Internet Explorer som SYSTEM og konfigurere en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="785f7-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="785f7-117">Når en genstart af Intune Connector-tjenesten er blevet genstartet, opretter NDES Connector forbindelse til Intune.</span><span class="sxs-lookup"><span data-stu-id="785f7-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="785f7-118">**Bruger enheder modtager ikke længere SCEP-certifikater fra NDES.**</span><span class="sxs-lookup"><span data-stu-id="785f7-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="785f7-119">Det er muligt, at det klientgodkendelsescertifikat, der er udstedt til NDES-serveren, og som blev angivet under installationen af NDES-connectoren, er udløbet eller mangler.</span><span class="sxs-lookup"><span data-stu-id="785f7-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="785f7-120">Sådan løser du:</span><span class="sxs-lookup"><span data-stu-id="785f7-120">To resolve:</span></span> 
 
1. <span data-ttu-id="785f7-121">Fjern NDES-connectoren.</span><span class="sxs-lookup"><span data-stu-id="785f7-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="785f7-122">Brug disse oplysninger til at anmode om en ny klientgodkendelse eller et servergodkendelsescertifikat:</span><span class="sxs-lookup"><span data-stu-id="785f7-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="785f7-123">Emnenavn: CN = eksternt FQDN</span><span class="sxs-lookup"><span data-stu-id="785f7-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="785f7-124">Alternativt emnenavn (kræver begge): DNS = eksternt FQDN, DNS = internt FQDN</span><span class="sxs-lookup"><span data-stu-id="785f7-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="785f7-125">Geninstaller NDES-connectoren med det nye certifikat.</span><span class="sxs-lookup"><span data-stu-id="785f7-125">Reinstall the NDES connector with the new certificate.</span></span>