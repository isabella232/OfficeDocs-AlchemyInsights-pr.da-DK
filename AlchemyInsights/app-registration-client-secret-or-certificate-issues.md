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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404460"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Klienthemmelighed for appregistrering eller certifikatproblemer

Udløber programklientens hemmelighed?

Uanset hvordan det registrerede program blev oprettet, skal der oprettes en ny klienthemmelighed før udløb af den aktuelle og opdateret i den relaterede programkode, uanset om det registrerede program blev oprettet via standardregistreringsprocessen på portalen til registrering af apps, eller hvis Tjenesteinspektøren blev oprettet i din lejer ved hjælp af programmets samtykke. Den maksimale gyldighedsperiode er 2 år. Som en påmindelse skal den hemmelige værdi registreres, da den ikke længere er synlig, når du har forladt siden appregistreringer på portalen. Få mere at vide under [Hurtigstarter: Registrer en app på Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) og [bedste fremgangsmåder for Microsoft-identitetsplatformen.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Du kan få mere at vide [under Opret en Azure AD-app & tjenesteinspektør på portalen – Microsoft-identitetsplatformen.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
