---
title: Problem med enkelt bruger
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429468"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="137fb-102">Problem med enkelt bruger</span><span class="sxs-lookup"><span data-stu-id="137fb-102">Problem with single user</span></span>

- <span data-ttu-id="137fb-103">Brugeren er muligvis ikke blevet klargjort, fordi tjenesten endnu ikke har haft mulighed for at evaluere brugeren.</span><span class="sxs-lookup"><span data-stu-id="137fb-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="137fb-104">Gennemgå vejledningen for, hvor lang tid klargøring tager, samt statuslinjen på konfigurationssiden for klargøring.</span><span class="sxs-lookup"><span data-stu-id="137fb-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="137fb-105">Hvis den konstante tilstand, der er angivet i sektionen med yderligere oplysninger, er før den dato, hvor brugeren blev oprettet/opdateret/slettet, betyder det, at vi endnu ikke har evalueret brugeren.</span><span class="sxs-lookup"><span data-stu-id="137fb-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="137fb-106">I dette scenarie er det bedste at vente på, at klargøringstjenesten afsluttes.</span><span class="sxs-lookup"><span data-stu-id="137fb-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="137fb-107">Bemærk, at vores tjeneste kun er opmærksom på ændringer for en bruger i kildesystemet (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="137fb-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="137fb-108">Der skal være en gyldig ændring i kildesystemet for Azure AD for at registrere ændringen og få den til at flyde ind i Active Directory.</span><span class="sxs-lookup"><span data-stu-id="137fb-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="137fb-109">Klargøringstjenesten evaluerede brugeren og vurderede, at den ikke skulle klargøres:</span><span class="sxs-lookup"><span data-stu-id="137fb-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="137fb-110">Hvis du har angivet en attribut baseret på et filter til angivelse af område, skal du sikre dig, at brugeren opfylder de kriterier, du har angivet.</span><span class="sxs-lookup"><span data-stu-id="137fb-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="137fb-111">Hvis brugerne allerede findes i destinationssystemet og brugerens tilstand i kilde- og målmatchet, vil vi ikke gøre yderligere.</span><span class="sxs-lookup"><span data-stu-id="137fb-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="137fb-112">Klargøringstjenesten forsøgte at klargøre brugeren, og det mislykkedes.</span><span class="sxs-lookup"><span data-stu-id="137fb-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="137fb-113">For disse scenarier skal du gennemgå fanen med fejlfinding og anbefalinger i klargøringslogfilerne:</span><span class="sxs-lookup"><span data-stu-id="137fb-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="137fb-114">En påkrævet attribut for brugeren mangler muligvis i Active Directory i det lokale miljø eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="137fb-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="137fb-115">For eksempel genererer userPrincipalName- eller sAMAccountName-regler ikke den rigtige værdi.</span><span class="sxs-lookup"><span data-stu-id="137fb-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="137fb-116">Den matchende attribut (som regel medarbejder-id) løses ikke til en entydig bruger i Active Directory i det lokale miljø eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="137fb-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="137fb-117">Der er f.eks. to brugere med det samme medarbejder-id i AD, og tjenesten returnerer en fejlkode, der angiver dublerede målposter for den samme kildepost.</span><span class="sxs-lookup"><span data-stu-id="137fb-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="137fb-118">Se klargøringslogfilerne for et problem med en bestemt bruger, hvis du vil gennemse [logfiler for enkeltbrugere](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)og grupper.</span><span class="sxs-lookup"><span data-stu-id="137fb-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
