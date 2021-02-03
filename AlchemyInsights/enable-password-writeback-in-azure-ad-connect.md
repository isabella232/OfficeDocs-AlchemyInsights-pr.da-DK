---
title: Aktivér tilbageførsel af adgangskode i Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093349"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e70a8-102">Aktivér tilbageførsel af adgangskode i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e70a8-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e70a8-103">Hvis du vil aktivere selvbetjening til nulstilling af adgangskode, skal du først aktivere indstillingen tilbageførsel i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e70a8-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e70a8-104">Fra azure AD Connect-serveren skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="e70a8-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e70a8-105">Log på din Azure AD Connect-server, og start **konfigurationsguiden til Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e70a8-106">Klik på **Konfigurer** på **velkomstsiden.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e70a8-107">Vælg Tilpas **synkroniseringsindstillinger** på siden Yderligere **opgaver,** og klik derefter på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e70a8-108">På siden **Opret forbindelse til Azure AD** skal du angive en global administratorlegitimationsoplysninger for din Azure-lejer og derefter klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e70a8-109">Klik på **Næste på filtreringssiderne** Forbind mapper og **Domæne/OU.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e70a8-110">På siden **Valgfrie funktioner** skal du markere feltet ud for tilbageførsel **af adgangskode og** klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e70a8-111">Klik på **Konfigurer på siden** Klar til konfiguration, **og** vent på, at processen afsluttes.</span><span class="sxs-lookup"><span data-stu-id="e70a8-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e70a8-112">Klik på Afslut, når konfigurationen **er færdig.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e70a8-113">Med tilbageførsel af adgangskode aktiveret i Azure AD Connect skal du konfigurere Azure AD SSPR til tilbageførsel.</span><span class="sxs-lookup"><span data-stu-id="e70a8-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e70a8-114">Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="e70a8-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e70a8-115">Log på Azure-portalen med en global administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="e70a8-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e70a8-116">Søg efter og vælg **Azure Active Directory,** klik på **Nulstil adgangskode,** og **klik derefter på integration i det lokale miljø.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e70a8-117">Angiv indstillingen for **Tilbageskrivning af adgangskoder til dit lokale katalog?** til **Ja.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e70a8-118">Angiv indstillingen for Tillad **brugere at låse konti op uden at nulstille deres adgangskode?** til **Ja.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e70a8-119">Klik på Gem, når du **er klar.**</span><span class="sxs-lookup"><span data-stu-id="e70a8-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e70a8-120">Du kan finde flere oplysninger [i Aktivere tilbageførsel af adgangskode til](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)Azure Active Directory til selvbetjening til nulstilling af adgangskode i et lokalt miljø.</span><span class="sxs-lookup"><span data-stu-id="e70a8-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e70a8-121">Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og den pågældende bruger er synkroniseret med organisationsnetværket eller adgangskodehash, skrives adgangskoden tilbage til det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="e70a8-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e70a8-122">Denne funktionalitet kræver Azure Premium-licens (P1 eller P2) og understøttes i øjeblikket ikke i Office-administrationsportalen.</span><span class="sxs-lookup"><span data-stu-id="e70a8-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
