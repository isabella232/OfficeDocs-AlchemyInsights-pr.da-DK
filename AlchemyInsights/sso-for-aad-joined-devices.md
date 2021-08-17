---
title: Single-Sign på til Azure Active Directory enheder, der er forbundet
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050004"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enkelt log på til Azure Active Directory enheder, der er forbundet

Hvis du har et lokalt Active Directory (AD)-miljø, og du vil forbinde dine AD-domænesammenføjede computere til Azure AD, kan du gøre dette ved at udføre en hybrid Azure AD-joinforbindelse. [Sådan gør du: Planlæg din hybride Azure Active Directory join-implementering](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) giver dig de relaterede trin til at implementere en hybrid Azure AD-joinforbindelse i dit miljø.

[Konfigurere enheder, der er forbundet til Azure AD, til lokale Single-Sign til brug Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemer med det primære opdateringstoken (PRT)** Et primært opdateringstoken (PRT) er en vigtig del af Azure AD-godkendelse på Windows 10, Windows Server 2016 og nyere versioner, iOS- og Android-enheder. Det er en JSON-webtoken (JWT), der er særligt udstedt til Microsofts tokenmæglere til at aktivere enkelt logon (SSO) på tværs af de programmer, der bruges på disse enheder. [I Hvad er et primært opdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), angiver vi oplysninger om, hvordan en PRT udstedes, bruges og beskyttes på Windows 10 enheder.

**WamDefaultSet: YES og AzureADPrt: YES** Disse felter angiver, om brugeren er blevet godkendt til Azure AD, når der logges på enheden. Hvis værdierne er **NEJ,** kan det være forfaldent:

- Ugyldig lagernøgle i den TPM, der er knyttet til enheden ved registrering (kontrollér KeySignTest, mens den kører med administrator administrator).
- Alternativt logon-id
- HTTP-proxy blev ikke fundet

Fejlfinding af enheder ved hjælp af kommandoen dsregcmd – [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
