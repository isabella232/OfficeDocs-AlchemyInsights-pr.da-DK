---
title: Privilegeret identitets styrings rolle
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088677"
---
# <a name="privileged-identity-managementpim-role"></a>PIM-rolle (Privileged Identity Management)

**Tilladelser tildeles ikke efter aktivering af en rolle**

Når du aktiverer en rolle i Azure AD privilegeret Identity Management (PIM), er aktiveringen muligvis ikke øjeblikkeligt overført til alle portaler, der kræver en privilegeret rolle. Nogle gange, selvom ændringen overføres, kan webcaching i en portal resultere i, at ændringen ikke træder i kraft med det samme.

Hvis din aktivering er forsinket, skal du følge disse trin:

1. Log af Azure-portalen, og log derefter på igen. Når du aktiverer en Azure AD-rolle eller en Azure-ressource rolle, får du vist faserne i din aktivering. Når alle faser er fuldført, får du vist linket "Log af". Du kan bruge dette link til at logge af. Dette løser de fleste tilfælde, hvor forsinkelsen er aktiveret.
2. Kontrollér, at du er angivet som medlem af rollen i PIM-program.
3. Hvis du aktiverer Exchange-administrator rollen, skal du kontrollere, at du logger af og logger på igen. Hvis problemet fortsætter, skal du åbne en supportanmodning og hæve dette som et problem. Hvis du bruger din Exchange-administrator rolle til at få adgang til sikkerheds-og overholdelses Center, skal du se næste trin.
4. Hvis du aktiverer en rolle for at få adgang til sikkerheds-og overholdelses Center, eller hvis du aktiverer SharePoint-administrator rollen, oplever du en vis ventetid fra et par minutter op til et par timer. Dette er et kendt problem, og vi arbejder aktivt sammen med disse teams for at løse problemet så hurtigt som muligt.

Du kan finde flere oplysninger under:

- [Aktivere mine Azure AD-roller i PIM-program](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivere mine Azure-ressource roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Tilladelser fjernes ikke, efter at du har deaktiveret en rolle, eller rolle aktiveringen udløber**

Når du deaktiverer en rolle i Azure AD privilegeret identitetsstyring, eller når en rolle aktiveringsperiode udløber, kan der være en forsinkelse, hvor du fortsat har adgang.

Hvis deaktiveringen forsinkes, skal du følge disse trin:

1. Hvis du deaktiverer Exchange-administrator rollen, eller hvis aktiveringsperioden for roller udløber, og du bemærker en alvorlig forsinkelse, før tilladelserne fjernes, skal du åbne en supportanmodning og bede din supporttekniker om at hjælpe dig med at arkivere en billet med det PAM-team (privilegeret Access Management) i Office om dette problem.
2. Hvis aktiveringsperioden er udløbet, men du stadig har browsersessionen åben, skal du lukke din browser. Du kan fortsætte med at bruge rollen, indtil du lukker sessionen. Dette er et kendt problem, og vi kigger på en mulig løsning for aktivt at tilbagekalde hver session, når aktiveringen er udløbet.

Hvis din forsinkelse er anderledes end disse to scenarier, skal du åbne en supportanmodning.
