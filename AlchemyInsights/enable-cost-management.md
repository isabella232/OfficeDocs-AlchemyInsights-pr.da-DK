---
title: Aktivér omkostningsstyring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677217"
---
# <a name="enable-cost-management"></a>Aktivér omkostningsstyring

**Hvad betyder ' omkostninger deaktiveres for din organisation '?**

Organisationer, der bruger en EA-konto (Enterprise Agreement) eller Microsoft-kunde aftale (MCA), kan deaktivere adgang til omkostningsoplysninger og prisoplysninger.

Når du har logget på Azure-portalen, kan de bruge fakturerings-API'erne til automatisk at få fakturaer (når de er tilmeldt) og oplysninger om forbrug.

**Sådan giver du yderligere brugere adgang til fakturaer**

1. Gå til **abonnements blade** i Azure-portalen.
2. Vælg **fakturaer** , og vælg derefter **adgang til fakturaer**.
3. Slå Access til, når du har gemt ændringerne, for at tillade brugere i abonnementsbaserede roller for at downloade fakturaer.

> [!NOTE]
> Konto administratoren kan også konfigurere for at få fakturaer sendt via mail. Hvis du vil have mere at vide, skal du se [Hent din faktura i en mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Sådan føjer du brugere til rollen fakturerings læser**

1. Gå til **abonnements blade** i Azure-portalen.
2. Vælg **adgangskontrol (IAM)** , og klik derefter på **Tilføj**.
3. Vælg **fakturerings læser** på siden **Vælg en rolle** .
4. Skriv mailadressen på den bruger, du vil invitere, og klik derefter på **OK** for at sende invitationen.
5. Følg instruktionerne i invitationen til mail for at logge på som en fakturerings læser. Hvis du vil have mere at vide, skal du se [Giv adgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Anbefalede dokumenter**

- [Aktivere DA-og AO-visninger via EA Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Omkostninger inkluderet i omkostningsstyring](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Understøttede Microsoft Azure-tilbud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Gennemse omkostninger i omkostningsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Giv adgang til faktureringsoplysninger](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrollér adgang til en Microsoft-kunde aftale](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






