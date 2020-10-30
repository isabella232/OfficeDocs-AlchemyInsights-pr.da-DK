---
title: Understøttede abonnements typer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807359"
---
# <a name="supported-subscription-types"></a>Understøttede abonnements typer

Gennemse de understøttede abonnements typer for at fortsætte yderligere.

[Understøttede abonnements typer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Overfør ejerskab til fakturering**

Azure-portalen som [kontoadministrator](https://ms.portal.azure.com/) for den faktureringskonto, der har det abonnement, du vil overføre

- Søg efter **omkostningsstyring + fakturering** . Vælg **abonnementer** fra venstre rude. Afhængigt af Access skal du muligvis vælge et fakturerings område og derefter **abonnementer** eller Azure- **abonnementer** .
- Vælg Overfør fakturerings ejerskab for det abonnement, du vil overføre
- Angiv mailadressen for en bruger, der er faktureringsadministrator for den konto, der skal være den nye ejer af abonnementet, og vælg derefter **Send anmodning om overførsel**
- Brugeren får en mail med instruktioner til at gennemgå din overførsels anmodning. Hvis du vil godkende overførselsanmodningen, skal brugeren vælge linket i mailen og følge vejledningen.

Bemærk! Hvis du overfører fakturerings ejerskabet af dit abonnement til en brugerkonto i en anden Azure AD-lejer, fjernes alle [Rollebaserede adgangskontrol (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) opgaver til administration af ressourcer i abonnementet permanent. Det er kun den nye ejer, der har adgang til at administrere ressourcer i abonnementet. Hvis du vil have mere at vide, skal du se [overføre abonnement til en bruger i en anden Azure ad-lejer](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Overføre ejerskabet af abonnement**

Abonnements ejerskab for overførsel forudsætninger rollebaseret adgang (RBAC) Hvis du vil administrere ressourcer i abonnementet, mister du deres adgang. Du kan finde flere oplysninger om at føje et eksisterende abonnement til en lejer i [tilknytte eller tilføje et Azure-abonnement til Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonnements overførsel med et eksisterende udestående beløb fra den aktuelle faktureringscyklus overføres ikke til det nye betalingsinstrument på den nye konto. De eneste oplysninger, der er tilgængelige for brugerne i den nye konto, er den sidste måneds omkostninger for dit abonnement. Resten af forbruget og fakturerings oversigten overføres ikke til abonnementet.
- Overdragelse af fakturerings ansvaret for EA-abonnementer understøttes i øjeblikket kun i Enterprise Agreement-portalen
- Overførsel af et kredit orienteret abonnement som Visual Studio, BizSpark, Microsoft Partner Network til en ny bruger skal have en Visual Studio/Microsoft Partner Network-licens for at acceptere overførselsanmodningen
- Alle ressourcer som virtuelle maskiner, diske og websteder overføres til den nye konto. Følgende ressourcer kan påvirkes i en abonnements overførsel på tværs af flere arkitekturer:

**Azure AD-domæne tjenester**

Legitimationsoplysninger for Azure-nøgle

- [SQL-relaterede brugere og databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kan blive påvirket, især hvis kunden bruger en Azure Active Directory-relateret godkendelse
- **App-tjenester** , der er konfigureret med Azure Active Directory-godkendelse, kan blive påvirket
- **Visual Studio Team** Tjenestekonti, der er forbundet til Azure-abonnementer, kan midlertidigt miste adgang, når det forbundne Azure-abonnement annulleres

**Anbefalede dokumenter**

Trin efter accept af fakturerings ejerskab:

- Hvis du vil bevare fakturerings ejerskab, men ændre abonnementstypen, skal du [gå til: Skift dit Azure-abonnement til et andet bud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overførsel af Visual Studio, Microsoft Partners Network (MPN) og betal efter din arbejde-dev/test abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Overfør fakturerings ejerskab for EA-abonnementer (Enterprise Agreement)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Ofte stillede spørgsmål om overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Fejlfinding af problemer med overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)