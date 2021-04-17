---
title: Annullering af reservation
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819686"
---
# <a name="cancelling-reservation"></a>Annullering af reservation

- **Selvbetjening:** Du kan selv annullere eller ombytte en reserveret instans ved hjælp af[Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg reservationen, og klik på refusion eller ombytning. Bemærk, at du skal have ejeradgang på reservationsordren for at ombytte eller få en refusion. Adgang til reservationen alene giver dig ikke adgang til at fortsætte med refusionen eller ombytningen. Bed ejeren af reservationsordren om at give dig ejeradgang til reservationsordren
- **Ombytningspolitik:** Du kan ombytte en reservation til en anden reservation af samme type – der er **ingen gebyrer** for ombytning af reservationer. Det samlede engagement med den nye reservation skal være større en summen for den ombyttede reservations refusionsbeløb og de fremtidige månedlige betalinger (hvis relevant)
- **Refusionspolitik:** Summen af refusionen af og de annullerede fremtidige betalinger kan ikke overstige 50.000 USD i løbet af en rullende periode på 12 måneder. Vi **opkræver i øjeblikket ikke noget gebyr** for refusioner, men vi kan opkræve det for fremtidige refusioner  
    **Undtagelser:** Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering
- **API/PS/CLI**-understøttelse er ikke tilgængelig for annullering og refusioner [Selvbetjente ombytninger og refusioner for Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering. Andre abonnementstyper for USA's regering, herunder Pay-As-You-Go og CSP, understøttes

Få mere at vide: [Sådan behandles returnerings- og ombytningstransaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Få mere at vide: [Ombytnings- og refusionspolitikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andre spørgsmål: [Besøg dokumenter vedrørende reserveret instans](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ombyt en eksisterende reserveret instans (selvbetjening)**

Du kan ombytte en reservation til en anden reservation af samme type. Du kan også få refusion for en reservation for op til 50.000 USD om året, hvis du ikke længere har brug for den. Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering. Andre abonnementstyper for USA's regering, herunder Pay-As-You-Go og CSP, understøttes. Du skal have ejeradgang på reservationsordren for at ombytte eller få en refusion for eksisterende reservation.

Følgende trin fører dig gennem proceduren til gennemførsel af transaktionen

1. Log på din [Azure-portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg de reservationer, du ønsker refunderet, og klik på **Ombyt**
2. Vælg det VM-produkt, du ønsker at købe, og angiv en mængde. Sørg for, at den nye købstotal overstiger returneringstotalen [Bestem den rigtige størrelse, før du køber](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Gennemse og gennemfør transaktionen

**Refusion for en reserveret instans**

Hvis du ønsker refusion for en reservation, skal du gå til **Reservationsoplysninger** og klikke på **Refusion**

**Forholdsmæssig refusion:**

**Eksempler på forholdsmæssige krav og minimumskrav for refusion og ombytning**  
Eksempel på forhåndsreservation:

- Du køber et års RI for 120 USD den 1. januar
- Den 7. april ønsker du refusion for eller ombytning af denne reservation
- Eftersom reservationen har være livet i 97 dage, får du (1-97/365)*120 USD tilbage. (dvs. 88,10 USD). Der er i øjeblikket ikke noget refusionsgebyr
- Ved ombytning skal dit nye køb være større end 88,10 USD
- Det er i øjeblikket ikke noget refusionsgebyr

**Eksempel på faktureringsplan for reservationer:**

- Du køber er års RI for 10 USD om måneden
- Den 7. april ønsker du refusion for eller ombytning af denne reservation
- Fordi den seneste betaling fandt sted for 7 dage siden, får du (1-7/31)*10 USD tilbage. (dvs. 7,74 USD).
- De fremtidige annullerede betalinger udgør 80 USD. Der er i øjeblikket ikke noget refusionsgebyr
- Denne annullering trækker 87,74 USD fra refusionsgrænsen på 50.000 USD
- Ved ombytning skal den samlede værdi af dit nye køb overstige 87,74 USD

**Anbefalede dokumenter**

- [Sådan behandles returnerings- og ombytningstransaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Ombytnings- og refusionspolitikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)