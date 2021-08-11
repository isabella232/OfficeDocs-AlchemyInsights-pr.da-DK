---
title: Klienthemmelighed for appregistrering eller certifikatproblemer
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951487"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Klienthemmelighed for appregistrering eller certifikatproblemer

Udløber programklientens hemmelighed?

Uanset hvordan det registrerede program blev oprettet, uanset om det sker via standardregistreringsprocessen på appregistreringsportalen, eller hvis tjenesteinspektøren blev oprettet i din lejer ved hjælp af programmets samtykke, skal der oprettes en ny klienthemmelighed før udløb af den aktuelle og opdateres i den relaterede programkode. Den maksimale gyldighedsperiode er 2 år. Som en påmindelse skal den hemmelige værdi registreres, da den ikke længere vil være synlig, når du har forladt siden Appregistreringer i portalen. Du kan finde flere oplysninger [i Hurtig start: Registrere en app i Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) og Bedste fremgangsmåder for [Microsoft-identitetsplatform.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Du kan få mere at [vide under Opret en Azure AD-&-tjenesteinspektør på portalen – Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
