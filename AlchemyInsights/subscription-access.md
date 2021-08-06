---
title: Abonnementsadgang
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999234"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kan ikke logge på Azure på grund af browserproblemer (browseren hænger, bliver ved med at dreje, indlæses ikke osv.)

Du kan blive påvirket af et strømsvigt. Kontrollér, om der er en løbende strømsvigt: [Azure Health Status](https://status.azure.com/status/history/).

Log af alle aktive Azure-sessioner. Starte en privat eller incognito-tilstand af din webbrowser.

Du kan også prøve at opdatere browseren, bruge en anden browser, slette cachecookies, hvis ovenstående ikke virker.

Få mere at [vide: Fejlfinding af logonproblemer](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Det er ikke muligt at få adgang til abonnementer**

I [Azure-portalen skal](https://portal.azure.com/)du sørge for, at den korrekte Azure-mappe er valgt fra kontoen øverst til højre.

I [Azure Account Center skal du](https://account.windowsazure.com/Subscriptions)kontrollere, om den konto, der bruges, er kontoadministratoren.

Få mere at vide: [Fejlfinding af fundet ingen abonnementer](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Faktureringsoversigten kunne ikke tilgås**

Kontoadministratoren skal sikre sig, at brugeren, der har adgang til faktureringsoplysningerne, tilføjes i Azure Active Directory som gæstebruger: [Tilføj eller slet en ny bruger.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Brugeren skal derefter tildeles en global administratorrolle: [Tildel rolle til brugere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Slå dette op, og brugeren kan få faktureringsadgang ved hjælp af RBAC-politikker: [Giv adgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalede dokumenter**

-   [Jeg kan ikke logge på for at administrere mit Azure-abonnement](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)