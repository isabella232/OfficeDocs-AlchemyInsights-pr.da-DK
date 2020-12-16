---
title: Overføre tjenester-flytte alle RDFE-tjenester til et andet abonnement
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691978"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="09508-102">Overføre tjenester-flytte alle RDFE-tjenester til et andet abonnement</span><span class="sxs-lookup"><span data-stu-id="09508-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="09508-103">**Flytte ressourcer**</span><span class="sxs-lookup"><span data-stu-id="09508-103">**Move resources**</span></span>

<span data-ttu-id="09508-104">Azure-ressourcer kan flyttes til enten et andet Azure-abonnement eller en ressourcegruppe under det samme abonnement ved hjælp af Azure-portalen, Azure PowerShell, Azure CLI eller The REST API til at flytte ressourcer.</span><span class="sxs-lookup"><span data-stu-id="09508-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="09508-105">Før du kan flytte ressourcer, skal du se:</span><span class="sxs-lookup"><span data-stu-id="09508-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="09508-106">Tjekliste før flytning af ressourcer</span><span class="sxs-lookup"><span data-stu-id="09508-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="09508-107">Tjenester, der kan flyttes</span><span class="sxs-lookup"><span data-stu-id="09508-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="09508-108">Sådan valideres flytningen</span><span class="sxs-lookup"><span data-stu-id="09508-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="09508-109">Flyt vejledning til tjenester</span><span class="sxs-lookup"><span data-stu-id="09508-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="09508-110">Hvis du vil flytte eksisterende ressourcer til en anden ressourcegruppe eller et abonnement, kan du bruge:</span><span class="sxs-lookup"><span data-stu-id="09508-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="09508-111">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="09508-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="09508-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="09508-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="09508-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="09508-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="09508-114">REST-API</span><span class="sxs-lookup"><span data-stu-id="09508-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="09508-115">Selvstudium: [flytte Azure-ressourcer til en anden ressourcegruppe eller et andet abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="09508-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="09508-116">**Fejlfinding af fejl med Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="09508-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="09508-117">Se artiklerne nedenfor for at få mere at vide om nogle almindelige Azure-installationsfejl og modtag oplysninger for at løse dem.</span><span class="sxs-lookup"><span data-stu-id="09508-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="09508-118">Hvis du ikke kan finde fejlkoden for installations fejlen, skal du se [finde fejlkode](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="09508-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="09508-119">Fejlfinding af installationsfejl</span><span class="sxs-lookup"><span data-stu-id="09508-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="09508-120">Fejlfinding ved flytning af Azure-ressourcer til en ny ressourcegruppe eller et abonnement</span><span class="sxs-lookup"><span data-stu-id="09508-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="09508-121">Bemærk, at hvis du vil opgradere dit Azure-abonnement, f. eks Skift fra at betale til at blive, skal du konvertere dit abonnement.</span><span class="sxs-lookup"><span data-stu-id="09508-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="09508-122">Hvis du vil opgradere en gratis prøveversion, skal du se [opgradere din gratis prøveversion eller Microsoft Forestil dig Azure-abonnement for at betale som dig](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="09508-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="09508-123">Hvis du vil ændre en løn som din Go-konto, skal du se [ændre dit abonnement på Azure-pay-Go-Go til et andet bud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="09508-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="09508-124">**Sådan tilføjer eller knytter du et Azure-abonnement til din Azure Active Directory-lejer:**</span><span class="sxs-lookup"><span data-stu-id="09508-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="09508-125">Log på, og vælg det abonnement, du vil bruge, på [siden abonnementer i Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="09508-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="09508-126">Vælg **Skift mappe**.</span><span class="sxs-lookup"><span data-stu-id="09508-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="09508-127">Gennemse eventuelle advarsler, der vises, og vælg derefter **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="09508-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="09508-128">Mappen er ændret for abonnementet, og du får en meddelelse om succes.</span><span class="sxs-lookup"><span data-stu-id="09508-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="09508-129">Brug *mappen* skifteren til at gå til den nye mappe.</span><span class="sxs-lookup"><span data-stu-id="09508-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="09508-130">Det kan tage op til 10 minutter, før alt vises korrekt.</span><span class="sxs-lookup"><span data-stu-id="09508-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="09508-131">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="09508-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="09508-132">Overføre ejerskabet af et Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="09508-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="09508-133">Flytte ressourcer til en ny ressourcegruppe eller et abonnement</span><span class="sxs-lookup"><span data-stu-id="09508-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="09508-134">Administrere ressourcer ved hjælp af Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="09508-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
