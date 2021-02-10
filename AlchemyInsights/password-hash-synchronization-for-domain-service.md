---
title: Synkronisering af adgangskodehash for domænetjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177418"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synkronisering af adgangskodehash for domænetjeneste

**Hvis din Azure AD DS-forekomst beder dig om at aktivere synkronisering af adgangskodehash**

Du støder på et scenarie, hvor du kører et hybridmiljø med brugere, der synkroniserer fra et lokalt Azure Active Directory-domæneservices (AD DS)-miljø. Dette scenarie opstår, selvom du har synkronisering af adgangskodehash fra den lokale AD DS til din Azure AD-lejer.

**Årsag**

Dette sker, fordi Azure AD Connect som standard ikke synkroniserer ældre new technology LAN Manager (NTLM) og Kerberos-adgangskodehashes, der er nødvendige for Azure AD DS.

**Løsning** 

Du skal konfigurere Azure AD Connect for at synkronisere de adgangskodehashes, der kræves til NTLM- og Kerberos-godkendelse.

Når Azure AD Connect er konfigureret, synkroniserer en lokal kontooprettelses- eller adgangskodeændringshændelse også de ældre adgangskodehashes til Azure AD. Se her [for at](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) få flere oplysninger om dette og for vejledning til, hvordan du aktiverer synkronisering af adgangskoder i Azure AD DS-hybridmiljøer.