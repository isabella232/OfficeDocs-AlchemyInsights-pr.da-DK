---
title: Fakturering for reserveret forekomstkøb
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820316"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for reserveret forekomstkøb

Købet af den reserverede forekomst debiteres med den betalingsmetode, der er bundet til det abonnement, du vælger på købstidspunktet. Abonnementstypen skal være en virksomhedsaftale (tilbudsnummer: MS-AZR-0017P), Pay-As-You-Go (tilbudsnummer: MS-AZR-0003P), Microsoft-kundeaftale eller CSP.

- For et Enterprise-abonnement trækkes gebyrerne fra registreringsbalancen for pengemæssige bindinger eller debiteres som overløb
- For betaling efter betaling efter betaling på farten faktureres gebyrerne til kreditkort- eller fakturabetalingsmetoden på abonnementet

**Annullerer reservation**

- **Selvbetjening:** Du kan selv annullere eller udveksle en reserveret forekomst ved hjælp [af Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vælg reservationen, og klik på refusion eller ombytning. Bemærk, at du skal have ejeradgang på reservationsordren for at kunne ombytte eller refundere. Du kan ikke fortsætte med refusion eller ombytning for at få adgang til reservationen. Bed ejeren af reservationsordren om at give dig ejeradgang til reservationsordren
- **Exchange-politik:** Du kan ombytte en reservation til en anden reservation af samme type – det er ikke **muligt** at foretage reservationer ved ombytning. Den samlede binding med nye reservationer skal være større end summen af ombyttede reservations refusionsbeløb og fremtidige månedlige ydelser (hvis det er relevant)
- **Refusionspolitik:** Summen af refusionen og de annullerede fremtidige betalinger kan ikke overstige $ 50.000 USD i et rullende vindue på 12 måneder. Vi **opkræver i øjeblikket ikke betaling for dine refusioner,** men kan kræve betaling for fremtidige refusioner

**Undtagelser:** Selvbetjenings- og annulleringsfunktionalitet er ikke tilgængelig for amerikanske Enterprise Agreement-kunder

- **API/PS/CLI-support** er ikke tilgængelig for annullering og refusion af [selvbetjeningsudvekslinger og -refusioner for Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selvbetjenings- og annulleringsfunktionalitet er ikke tilgængelig for amerikanske Enterprise Agreement-kunder. Andre amerikanske myndigheder-abonnementstyper, herunder Pay-As-You-Go og CSP, understøttes

Få mere at vide: [Sådan behandles retur- og exchange-transaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Få mere at vide: Politikker for Exchange og [Refusion](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Andre spørgsmål: [Besøg reserverede forekomstdokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange en eksisterende reserveret forekomst (selvbetjening)**

Du kan ombytte en reservation til en anden reservation af samme type. Du kan også refundere en reservation på op til $ 50.000 USD om året, hvis du ikke længere har brug for det. Selvbetjenings- og annulleringsfunktionalitet er ikke tilgængelig for amerikanske Enterprise Agreement-kunder. Andre amerikanske myndigheder-abonnementstyper, herunder Pay-As-You-Go og CSP, understøttes. Du skal have ejeradgang på reservationsordren for at ombytte eller refundere en eksisterende reservation.

Følgende trin hjælper dig med proceduren for at fuldføre transaktionen

1.Log på [Azure-portalen.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vælg de reservationer, du vil refundere, og klik på **Exchange** 2.Vælg det VM-produkt, du vil købe, og angiv et antal. Sørg for, at den nye købstotal er mere end den returnerede total [Bestem den rigtige størrelse, før du køber](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Gennemse og fuldfør transaktionen

**Refusion for en reserveret forekomst**

Hvis du vil refundere en reservation, skal du gå **til Reservationsoplysninger** og klikke på **Refusion**

**Forholdsmæssig refusion:**

**Eksempler på pro-ration og minimumskrav til refusion og ombytning** Eksempel på forhåndsreservation:

- Du køber en periode på et år, RI for $ 120 den 1. januar
- Den 7. april vil du refundere eller ombytte denne reservation
- Da reservationen har været live i 97 dage, får du (1-97/365) * $ 120 tilbage. (dvs. DKK 88,1). Der er i øjeblikket ingen no no-on refundering
- Hvis du udveksler, bør dit nye køb være større end DKK 88,1
- Der er i øjeblikket ingen ytrige refusioner

**Eksempel på reservation af faktureringsplan:**

- Du køber en periode på et år, RI for 10 USD pr. måned
- Den 7. april vil du refundere eller ombytte denne reservation
- Da den sidste betaling skete 7 dage, får du (1-7/31) * $ 10 tilbage. (dvs. DKK 7,74)
- De fremtidige betalinger annulleres, er 80 USD. Der er i øjeblikket ingen no no-on refundering
- Denne annullering trækker $ 87,74 fra dig er refusionsgrænsen på $ 50.000
- Hvis du udveksler, bør den samlede værdi af nyt køb være større end DKK 87,74

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

Andre spørgsmål: [Besøg reserverede forekomstdokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalede dokumenter**

- [Grundlæggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan rabatten Reserveret forekomst anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Download eller få vist din Azure-faktura og dine daglige brugsdata](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå, hvordan rabatten Reserveret forekomst anvendes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret brug af forekomst for dit Pay-As-You-Go-abonnement](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reserveret anvendelse af forekomst for din Enterprise-registrering](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-softwareomkostninger er ikke inkluderet i reserverede forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverede forekomster i CSP-programmet (Partner Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)