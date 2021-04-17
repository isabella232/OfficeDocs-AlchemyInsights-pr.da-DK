---
title: Overfør ejerskab af Azure Fakturering
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820604"
---
# <a name="transfer-azure-billing-ownership"></a>Overfør ejerskab af Azure Fakturering

Log på [Azure-portalen](https://portal.azure.com/) som administrator af faktureringskontoen med det abonnement, du vil overføre. Hvis du ikke er sikker på, om du er administrator, eller hvis du har brug for at finde ud af, hvem der er, skal du se [Bestem Administrator for faktureringskonto](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Søg efter _Cost Management + Fakturering_.
1. Vælg **Abonnementer** fra venstre rude. Afhængigt af adgangen skal du muligvis vælge et faktureringsområde og derefter **Abonnementer** eller **Azure-abonnementer**.
1. Vælg **Overfør faktureringsejerskab** for det abonnement, du vil overføre.
1. Angiv mailadressen på den bruger, der er faktureringsadministrator for den konto, der skal være den nye ejer af abonnementet, og vælg derefter **Send anmodning om overførsel**.
1. Brugeren får en mail med en vejledning i at gennemse anmodningen om overførsel. For at godkende anmodningen om overførsel, skal brugeren markere linket i mailen og følge vejledningen.

Bemærk, at hvis du overfører faktureringsejerskabet for dit abonnement til en brugerkonto i en anden Azure AD-lejer, fjernes alle tildelinger af [rollebaseret adgangskontrol (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) til administration af ressourcer i abonnementet permanent. Det er kun den nye ejer, der har adgang til at administrere ressourcer i abonnementet. Hvis du vil have mere at vide om, hvordan du ændrer en mappe for et abonnement, skal du se [Sådan overfører du abonnement til en bruger i en anden Azure AD-lejer](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Vigtig indvirkning på dine fakturaer**_: Hvis du har overført faktureringsejerskab for et Azure-abonnement, vil dine omkostninger være forholdsmæssigt beregnet. Du kan få adgang til fakturaer som følgende:  

1. Vælg dit abonnement på siden [Abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure-portalen som [en bruger med adgang til fakturaer](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), og vælg derefter **Fakturaer**.
1. Klik på **Download faktura** for at få vist en kopi af din PDF-faktura. Hvis der står _Ikke tilgængelig_, kan du gå til [Hvorfor kan jeg ikke se en faktura for den seneste faktureringsperiode?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Du kan også få vist dit daglige forbrug ved at klikke på **faktureringsperioden** for at få en PDF-fil med din faktura og en kopi af din detaljerede fil for dagligt forbrug (.csv). Hvis du vil have mere at vide, skal du se [Få oplysninger om fakturaer og brugsdata](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalede dokumenter**

- [Overfør faktureringsejerskab for et Azure-abonnement til en anden konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om overførsel af faktureringsejerskab for et Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Overførsel af Visual Studio, Microsoft Partner Network (MPN) og Dev/Test-abonnementer betalt efter forbrug](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Ofte stillede spørgsmål om overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Fejlfinding af problemer med overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
