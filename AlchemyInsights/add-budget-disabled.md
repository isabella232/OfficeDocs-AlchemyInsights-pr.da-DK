---
title: Hvorfor er knappen Tilføj budget deaktiveret for mig?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807279"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Hvorfor er knappen Tilføj budget deaktiveret for mig?

Hvis du vil oprette et budget, skal du have en af følgende tilladelser:

- Administrationsgruppe, abonnement, ressourcegruppe områder
- Bidragyder til omkostningsstyring
- Stand
- Bidrag
- Virksomhedens kunder: tilmelding, afdeling, konto områder
- Registrerings administrator (Angiv budget ved tilmeldings område)
- Afdelings administrator (Angiv budget på afdelings område)
- Konto ejer (Angiv budget på konto område)
- Kun moderne kunde aftale: faktureringskonto, fakturerings profil, faktura sektions områder
- Azure-abonnements oprettelse

**Jeg har oprettet et budget, når mine omkostninger for den aktuelle måned allerede er overskredet budget. Hvorfor har jeg ikke modtaget en besked?**  
Hvis du allerede har overskredet en bestemt omkostnings tærskel, når du opretter et budget, som beskeden ikke skal udløse. Når en ny cyklus starter, og hvis du brud tærsklen, bliver beskeden fire.

**Hvornår skal jeg forvente at modtage en besked, når jeg har overskredet en af mine definerede tidsgrænser for budget beskeder?**  
Budgetter evalueres hver fjerde time. Det kræver mindst 8 timer, før du kan få adgang til budget systemet. Når du har overskredet en tærskel, kan beskederne tage op til 12 timer.

**Hvorfor er knappen Start dato deaktiveret, når jeg vælger en periode for nulstilling af måned eller fakturerings måned?**  
Budgetter er justeret efter den aktuelle kalendermåned eller aktuelle faktureringsperiode (hvis fakturerings måned er valgt). Vi skal derfor forhåndsudfylde denne værdi for dig.

**Hvorfor kan jeg ikke se en graf over mine omkostninger i budget oprettelses oplevelsen?**  
Vi skal have mindst 2 måneders omkostningsoplysninger, før vi kan gengive et diagram, der kan hjælpe dig med at oprette budgettet.

**Hvorfor kan jeg ikke angive et budget mod et abonnement, jeg lige har oprettet?**  
Når du har oprettet et abonnement, tager det 24-48-timer at behandle dataene, før du angiver et budget mod det.

**Budget-API-ressourcer**

- [Budget API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): indeholder handlinger til at oprette og opdatere budgetter. Når du bruger budget-API'ET, kan du angive en budgettærskel og konfigurere flere vigtige beskeder til at blive fire, når du nærmer dig, hvilken grænse. Beskeder kan udløse en mail eller en Azure-handlings gruppe for at udføre automatisering. Bemærk! filtrering for denne API justerer ikke med forespørgsels-API-filtrering/dimensioner.
- [Budget-API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Opret budgetter med større omkostnings filtreringsfunktioner end v1. Filtrering justeres efter den kontrakt, der bruges i vores forespørgsels-og dimension-API'er. Dette er det anbefalede budget-API, der kan bruges til at bevæge sig fremad.
- [Dimensioner](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): indeholder handlinger, der skal bruges til at få understøttede dimensioner til dit forbrug under forskellige områder. Ved hjælp af dimensions-API'ET kan du hente en liste over dimensioner, der kan bruges som input til at oprette forespørgsler med forespørgsels-API'ET.
- [Forespørgsel](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): indeholder handlinger til at få aggregerede omkostnings-og brugsdata baseret på den forespørgsel, du angiver. Ved hjælp af forespørgsels-API'ET kan du angive den ønskede filtrering, sortering og gruppering på alle tilgængelige dimensioner (som fås adgang til fra dimensionerne API).

**Budgetterede omkostninger**

**Hvorfor kan jeg ikke se prognoser for mine omkostninger i omkostningsanalyse?**  
Der er flere årsager til, at prognose projiceringen mangler for dig i omkostningsanalyse, men nogle af dem er som følger:

1. Hvis dine omkostningsoplysninger er mindre end 10 dage gamle, bliver prognose diagrammet ikke indlæst. Modellen kræver mindst 10 dage af de seneste omkostningsdata for nøjagtige projektioner
2. Hvis du har valgt historiske datoer, vil prognose diagrammet ikke være synligt. Vælg et datointerval med fremtidige datoer, hvor prognose diagrammet skal vises
3. Hvis din konto har flere valutaer, er prognose diagrammet kun projektomkostninger for alle omkostninger i DKK

**Hvorfor ændres prognosen ikke, når jeg foretager ændringer i mine ressourcer?**  
Prognosemodellen kræver et par dage til at redegøre for ændringer på kontoen og laver ikke umiddelbare prognoser baseret på ændringer i ressourcer  
Hvis du vil have flere trin til at øge eller mindske ressourcer, tager modellen lidt længere tid for at justere til disse ændringer, så de stemmer overens med hensyn til afvigelser

**Hvorfor stiger min prognose, efter jeg har foretaget en reservation eller et markedsplads køb?**  
Prognosemodellen tager højde for dine faktiske omkostninger og tager ikke hensyn til forbrug og Køb separat. Hvis der er købt én gang, vil modellen reducere afgangen efter 10 dage for at tage højde for den pludselige stigning i omkostningerne

**Jeg vil se prognoser for en enkelt dimension (f. eks. Måler**  
Prognose understøtter i øjeblikket de samlede omkostningsprojekter og ikke for individuelle målere. Derfor vil projekterne blive samlet for alle elementer i dimensionen, når ' grupperet efter ' en dimension

**Anbefalede dokumenter**

- [Hvad er Azure cost management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [De bedste fremgangsmåder for omkostningsstyring i Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysér dine omkostninger og forbrug](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Udforsk og analysér omkostninger med omkostningsanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure cost management: priser](https://azure.microsoft.com/services/cost-management/#pricing)
- [Gennemse omkostninger i omkostningsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video selvstudium: oprette et budget i Azure-portalen](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Forudsætninger for at få vist og tilpasse budgetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Oprette og administrere budgetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurere automatisering med Azure-handlings grupper og budget-API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Brug af omkostnings beskeder til at overvåge forbrug og forbrug](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bedste fremgangsmåder for omkostningsstyring](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videoer med selvstudier**

- [Oprette et budget i Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrere omkostninger med budgetterne API og handlings grupperne](https://go.microsoft.com/fwlink/?linkid=2147038)