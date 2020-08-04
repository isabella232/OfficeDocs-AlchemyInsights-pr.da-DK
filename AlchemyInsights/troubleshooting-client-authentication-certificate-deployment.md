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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Fejlfinding af installation af certifikat til klientgodkendelse

Intune NDES/SCEP- og PKCS/PFX Client-certifikatprofiler bruges ofte sammen med andre profiltyper som Wifi, VPN og e-mail for at give brugerne mulighed for at godkende virksomhedens ressourcer. Når disse profiltyper er knyttet til en klientcertifikatprofil, afhænger af en vellykket installation af den pågældende profil.

Den indledende konfiguration af infrastrukturen og den tilknyttede konfiguration af klientcertifikatprofilen kræver ofte fejlfinding. Du kan finde en trinvis vejledning i en vellykket konfiguration af NDES-forbindelsen og fejlfindingsvejledning til isolering af problemer med certifikatinstallation under: 

- [Konfigurer infrastruktur til at understøtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Brug de powershell-scripts, der refereres til, til at kontrollere konfigurationen. Du kan finde flere oplysninger under [Intune Certificate Connector Verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andre fælles spørgsmål**

**Når jeg forsøger at installere Intune-certifikatforbindelsen på NDES-stikserveren, får jeg vist meddelelsen "Adgangskoden i certifikatanmodningen kan ikke bekræftes. Det kan have været brugt allerede. Få en ny adgangskode, der skal sendes sammen med denne anmodning."**  

Denne meddelelse betyder, at du skal køre installationen af certifikatforbindelsen som administrator.

I nogle miljøer skal de servere, hvor Intune-certifikatet kører, bruge en proxyserver til at oprette forbindelse til Intune, og derfor skal certifikatforbindelsen bruge en proxy. I nogle tilfælde ignorerer NDES Connector de konfigurerede proxyindstillinger, og det kan være nødvendigt at konfigurere proxyindstillingerne, mens du kører i sikkerhedskonteksten i LocalSystem. 
 
Løsningen er at køre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Efter en genstart af Intune Connector-tjenesten opretter NDES-forbindelsen forbindelse til Intune.

**Brugerenheder modtager ikke længere SCEP-certifikater fra NDES.**

Det er muligt, at det klientgodkendelsescertifikat, der er udstedt til NDES-serveren, og som er angivet under installationen af NDES-forbindelsen, er udløbet eller mangler. Sådan løses: 
 
1. Fjern NDES-forbindelsen.  
2. Brug disse oplysninger til at anmode om et nyt klientgodkendelses- eller servergodkendelsescertifikat: 
 
    - Emnenavn: CN=ekstern fqdn  
    - Emnealternativt navn (begge er påkrævet): DNS=ekstern fqdn, DNS=internal fqdn 
 
3. Geninstaller NDES-forbindelsen med det nye certifikat.