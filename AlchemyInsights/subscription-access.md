---
title: Abonnements adgang
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807291"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="f2007-102">Der kan ikke logges på Azure pga. problemer med browseren (browseren hænger, beholder rotationen, men ikke indlæses osv.)</span><span class="sxs-lookup"><span data-stu-id="f2007-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="f2007-103">Du kan blive påvirket af et udfald.</span><span class="sxs-lookup"><span data-stu-id="f2007-103">You might be impacted by an outage.</span></span> <span data-ttu-id="f2007-104">Kontrollér, om der er et vedvarende udfald: [Azure Health status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="f2007-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="f2007-105">Log af alle de aktive Azure-sessioner.</span><span class="sxs-lookup"><span data-stu-id="f2007-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="f2007-106">Start en in-private-eller Incognito-tilstand for din webbrowser.</span><span class="sxs-lookup"><span data-stu-id="f2007-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="f2007-107">Du kan også forsøge at opdatere browseren, bruge en anden browser, slette cache cookies, hvis de ikke virker.</span><span class="sxs-lookup"><span data-stu-id="f2007-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="f2007-108">Få mere at vide: [fejlfinding af problemer med logon](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="f2007-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="f2007-109">**Kan ikke få adgang til abonnementer**</span><span class="sxs-lookup"><span data-stu-id="f2007-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="f2007-110">I [Azure-portalen](https://portal.azure.com/)skal du sørge for, at den korrekte Azure-mappe er valgt fra kontoen øverst til højre.</span><span class="sxs-lookup"><span data-stu-id="f2007-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="f2007-111">I [Azure-konto Center](https://account.windowsazure.com/Subscriptions)skal du kontrollere, om kontoen, der bruges, er administrator af kontoen.</span><span class="sxs-lookup"><span data-stu-id="f2007-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="f2007-112">Få mere at vide: [fejlfinding der blev ikke fundet nogen abonnementer](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="f2007-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="f2007-113">**Kan ikke få adgang til fakturerings historik**</span><span class="sxs-lookup"><span data-stu-id="f2007-113">**Unable to access billing history**</span></span>

<span data-ttu-id="f2007-114">Konto administratoren skal sørge for, at den bruger, der får adgang til faktureringsoplysningerne, er tilføjet i Azure Active Directory som gæstebruger: [tilføje eller slette en ny bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f2007-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f2007-115">Brugeren skal derefter tildeles en Global administratorrolle: [Tildel rolle til brugere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f2007-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f2007-116">Bogfør dette, brugeren kan få adgang til fakturering ved hjælp af RBAC-politikker: [Tildel adgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f2007-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f2007-117">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="f2007-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="f2007-118">Jeg kan ikke logge på for at administrere mit Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="f2007-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)