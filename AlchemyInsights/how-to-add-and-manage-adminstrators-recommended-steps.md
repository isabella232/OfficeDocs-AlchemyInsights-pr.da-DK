---
title: Sådan tilføjer og administrerer du administratorer – anbefalede trin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677256"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Sådan tilføjer og administrerer du administratorer – anbefalede trin

**Rediger abonnements administratoren eller kollegaen**

- Konto administratoren kan redigere begge roller, hvorimod abonnements administratoren kun kan ændre samtidig administratorer i Azure- [portalen](https://ms.portal.azure.com/#home).
- [Tilføje eller ændre Azure-abonnements administratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Opdatere abonnements administratoren eller Co-Administrator for interne (AIRS)-abonnementer**

Tjenesteadministratoren eller samtidig administrator kan selv behandle denne handling ved hjælp af følgende trin:

1. Log på Azure- [portalen](https://ms.portal.azure.com/#home) , og klik på **omkostningsstyring + fakturering** i venstre blade.
2. Klik på linjeelementet med dit abonnement. Dette åbner oversigten over dit abonnement.
3. Klik på **Egenskaber** på **abonnements** bladet. 
4. Klik på knappen **tjenesteadministrator** .
5. Skriv mailadressen på den bruger, du vil angive som tjeneste administrator, og klik på **OK**.

**Tilføj/Rediger/fjern samtidig administrator**

1. Log på Azure- [portalen](https://ms.portal.azure.com/#home) som tjeneste administrator.
2. Åbn [abonnementer](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , og vælg et abonnement. (Co-administratorer kan kun tildeles til abonnements området).
3. Naviger til Classic-administratorer **(Access Control)**  >  **Classic-administratorer**  >  **Tilføj**  >  **Tilføj administrator** for at åbne ruden **Tilføj Co-administrator** (hvis indstillingen Tilføj Co-administrator er deaktiveret, angiver det, at du ikke har tilladelse).
4. Vælg den bruger, du vil tilføje, og klik på **Tilføj**.

**Lær mere:**
- [Tilføj en administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Fjerne en administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ændre tjeneste administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Få vist konto administratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Administrere adgang ved hjælp af RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Tilføj/slet brugere ved hjælp af Azure Active Directory (AD)**

Du kan tilføje nye brugere eller slette eksisterende brugere fra din Azure Active Directory-organisation (Azure AD):

1. Hvis du vil tilføje en ny bruger, skal du logge på [Azure-portalen](https://ms.portal.azure.com/#home) som Brugeradministrator for organisationen.
2. Vælg **Azure Active Directory**, Vælg **brugere** , og klik derefter på **ny bruger**.
3. På siden **bruger** skal du udfylde de nødvendige oplysninger. Klik på **Opret**. Brugeren oprettes og føjes til din Azure AD-lejer.

**Få mere at vide**:

- [Tilføje en ny bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Slette en bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Tilføje eller opdatere en brugers profiloplysninger ved hjælp af Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Anbefalede dokumenter**

- [Hvad er rollebaseret adgangskontrol (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Forstå de forskellige roller i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Tilladelser som administrator roller i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Selvstudium: give adgang til en bruger ved hjælp af RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Fejlfinding af RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organisere dine ressourcer med Azure Management groups](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Sådan anmoder du om en kopi af Azure-faktura via mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Sådan tilføjer, opdaterer eller fjerner du et kredit-eller debetkort fra Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Administrer abonnementet (Genaktiver/Annuller/Skift)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



