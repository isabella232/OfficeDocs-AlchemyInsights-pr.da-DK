---
title: Adgangskodepolitikker
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040824"
---
# <a name="password-policies"></a>Adgangskodepolitikker

**Jeg har problemer med adgangskodepolitikken for en bruger**

- Adgangskodepolitikken for en bruger afhænger af, om brugeren kun er skybaseret eller lokal.
- Kun skybrugere skal vælge en adgangskode, der opfylder kravene i denne artikel: Adgangskodepolitikker, [der kun gælder for skybrugerkonti](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokale brugere skal vælge en adgangskode, der opfylder de lokale krav. Hvis en lokal bruger ikke kan angive sin adgangskode, skal du kontrollere dine lokale krav.

**Jeg ved ikke, hvordan jeg angiver eller kontrollerer udløbspolitikker for adgangskoder**

- Du kan angive og kontrollere udløbspolitikken for skybrugere i din lejer ved hjælp af PowerShell. Følg instruktionerne i denne artikel: [Angiv eller kontrollér adgangskodepolitikker ved hjælp af PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Udløbspolitikken for adgangskoder for lokale brugere er angivet i dit lokale AD.

**Andre nyttige links:**
- [Introduktion til nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Fejlfinding af administrator-startet nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
