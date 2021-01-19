---
title: Problemer med administratortilladelse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900928"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="981c2-102">Problemer med administratortilladelse</span><span class="sxs-lookup"><span data-stu-id="981c2-102">Admin consent issues</span></span>

1. <span data-ttu-id="981c2-103">Aktivere [arbejdsgangen for administrator samtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) for at give brugerne mulighed for at anmode om administratorgodkendelse direkte fra samtykke skærmen.</span><span class="sxs-lookup"><span data-stu-id="981c2-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="981c2-104">Hvis du eller dit programs brugere får uventede fejl under tilladelses processen, skal du læse denne artikel for at få fejlfindingstrin: [uventet fejl, når du udfører et samtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="981c2-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="981c2-105">Få mere at vide om [administrator samtykke på Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hvordan [samtykkes meddelelsen](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerer, og hvordan du [evaluerer en anmodning om administratortilladelse i hele lejeren](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="981c2-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="981c2-106">Programmer, der integreres med Microsoft Identity platform, følger en godkendelsesmodel, der giver brugere og administratorer kontrol over, hvordan data kan åbnes.</span><span class="sxs-lookup"><span data-stu-id="981c2-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="981c2-107">Implementeringen af godkendelses modellen er blevet opdateret på Microsoft Identity platform Endpoint, og det ændrer, hvordan en app skal interagere med Microsoft Identity platform.</span><span class="sxs-lookup"><span data-stu-id="981c2-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="981c2-108">Se [tilladelser og samtykke i Microsoft Identity platform Endpoint for at](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) få en oversigt over denne godkendelsesmodel, herunder områder, tilladelser og samtykke.</span><span class="sxs-lookup"><span data-stu-id="981c2-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>