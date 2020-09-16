---
title: Teams tillader eller deaktiverer IP-video
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
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670178"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="ee470-102">Teams tillader eller deaktiverer IP-video</span><span class="sxs-lookup"><span data-stu-id="ee470-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="ee470-103">**Ændre eller oprette en møde politik**</span><span class="sxs-lookup"><span data-stu-id="ee470-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="ee470-104">Hvis du vil ændre eller oprette en møde politik, skal du gå til **Microsoft teams Administrationscenter > møder > møde politikker**.</span><span class="sxs-lookup"><span data-stu-id="ee470-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="ee470-105">Vælg en politik fra listen eller klik på **Tilføj**.</span><span class="sxs-lookup"><span data-stu-id="ee470-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="ee470-106">Hvis du opretter en ny politik, skal du tilføje et navn og en beskrivelse.</span><span class="sxs-lookup"><span data-stu-id="ee470-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="ee470-107">Navnet må ikke indeholde specialtegn eller være længere end 64 tegn.</span><span class="sxs-lookup"><span data-stu-id="ee470-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="ee470-108">Vælg dine indstillinger, og klik derefter på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="ee470-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="ee470-109">Antag f. eks., at du har mange brugere, og du vil begrænse den mængde båndbredde, som deres møde kræver.</span><span class="sxs-lookup"><span data-stu-id="ee470-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="ee470-110">Du skal oprette en ny brugerdefineret politik kaldet "begrænset båndbredde" og deaktivere de følgende indstillinger:</span><span class="sxs-lookup"><span data-stu-id="ee470-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="ee470-111">Under **lyd og video**:</span><span class="sxs-lookup"><span data-stu-id="ee470-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="ee470-112">Deaktiver Tillad optagelse i skyen.</span><span class="sxs-lookup"><span data-stu-id="ee470-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="ee470-113">Deaktiver Tillad IP-video.</span><span class="sxs-lookup"><span data-stu-id="ee470-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="ee470-114">Tildel derefter politikken til brugerne.</span><span class="sxs-lookup"><span data-stu-id="ee470-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="ee470-115">**Tildel en mødepolitik til brugere**</span><span class="sxs-lookup"><span data-stu-id="ee470-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="ee470-116">I venstre navigationsrude i Microsoft Teams Administration skal du gå til \*\*Brugere \*\*og derefter klikke på brugeren.</span><span class="sxs-lookup"><span data-stu-id="ee470-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="ee470-117">Markér brugeren ved at klikke til venstre for brugernavnet, og klik derefter på **Rediger indstillinger**.</span><span class="sxs-lookup"><span data-stu-id="ee470-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="ee470-118">Under **møde politik**skal du vælge den politik, du vil tildele, og derefter klikke på **Anvend**.</span><span class="sxs-lookup"><span data-stu-id="ee470-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="ee470-119">Du kan finde flere oplysninger i [administrere møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ee470-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
