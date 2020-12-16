---
title: Sådan tilføjer og administrerer du administratorer-MCA FL/CL
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
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692014"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="9a6b6-102">Sådan tilføjer og administrerer du administratorer-MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="9a6b6-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="9a6b6-103">Hvis du vil administrere din faktureringskonto for en Microsoft-kunde aftale (MCA), kan du bruge forskellige roller med det ønskede adgangsniveau.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="9a6b6-104">Disse roller er sammen med de indbyggede Azure-tjeneste roller, der hjælper dig med at styre dine ressourcer.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="9a6b6-105">**Sådan tilføjes fakturerings roller i Azure-portalen:**</span><span class="sxs-lookup"><span data-stu-id="9a6b6-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="9a6b6-106">Log på Azure- [portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="9a6b6-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="9a6b6-107">Søg efter *omkostningsstyring + fakturering*.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="9a6b6-108">Vælg adgangskontrol (IAM) i et område som f. eks faktureringskonto, fakturerings profil eller faktura sektion, hvor du vil give adgang.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="9a6b6-109">På siden adgangskontrol (IAM) vises de brugere og grupper, der er tildelt hver rolle for det pågældende område.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="9a6b6-110">Hvis du vil give adgang til en bruger, skal du vælge **Tilføj** fra toppen af siden.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="9a6b6-111">Vælg en rolle på rullelisten *rolle* .</span><span class="sxs-lookup"><span data-stu-id="9a6b6-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="9a6b6-112">Indtast mailadressen på den bruger, du vil give adgang.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="9a6b6-113">Vælg **Gem** for at tildele rollen.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="9a6b6-114">Hvis du vil fjerne adgang for en bruger, skal du vælge brugeren med den rolletildeling, du vil fjerne.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="9a6b6-115">Vælg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="9a6b6-115">Select **Remove**.</span></span>

<span data-ttu-id="9a6b6-116">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="9a6b6-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="9a6b6-117">Definitioner af fakturerings rolle</span><span class="sxs-lookup"><span data-stu-id="9a6b6-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="9a6b6-118">Faktureringskonto roller og opgaver</span><span class="sxs-lookup"><span data-stu-id="9a6b6-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="9a6b6-119">Kom godt i gang med din MCA-faktureringskonto</span><span class="sxs-lookup"><span data-stu-id="9a6b6-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="9a6b6-120">Kontrollér adgang til en Microsoft-kunde aftale</span><span class="sxs-lookup"><span data-stu-id="9a6b6-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
