---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737867"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="627b9-102">Føje eksterne brugere til en distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="627b9-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="627b9-103">Tilføjelse af en ekstern kontakt til en distributionsgruppe (DG) er en proces i to trin:</span><span class="sxs-lookup"><span data-stu-id="627b9-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="627b9-104">Opret en e-mail-kontakt for den eksterne bruger:</span><span class="sxs-lookup"><span data-stu-id="627b9-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="627b9-105">Gå til siden **brugere** > [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) i Admin Center.</span><span class="sxs-lookup"><span data-stu-id="627b9-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="627b9-106">Vælg **Tilføj en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="627b9-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="627b9-107">Skriv oplysningerne for kontakten, og vælg **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="627b9-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="627b9-108">Føj e-mail-kontakten til dit Generaldirektorat:</span><span class="sxs-lookup"><span data-stu-id="627b9-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="627b9-109">Gå til siden **grupper** > [grupper](https://admin.microsoft.com/adminportal/home#/groups) i Admin Center.</span><span class="sxs-lookup"><span data-stu-id="627b9-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="627b9-110">Find det generaldirektorat, du vil føje den eksterne bruger til, og vælg det for at åbne redigeringsdialogen.</span><span class="sxs-lookup"><span data-stu-id="627b9-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="627b9-111">Under fanen **medlemmer** skal du vælge **Vis alle og Administrer medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="627b9-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="627b9-112">Vælg **Tilføj medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="627b9-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="627b9-113">Vælg den mail kontakt, du oprettede på det forrige trin, og vælg derefter **Gem**.</span><span class="sxs-lookup"><span data-stu-id="627b9-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="627b9-114">Hvis efterfølgende trin dine eksterne brugere ikke kan sende e-mails til Generaldirektoratet eller ikke modtager e-mails fra det, kan det være, at Generaldirektoratet er markeret til kun at tillade e-mails fra interne brugere.</span><span class="sxs-lookup"><span data-stu-id="627b9-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="627b9-115">Du kan kontrollere denne konfiguration og ordne det efter anvisningerne [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="627b9-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="627b9-116">**Bemærk:** Disse instruktioner gælder ikke, hvis gruppens type er "Office 365 Group" i stedet for "distributionsgruppe".</span><span class="sxs-lookup"><span data-stu-id="627b9-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="627b9-117">Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook.</span><span class="sxs-lookup"><span data-stu-id="627b9-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="627b9-118">Detaljerede oplysninger om Office 365-grupper gæster samt instruktioner til tilføjelse af eksterne Gæster kan findes i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="627b9-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  