---
title: Moderne Azure fakturering per email
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820820"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="3589f-102">Fakturering per email i Azure</span><span class="sxs-lookup"><span data-stu-id="3589f-102">Email invoicing in Azure</span></span>

<span data-ttu-id="3589f-103">Du skal have en ejer- eller en bidragsyder rolle på faktureringsprofilen eller dens faktureringskonto for at opdatere dens indstillinger for fakturering med email.</span><span class="sxs-lookup"><span data-stu-id="3589f-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="3589f-104">Når du har tilmeldt dig, får alle brugere med en ejer-, bidragsyder-, læser- og fakturaadministrator roller på en faktureringsprofil sin faktura pr. mail.</span><span class="sxs-lookup"><span data-stu-id="3589f-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="3589f-105">Log på portalen[Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3589f-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3589f-106">Søg efter **Omkostningsstyring + Fakturering**.</span><span class="sxs-lookup"><span data-stu-id="3589f-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="3589f-107">Vælg **Fakturaer** i venstre side, og vælg derefter **Faktura pr. mail** øverst på siden.</span><span class="sxs-lookup"><span data-stu-id="3589f-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="3589f-108">Hvis du har flere faktureringsprofiler, skal du vælge en faktureringsprofil og derefter vælge **Tilmeld dig**.</span><span class="sxs-lookup"><span data-stu-id="3589f-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="3589f-109">Vælg **Opdater**.</span><span class="sxs-lookup"><span data-stu-id="3589f-109">Select **Update**.</span></span>
6. <span data-ttu-id="3589f-110">Hvis du har flere faktureringsprofiler, skal du vælge en faktureringsprofil og derefter vælge **Tilmeld dig**.</span><span class="sxs-lookup"><span data-stu-id="3589f-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="3589f-111">Du giver andre adgang til at få vist, downloade og betale fakturaer ved at tildele dem rollen som fakturaadministrator for en MCA- eller MPA-faktureringsprofil.</span><span class="sxs-lookup"><span data-stu-id="3589f-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="3589f-112">Hvis du har tilvalgt at få din faktura via mail, får brugerne også fakturaer via mail.</span><span class="sxs-lookup"><span data-stu-id="3589f-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="3589f-113">Log på portalen[Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3589f-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3589f-114">Søg efter **Omkostningsstyring + Fakturering**.</span><span class="sxs-lookup"><span data-stu-id="3589f-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="3589f-115">Vælg **faktureringsprofiler** du vælger fra venstre side.</span><span class="sxs-lookup"><span data-stu-id="3589f-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="3589f-116">Fra listen over faktureringsprofier vælg en faktureringsprofill, som du vil tildele en rolle som fakturaadministrator.</span><span class="sxs-lookup"><span data-stu-id="3589f-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="3589f-117">Vælg **Adgangskontrol (IAM)** i venstre side, og vælg derefter **Tilføj** øverst på siden.</span><span class="sxs-lookup"><span data-stu-id="3589f-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="3589f-118">I rullemenuen skal du vælge **Fakturaadministrator på**.</span><span class="sxs-lookup"><span data-stu-id="3589f-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="3589f-119">Indtast brugerens mailadresse for at give adgang.</span><span class="sxs-lookup"><span data-stu-id="3589f-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="3589f-120">Vælg **Gem** for at tildele rollen.</span><span class="sxs-lookup"><span data-stu-id="3589f-120">Select **Save** to assign the role.</span></span>
