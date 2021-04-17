---
title: Opret en organisationsrelation for at give brugerne mulighed for at samarbejde med en anden organisation
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816122"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="85fe8-102">Opret en organisationsrelation for at give brugerne mulighed for at samarbejde med en anden organisation</span><span class="sxs-lookup"><span data-stu-id="85fe8-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="85fe8-103">Fra dashboardet i Microsoft 365 Administration skal du gå til **Administration**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="85fe8-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="85fe8-104">Gå til **deling af**  >  **organisation**.</span><span class="sxs-lookup"><span data-stu-id="85fe8-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="85fe8-105">Under **Organisationsdeling skal** du klikke på **Ny** .</span><span class="sxs-lookup"><span data-stu-id="85fe8-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="85fe8-106">Skriv **et brugervenligt** navn på **organisationsrelationen** i feltet Relationsnavn i ny organisationsrelation.</span><span class="sxs-lookup"><span data-stu-id="85fe8-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="85fe8-107">I feltet **Domæner,** der skal deles med skal du skrive domænet for den eksterne Office 365- eller Exchange-organisation i det lokale miljø, som du vil give vist dine kalendere.</span><span class="sxs-lookup"><span data-stu-id="85fe8-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="85fe8-108">Hvis du vil angive mere end ét domæne, skal du adskille domænenavnene med et komma.</span><span class="sxs-lookup"><span data-stu-id="85fe8-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="85fe8-109">For eksempel contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="85fe8-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="85fe8-110">Markér **afkrydsningsfeltet Aktivér deling af oplysninger om ledig/optaget** tid i kalenderen for at aktivere kalenderdeling med de domæner, du har angivet.</span><span class="sxs-lookup"><span data-stu-id="85fe8-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="85fe8-111">Angiv delingsniveauet for oplysninger om ledig/optaget i kalender, og angiv, hvilke brugere der kan dele oplysninger om ledig/optaget i kalenderen.</span><span class="sxs-lookup"><span data-stu-id="85fe8-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="85fe8-112">Hvis du vil angive ledig/optaget-adgangsniveauet, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="85fe8-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="85fe8-113">**Udelukkende oplysninger om ledig/optaget tid i kalenderen**</span><span class="sxs-lookup"><span data-stu-id="85fe8-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="85fe8-114">**Ledig/optaget i kalenderen med tid, emne og placering**</span><span class="sxs-lookup"><span data-stu-id="85fe8-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="85fe8-115">Hvis du vil angive, hvilke brugere der skal dele oplysninger om ledig/optaget tid i kalenderen, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="85fe8-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="85fe8-116">**Alle i din organisation**</span><span class="sxs-lookup"><span data-stu-id="85fe8-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="85fe8-117">**En angivet sikkerhedsgruppe**</span><span class="sxs-lookup"><span data-stu-id="85fe8-117">**A specified security group**</span></span>  

<span data-ttu-id="85fe8-118">Klik **på gennemse** for at vælge sikkerhedsgruppen på en liste, og klik derefter på **OK.**</span><span class="sxs-lookup"><span data-stu-id="85fe8-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="85fe8-119">Klik **på Gem** for at oprette organisationsrelationen.</span><span class="sxs-lookup"><span data-stu-id="85fe8-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="85fe8-120">**Bemærk!** Konfigurationer på tværs af lejere understøtter ikke personlige kontakter ved opslag med ledig/optaget tid.</span><span class="sxs-lookup"><span data-stu-id="85fe8-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="85fe8-121">Kontakter skal medtages i den globale adresseliste, for at opslaget Ledig/Optaget kan fungere.</span><span class="sxs-lookup"><span data-stu-id="85fe8-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="85fe8-122">**For at få fuld forståelse for dette emne skal du læse:**</span><span class="sxs-lookup"><span data-stu-id="85fe8-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="85fe8-123">Opret en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="85fe8-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="85fe8-124">Rediger en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="85fe8-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="85fe8-125">Fjern en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="85fe8-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
