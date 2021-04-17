---
title: Understøttede abonnementstyper
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
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820676"
---
# <a name="supported-subscription-types"></a>Understøttede abonnementstyper

Gennemgå de understøttede abonnementstyper for at fortsætte.

[Understøttede abonnementstyper](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Overfør faktureringsejerskabet**

Azure-portalen som [Kontoadministrator](https://ms.portal.azure.com/) for den faktureringskonto, der har det abonnement, du ønsker at overføre

- Søg på **Cost Management + Fakturering**. Vælg **Abonnementer** fra venstre rude. Afhængigt af adgangen skal du muligvis vælge et faktureringsområde og derefter **Abonnementer** eller **Azure-abonnementer**.
- Vælg Overfør faktureringsejerskab for det abonnement, du vil overføre.
- Angiv mailadressen på den bruger, der er faktureringsadministrator for den konto, der skal være den nye ejer af abonnementet, og vælg derefter **Send anmodning om overførsel**
- Brugeren får en mail med en vejledning i at gennemse anmodningen om overførsel. For at godkende anmodningen om overførsel, skal brugeren markere linket i mailen og følge vejledningen.

Bemærk: Hvis du overfører faktureringsejerskabet for dit abonnement til en brugerkonto i en anden Azure Active Directory-lejer, fjernes alle tildelinger af [rollebaseret adgangskontrol (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) til administration af ressourcer i abonnementet permanent. Det er kun den nye ejer, der har adgang til at administrere ressourcer i abonnementet. Hvis du vil have mere at vide, skal du se [Overførsel af et abonnement til en bruger i en anden Azure Active Directory-lejer](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Overfør abonnementsejerskab**

Overførsel af abonnementsejerskab forudsætter rollebaseret adgang (TBAC) for at administrere ressourcer i abonnementet mister deres adgang. Du kan finde flere oplysninger om tilføjelse af et eksisterende abonnement til en lejer: Se [Tilknyt eller føj et Azure-abonnement til Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonnementsoverførsel med et eksisterende udestående beløb fra den aktuelle faktureringscyklus overføres ikke til det nye betalingsinstrument på den nye konto. De eneste oplysninger, der er tilgængelige til brugerne på den nye konto, er den sidste måneds pris for dit abonnement. Resten af brugs- og faktureringshistorikken overføres ikke med abonnementet.
- Overførsel af faktureringsejerskab for abonnementer med Enterprise-aftale (EA) understøttes i øjeblikket kun i Enterprise-aftaleportalen
- Overførsel af et kreditorienteret abonnement, f.eks. Visual Studio, BizSpark, Microsoft Partner Network, til en ny bruger, kræver en Visual Studio-/Microsoft Partner Network-licens for at acceptere overførselsanmodningen
- Alle ressourcer, som f.eks. virtuelle maskiner, diske og websteder overføres til den nye konto. Følgende ressourcer kan blive påvirket i en abonnementsoverførsel på tværs af lejere:

**Azure Active Directory-domænetjenester**

Azure-nøglebokse

- [SQL-relaterede brugere og databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kan blive påvirket, særligt hvis kunden bruger en Azure Active Directory-relateret godkendelse
- **Apptjenester**, der er konfigureret med Azure Active Directory-godkendelse, kan blive påvirket
- **Visual Studio Team**-tjenestekonti, der er forbundet til Azure-abonnementer, kan midlertidigt miste adgangen, når det tilknyttede Azure-abonnement annulleres

**Anbefalede dokumenter**

Trin efter accept af faktureringsejerskab:

- Hvis du vil bevare faktureringsejerskabet, men ændre abonnementstypen, skal du se: [Skift dit Azure-abonnement til et andet tilbud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overførsel af Visual Studio, Microsoft Partner Network (MPN) og Dev/Test-abonnementer betalt efter forbrug](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Overfør faktureringsejerskab for abonnementer med Enterprise-aftale (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Ofte stillede spørgsmål om overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Fejlfinding af problemer med overførsel af ejerskab](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)