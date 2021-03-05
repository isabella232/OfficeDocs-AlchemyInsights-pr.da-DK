---
title: Problem med attribut og angivelse af filter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481100"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="a0f42-102">Problem med attribut og angivelse af filter</span><span class="sxs-lookup"><span data-stu-id="a0f42-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="a0f42-103">**Problem med modstridende UPN-værdier**</span><span class="sxs-lookup"><span data-stu-id="a0f42-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="a0f42-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="a0f42-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="a0f42-105">Handlingen mislykkedes, fordi UPN-værdien, der er angivet til tilføjelse/ændring, ikke er entydig for hele skoven.</span><span class="sxs-lookup"><span data-stu-id="a0f42-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="a0f42-106">Fejldetaljer: **CONSTRAINT_ATT_TYPE – userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="a0f42-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="a0f42-107">**UserPrincipalName-værdien,** som Forbindelseskomponent Arbejdsdag forsøger at angive, når du opretter AD-brugerkontoen, findes allerede i AD-destinationsdomænet.</span><span class="sxs-lookup"><span data-stu-id="a0f42-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="a0f42-108">Dette antyder, at enten (1) brugeren allerede findes, og den matchende id-kontrol mislykkedes for brugeren, eller (2) upn-generationreglen genererede en modstridende værdi.</span><span class="sxs-lookup"><span data-stu-id="a0f42-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="a0f42-109">Her er de foreslåede trin til løsning:</span><span class="sxs-lookup"><span data-stu-id="a0f42-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="a0f42-110">Hvis brugeren allerede findes, og den matchende id-kontrol ikke kunne sammenkæde arbejdsdagskontoen med Active Directory-kontoen, skal du kontrollere, om den matchende id-attribut (typisk medarbejder-id) i både Arbejdsdag og AD har et nøjagtigt match.</span><span class="sxs-lookup"><span data-stu-id="a0f42-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="a0f42-111">Hvis de ikke har et match, er det et dataproblem, der skal rettes.</span><span class="sxs-lookup"><span data-stu-id="a0f42-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="a0f42-112">Hvis medarbejder-id'et i arbejdsdagen f.eks. er 001052, og i AD er det 1052, så kan klargøringsprogrammet ikke sammenkæde de to konti og forsøger at oprette en bruger, der allerede findes.</span><span class="sxs-lookup"><span data-stu-id="a0f42-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="a0f42-113">Løsningen i dette tilfælde er at ændre værdien for **Medarbejder-id** i AD, så den medtager de foranstillede nuller for at gøre den til 001052.</span><span class="sxs-lookup"><span data-stu-id="a0f42-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="a0f42-114">Hvis det UPN-genererende udtryk ikke genererer en entydig værdi, kan du overveje at bruge duplikeringsfunktionen **SelectUniqueValue** til at generere en entydig værdi hver gang.</span><span class="sxs-lookup"><span data-stu-id="a0f42-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="a0f42-115">**Arbejdsdag til AD-bruger klargøring angiver ikke administratorattributværdien for AD-brugerkonto**</span><span class="sxs-lookup"><span data-stu-id="a0f42-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="a0f42-116">Jobbet til klargøring af arbejdsdag til AD-bruger angiver ikke **administratorattributværdien** for AD-brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="a0f42-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="a0f42-117">Der er to mulige scenarier, når denne funktionsmåde kan ses:</span><span class="sxs-lookup"><span data-stu-id="a0f42-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="a0f42-118">Chefen i Arbejdsdag kan ikke løses til en tilsvarende AD-brugerkonto, fordi lederen ikke er omfattet.</span><span class="sxs-lookup"><span data-stu-id="a0f42-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="a0f42-119">I et **scenarie med flere AD-domæner** er chefen i Arbejdsdag ikke til stede i det samme domæne som brugeren.</span><span class="sxs-lookup"><span data-stu-id="a0f42-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="a0f42-120">Prøv disse trin for at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="a0f42-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="a0f42-121">Hvis du har defineret områdefiltre, skal du først kontrollere, om den overordnede er i omfang, og at den opfylder angivelsessætningen.</span><span class="sxs-lookup"><span data-stu-id="a0f42-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="a0f42-122">Hvis lederen ikke opfylder filterets område, skal du ændre filteret, så lederen også er i forbindelse med klargøringshandlingen.</span><span class="sxs-lookup"><span data-stu-id="a0f42-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="a0f42-123">Hvis du har flere AD-domæner, har forbindelsen en kendt begrænsning for manglende mulighed for at løse referencer til administration på tværs af domæner.</span><span class="sxs-lookup"><span data-stu-id="a0f42-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="a0f42-124">Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk klargøring af brugere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="a0f42-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













