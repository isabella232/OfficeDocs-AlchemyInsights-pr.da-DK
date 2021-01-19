---
title: Foretag fejlfinding af brugersamtykke
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900961"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="d2880-102">Foretag fejlfinding af brugersamtykke</span><span class="sxs-lookup"><span data-stu-id="d2880-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="d2880-103">Du kan konfigurere, hvordan slutbrugere skal have tilladelse til at bruge programmer via Azure-portalen eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2880-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="d2880-104">Se [Indstillinger for brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="d2880-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="d2880-105">En administrator kan også bruge [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til at give samtykke til uddelegerede tilladelser på vegne af en enkelt bruger.</span><span class="sxs-lookup"><span data-stu-id="d2880-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="d2880-106">Hvis du vil have mere at vide, skal du se [få adgang på vegne af en bruger](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="d2880-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="d2880-107">[Fejl i brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): denne artikel omhandler fejl, der kan opstå under processen med at sende til et program.</span><span class="sxs-lookup"><span data-stu-id="d2880-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="d2880-108">Hvis du foretager fejlfinding af uventede samtykke anmodninger, der ikke indeholder nogen fejlmeddelelser, skal du se [godkendelses scenarier for Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="d2880-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>