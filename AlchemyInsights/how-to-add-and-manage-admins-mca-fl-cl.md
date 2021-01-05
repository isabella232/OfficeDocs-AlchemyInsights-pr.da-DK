---
title: Sådan tilføjer og administrerer du administratorer
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755433"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="be59e-102">Sådan tilføjer og administrerer du administratorer</span><span class="sxs-lookup"><span data-stu-id="be59e-102">How to add and manage admins</span></span>

<span data-ttu-id="be59e-103">Afhængigt af din problembeskrivelse har vi fundet en løsning til dig.</span><span class="sxs-lookup"><span data-stu-id="be59e-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="be59e-104">De fleste kunder har kunnet løse deres problemer efter eget efter at have fulgt vores dokumentation.</span><span class="sxs-lookup"><span data-stu-id="be59e-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="be59e-105">Hvis du vil administrere din faktureringskonto for en Microsoft-kunde aftale (MCA), kan du bruge forskellige roller med det ønskede adgangsniveau.</span><span class="sxs-lookup"><span data-stu-id="be59e-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="be59e-106">Disse roller er sammen med de indbyggede Azure-tjeneste roller, der hjælper dig med at styre dine ressourcer.</span><span class="sxs-lookup"><span data-stu-id="be59e-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="be59e-107">**Sådan tilføjes fakturerings roller i Azure-portalen:**</span><span class="sxs-lookup"><span data-stu-id="be59e-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="be59e-108">Log på Azure- [portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="be59e-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="be59e-109">Søg efter *omkostningsstyring + fakturering*.</span><span class="sxs-lookup"><span data-stu-id="be59e-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="be59e-110">Vælg adgangskontrol (IAM) i et område som f. eks faktureringskonto, fakturerings profil eller faktura sektion, hvor du vil give adgang.</span><span class="sxs-lookup"><span data-stu-id="be59e-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="be59e-111">På siden adgangskontrol (IAM) vises de brugere og grupper, der er tildelt hver rolle for det pågældende område.</span><span class="sxs-lookup"><span data-stu-id="be59e-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="be59e-112">Hvis du vil give adgang til en bruger, skal du vælge **Tilføj** fra toppen af siden.</span><span class="sxs-lookup"><span data-stu-id="be59e-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="be59e-113">Vælg en rolle på rullelisten *rolle* .</span><span class="sxs-lookup"><span data-stu-id="be59e-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="be59e-114">Indtast mailadressen på den bruger, du vil give adgang.</span><span class="sxs-lookup"><span data-stu-id="be59e-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="be59e-115">Vælg **Gem** for at tildele rollen.</span><span class="sxs-lookup"><span data-stu-id="be59e-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="be59e-116">Hvis du vil fjerne adgang for en bruger, skal du vælge brugeren med den rolletildeling, du vil fjerne.</span><span class="sxs-lookup"><span data-stu-id="be59e-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="be59e-117">Vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="be59e-117">Select **Remove**.</span></span>

<span data-ttu-id="be59e-118">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="be59e-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="be59e-119">Definitioner af fakturerings rolle</span><span class="sxs-lookup"><span data-stu-id="be59e-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="be59e-120">Faktureringskonto roller og opgaver</span><span class="sxs-lookup"><span data-stu-id="be59e-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="be59e-121">Kom godt i gang med din MCA-faktureringskonto</span><span class="sxs-lookup"><span data-stu-id="be59e-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="be59e-122">Kontrollér adgang til en Microsoft-kunde aftale</span><span class="sxs-lookup"><span data-stu-id="be59e-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
