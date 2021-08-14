---
title: Privileged Identity Management rolle
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973223"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)-rolle

**Tilladelser tildeles ikke efter aktivering af en rolle**

Når du aktiverer en rolle i Azure AD Privileged Identity Management (PIM), overføres aktiveringen muligvis ikke øjeblikkeligt til alle portaler, der kræver den privilegerede rolle. Nogle gange kan det medføre, at ændringen ikke træder i kraft med det samme, selvom ændringen overføres.

Hvis din aktivering forsinkes, skal du følge disse trin:

1. Log af Azure-portalen, og log derefter på igen. Når du aktiverer en Azure AD-rolle eller en Azure-ressourcerolle, kan du se faserne i din aktivering. Når alle trin er fuldført, får du vist linket "Log af". Du kan bruge dette link til at logge af. Dette løser de fleste tilfælde i forbindelse med aktiveringsforsinkelse.
2. I PIM skal du kontrollere, at du er angivet som medlem af rollen.
3. Hvis du aktiverer rollen Exchange administrator, skal du sørge for at logge af og logge på igen. Hvis problemet fortsætter, skal du åbne en supportbillet og rejse dette som et problem. Hvis du bruger din Exchange administratorrolle til at få adgang til Security and Compliance Center, skal du se næste trin.
4. Hvis du aktiverer en rolle for at få adgang til Security and Compliance Center, eller hvis du aktiverer SharePoint-administratorrollen, vil du opleve en aktiveringsforsinkelse fra et par minutter og op til et par timer. Dette er et kendt problem, og vi arbejder aktivt med disse teams for at løse problemet hurtigst muligt.

Du kan finde flere oplysninger under:

- [Aktivere mine Azure AD-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivér mine Azure-ressourceroller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Tilladelser fjernes ikke, når en rolle deaktiveres, eller rolleaktivering udløber**

Når du deaktiverer en rolle i Azure AD Privileged Identity Management, eller når en aktiveringsperiode for en rolle udløber, kan der være en forsinkelse, hvor du fortsat har adgang.

Hvis din deaktivering forsinkes, skal du følge disse trin:

1. Hvis du deaktiverer rollen Exchange-administrator, eller aktiveringsperioden for rollen udløber, og du bemærker en betydelig forsinkelse, før tilladelserne fjernes, skal du åbne en supportbillet og bede din supporttekniker om at hjælpe dig med at arkivere en billet hos pam-teamet (Privileged Access Management) i Office om dette problem.
2. Hvis aktiveringsperioden er udløbet, men du stadig har browsersessionen åben, skal du lukke browseren. Du kan fortsætte med at bruge rollen, indtil du lukker sessionen. Dette er et kendt problem, og vi kigger på en mulig løsning til aktivt at tilbagekalde hver session, når aktiveringen er udløbet.

Hvis din forsinkelse er anderledes end disse to scenarier, skal du åbne en supportanmodning.
