---
title: Oprette en organisations relation for at give brugerne mulighed for at samarbejde med en anden organisation
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
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712727"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="c687e-102">Oprette en organisations relation for at give brugerne mulighed for at samarbejde med en anden organisation</span><span class="sxs-lookup"><span data-stu-id="c687e-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="c687e-103">Fra Microsoft 365 administration-dashboardet skal du gå til **admin**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c687e-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="c687e-104">Gå til **organization**  >  **deling**af organisationer.</span><span class="sxs-lookup"><span data-stu-id="c687e-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="c687e-105">Klik på **ny** under **deling af organisation**.</span><span class="sxs-lookup"><span data-stu-id="c687e-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="c687e-106">I den **nye organisations relation**skal du skrive et brugervenligt navn for organisationens relation i feltet **Relationsnavn** .</span><span class="sxs-lookup"><span data-stu-id="c687e-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="c687e-107">I feltet **domæner, der skal deles med** skal du skrive domænet for den eksterne Office 365-eller Exchange lokalt-organisation, du vil give dig mulighed for at se dine kalendere.</span><span class="sxs-lookup"><span data-stu-id="c687e-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="c687e-108">Hvis du har brug for at angive mere end ét domæne, skal du adskille domænenavnene med et komma.</span><span class="sxs-lookup"><span data-stu-id="c687e-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="c687e-109">For eksempel contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c687e-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="c687e-110">Markér afkrydsningsfeltet **Aktivér deling af oplysninger om ledig/optaget-kalender** for at aktivere kalender deling med de domæner, du har angivet.</span><span class="sxs-lookup"><span data-stu-id="c687e-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="c687e-111">Angiv delings niveauet for oplysninger om ledig/optaget tid i kalenderen, og Angiv, hvilke brugere der kan dele kalenderoplysninger om ledig/optaget tid.</span><span class="sxs-lookup"><span data-stu-id="c687e-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="c687e-112">Hvis du vil angive adgangsniveauet ledig/optaget, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="c687e-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="c687e-113">**Oplysninger om ledig/optaget tid i kalenderen**</span><span class="sxs-lookup"><span data-stu-id="c687e-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="c687e-114">**Kalender ledig/optaget til tid, emne og placering**</span><span class="sxs-lookup"><span data-stu-id="c687e-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="c687e-115">Hvis du vil angive, hvilke brugere der skal dele kalenderoplysninger om ledig/optaget tid, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="c687e-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="c687e-116">**Alle i organisationen**</span><span class="sxs-lookup"><span data-stu-id="c687e-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="c687e-117">**En angivet sikkerhedsgruppe**</span><span class="sxs-lookup"><span data-stu-id="c687e-117">**A specified security group**</span></span>  

<span data-ttu-id="c687e-118">Klik på **Gennemse** for at vælge sikkerhedsgruppen fra en liste, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="c687e-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="c687e-119">Klik på **Gem** for at oprette organisations relationen.</span><span class="sxs-lookup"><span data-stu-id="c687e-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="c687e-120">**Bemærk:** Konfigurationer på tværs af flere arkitekturer understøtter ikke personlige kontakter til opslag i ledig/optaget tid.</span><span class="sxs-lookup"><span data-stu-id="c687e-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="c687e-121">Kontaktpersoner skal medtages på den globale adresseliste, hvor opslag i ledig/optaget tid fungerer.</span><span class="sxs-lookup"><span data-stu-id="c687e-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="c687e-122">**Hvis du vil have mere at vide om dette emne, skal du læse:**</span><span class="sxs-lookup"><span data-stu-id="c687e-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="c687e-123">Oprette en organisations relation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c687e-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="c687e-124">Ændre en organisations relation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c687e-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="c687e-125">Fjerne en organisations relation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c687e-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
