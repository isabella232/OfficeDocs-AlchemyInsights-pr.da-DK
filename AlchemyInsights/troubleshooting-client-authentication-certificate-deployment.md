---
title: Fejlfinding i forbindelse med installation af klientgodkendelsescertifikat
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020798"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Fejlfinding i forbindelse med installation af klientgodkendelsescertifikat

Intune NDES-/SCEP- og PKCS-/PFX-klientcertifikater bruges ofte sammen med andre profiler, f.eks. Wifi, VPN og mail, for at give brugerne mulighed for at godkende virksomhedens ressourcer. Når disse profiltyper er sammenkædet med en klientcertifikatprofil, afhænger det af den vellykkede installation af den pågældende profil.

Startkonfiguration af infrastruktur og tilknyttet konfiguration af klientcertifikatprofilen kræver ofte fejlfinding. Du kan finde en trinvis vejledning til vellykket konfiguration af NDES-forbindelsen og fejlfindingsvejledning til at isolere problemer med certifikatinstallation under: 

- [Konfigurer infrastruktur til at understøtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversigt over fejlfinding af SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Brug de refererede PowerShell-scripts til at bekræfte din konfiguration. Du kan få mere at vide under [Scripts til bekræftelse af intune-certifikatforbindelse.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Andre almindelige problemer**

**Når jeg forsøger at installere Intune-certifikatforbindelse på NDES-forbindelsesserveren, får jeg vist meddelelsen "Adgangskoden i certifikatanmodningen kan ikke bekræftes. Den er muligvis allerede blevet brugt. Hent en ny adgangskode, der skal indsendes med denne anmodning."**  

Denne meddelelse betyder, at du skal køre installationen af certifikatforbindelse som administrator.

I nogle miljøer skal de servere, hvor Intune-certifikatet kører, bruge en proxyserver til at oprette forbindelse til Intune, og så certifikatforbindelse skal bruge en proxy. I nogle tilfælde ignorerer NDES-forbindelsen de konfigurerede proxyindstillinger, og det kan være nødvendigt at konfigurere proxyindstillingerne, mens de kører i sikkerhedskontekst for LocalSystem. 
 
Løsningen er at køre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Efter en genstart af Intune-forbindelsestjenesten opretter NDES-forbindelsen forbindelse til Intune.

**Brugerenheder modtager ikke længere SCEP-certifikater fra NDES.**

Det er muligt, at det klientgodkendelsescertifikat, der er udstedt til NDES-serveren og angivet under installationen af NDES-forbindelsen, er udløbet eller mangler. Sådan løser du det: 
 
1. Fjern NDES-forbindelsen.  
2. Brug disse oplysninger til at anmode om et nyt klientgodkendelses- eller servergodkendelsescertifikat: 
 
    - Emnenavn: CN=ekstern fqdn  
    - Emnealternativ (begge er påkrævet): DNS=ekstern fqdn, DNS=intern fqdn 
 
3. Geninstaller NDES-forbindelsen med det nye certifikat.