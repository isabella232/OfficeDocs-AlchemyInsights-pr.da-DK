---
title: Annullere reservation
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807364"
---
# <a name="cancelling-reservation"></a>Annullere reservation

- Selvbetjenings **tjeneste:** Du kan selv annullere eller udveksle en reserveret forekomst ved hjælp af [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg reservationen, og klik på refusion eller Exchange. Bemærk, at du skal have ejerens adgang til reservations ordren for at kunne udveksle eller refundere. Adgang til kun reservationen gør det ikke muligt at fortsætte med refusion eller Exchange. Bed ejeren af reservations ordren om at give dig ejer adgang til reservations ordren
- **Exchange-politik:** Du kan udveksle en reservation for en anden reservation af samme type – der er **ingen sanktioner** over reservations udveksling. Det samlede engagement med ny reservation skal være større end summen af beløbene for kurs refusion og de fremtidige månedlige betalinger (hvis relevant)
- **Refusions politik:** Summen af refusion og de annullerede fremtidige betalinger må ikke overstige $50.000 USD i et rullende vindue i 12 måneder. Vi **opkræver i øjeblikket ikke nogen straf** for refusioner, men kan opkræve betaling for fremtidige refusioner  
    **Undtagelser:** Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler
- **API/PS/CLI** -understøttelse er ikke tilgængelig for annullering og refusion af selvbetjenings [børs og refusioner for Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler. Andre os-abonnements typer, herunder løn-til-og CSP understøttes

Få mere at vide: [Sådan behandles retur-og Exchange-transaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Få mere at vide: [Exchange-og refusions politikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andre spørgsmål: [besøg reserverede forekomster af dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange en eksisterende reserveret forekomst (selvbetjenings tjeneste)**

Du kan udveksle en reservation for en anden reservation af samme type. Du kan også refundere en reservation op til $50.000 USD pr. år, hvis du ikke længere har brug for det. Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler. Andre os-abonnements typer, herunder betal-da-Go-Go og CSP, understøttes. Du skal have ejerens adgang til reservations ordren for at udveksle eller refundere en eksisterende reservation.

Følgende trin fører til fremgangsmåden for at fuldføre transaktionen

1. Log på Azure- [portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg de reservationer, du vil refundere, og klik på **Exchange**
2. Vælg det VM-produkt, du vil købe, og skriv et antal. Sørg for, at den nye købs total er større end det samlede afkast, der [bestemmer den rigtige størrelse, før du køber](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Gennemse og fuldføre transaktionen

**Refusion for en reserveret forekomst**

Hvis du vil refundere en reservation, skal du gå til **reservations detaljer** og klikke på **refundering**

**Pro-vurderet refusion:**

**Pro-ration-og minimumkrav til refusion og Exchange**  
Eksempel på reservation af forrest.

- Du køber en treårig periode på RI for $120 d. 1.
- På april 7th, du vil refundere eller udveksle denne reservation
- Da reservationen er blevet levende i 97 dage, får du (1-97/365) * $120 tilbage. (dvs. $88,1). Der er i øjeblikket ingen straf for restitutioner
- Hvis du er ved at udveksle, skal dit nye køb være større end $88,1
- Der ikke er nogen straf for restitutioner i øjeblikket

**Eksempel på reservation af faktureringsplan:**

- Du køber en periode på et enkelt år på RI for $10 om måneden
- På april 7th, du vil refundere eller udveksle denne reservation
- Da den sidste betaling skete 7 dage, får du (1-7/31) * $10 tilbage. (dvs. $7,74)
- De fremtidige betalinger, der annulleres, er $80. Der er i øjeblikket ingen straf for restitutioner
- Denne annullering trækker $87,74 fra dig til $50.000-restitutions grænsen
- Hvis du udveksler, skal den samlede værdi af det nye køb være større end $87,74

**Anbefalede dokumenter**

- [Sådan behandles retur-og Exchange-transaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange-og refusions politikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)