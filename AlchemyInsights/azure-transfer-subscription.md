---
title: Overfør Azure fakturerings ejerskab
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922030"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="d8abc-102">Overfør Azure fakturerings ejerskab</span><span class="sxs-lookup"><span data-stu-id="d8abc-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="d8abc-103">Log på Azure- [portalen](https://portal.azure.com/) som administrator af faktureringskontoen med det abonnement, du vil overføre.</span><span class="sxs-lookup"><span data-stu-id="d8abc-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="d8abc-104">Hvis du ikke er sikker på, om du er administrator, eller hvis du har brug for at finde ud af, hvem der er, skal du se [bestemme konto faktureringsadministrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="d8abc-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="d8abc-105">Søg efter **omkostningsstyring + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="d8abc-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="d8abc-106">Vælg **abonnementer** i venstre rude.</span><span class="sxs-lookup"><span data-stu-id="d8abc-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="d8abc-107">Afhængigt af Access skal du muligvis vælge et fakturerings område og derefter **abonnementer** eller Azure- **abonnementer**.</span><span class="sxs-lookup"><span data-stu-id="d8abc-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="d8abc-108">Vælg **Overfør fakturerings ejerskab** for det abonnement, du vil overføre</span><span class="sxs-lookup"><span data-stu-id="d8abc-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="d8abc-109">Angiv mailadressen for en bruger, der er faktureringsadministrator for den konto, der skal være den nye ejer af abonnementet, og vælg derefter **Send anmodning om overførsel**</span><span class="sxs-lookup"><span data-stu-id="d8abc-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="d8abc-110">Brugeren får en mail med instruktioner til at gennemgå din overførsels anmodning.</span><span class="sxs-lookup"><span data-stu-id="d8abc-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="d8abc-111">Hvis du vil godkende overførselsanmodningen, skal brugeren vælge linket i mailen og følge vejledningen.</span><span class="sxs-lookup"><span data-stu-id="d8abc-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="d8abc-112">**Bemærk** ! hvis du overfører fakturerings ejerskabet af dit abonnement til en brugerkonto i en anden Azure ad-lejer, fjernes alle [Rollebaserede adgangskontrol (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)opgaver til administration af ressourcer i abonnementet permanent.</span><span class="sxs-lookup"><span data-stu-id="d8abc-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="d8abc-113">Det er kun den nye ejer, der har adgang til at administrere ressourcer i abonnementet.</span><span class="sxs-lookup"><span data-stu-id="d8abc-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="d8abc-114">Hvis du vil have mere at vide, skal du se [overføre abonnement til en bruger i en anden Azure ad-lejer](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d8abc-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="d8abc-115">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="d8abc-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="d8abc-116">Overfør fakturerings ejerskabet af et Azure-abonnement til en anden konto</span><span class="sxs-lookup"><span data-stu-id="d8abc-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="d8abc-117">Om overførsel af fakturerings ejerskab for et Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="d8abc-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="d8abc-118">Overførsel af Visual Studio, Microsoft Partners Network (MPN) og betal efter din arbejde-dev/test abonnementer</span><span class="sxs-lookup"><span data-stu-id="d8abc-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="d8abc-119">Ofte stillede spørgsmål om overførsel af ejerskab</span><span class="sxs-lookup"><span data-stu-id="d8abc-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="d8abc-120">Fejlfinding af problemer med overførsel af ejerskab</span><span class="sxs-lookup"><span data-stu-id="d8abc-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
