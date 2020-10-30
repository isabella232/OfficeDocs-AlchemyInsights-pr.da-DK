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
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Der kan ikke logges på Azure pga. problemer med browseren (browseren hænger, beholder rotationen, men ikke indlæses osv.)

Du kan blive påvirket af et udfald. Kontrollér, om der er et vedvarende udfald: [Azure Health status](https://status.azure.com/status/history/).

Log af alle de aktive Azure-sessioner. Start en in-private-eller Incognito-tilstand for din webbrowser.

Du kan også forsøge at opdatere browseren, bruge en anden browser, slette cache cookies, hvis de ikke virker.

Få mere at vide: [fejlfinding af problemer med logon](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Kan ikke få adgang til abonnementer**

I [Azure-portalen](https://portal.azure.com/)skal du sørge for, at den korrekte Azure-mappe er valgt fra kontoen øverst til højre.

I [Azure-konto Center](https://account.windowsazure.com/Subscriptions)skal du kontrollere, om kontoen, der bruges, er administrator af kontoen.

Få mere at vide: [fejlfinding der blev ikke fundet nogen abonnementer](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kan ikke få adgang til fakturerings historik**

Konto administratoren skal sørge for, at den bruger, der får adgang til faktureringsoplysningerne, er tilføjet i Azure Active Directory som gæstebruger: [tilføje eller slette en ny bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Brugeren skal derefter tildeles en Global administratorrolle: [Tildel rolle til brugere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Bogfør dette, brugeren kan få adgang til fakturering ved hjælp af RBAC-politikker: [Tildel adgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalede dokumenter**

-   [Jeg kan ikke logge på for at administrere mit Azure-abonnement](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)