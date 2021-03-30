---
title: Single-Sign aktiveret til Enheder, der er forbundet med Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404589"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enkelt-logon til Azure Active Directory-enheder, der er forbundet

Hvis du har et lokalt Active Directory-miljø (AD), og du vil slutte dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse. [Sådan gør du: Planlæg din hybride](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) implementering af Azure Active Directory-joinforbindelse giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.

[Konfigurere enheder, der er forbundet til Azure AD, til lokale Single-Sign til ved hjælp af Windows Hello til virksomheder](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemer med primær opdateringstoken (PRT)** Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10-, Windows Server 2016- og nyere versioner, iOS- og Android-enheder. Det er en JSON Web Token (JWT), der er særligt udstedt til Microsofts token-formidlere af første part for at aktivere enkelt-logon (SSO) på tværs af de programmer, der bruges på disse enheder. [I Hvad er en primær opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), angiver vi oplysninger om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10-enheder.

**WamDefaultSet: YES og AzureADPrt: YES** Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når der logges på enheden. Hvis værdierne er NEJ, **kan** det være forfaldent:

- Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (kontrollér KeySignTest, mens den kører med administrator administrator).
- Alternativt logon-id
- HTTP-proxy blev ikke fundet

Fejlfinding af enheder ved hjælp af kommandoen dsregcmd – [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
