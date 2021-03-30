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
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="2c244-102">Klienthemmelighed for appregistrering eller certifikatproblemer</span><span class="sxs-lookup"><span data-stu-id="2c244-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="2c244-103">Udløber programklientens hemmelighed?</span><span class="sxs-lookup"><span data-stu-id="2c244-103">Application client secret expiring?</span></span>

<span data-ttu-id="2c244-104">Uanset hvordan det registrerede program blev oprettet, skal der oprettes en ny klienthemmelighed før udløb af den aktuelle og opdateret i den relaterede programkode, uanset om det registrerede program blev oprettet via standardregistreringsprocessen på portalen til registrering af apps, eller hvis Tjenesteinspektøren blev oprettet i din lejer ved hjælp af programmets samtykke.</span><span class="sxs-lookup"><span data-stu-id="2c244-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="2c244-105">Den maksimale gyldighedsperiode er 2 år.</span><span class="sxs-lookup"><span data-stu-id="2c244-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="2c244-106">Som en påmindelse skal den hemmelige værdi registreres, da den ikke længere er synlig, når du har forladt siden appregistreringer på portalen.</span><span class="sxs-lookup"><span data-stu-id="2c244-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="2c244-107">Få mere at vide under [Hurtigstarter: Registrer en app på Microsoft-identitetsplatformen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) og [bedste fremgangsmåder for Microsoft-identitetsplatformen.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="2c244-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="2c244-108">Du kan få mere at vide [under Opret en Azure AD-app & tjenesteinspektør på portalen – Microsoft-identitetsplatformen.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="2c244-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
