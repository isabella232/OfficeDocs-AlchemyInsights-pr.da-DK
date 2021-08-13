---
title: Hvorfor er knappen Tilføj budget deaktiveret for mig?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954659"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Hvorfor er knappen Tilføj budget deaktiveret for mig?

Hvis du vil oprette et budget, skal du have en af følgende tilladelser:

- Administrationsgruppe, Abonnement, Ressourcegruppeomfang
- Bidragyder til omkostningsstyring
- Ejer
- Bidragyder
- Kun enterprise-kunde: Registrering, afdeling, kontoomfang
- Tilmeldingsadministrator (angiv budget for registreringsområde)
- Afdelingsadministrator (angiv budget for området Afdeling)
- Kontoejer (angiv budget i kontoområde)
- Kun moderne kundeaftale: Faktureringskonto, faktureringsprofil, fakturasektionens omfang
- Azure-abonnementsopretter

**Jeg har oprettet et budget, når omkostningerne for den aktuelle måned allerede var overbudgettet. Hvorfor har jeg ikke modtaget en besked?**  
Hvis du allerede har overskredet en given omkostningstærskel, når du opretter et budget, udløses denne besked ikke. Når der startes en ny cyklus, udløses beskeden, hvis du ikke når tærskelværdien.

**Hvornår skal jeg forvente at modtage en besked, når jeg overskrider en af mine definerede grænseværdier for budgetadvarsler?**  
Der evalueres budgetter hver 4. time. Det tager minimum 8 timer, før forbrugsdata når budgetsystemet. På den måde kan det tage op til 12 timer, før beskederne udløses, efter at du har overskredet en grænseværdi.

**Hvorfor er knappen Startdato deaktiveret, når jeg vælger en nulstillingsperiode for måned eller faktureringsmåned?**  
Budgetter er justeret efter den aktuelle kalendermåned eller aktuelle faktureringsperiode (i tilfælde hvor Faktureringsmåned er valgt). Derfor udfylder vi denne værdi på forhånd for dig.

**Hvorfor kan jeg ikke se en graf over mine omkostninger i budgetoprettelsesoplevelsen?**  
Vi har brug for mindst 2 måneders omkostningsdata, før vi kan gengive en graf for at hjælpe dig med budgetoprettelsen.

**Hvorfor kan jeg ikke sætte et budget i forhold til et abonnement, jeg lige har oprettet?**  
Efter oprettelse af et abonnement tager det 24-48 timer, før dataene behandles, før du angiver et budget for det.

**Budget API-ressourcer**

- [Budget API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Indeholder handlinger til oprettelse og opdatering af budgetter. Ved hjælp af budget-API'en kan du angive en budgettærskel og konfigurere flere vigtige beskeder, så de udløses, når du nærmer dig denne grænse. Beskeder kan udløse en mail eller en Azure-handlingsgruppe for at udføre automatisering. Bemærk! Filtrering af denne API passer ikke til forespørgsels-API-filtrering/-dimensioner.
- [Budget API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Opret budgetter med større muligheder for omkostningsfiltrering end v1. Filtrering er justeret i forhold til den kontrakt, der bruges i vores API'er forespørgsel og dimensioner. Dette er API'en med anbefalede budgetter, som du kan bruge fremover.
- [Dimensioner:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Indeholder handlinger, der kan bruges til at få understøttede dimensioner til dit brug under en række forskellige områder. Ved hjælp af dimensions-API'en kan du hente en liste over dimensioner, der kan bruges som input til at generere forespørgsler med forespørgsels-API'en.
- [Forespørgsel:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Indeholder handlinger, der henter aggregerede omkostnings- og forbrugsdata baseret på den forespørgsel, du angiver. Ved hjælp af forespørgsels-API'en kan du angive den ønskede filtrering, sortering og gruppering efter alle tilgængelige dimensioner (som tilgås via dimensions-API'en).

**Forventede omkostninger**

**Hvorfor kan jeg ikke se prognoser for mine omkostninger i Omkostningsanalyse?**  
Der kan være flere årsager til, at prognoseprojektionen mangler for dig i Omkostningsanalyse, og nogle af dem er som følger:

1. Hvis dine omkostningsdata er mindre end 10 dage gamle, indlæses prognosediagrammet ikke. Modellen kræver mindst 10 dages seneste omkostningsdata for nøjagtige prognoser
2. Hvis du har valgt historiske datoer, vil prognosediagrammet ikke være synligt. Vælg et datointerval med fremtidige datoer, som prognosediagrammet skal vises i
3. Hvis din konto har flere valutaer, vil prognosediagrammet kun projektomkostningerne for "Alle omkostninger i USD"

**Hvorfor ændres prognosen ikke, når jeg foretager ændringer i mine ressourcer?**  
Prognosemodellen kræver et par dage, før der tages højde for ændringer i kontoen, og der foretages ikke øjeblikkelige prognoser baseret på ændringer i ressourcer  
Ved større trin med større eller mindre ressourcer vil modellen tage lidt længere tid at tilpasse sig disse ændringer for at tage højde for anomomier

**Hvorfor øges min prognose, når jeg foretager et reservationskøb eller foretager et Marketplace-køb?**  
Prognosemodellen tager højde for dine "Faktiske omkostninger" og tager ikke højde for brug og køb separat. Ved et engangskøb vil modellen reducere projektionerne efter 10 dage for at tage højde for den pludselige stigning i omkostningerne

**Jeg vil se prognoser for en enkelt dimension (f.eks. Meter)**  
Prognosen understøtter i øjeblikket de samlede omkostninger og ikke for individuelle meter. Når der derfor er "Grupperet efter" en dimension, vil projektionerne være for totalen af alle elementer i dimensionen

**Anbefalede dokumenter**

- [Hvad er Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bedste fremgangsmåder for Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysér dine omkostninger og dit forbrug](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Udforsk og analysér omkostninger med omkostningsanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Priser](https://azure.microsoft.com/services/cost-management/#pricing)
- [Gennemse omkostninger i omkostningsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videoselstudium: Opret et budget i Azure-portalen](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Forudsætninger for visning og tilpasning af budgetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Opret og administrer budgetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurer automatisering med API'en Azure Action Groups and Budgets](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Brug omkostningsbeskeder til at overvåge forbrug og forbrug](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Bedste fremgangsmåder for omkostningsstyring](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Selvstudievideoer**

- [Opret et budget i Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrer omkostninger med budget-API og handlingsgrupper](https://go.microsoft.com/fwlink/?linkid=2147038)