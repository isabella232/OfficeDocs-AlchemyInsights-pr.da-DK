---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910926"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="7a7c3-102">Føje eksterne brugere til en distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="7a7c3-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="7a7c3-103">Tilføjelse af en ekstern kontakt til en distributionsgruppe (DG) er en totrinsproces:</span><span class="sxs-lookup"><span data-stu-id="7a7c3-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="7a7c3-104">Opret en mailkontaktperson for den eksterne bruger:</span><span class="sxs-lookup"><span data-stu-id="7a7c3-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="7a7c3-105">Gå til siden **Brugere** > [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i Administration.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="7a7c3-106">Vælg **Tilføj en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="7a7c3-107">Skriv oplysningerne til kontaktpersonen, og vælg **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="7a7c3-108">Føj mailkontakten til dit generaldirektorat:</span><span class="sxs-lookup"><span data-stu-id="7a7c3-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="7a7c3-109">Gå til siden Grupper **i** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) Administration.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="7a7c3-110">Find det Dg, du vil føje den eksterne bruger til, og vælg det for at åbne dialogboksen Rediger.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="7a7c3-111">Vælg Vis alle **og administrer medlemmer**under fanen **Medlemmer** .</span><span class="sxs-lookup"><span data-stu-id="7a7c3-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="7a7c3-112">Vælg **Tilføj medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="7a7c3-113">Vælg den mailkontakt, du oprettede i forrige trin, og vælg derefter **Gem**.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="7a7c3-114">Hvis dine eksterne brugere efter at have fulgt disse trin ikke kan sende e-mails til generaldirektoratet eller ikke modtager e-mails fra det, kan det skyldes, at gD'et er markeret, så de kun tillader e-mails fra interne brugere.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="7a7c3-115">Du kan kontrollere denne konfiguration og rette den efter anvisningerne [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="7a7c3-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="7a7c3-116">**Bemærk:** Disse instruktioner gælder ikke, hvis gruppens type er "Microsoft 365-gruppe" i stedet for "Distributionsgruppe".</span><span class="sxs-lookup"><span data-stu-id="7a7c3-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="7a7c3-117">Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook.</span><span class="sxs-lookup"><span data-stu-id="7a7c3-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="7a7c3-118">Detaljerede oplysninger om gæster i Microsoft 365 Grupper samt instruktioner til tilføjelse af eksterne gæster findes i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="7a7c3-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  