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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963781"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Sådan tilføjer og administrerer du administratorer – anbefalede trin

Baseret på din beskrivelse af problemet har vi fundet en løsning til dig. De fleste kunder kunne selv løse deres problem efter at have fulgt vores dokumentation.

**Rediger abonnementsadministratoren eller medadministratoren**

- Kontoadministratoren kan redigere begge roller, mens abonnementsadministratoren kun kan ændre administratorer i [Azure-portalen](https://ms.portal.azure.com/#home).
- [Tilføje eller ændre Azure-abonnementsadministratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Opdater abonnementsadministratoren eller Co-Administrator for interne (AIRS) abonnementer**

Tjenesteadministratoren eller medadministratoren kan selv betjene denne handling ved at benytte følgende fremgangsmåde:

1. Log på [Azure-portalen, og](https://ms.portal.azure.com/#home) klik **på Omkostningsstyring + Fakturering** i venstre blade.
2. Klik på linjeelementet med dit abonnement. Dette åbner Oversigt for dit abonnement.
3. På **bladet Abonnement** skal du klikke på **Egenskaber**. 
4. Klik på **knappen Tjenesteadministrator.**
5. Angiv mailadressen på den bruger, du vil angive som tjenesteadministrator, og klik på **OK.**

**Tilføj/rediger/fjern medadministrator**

1. Log på [Azure-portalen](https://ms.portal.azure.com/#home) som tjenesteadministrator.
2. Åbn [Abonnementer,](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) og vælg et abonnement. (Medadministratorer kan kun tildeles i abonnementsomfanget).)
3. Gå til  >    >    >  **Access-kontrol**  (IAM) Klassiske administratorer Tilføj medadministrator Tilføj medadministrator for at åbne ruden Tilføj medadministrator (hvis indstillingen Tilføj medadministrator er deaktiveret, betyder det, at du ikke har tilladelser).
4. Vælg den bruger, du vil tilføje, og klik på **Tilføj.**

**Lær mere:**
- [Tilføj en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Fjerne en medadministrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ændre tjenesteadministratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Få vist kontoadministratoren](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Administrer adgang ved hjælp af RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Tilføj/slet brugere ved hjælp Azure Active Directory (AD)**

Du kan tilføje nye brugere eller slette eksisterende brugere fra din Azure Active Directory (Azure AD):

1. Hvis du vil tilføje en ny bruger, skal du [logge på Azure-portalen](https://ms.portal.azure.com/#home) som brugeradministrator for organisationen.
2. Vælg **Azure Active Directory**, vælg **Brugere,** og klik derefter på **Ny bruger**.
3. På siden **Bruger** skal du udfylde de påkrævede oplysninger. Klik **på Opret.** Brugeren oprettes og føjes til din Azure AD-lejer.

**Få mere at vide:**

- [Tilføj en ny bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Slet en bruger](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Tilføj eller opdater en brugers profiloplysninger ved hjælp af Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Anbefalede dokumenter**

- [Hvad er rollebaseret adgangskontrol ?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Forstå de forskellige roller i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorrolletilladelser i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Selvstudium: Giv en bruger adgang ved hjælp af RBAC og Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Fejlfinding af RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organiser dine ressourcer med Azure-administrationsgrupper](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Sådan anmoder du om kopi af Azure-faktura via mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Sådan tilføjer, opdaterer eller fjerner du et kredit- eller debetkort fra Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Administrere (Genaktiver/Annuller/Skift) abonnement](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



