---
title: Aktivere tilbageførsel af adgangskode i Azure AD Connect
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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709721"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="cd128-102">Aktivere tilbageførsel af adgangskode i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="cd128-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="cd128-103">Hvis du vil aktivere tilbageførsel af adgangskode for selvbetjening, skal du først aktivere indstillingen tilbageskrivning i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="cd128-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="cd128-104">I Azure AD Connect-serveren skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="cd128-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="cd128-105">Log på din Azure AD Connect-server, og Start guiden **Azure ad Connect** Configuration.</span><span class="sxs-lookup"><span data-stu-id="cd128-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="cd128-106">Klik på **Konfigurer**på siden **Velkommen** .</span><span class="sxs-lookup"><span data-stu-id="cd128-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="cd128-107">Vælg **Tilpas synkroniseringsindstillinger**på siden **flere opgaver** , og klik derefter på **næste**.</span><span class="sxs-lookup"><span data-stu-id="cd128-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="cd128-108">På siden **Opret forbindelse til Azure ad** skal du angive en global administrators legitimationsoplysninger for din Azure-lejer, og derefter skal du klikke på næste.</span><span class="sxs-lookup"><span data-stu-id="cd128-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="cd128-109">Klik på **næste**på siden **Opret forbindelse til mapper** og **domæne/ou** -filtrering.</span><span class="sxs-lookup"><span data-stu-id="cd128-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="cd128-110">På siden **valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **adgangskode tilbageførsel** og klikke på **næste**.</span><span class="sxs-lookup"><span data-stu-id="cd128-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="cd128-111">På siden **klar til at konfigurere** skal du klikke på **Konfigurer** og vente på, at processen afsluttes.</span><span class="sxs-lookup"><span data-stu-id="cd128-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="cd128-112">Når du får vist konfigurations slutdatoen, skal du klikke på **Afslut**.</span><span class="sxs-lookup"><span data-stu-id="cd128-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="cd128-113">Når tilbageførsel af adgangskode er aktiveret i Azure AD Connect, skal du nu konfigurere Azure AD SSPR for tilbageførsel.</span><span class="sxs-lookup"><span data-stu-id="cd128-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="cd128-114">Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="cd128-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="cd128-115">Log på Azure-portalen ved hjælp af en global administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="cd128-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="cd128-116">Søg efter og vælg **Azure Active Directory**, klik på **Nulstil adgangskode**, og vælg derefter **lokal integration**.</span><span class="sxs-lookup"><span data-stu-id="cd128-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="cd128-117">Angiv indstillingen for **skrivning af adgangskoder til din lokale adresseliste?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="cd128-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="cd128-118">Angiv indstillingen for **Tillad brugere at låse konti op uden at nulstille deres adgangskode?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="cd128-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="cd128-119">Klik på **Gem**, når du er klar.</span><span class="sxs-lookup"><span data-stu-id="cd128-119">When ready, click **Save**.</span></span>

<span data-ttu-id="cd128-120">Hvis du vil have mere at vide, skal du se [aktivere tilbageførsel af Active Directory-selvbetjenings funktionen til nulstilling af adgangskode til et lokalt miljø](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="cd128-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
