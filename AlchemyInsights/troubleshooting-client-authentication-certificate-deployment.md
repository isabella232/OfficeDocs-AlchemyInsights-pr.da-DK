---
title: Fejlfinding af installation af certifikat til klientgodkendelse
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554854"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="d7f87-102">Fejlfinding af installation af certifikat til klientgodkendelse</span><span class="sxs-lookup"><span data-stu-id="d7f87-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="d7f87-103">Intune NDES/SCEP- og PKCS/PFX Client-certifikatprofiler bruges ofte sammen med andre profiltyper som Wifi, VPN og e-mail for at give brugerne mulighed for at godkende virksomhedens ressourcer.</span><span class="sxs-lookup"><span data-stu-id="d7f87-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="d7f87-104">Når disse profiltyper er knyttet til en klientcertifikatprofil, afhænger af en vellykket installation af den pågældende profil.</span><span class="sxs-lookup"><span data-stu-id="d7f87-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="d7f87-105">Den indledende konfiguration af infrastrukturen og den tilknyttede konfiguration af klientcertifikatprofilen kræver ofte fejlfinding.</span><span class="sxs-lookup"><span data-stu-id="d7f87-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="d7f87-106">Du kan finde en trinvis vejledning i en vellykket konfiguration af NDES-forbindelsen og fejlfindingsvejledning til isolering af problemer med certifikatinstallation under:</span><span class="sxs-lookup"><span data-stu-id="d7f87-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="d7f87-107">Konfigurer infrastruktur til at understøtte SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="d7f87-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="d7f87-108">Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d7f87-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="d7f87-109">Brug de powershell-scripts, der refereres til, til at kontrollere konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="d7f87-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="d7f87-110">Du kan finde flere oplysninger under [Intune Certificate Connector Verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="d7f87-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="d7f87-111">**Andre fælles spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="d7f87-111">**Other common issues**</span></span>

<span data-ttu-id="d7f87-112">**Når jeg forsøger at installere Intune-certifikatforbindelsen på NDES-stikserveren, får jeg vist meddelelsen "Adgangskoden i certifikatanmodningen kan ikke bekræftes. Det kan have været brugt allerede. Få en ny adgangskode, der skal sendes sammen med denne anmodning."**</span><span class="sxs-lookup"><span data-stu-id="d7f87-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="d7f87-113">Denne meddelelse betyder, at du skal køre installationen af certifikatforbindelsen som administrator.</span><span class="sxs-lookup"><span data-stu-id="d7f87-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="d7f87-114">I nogle miljøer skal de servere, hvor Intune-certifikatet kører, bruge en proxyserver til at oprette forbindelse til Intune, og derfor skal certifikatforbindelsen bruge en proxy.</span><span class="sxs-lookup"><span data-stu-id="d7f87-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="d7f87-115">I nogle tilfælde ignorerer NDES Connector de konfigurerede proxyindstillinger, og det kan være nødvendigt at konfigurere proxyindstillingerne, mens du kører i sikkerhedskonteksten i LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="d7f87-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="d7f87-116">Løsningen er at køre Internet Explorer som SYSTEM og konfigurere en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="d7f87-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="d7f87-117">Efter en genstart af Intune Connector-tjenesten opretter NDES-forbindelsen forbindelse til Intune.</span><span class="sxs-lookup"><span data-stu-id="d7f87-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="d7f87-118">**Brugerenheder modtager ikke længere SCEP-certifikater fra NDES.**</span><span class="sxs-lookup"><span data-stu-id="d7f87-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="d7f87-119">Det er muligt, at det klientgodkendelsescertifikat, der er udstedt til NDES-serveren, og som er angivet under installationen af NDES-forbindelsen, er udløbet eller mangler.</span><span class="sxs-lookup"><span data-stu-id="d7f87-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="d7f87-120">Sådan løses:</span><span class="sxs-lookup"><span data-stu-id="d7f87-120">To resolve:</span></span> 
 
1. <span data-ttu-id="d7f87-121">Fjern NDES-forbindelsen.</span><span class="sxs-lookup"><span data-stu-id="d7f87-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="d7f87-122">Brug disse oplysninger til at anmode om et nyt klientgodkendelses- eller servergodkendelsescertifikat:</span><span class="sxs-lookup"><span data-stu-id="d7f87-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="d7f87-123">Emnenavn: CN=ekstern fqdn</span><span class="sxs-lookup"><span data-stu-id="d7f87-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="d7f87-124">Emnealternativt navn (begge er påkrævet): DNS=ekstern fqdn, DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="d7f87-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="d7f87-125">Geninstaller NDES-forbindelsen med det nye certifikat.</span><span class="sxs-lookup"><span data-stu-id="d7f87-125">Reinstall the NDES connector with the new certificate.</span></span>