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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Fejlfinding af installation af klientgodkendelsescertifikat

Intune-certifikater til NDES/SCEP-og PKCS/PFX-klientcertifikater bruges normalt sammen med andre profiltyper som WiFi, VPN og mail, så brugerne kan godkende virksomhedens ressourcer. Når disse profiltyper er sammenkædet med en klients certifikatprofil, afhænger af den vellykkede installation af profilen.

Startkonfigurationen af infrastrukturen og den tilknyttede konfiguration af klientcertifikat profilen kræver ofte fejlfinding. Hvis du vil have en trinvis vejledning til, hvordan du kan konfigurere NDES Connector og fejlfindingsvejledning til at isolere problemer med certifikat installation, skal du se: 

- [Konfigurere infrastruktur til at understøtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversigt over fejlfinding af SCEP-certifikat profiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Brug de henvisende PowerShell-scripts til at bekræfte konfigurationen. Du kan få mere at vide under [bekræftelses scripts til Intune-certifikat forbindelser](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andre almindelige problemer**

**Når jeg forsøger at installere Intune Certificate Connector på NDES Connector-serveren, får jeg meddelelsen "adgangskoden i certifikatanmodningen kan ikke bekræftes. Det er muligvis allerede blevet brugt. Få en ny adgangskode, der skal sendes med denne anmodning.**  

Denne meddelelse betyder, at du skal køre installationen af certifikat forbindelse som administrator.

I nogle miljøer skal de servere, hvor Intune-certifikatet kører, bruge en proxyserver til at oprette forbindelse til Intune, og certifikat forbindelsen skal derfor bruge en proxy. Under visse omstændigheder ignorerer NDES-connectoren de konfigurerede proxyindstillinger, og det kan være nødvendigt at konfigurere proxyindstillingerne, mens du kører i sikkerhedskonteksten for LocalSystem. 
 
Løsningen er at køre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Når en genstart af Intune Connector-tjenesten er blevet genstartet, opretter NDES Connector forbindelse til Intune.

**Bruger enheder modtager ikke længere SCEP-certifikater fra NDES.**

Det er muligt, at det klientgodkendelsescertifikat, der er udstedt til NDES-serveren, og som blev angivet under installationen af NDES-connectoren, er udløbet eller mangler. Sådan løser du: 
 
1. Fjern NDES-connectoren.  
2. Brug disse oplysninger til at anmode om en ny klientgodkendelse eller et servergodkendelsescertifikat: 
 
    - Emnenavn: CN = eksternt FQDN  
    - Alternativt emnenavn (kræver begge): DNS = eksternt FQDN, DNS = internt FQDN 
 
3. Geninstaller NDES-connectoren med det nye certifikat.