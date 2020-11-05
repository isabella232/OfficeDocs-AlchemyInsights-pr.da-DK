---
title: Overfør Azure fakturerings ejerskab
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922030"
---
# <a name="transfer-azure-billing-ownership"></a>Overfør Azure fakturerings ejerskab

Log på Azure- [portalen](https://portal.azure.com/) som administrator af faktureringskontoen med det abonnement, du vil overføre. Hvis du ikke er sikker på, om du er administrator, eller hvis du har brug for at finde ud af, hvem der er, skal du se [bestemme konto faktureringsadministrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Søg efter **omkostningsstyring + fakturering**.
- Vælg **abonnementer** i venstre rude. Afhængigt af Access skal du muligvis vælge et fakturerings område og derefter **abonnementer** eller Azure- **abonnementer**.
- Vælg **Overfør fakturerings ejerskab** for det abonnement, du vil overføre
- Angiv mailadressen for en bruger, der er faktureringsadministrator for den konto, der skal være den nye ejer af abonnementet, og vælg derefter **Send anmodning om overførsel**
- Brugeren får en mail med instruktioner til at gennemgå din overførsels anmodning. Hvis du vil godkende overførselsanmodningen, skal brugeren vælge linket i mailen og følge vejledningen.

**Bemærk** ! hvis du overfører fakturerings ejerskabet af dit abonnement til en brugerkonto i en anden Azure ad-lejer, fjernes alle [Rollebaserede adgangskontrol (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)opgaver til administration af ressourcer i abonnementet permanent. Det er kun den nye ejer, der har adgang til at administrere ressourcer i abonnementet. Hvis du vil have mere at vide, skal du se [overføre abonnement til en bruger i en anden Azure ad-lejer](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalede dokumenter**

- [Overfør fakturerings ejerskabet af et Azure-abonnement til en anden konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om overførsel af fakturerings ejerskab for et Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Overførsel af Visual Studio, Microsoft Partners Network (MPN) og betal efter din arbejde-dev/test abonnementer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Ofte stillede spørgsmål om overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Fejlfinding af problemer med overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
