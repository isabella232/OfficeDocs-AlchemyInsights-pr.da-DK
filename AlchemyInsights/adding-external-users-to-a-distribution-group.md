---
title: Føje eksterne brugere til en distributionsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663507"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="5f707-102">Føje eksterne brugere til en distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="5f707-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="5f707-103">Tilføjelse af en ekstern kontakt til en distributionsgruppe er en proces i to trin:</span><span class="sxs-lookup"><span data-stu-id="5f707-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="5f707-104">Opret en mail kontakt for den eksterne bruger:</span><span class="sxs-lookup"><span data-stu-id="5f707-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="5f707-105">I administration skal du gå til siden med **Users**  >  [Kontaktpersoner](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="5f707-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="5f707-106">Vælg **Tilføj en kontaktperson**.</span><span class="sxs-lookup"><span data-stu-id="5f707-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="5f707-107">Skriv oplysningerne for kontakten, og vælg **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="5f707-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="5f707-108">Føj mail kontakten til din DG:</span><span class="sxs-lookup"><span data-stu-id="5f707-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="5f707-109">I administration skal du gå til siden **grupper**-  >  [grupper](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="5f707-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="5f707-110">Find den DG, du vil føje den eksterne bruger til, og vælg den for at åbne dialogboksen Rediger.</span><span class="sxs-lookup"><span data-stu-id="5f707-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="5f707-111">På fanen **medlemmer** skal du vælge **Vis alle og Administrer medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="5f707-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="5f707-112">Vælg **Tilføj medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="5f707-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="5f707-113">Vælg den mail kontakt, du oprettede på det forrige trin, og vælg derefter **Gem**.</span><span class="sxs-lookup"><span data-stu-id="5f707-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="5f707-114">Hvis dine eksterne brugere efter at have fulgt disse trin ikke kan sende mails til DG eller ikke modtager mails fra den, kan det være, at DG er markeret til kun at tillade mails fra interne brugere.</span><span class="sxs-lookup"><span data-stu-id="5f707-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="5f707-115">Du kan kontrollere denne konfiguration og rette den ved at følge vejledningen [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="5f707-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="5f707-116">**Bemærk:** Disse instruktioner gælder ikke, hvis din gruppes type er "Microsoft 365-gruppe" i stedet for "distributionsgruppe".</span><span class="sxs-lookup"><span data-stu-id="5f707-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="5f707-117">Hvis det er tilfældet, kan du føje den eksterne bruger direkte til gruppen fra Outlook.</span><span class="sxs-lookup"><span data-stu-id="5f707-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="5f707-118">Du kan finde detaljerede oplysninger om Microsoft 365-grupper gæster samt instruktioner til at tilføje eksterne gæster i [denne artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="5f707-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  