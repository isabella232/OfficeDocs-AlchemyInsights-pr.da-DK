---
title: Overførsel fra AIP til MIP/samlet mærkning i overholdelses Center
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674320"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="78ca3-102">Overførsel fra AIP til MIP/samlet mærkning i overholdelses Center</span><span class="sxs-lookup"><span data-stu-id="78ca3-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="78ca3-103">Hvis du vil overføre fra AIP-navne til samlet Etiketing i sikkerheds-og Overholdelsescenter, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="78ca3-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="78ca3-104">**Aktivere beskyttelse fra Azure-portalen**</span><span class="sxs-lookup"><span data-stu-id="78ca3-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="78ca3-105">Hvis du ikke allerede har gjort det, skal du åbne et nyt browservindue og [logge på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="78ca3-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="78ca3-106">Gå til bladet **Azure information Protection** .</span><span class="sxs-lookup"><span data-stu-id="78ca3-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="78ca3-107">I menuen hub skal du for eksempel klikke på **alle tjenester** og begynde at skrive **oplysninger** i feltet Filter.</span><span class="sxs-lookup"><span data-stu-id="78ca3-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="78ca3-108">Vælg **Azure information Protection**.</span><span class="sxs-lookup"><span data-stu-id="78ca3-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="78ca3-109">Hvis du ikke har åbnet bladet til Azure-informations beskyttelse før, skal du se de [trin](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , der er en gang til at føje denne kørsel til portalen.</span><span class="sxs-lookup"><span data-stu-id="78ca3-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="78ca3-110">Hvis du vil åbne bladet til Azure-beskyttelse af oplysninger, skal du enten have en [Azure-informations beskyttelses-Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan, der omfatter rettighedsstyring.</span><span class="sxs-lookup"><span data-stu-id="78ca3-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="78ca3-111">Hvis du har et af disse abonnementer, men se en meddelelse om, at et gyldigt abonnement ikke kan findes, skal du [kontakte Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruge standard support kanalerne.</span><span class="sxs-lookup"><span data-stu-id="78ca3-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="78ca3-112">Find indstillinger for menuen **Administrer** , og vælg **beskyttelse af aktiver**.</span><span class="sxs-lookup"><span data-stu-id="78ca3-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="78ca3-113">Klik på **Aktivér**, og bekræft derefter din handling.</span><span class="sxs-lookup"><span data-stu-id="78ca3-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="78ca3-114">Når aktiveringen er fuldført, viser informationslinjen **aktiveringen fuldført**.</span><span class="sxs-lookup"><span data-stu-id="78ca3-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="78ca3-115">**Overføre Azure information Protection-etiketter til Office 365 Security & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="78ca3-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="78ca3-116">Kontrollér, at du er logget på som bruger med Global administrator tilladelse.</span><span class="sxs-lookup"><span data-stu-id="78ca3-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="78ca3-117">Gå til bladet **Azure information Protection** .</span><span class="sxs-lookup"><span data-stu-id="78ca3-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="78ca3-118">I menuen **Administrer** skal du vælge **samlet etiketing**.</span><span class="sxs-lookup"><span data-stu-id="78ca3-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="78ca3-119">På bladet **Azure information Protection-samlet etikette** ring skal du klikke på **Aktivér** og følge instruktionerne online.</span><span class="sxs-lookup"><span data-stu-id="78ca3-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="78ca3-120">**Bemærk**! Kontrollér, at du har de rette tilladelser, før du aktiverer overflytning af sikkerheds & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="78ca3-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="78ca3-121">Du kan finde flere oplysninger i disse artikler:</span><span class="sxs-lookup"><span data-stu-id="78ca3-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="78ca3-122">Skal du være global administrator for at konfigurere Azure information Protection eller kan jeg uddelegere til andre administratorer?</span><span class="sxs-lookup"><span data-stu-id="78ca3-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="78ca3-123">Vigtige oplysninger om administrative roller, når du har overført til sikkerheds & overholdelses Center.</span><span class="sxs-lookup"><span data-stu-id="78ca3-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="78ca3-124">Hvis du vil have mere at vide om AIP til at give samlet etikettering til sikkerheds-og overholdelses Center, skal du se [overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="78ca3-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
