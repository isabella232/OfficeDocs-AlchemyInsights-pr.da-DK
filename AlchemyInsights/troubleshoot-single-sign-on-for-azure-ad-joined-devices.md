---
title: Fejlfinding af enkelt log på til Enheder, der er forbundet til Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039240"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Fejlfinding af enkelt log på til Enheder, der er forbundet til Azure AD

Hvis du har et lokalt Active Directory (AD)-miljø, og du vil forbinde dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse. [Sådan gør du: Planlæg din hybride Azure Active Directory join-implementering](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.

Få mere at vide under [Konfigurer Azure AD-enheder](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)til lokale Single-Sign On using Windows Hello for Business.

**Problemer med det primære opdateringstoken (PRT)**

Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10, Windows Server 2016 og nyere versioner, iOS- og Android-enheder. Det er en JSON-webtoken (JWT), der er særligt udstedt til Microsofts tokenmæglere til at aktivere enkelt logon (SSO) på tværs af de programmer, der bruges på disse enheder. Hvis du vil have mere at vide om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10-enheder, skal du se Hvad [er et primært opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES og AzureADPrt: YES**

Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når der logges på enheden. Hvis værdierne er **NEJ,** kan det skyldes:

- Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (kontrollér KeySignTest, mens den kører med administrator administrator)
- Alternativt logon-id
- HTTP-proxy blev ikke fundet

Hvis du vil udføre fejlfinding af enheder ved hjælp af kommandoen dsregcmd, skal du se [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
