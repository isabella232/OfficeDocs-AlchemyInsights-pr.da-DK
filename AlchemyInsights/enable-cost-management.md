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
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325457"
---
# <a name="enable-cost-management"></a>Aktivér omkostningsstyring

**Hvad betyder "omkostninger er deaktiveret for din organisation"?**

Organisationer, der Enterprise Agreement (EA) eller Microsoft-kundeaftalekonti (MCA), kan deaktivere adgang til oplysninger om omkostninger og prisoplysninger.

Når de har logget på Azure-portalen, kan de bruge fakturerings-API'er til programmeringligt at hente fakturaer (når de er tilmeldt) og oplysninger om brug.

**Sådan giver du flere brugere adgang til fakturaer**

1. Gå til **Blade (Abonnementer)** i Azure-portalen.
2. Vælg **Fakturaer og** derefter Adgang til **fakturaer.**
3. Slå adgangen til efterfulgt af at gemme ændringerne for at tillade brugere i abonnementsbaserede roller at hente fakturaer.

**Bemærk!** Kontoadministratoren kan også konfigurere, at fakturaer sendes via mail. Du kan få mere at vide [under Få din faktura i en mail.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Sådan føjer du brugere til faktureringslæserrollen**

1. Gå til **Blade (Abonnementer)** i Azure-portalen.
2. Vælg **Access-kontrolelement (IAM), og** klik derefter på **Tilføj**.
3. Vælg **Faktureringslæser** på **siden Vælg en** rolle.
4. Skriv mailadressen på den bruger, du vil invitere, og klik derefter på **OK** for at sende invitationen.
5. Følg vejledningen i invitationsmailen til at logge på som faktureringslæser. Få mere at vide under [Giv adgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Anbefalede dokumenter**

- [Aktivér DA- og AO-visninger via EA-portalen](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Omkostninger inkluderet i Omkostningsstyring](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Understøttede Microsoft Azure tilbud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Gennemse omkostninger i omkostningsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Give adgang til faktureringsoplysninger](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrollér adgang til en Microsoft-kundeaftale](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






