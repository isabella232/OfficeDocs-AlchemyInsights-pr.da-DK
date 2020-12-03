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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560434"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="30f33-102">Aktivere tilbageførsel af adgangskode i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="30f33-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="30f33-103">Hvis du vil aktivere tilbageførsel af adgangskode for selvbetjening, skal du først aktivere indstillingen tilbageskrivning i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="30f33-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="30f33-104">I Azure AD Connect-serveren skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="30f33-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="30f33-105">Log på din Azure AD Connect-server, og Start guiden **Azure ad Connect** Configuration.</span><span class="sxs-lookup"><span data-stu-id="30f33-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="30f33-106">Klik på **Konfigurer** på siden **Velkommen** .</span><span class="sxs-lookup"><span data-stu-id="30f33-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="30f33-107">Vælg **Tilpas synkroniseringsindstillinger** på siden **flere opgaver** , og klik derefter på **næste**.</span><span class="sxs-lookup"><span data-stu-id="30f33-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="30f33-108">På siden **Opret forbindelse til Azure ad** skal du angive en global administrators legitimationsoplysninger for din Azure-lejer, og derefter skal du klikke på **næste**.</span><span class="sxs-lookup"><span data-stu-id="30f33-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="30f33-109">Klik på **næste** på siden **Opret forbindelse til mapper** og **domæne/ou** -filtrering.</span><span class="sxs-lookup"><span data-stu-id="30f33-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="30f33-110">På siden **valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **adgangskode tilbageførsel** og klikke på **næste**.</span><span class="sxs-lookup"><span data-stu-id="30f33-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="30f33-111">På siden **klar til at konfigurere** skal du klikke på **Konfigurer** og vente på, at processen afsluttes.</span><span class="sxs-lookup"><span data-stu-id="30f33-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="30f33-112">Når du får vist konfigurations slutdatoen, skal du klikke på **Afslut**.</span><span class="sxs-lookup"><span data-stu-id="30f33-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="30f33-113">Når tilbageførsel af adgangskode er aktiveret i Azure AD Connect, skal du konfigurere Azure AD SSPR for tilbageførsel.</span><span class="sxs-lookup"><span data-stu-id="30f33-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="30f33-114">Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="30f33-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="30f33-115">Log på Azure-portalen ved hjælp af en global administratorkonto.</span><span class="sxs-lookup"><span data-stu-id="30f33-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="30f33-116">Søg efter og vælg **Azure Active Directory**, klik på **nulstilling af adgangskode**, og klik derefter på **lokal integration**.</span><span class="sxs-lookup"><span data-stu-id="30f33-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="30f33-117">Angiv indstillingen for **skrivning af adgangskoder til din lokale adresseliste?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="30f33-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="30f33-118">Angiv indstillingen for **Tillad brugere at låse konti op uden at nulstille deres adgangskode?** til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="30f33-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="30f33-119">Klik på **Gem**, når du er klar.</span><span class="sxs-lookup"><span data-stu-id="30f33-119">When ready, click **Save**.</span></span>

<span data-ttu-id="30f33-120">Hvis du vil have mere at vide, skal du se [aktivere tilbageførsel af Active Directory-selvbetjenings funktionen til nulstilling af adgangskode til et lokalt miljø](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="30f33-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="30f33-121">Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og hvis den pågældende bruger er sammenkædet med en adgangskode, der er synkroniseret, skrives adgangskoden tilbage til det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="30f33-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="30f33-122">Denne funktion understøttes i øjeblikket ikke i Office-administratorportalen.</span><span class="sxs-lookup"><span data-stu-id="30f33-122">This functionality is currently not supported in the Office Admin portal.</span></span>