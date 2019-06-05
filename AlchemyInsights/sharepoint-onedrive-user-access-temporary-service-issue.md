---
title: Problemer med ydeevne-SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719511"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="89382-102">SharePoint- eller OneDrive langsomt, utilgængelig eller ikke tilgængeligt for flere brugere</span><span class="sxs-lookup"><span data-stu-id="89382-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="89382-103">Hvis en OneDrive eller SharePoint-webstedet ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et problem med den midlertidige tjeneste.</span><span class="sxs-lookup"><span data-stu-id="89382-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="89382-104">[Kontroller service sundhed dashboardet](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="89382-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="89382-105">Tilføje og licens til brugeren</span><span class="sxs-lookup"><span data-stu-id="89382-105">Add and license the user</span></span>

<span data-ttu-id="89382-106">Sikre, at du [tildele licenser til brugere i Office 365 til virksomheder](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="89382-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="89382-107">Tildele tilladelser</span><span class="sxs-lookup"><span data-stu-id="89382-107">Assign Permissions</span></span>

<span data-ttu-id="89382-108">Hvis brugeren har fået tildelt en licens til Sharepoint og stadig modtager en meddelelse om nægtet adgang, Kontroller, at de har [passende tilladelsesniveau](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) , der er tildelt.</span><span class="sxs-lookup"><span data-stu-id="89382-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="89382-109">Overvej at bruge funktionen anmodning</span><span class="sxs-lookup"><span data-stu-id="89382-109">Consider using the access request feature</span></span>

<span data-ttu-id="89382-110">[Anmodning om funktion i access](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gør det muligt at anmode om adgang til indhold, de ikke har tilladelse til at se.</span><span class="sxs-lookup"><span data-stu-id="89382-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="89382-111">Tillad brugerdefinerede script kan forårsage adgang nægtet problemer</span><span class="sxs-lookup"><span data-stu-id="89382-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="89382-112">Der er visse situationer, hvor funktionen *Tillad brugerdefineret script* kan være præsenterer en adgang nægtet.</span><span class="sxs-lookup"><span data-stu-id="89382-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="89382-113">For en liste over funktioner, der påvirkes, sikkerhedsovervejelser og muligheden for at deaktivere funktionen.</span><span class="sxs-lookup"><span data-stu-id="89382-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="89382-114">Besøg [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="89382-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

