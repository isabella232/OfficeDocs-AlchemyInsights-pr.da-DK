---
title: Fejlfinding af enkelt-logon til Azure AD-enheder, der er forbundet
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035465"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Fejlfinding af enkelt-logon til Azure AD-enheder, der er forbundet

Hvis du har et lokalt Active Directory-miljø (AD), og du vil slutte dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse. [Sådan gør du: Planlæg din hybride](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) implementering af Azure Active Directory-joinforbindelse giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.

Du kan finde flere oplysninger i Konfigurere enheder, der er forbundet til Azure AD, til [lokale Single-Sign Til ved hjælp af Windows Hello til virksomheder.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Problemer med primær opdateringstoken (PRT)**

Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10-, Windows Server 2016- og nyere versioner, iOS- og Android-enheder. Det er en JSON Web Token (JWT), der er særligt udstedt til Microsofts token-formidlere af første part for at aktivere enkelt-logon (SSO) på tværs af de programmer, der bruges på disse enheder. Hvis du vil have mere at vide om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10-enheder, skal du se [Hvad er et primært opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES og AzureADPrt: YES**

Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når han/hun logger på enheden. Hvis værdierne er **NEJ,** kan det skyldes:

- Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (markér KeySignTest, mens den kører med administrator)
- Alternativt logon-id
- HTTP-proxy blev ikke fundet

Hvis du vil foretage fejlfinding af enheder, der bruger kommandoen dsregcmd, skal du se [SSO-tilstand.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
