---
title: Moderne Azure-mail fakturering
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922024"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="737b7-102">Mail fakturering i Azure</span><span class="sxs-lookup"><span data-stu-id="737b7-102">Email invoicing in Azure</span></span>

<span data-ttu-id="737b7-103">Du skal have rollen ejer eller bidragyder på fakturerings profilen eller dens faktureringskonto for at opdatere dens mail faktura indstilling.</span><span class="sxs-lookup"><span data-stu-id="737b7-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="737b7-104">Når du har tilmeldt dig, får alle brugere med en rolle som ejer, bidragyder, læsere og faktura administrator på en fakturerings profil sin faktura i en mail.</span><span class="sxs-lookup"><span data-stu-id="737b7-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="737b7-105">Log på Azure- [portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="737b7-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="737b7-106">Søg efter **omkostningsstyring + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="737b7-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="737b7-107">Vælg **fakturaer** fra venstre side, og vælg derefter **mail faktura** øverst på siden.</span><span class="sxs-lookup"><span data-stu-id="737b7-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="737b7-108">Hvis du har flere fakturerings profiler, skal du vælge en fakturerings profil og derefter vælge **Tilmeld**.</span><span class="sxs-lookup"><span data-stu-id="737b7-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="737b7-109">Vælg **Opdater**.</span><span class="sxs-lookup"><span data-stu-id="737b7-109">Select **Update**.</span></span>
6. <span data-ttu-id="737b7-110">Hvis du har flere fakturerings profiler, skal du vælge en fakturerings profil og derefter vælge **Tilmeld**.</span><span class="sxs-lookup"><span data-stu-id="737b7-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="737b7-111">Du giver andre adgang til at få vist, downloade og betale fakturaer ved at tildele dem rollen faktura administrator til en MCA-eller MPA-fakturerings profil.</span><span class="sxs-lookup"><span data-stu-id="737b7-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="737b7-112">Hvis du har valgt at få din faktura i en mail, får brugerne også fakturaen i mail.</span><span class="sxs-lookup"><span data-stu-id="737b7-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="737b7-113">Log på Azure- [portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="737b7-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="737b7-114">Søg efter **omkostningsstyring + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="737b7-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="737b7-115">Vælg **fakturerings profiler** fra venstre side.</span><span class="sxs-lookup"><span data-stu-id="737b7-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="737b7-116">Vælg en fakturerings profil, som du vil tildele en faktura administratorrolle, på listen fakturerings profiler.</span><span class="sxs-lookup"><span data-stu-id="737b7-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="737b7-117">Vælg **adgangskontrol (IAM)** fra venstre side, og vælg derefter **Tilføj** fra toppen af siden.</span><span class="sxs-lookup"><span data-stu-id="737b7-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="737b7-118">Vælg **faktura administrator** på rullelisten rolle.</span><span class="sxs-lookup"><span data-stu-id="737b7-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="737b7-119">Indtast mailadressen på den bruger, der skal give adgang.</span><span class="sxs-lookup"><span data-stu-id="737b7-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="737b7-120">Vælg **Gem** for at tildele rollen.</span><span class="sxs-lookup"><span data-stu-id="737b7-120">Select **Save** to assign the role.</span></span>
