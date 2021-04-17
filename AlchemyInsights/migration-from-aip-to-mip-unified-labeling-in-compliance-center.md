---
title: Overførsel fra AIP til MIP/Unified Labeling i Overholdelsescenter
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825365"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="93227-102">Overførsel fra AIP til MIP/Unified Labeling i Overholdelsescenter</span><span class="sxs-lookup"><span data-stu-id="93227-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="93227-103">Hvis du vil overføre fra AIP-navne til samlet mærkning i Security and Compliance Center, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="93227-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="93227-104">**Aktivér beskyttelse fra Azure-portalen**</span><span class="sxs-lookup"><span data-stu-id="93227-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="93227-105">Hvis du ikke allerede har gjort det, skal du åbne et nyt browservindue [og logge på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="93227-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="93227-106">Gå til **Azure Information Protection-bladet.**</span><span class="sxs-lookup"><span data-stu-id="93227-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="93227-107">Klik f.eks. på Alle tjenester i **hubmenuen,** og begynd at **skrive** Oplysninger i feltet Filter.</span><span class="sxs-lookup"><span data-stu-id="93227-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="93227-108">Vælg **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="93227-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="93227-109">Hvis du ikke har åbnet Azure Information Protection-bladet [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) før, skal du se de ekstra engangstrin for at føje denne blade til portalen.</span><span class="sxs-lookup"><span data-stu-id="93227-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="93227-110">Hvis du vil åbne Azure Information Protection-bladet, skal du enten have en [Azure Information Protection Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan, der omfatter Rights Management.</span><span class="sxs-lookup"><span data-stu-id="93227-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="93227-111">Hvis du har et af disse abonnementer, men får vist en meddelelse om, at et gyldigt abonnement ikke kan findes, skal du kontakte [Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruge dine standard-supportkanaler.</span><span class="sxs-lookup"><span data-stu-id="93227-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="93227-112">Find **menuindstillingerne Administrer,** og vælg Beskyttelse **aktivering.**</span><span class="sxs-lookup"><span data-stu-id="93227-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="93227-113">Klik **på Aktivér**, og bekræft derefter handlingen.</span><span class="sxs-lookup"><span data-stu-id="93227-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="93227-114">Når aktiveringen er fuldført, vises Aktiveringen er **fuldført på informationslinjen.**</span><span class="sxs-lookup"><span data-stu-id="93227-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="93227-115">**Overfør Azure Information Protection-etiketter til Office 365 Security & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="93227-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="93227-116">Sørg for, at du er logget på som bruger med tilladelsen Global administrator.</span><span class="sxs-lookup"><span data-stu-id="93227-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="93227-117">Gå til **Azure Information Protection-bladet.**</span><span class="sxs-lookup"><span data-stu-id="93227-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="93227-118">Fra **menuindstillingen** Administrer skal du **vælge Samlet mærkat**.</span><span class="sxs-lookup"><span data-stu-id="93227-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="93227-119">På **Azure Information Protection – Samlet etiket blade skal du** klikke på **Aktivér og** følge onlinevejledningen.</span><span class="sxs-lookup"><span data-stu-id="93227-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="93227-120">**Bemærk!** Kontrollér, at du har de rette tilladelser, før du aktiverer sikkerheds- & Compliance Center-overførslen.</span><span class="sxs-lookup"><span data-stu-id="93227-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="93227-121">Se disse artikler for at få flere oplysninger:</span><span class="sxs-lookup"><span data-stu-id="93227-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="93227-122">Skal du være global administrator for at konfigurere Azure Information Protection, eller kan jeg uddelegere til andre administratorer?</span><span class="sxs-lookup"><span data-stu-id="93227-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="93227-123">Vigtige oplysninger om administrative roller efter overførsel til Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="93227-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="93227-124">Du kan finde flere oplysninger om overførsel af AIP til Samlet mærkning til Security and Compliance Center under [Overfør navne](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="93227-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
