---
title: Fakturering for købt reserveret forekomst
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823030"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for købt reserveret forekomst

Det reserverede instance-Køb debiteres på betalingsmetoden, der er knyttet til det abonnement, som du vælger på købstidspunktet. Abonnementstypen skal være en Enterprise-aftale (tilbuddets nummer: MS-AZR-0017P), løn-as-Go (tilbuddets nummer: MS-AZR-0003P), Microsoft kunde aftale eller CSP.

- For et virksomhedsabonnement trækkes gebyrerne fra tilmeldingens pengemæssige forpligtelses saldo eller opkræves som overskredet
- For Betal efter forbrug-abonnementet faktureres gebyrerne til betalingsmåden kreditkort eller faktura på abonnementet

**Annullere reservation**

- Selvbetjenings **tjeneste:** Du kan selv annullere eller udveksle en reserveret forekomst ved hjælp af [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg reservationen, og klik på refusion eller Exchange. Bemærk, at du skal have ejerens adgang til reservations ordren for at kunne udveksle eller refundere. Adgang til kun reservationen gør det ikke muligt at fortsætte med refusion eller Exchange. Bed ejeren af reservations ordren om at give dig ejer adgang til reservations ordren
- **Exchange-politik:** Du kan udveksle en reservation for en anden reservation af samme type – der er **ingen sanktioner** over reservations udveksling. Det samlede engagement med ny reservation skal være større end summen af beløbene for kurs refusion og de fremtidige månedlige betalinger (hvis relevant)
- **Refusions politik:** Summen af refusion og de annullerede fremtidige betalinger må ikke overstige $50.000 USD i et rullende vindue i 12 måneder. Vi **opkræver i øjeblikket ikke nogen straf** for refusioner, men kan opkræve betaling for fremtidige refusioner

**Undtagelser:** Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler

- **API/PS/CLI** -understøttelse er ikke tilgængelig for annullering og refusion af selvbetjenings [børs og refusioner for Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler. Andre os-abonnements typer, herunder løn-til-og CSP understøttes

Få mere at vide: [hvordan retur-og Exchange-transaktioner behandles](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) få mere at vide: [Exchange-og refusions politikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) andre spørgsmål: [besøg reserverede forekomster af dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange en eksisterende reserveret forekomst (selvbetjenings tjeneste)**

Du kan udveksle en reservation for en anden reservation af samme type. Du kan også refundere en reservation op til $50.000 USD pr. år, hvis du ikke længere har brug for det. Det er ikke muligt at bruge selvbetjenings service og annullerings funktion for kunder med amerikanske offentlige Enterprise-aftaler. Andre os-abonnements typer, herunder betal-da-Go-Go og CSP, understøttes. Du skal have ejerens adgang til reservations ordren for at udveksle eller refundere en eksisterende reservation.

Følgende trin fører til fremgangsmåden for at fuldføre transaktionen

1. log på din [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg de reservationer, du vil refundere, og klik på **Exchange** 2. Vælg det VM-produkt, du vil købe, og skriv et antal. Sørg for, at den nye købs total er større end det samlede afkast, der [bestemmer den rigtige størrelse, før du køber](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Gennemse og fuldføre transaktionen

**Refusion for en reserveret forekomst**

Hvis du vil refundere en reservation, skal du gå til **reservations detaljer** og klikke på **refundering**

**Pro-vurderet refusion:**

**Pro-ration-og minimumkrav til refusion og Exchange** Eksempel på reservation af forrest.

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

**Det er ikke muligt at få vist faktura for den sidste faktureringsperiode**

Mulige årsager til, at du ikke kan se en faktura:

- Du har et månedligt kreditbeløb med dit abonnement, som du ikke har overskredet, eller du har en gratis prøveperiode. Der genereres kun en faktura, når du skylder penge
- Det er mindre end 30 dage fra den dag, du abonnerer på Azure
- Fakturaen er endnu ikke oprettet. Vente indtil slutningen af faktureringsperioden
- Hvis du ikke er konto administrator, er gamle fakturaer muligvis ikke tilgængelige for dig

**Hent din faktura fra Azure-portalen (. pdf)**

- Vælg dit abonnement fra siden [abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure-portalen som [en bruger med adgang til fakturaer](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vælg **fakturaer**
- Klik på **Hent faktura** for at få vist en kopi af din PDF-faktura. Hvis der ikke står nogen **tilgængelig** , skal du se [Hvorfor kan jeg ikke se en faktura for den sidste faktureringsperiode?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Modtage din faktura via mail (. pdf)**

- Vælg dit abonnement på siden [abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Klik på **fakturaer** , og send derefter min faktura
- Klik på **Tilmeld** dig, og Accepter betingelserne. Du skal tilmelde dig hvert abonnement, du ejer

Bemærk! Hvis du ikke får en mail, efter at du har fulgt trinnene, skal du sikre dig, at din mailadresse er korrekt i [kommunikations præferencerne på din profil](https://account.windowsazure.com/profile)

**Hente dine brugerdata fra Azure-portalen**

- Logge på [Azure-konto centeret](https://account.windowsazure.com/Subscriptions) som [administrator for kontoen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Vælg det abonnement, som du vil have oplysninger om faktura og brug for
- Vælg **fakturerings oversigt**
- Vælg **få vist den aktuelle opgørelse** for at få vist et skøn over dine gebyrer på det tidspunkt, estimatet blev genereret
- Vælg **download-forbrug** for at downloade de daglige brugsdata som en CSV-fil. Hvis du ser to tilgængelige versioner, skal du hente version 2

Andre spørgsmål: [besøg reserverede forekomster af dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalede dokumenter**

- [Grundlæggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan den reserverede forekomst rabat anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Hente eller få vist din Azure fakturerings faktura og oplysninger om daglig forbrug](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan den reserverede forekomst rabat anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret brug af forekomster til dit abonnement på din rejse abonnement](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret brug af forekomster for virksomhedens tilmelding](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-software omkostninger, der ikke er inkluderet med reserverede forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverede forekomster i partnerens centrale program til skybaseret Cloud Solution (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)