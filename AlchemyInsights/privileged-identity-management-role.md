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
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="eb93c-102">PIM-rolle (Privileged Identity Management)</span><span class="sxs-lookup"><span data-stu-id="eb93c-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="eb93c-103">**Tilladelser tildeles ikke efter aktivering af en rolle**</span><span class="sxs-lookup"><span data-stu-id="eb93c-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="eb93c-104">Når du aktiverer en rolle i Azure AD privilegeret Identity Management (PIM), er aktiveringen muligvis ikke øjeblikkeligt overført til alle portaler, der kræver en privilegeret rolle.</span><span class="sxs-lookup"><span data-stu-id="eb93c-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="eb93c-105">Nogle gange, selvom ændringen overføres, kan webcaching i en portal resultere i, at ændringen ikke træder i kraft med det samme.</span><span class="sxs-lookup"><span data-stu-id="eb93c-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="eb93c-106">Hvis din aktivering er forsinket, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="eb93c-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="eb93c-107">Log af Azure-portalen, og log derefter på igen.</span><span class="sxs-lookup"><span data-stu-id="eb93c-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="eb93c-108">Når du aktiverer en Azure AD-rolle eller en Azure-ressource rolle, får du vist faserne i din aktivering.</span><span class="sxs-lookup"><span data-stu-id="eb93c-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="eb93c-109">Når alle faser er fuldført, får du vist linket "Log af".</span><span class="sxs-lookup"><span data-stu-id="eb93c-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="eb93c-110">Du kan bruge dette link til at logge af. Dette løser de fleste tilfælde, hvor forsinkelsen er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="eb93c-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="eb93c-111">Kontrollér, at du er angivet som medlem af rollen i PIM-program.</span><span class="sxs-lookup"><span data-stu-id="eb93c-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="eb93c-112">Hvis du aktiverer Exchange-administrator rollen, skal du kontrollere, at du logger af og logger på igen.</span><span class="sxs-lookup"><span data-stu-id="eb93c-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="eb93c-113">Hvis problemet fortsætter, skal du åbne en supportanmodning og hæve dette som et problem.</span><span class="sxs-lookup"><span data-stu-id="eb93c-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="eb93c-114">Hvis du bruger din Exchange-administrator rolle til at få adgang til sikkerheds-og overholdelses Center, skal du se næste trin.</span><span class="sxs-lookup"><span data-stu-id="eb93c-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="eb93c-115">Hvis du aktiverer en rolle for at få adgang til sikkerheds-og overholdelses Center, eller hvis du aktiverer SharePoint-administrator rollen, oplever du en vis ventetid fra et par minutter op til et par timer.</span><span class="sxs-lookup"><span data-stu-id="eb93c-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="eb93c-116">Dette er et kendt problem, og vi arbejder aktivt sammen med disse teams for at løse problemet så hurtigt som muligt.</span><span class="sxs-lookup"><span data-stu-id="eb93c-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="eb93c-117">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="eb93c-117">For more information, see:</span></span>

- [<span data-ttu-id="eb93c-118">Aktivere mine Azure AD-roller i PIM-program</span><span class="sxs-lookup"><span data-stu-id="eb93c-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="eb93c-119">Aktivere mine Azure-ressource roller i PIM</span><span class="sxs-lookup"><span data-stu-id="eb93c-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="eb93c-120">**Tilladelser fjernes ikke, efter at du har deaktiveret en rolle, eller rolle aktiveringen udløber**</span><span class="sxs-lookup"><span data-stu-id="eb93c-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="eb93c-121">Når du deaktiverer en rolle i Azure AD privilegeret identitetsstyring, eller når en rolle aktiveringsperiode udløber, kan der være en forsinkelse, hvor du fortsat har adgang.</span><span class="sxs-lookup"><span data-stu-id="eb93c-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="eb93c-122">Hvis deaktiveringen forsinkes, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="eb93c-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="eb93c-123">Hvis du deaktiverer Exchange-administrator rollen, eller hvis aktiveringsperioden for roller udløber, og du bemærker en alvorlig forsinkelse, før tilladelserne fjernes, skal du åbne en supportanmodning og bede din supporttekniker om at hjælpe dig med at arkivere en billet med det PAM-team (privilegeret Access Management) i Office om dette problem.</span><span class="sxs-lookup"><span data-stu-id="eb93c-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="eb93c-124">Hvis aktiveringsperioden er udløbet, men du stadig har browsersessionen åben, skal du lukke din browser.</span><span class="sxs-lookup"><span data-stu-id="eb93c-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="eb93c-125">Du kan fortsætte med at bruge rollen, indtil du lukker sessionen.</span><span class="sxs-lookup"><span data-stu-id="eb93c-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="eb93c-126">Dette er et kendt problem, og vi kigger på en mulig løsning for aktivt at tilbagekalde hver session, når aktiveringen er udløbet.</span><span class="sxs-lookup"><span data-stu-id="eb93c-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="eb93c-127">Hvis din forsinkelse er anderledes end disse to scenarier, skal du åbne en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="eb93c-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
