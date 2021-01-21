---
title: Konfigurere og udvide levetid for tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916732"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurere og udvide levetid for tokens

Du kan angive levetiden for en Access-, SAML-eller ID-token, der er udstedt af Microsoft Identity platform. Du kan angive levetiden for tokens for alle apps i organisationen, for et program med flere arkitekturer (flere virksomheder) eller for en bestemt tjeneste Principal i organisationen. Du kan få mere at vide ved at læse [levetid for konfigurerbare tokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

For eksempler kan [du læse eksempler på, hvordan du konfigurerer levetid for tokens](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Du kan få mere at vide om, hvordan du konfigurerer levetiden og kompatibiliteten af et token i Azure Active Directory B2C (Azure AD B2C) i [konfigurere tokens i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Artiklen [konfigurere sessions funktionsmåde i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskriver de enkeltlogon-metoder (SSO), der bruges i Azure ad B2C og hjælper dig med at vælge den mest relevante SSO-metode, når du konfigurerer din politik.

**Hvor lang tid er tokens sidst? Hvor lang tid gælder de for?**

Levetid for tokens er 1 time, og sessionens levetid er 24 timer. Det betyder, at hvis der ikke er foretaget nogen anmodninger inden for 24 timer, skal du logge på igen, før du anmoder om en ny token.

> [!NOTE]
> Efter 30, 2020, er der ingen ny lejer, der kan bruge politikken for levetiden for konfigurerbare tokens til at konfigurere session og opdatere tokens. Frarådelsen sker inden for flere måneder efter dette, hvilket betyder, at vi stopper med at overholde eksisterende sessioner og opdaterer tokens. Du kan stadig konfigurere levetiden for adgangs tokens efter dette frarådes.






