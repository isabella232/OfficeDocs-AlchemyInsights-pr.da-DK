---
title: Oprette en organisationsrelation for at give brugerne mulighed for at samarbejde med en anden organisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862065"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="3f27e-102">Oprette en organisationsrelation for at give brugerne mulighed for at samarbejde med en anden organisation</span><span class="sxs-lookup"><span data-stu-id="3f27e-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="3f27e-103">Gå til **Administrator**Exchange fra Microsoft 365 Administration-dashboardet  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="3f27e-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="3f27e-104">Gå **organization**til  >  **organisationsdeling**.</span><span class="sxs-lookup"><span data-stu-id="3f27e-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="3f27e-105">Klik på **Ny** **under Organisationsdeling**.</span><span class="sxs-lookup"><span data-stu-id="3f27e-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="3f27e-106">Skriv et fuldt navn til **organisationsrelationen**i feltet **Relationsnavn** i den nye organisationsrelation.</span><span class="sxs-lookup"><span data-stu-id="3f27e-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="3f27e-107">Skriv domænet for den eksterne lokale Office 365- eller Exchange-organisation, du vil kunne se dine kalendere, i feltet **Domæner,** du vil dele med.</span><span class="sxs-lookup"><span data-stu-id="3f27e-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="3f27e-108">Hvis du har brug for at angive mere end ét domæne, skal du adskille domænenavnene med et komma.</span><span class="sxs-lookup"><span data-stu-id="3f27e-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="3f27e-109">contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="3f27e-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="3f27e-110">Markér **afkrydsningsfeltet Aktivér deling af ledig/optaget-tid-oplysninger** for at aktivere kalenderdeling med de domæner, du har angivet.</span><span class="sxs-lookup"><span data-stu-id="3f27e-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="3f27e-111">Angiv delingsniveauet for oplysninger om ledig/optaget tid i kalenderen, og angiv, hvilke brugere der kan dele oplysninger om ledig/optaget tid.</span><span class="sxs-lookup"><span data-stu-id="3f27e-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="3f27e-112">Hvis du vil angive adgangsniveauet ledig/optaget, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="3f27e-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="3f27e-113">**Oplysninger om ledig/optaget tid i kalender med kun tid**</span><span class="sxs-lookup"><span data-stu-id="3f27e-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="3f27e-114">**Kalender ledig/optaget med tid, emne og placering**</span><span class="sxs-lookup"><span data-stu-id="3f27e-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="3f27e-115">Hvis du vil angive, hvilke brugere der skal dele oplysninger om ledig/optaget tid i kalenderen, skal du vælge en af følgende:</span><span class="sxs-lookup"><span data-stu-id="3f27e-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="3f27e-116">**Alle i organisationen**</span><span class="sxs-lookup"><span data-stu-id="3f27e-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="3f27e-117">**En angivet sikkerhedsgruppe**</span><span class="sxs-lookup"><span data-stu-id="3f27e-117">**A specified security group**</span></span>  

<span data-ttu-id="3f27e-118">Klik på **Gå** for at vælge sikkerhedsgruppen på en liste, og klik derefter på **ok**.</span><span class="sxs-lookup"><span data-stu-id="3f27e-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="3f27e-119">Klik på **Gem** for at oprette organisationsrelationen.</span><span class="sxs-lookup"><span data-stu-id="3f27e-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="3f27e-120">**Bemærk:** Konfigurationer på tværs af lejere understøtter ikke personlige kontakter til ledig/optaget opslag.</span><span class="sxs-lookup"><span data-stu-id="3f27e-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="3f27e-121">Kontaktpersoner skal medtages på den globale adresseliste, for at opslaget/optaget er ledigt, så de kan fungere.</span><span class="sxs-lookup"><span data-stu-id="3f27e-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="3f27e-122">**For fuld forståelse af dette emne kan du læse:**</span><span class="sxs-lookup"><span data-stu-id="3f27e-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="3f27e-123">Oprette en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3f27e-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="3f27e-124">Ændre en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3f27e-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="3f27e-125">Fjerne en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3f27e-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
