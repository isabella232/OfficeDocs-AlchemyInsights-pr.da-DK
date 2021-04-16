---
title: Aktivér tilbageførsel af adgangskode i Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814006"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="a6d1a-102">Aktivér tilbageførsel af adgangskode i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a6d1a-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="a6d1a-103">Hvis du vil aktivere selvbetjening til nulstilling af adgangskode, skal du først aktivere indstillingen tilbageførsel i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="a6d1a-104">Fra Azure AD Connect-serveren skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="a6d1a-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="a6d1a-105">Log på din Azure AD Connect-server, og start **konfigurationsguiden til Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="a6d1a-106">På siden **Velkommen skal** du klikke på **Konfigurer.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="a6d1a-107">På siden **Yderligere opgaver skal** du vælge Tilpas **synkroniseringsindstillinger** og derefter klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="a6d1a-108">På siden **Opret forbindelse til Azure AD** skal du angive legitimationsoplysninger som global administrator for din Azure-lejer og derefter klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="a6d1a-109">På siderne **Forbind kataloger** **og Domæne/OU-filtrering** skal du klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="a6d1a-110">På siden **Valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **Tilbageførsel af adgangskode og** klikke på **Næste.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="a6d1a-111">Klik på **Konfigurer på siden** Klar til konfiguration, og vent på, at processen afsluttes. </span><span class="sxs-lookup"><span data-stu-id="a6d1a-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="a6d1a-112">Når du ser konfigurationen færdig, skal du klikke på **Afslut.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="a6d1a-113">Med tilbageførsel af adgangskode aktiveret i Azure AD Connect skal du konfigurere Azure AD SSPR til tilbageførsel.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="a6d1a-114">Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="a6d1a-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="a6d1a-115">Log på Azure-portalen med en global administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="a6d1a-116">Søg efter og vælg **Azure Active Directory**, klik på **Nulstil adgangskode**, og klik derefter på Integration i det lokale **miljø**.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="a6d1a-117">Angiv indstillingen for **Tilbageskrivning af adgangskoder til din lokale mappe?** til **Ja.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="a6d1a-118">Angiv indstillingen tillad brugere **at låse konti op uden at nulstille deres adgangskode?** til **Ja.**</span><span class="sxs-lookup"><span data-stu-id="a6d1a-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="a6d1a-119">Når du er klar, skal du klikke **på Gem**.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-119">When ready, click **Save**.</span></span>

<span data-ttu-id="a6d1a-120">Få mere at vide under [Aktivér tilbageførsel](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)af adgangskode til nulstilling af adgangskode til Azure Active Directory i et lokalt miljø.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="a6d1a-121">Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og den pågældende bruger er organisationsnetværks- eller adgangskodehash synkroniseret, skrives adgangskoden tilbage til det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="a6d1a-122">Denne funktionalitet kræver Azure Premium-licens (P1 eller P2) og understøttes ikke i øjeblikket i Office-administrationsportalen.</span><span class="sxs-lookup"><span data-stu-id="a6d1a-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
