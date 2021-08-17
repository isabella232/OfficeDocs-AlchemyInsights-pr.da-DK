---
title: 'Fakturering for køb af en reserveret forekomst '
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104014"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for køb af en reserveret forekomst 

Betaling for den reserverede forekomst opkræves i forhold til den betalingsmetode, der er knyttet til det abonnement, du vælger på købstidspunktet. Abonnementstypen skal være en Enterprise-aftale (tilbudsnummer: MS-AZR-0017P), betalt efter forbrug (tilbudsnummer: MS-AZR-0003P), Microsoft-kundeaftale eller CSP.

- For et Enterprise-abonnement afregnes gebyrerne fra tilmeldingens økonomiske binding, eller de opkræves som overforbrug
- I forbindelse med et abonnement betalt efter forbrug faktureres gebyrerne til kreditkortet eller metoden til betaling af fakturaer for abonnementet

**Annullering af reservation**

- **Selvbetjening:** Du kan selv annullere eller ombytte en reserveret instans ved hjælp af [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg reservationen, og klik på refusion eller ombytning. Bemærk, at du skal have ejeradgang på reservationsordren for at ombytte eller få en refusion. Adgang til reservationen alene giver dig ikke adgang til at fortsætte med refusionen eller ombytningen. Bed ejeren af reservationsordren om at give dig ejeradgang til reservationsordren
- **Ombytningspolitik:** Du kan ombytte en reservation til en anden reservation af samme type – der er **ingen gebyrer** for ombytning af reservationer. Det samlede engagement med den nye reservation skal være større en summen for den ombyttede reservations refusionsbeløb og de fremtidige månedlige betalinger (hvis relevant)
- **Refusionspolitik:** Summen af refusionen af og de annullerede fremtidige betalinger kan ikke overstige 50.000 USD i løbet af en rullende periode på 12 måneder. Vi **opkræver i øjeblikket ikke noget gebyr** for refusioner, men vi kan opkræve det for fremtidige refusioner

**Undtagelser:** Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering

- **API/PS/CLI**-understøttelse er ikke tilgængelig for annullering og refusioner [Selvbetjente ombytninger og refusioner for Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering. Andre abonnementstyper for USA's regering, herunder Pay-As-You-Go og CSP, understøttes

Få mere at vide: [Hvordan retur-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) og ombytningstransaktioner behandles Få mere at vide: Exchange- og [refusionspolitikker](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Andre spørgsmål: [Besøg reserverede dokumenter om forekomst](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ombyt en eksisterende reserveret instans (selvbetjening)**

Du kan ombytte en reservation til en anden reservation af samme type. Du kan også få refusion for en reservation for op til 50.000 USD om året, hvis du ikke længere har brug for den. Muligheden for selvbetjent ombytning og annullering er ikke tilgængelig for kunder med en Enterprise-aftale for USA's regering. Andre abonnementstyper for USA's regering, herunder Pay-As-You-Go og CSP, understøttes. Du skal have ejeradgang på reservationsordren for at ombytte eller få en refusion for eksisterende reservation.

Følgende trin fører dig gennem proceduren til gennemførsel af transaktionen

1.Log på [Azure-portalen.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vælg de reservationer, du vil refundere, og klik **Exchange** 2.Vælg det VM-produkt, du vil købe, og angiv et antal. Sørg for, at den nye købstotal er mere end den returnerede total [Bestem den rigtige størrelse, før du køber](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Gennemse og fuldfør transaktionen

**Refusion for en reserveret instans**

Hvis du ønsker refusion for en reservation, skal du gå til **Reservationsoplysninger** og klikke på **Refusion**

**Forholdsmæssig refusion:**

**Pro eksempler på minimumskrav til refusion og ombytning** Eksempel på forhåndsreservation:

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

**Fakturaen for den sidste faktureringsperiode kan ikke vises**

Der kan være mulige årsager til, at du ikke får vist en faktura:

- Du har et månedligt kreditbeløb med dit abonnement, som du ikke har overskredet, eller du har en gratis prøveversion. En faktura genereres kun, når du skylder penge
- Det er mindre end 30 dage fra den dag, du abonnerede på Azure
- Fakturaen er endnu ikke oprettet. Vent, indtil faktureringsperioden er slut
- Hvis du ikke er kontoadministrator, er ældre fakturaer muligvis ikke tilgængelige for dig

**Download din faktura fra Azure-portalen (.pdf)**

- Vælg dit abonnement på [siden Abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure-portalen som en bruger med adgang [til fakturaer](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vælg **fakturaer**
- Klik **på Download faktura for** at få vist en kopi af din PDF-faktura. Hvis der står **Ikke tilgængelig**, skal du se Hvorfor kan jeg ikke se en faktura for den [seneste faktureringsperiode?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Modtag din faktura i en mail (.pdf)**

- Vælg dit abonnement på [siden](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Abonnementer. Klik **på Fakturaer og** derefter Send min faktura via mail
- Klik **på Tilmeld dig,** og acceptér vilkårene. Du skal tilmelde dig for hvert abonnement, du ejer

Bemærk! Hvis du ikke får en mail, når du har fulgt trinnene, skal du kontrollere, at din mailadresse er korrekt i [kommunikationsindstillingerne på din profil](https://account.windowsazure.com/profile)

**Download dine brugsdata fra Azure-portalen**

- Log på [Azure-kontocenter](https://account.windowsazure.com/Subscriptions) som [kontoadministrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Vælg det abonnement, du vil have fakturaen og brugsoplysningerne for.
- Vælg **faktureringsoversigt**
- Vælg **Vis aktuel erklæring for** at få vist et skøn over dine gebyrer på det tidspunkt, hvor estimatet blev genereret
- Vælg **Download brug for** at downloade de daglige brugsdata som en CSV-fil. Hvis du ser to tilgængelige versioner, skal du downloade version 2

Andre spørgsmål: [Besøg dokumenter vedrørende reserveret instans](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalede dokumenter**

- [Grundlæggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan rabatten Reserveret forekomst anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Download eller få vist din Azure-faktura og dine daglige brugsdata](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan rabatten Reserveret forekomst anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret brug af forekomst for dit Pay-As-You-Go-abonnement](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret anvendelse af forekomst for din Enterprise-registrering](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows softwareomkostningerne er ikke inkluderet i reserverede forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverede forekomster i programmet Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)