---
title: Aktivér omkostningsstyring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677217"
---
# <a name="enable-cost-management"></a><span data-ttu-id="f09bf-102">Aktivér omkostningsstyring</span><span class="sxs-lookup"><span data-stu-id="f09bf-102">Enable cost management</span></span>

<span data-ttu-id="f09bf-103">**Hvad betyder ' omkostninger deaktiveres for din organisation '?**</span><span class="sxs-lookup"><span data-stu-id="f09bf-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="f09bf-104">Organisationer, der bruger en EA-konto (Enterprise Agreement) eller Microsoft-kunde aftale (MCA), kan deaktivere adgang til omkostningsoplysninger og prisoplysninger.</span><span class="sxs-lookup"><span data-stu-id="f09bf-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="f09bf-105">Når du har logget på Azure-portalen, kan de bruge fakturerings-API'erne til automatisk at få fakturaer (når de er tilmeldt) og oplysninger om forbrug.</span><span class="sxs-lookup"><span data-stu-id="f09bf-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="f09bf-106">**Sådan giver du yderligere brugere adgang til fakturaer**</span><span class="sxs-lookup"><span data-stu-id="f09bf-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="f09bf-107">Gå til **abonnements blade** i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="f09bf-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="f09bf-108">Vælg **fakturaer** , og vælg derefter **adgang til fakturaer**.</span><span class="sxs-lookup"><span data-stu-id="f09bf-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="f09bf-109">Slå Access til, når du har gemt ændringerne, for at tillade brugere i abonnementsbaserede roller for at downloade fakturaer.</span><span class="sxs-lookup"><span data-stu-id="f09bf-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="f09bf-110">Konto administratoren kan også konfigurere for at få fakturaer sendt via mail.</span><span class="sxs-lookup"><span data-stu-id="f09bf-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="f09bf-111">Hvis du vil have mere at vide, skal du se [Hent din faktura i en mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="f09bf-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="f09bf-112">**Sådan føjer du brugere til rollen fakturerings læser**</span><span class="sxs-lookup"><span data-stu-id="f09bf-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="f09bf-113">Gå til **abonnements blade** i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="f09bf-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="f09bf-114">Vælg **adgangskontrol (IAM)** , og klik derefter på **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="f09bf-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="f09bf-115">Vælg **fakturerings læser** på siden **Vælg en rolle** .</span><span class="sxs-lookup"><span data-stu-id="f09bf-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="f09bf-116">Skriv mailadressen på den bruger, du vil invitere, og klik derefter på **OK** for at sende invitationen.</span><span class="sxs-lookup"><span data-stu-id="f09bf-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="f09bf-117">Følg instruktionerne i invitationen til mail for at logge på som en fakturerings læser.</span><span class="sxs-lookup"><span data-stu-id="f09bf-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="f09bf-118">Hvis du vil have mere at vide, skal du se [Giv adgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="f09bf-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="f09bf-119">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="f09bf-119">**Recommended documents**</span></span>

- [<span data-ttu-id="f09bf-120">Aktivere DA-og AO-visninger via EA Portal</span><span class="sxs-lookup"><span data-stu-id="f09bf-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="f09bf-121">Omkostninger inkluderet i omkostningsstyring</span><span class="sxs-lookup"><span data-stu-id="f09bf-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="f09bf-122">Understøttede Microsoft Azure-tilbud</span><span class="sxs-lookup"><span data-stu-id="f09bf-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="f09bf-123">Gennemse omkostninger i omkostningsanalyse</span><span class="sxs-lookup"><span data-stu-id="f09bf-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="f09bf-124">Giv adgang til faktureringsoplysninger</span><span class="sxs-lookup"><span data-stu-id="f09bf-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f09bf-125">Kontrollér adgang til en Microsoft-kunde aftale</span><span class="sxs-lookup"><span data-stu-id="f09bf-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






