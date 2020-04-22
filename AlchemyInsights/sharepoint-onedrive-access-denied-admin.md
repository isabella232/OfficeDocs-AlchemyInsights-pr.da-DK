---
title: Fejlfinding i forbindelse med meddelelser, der er nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758388"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="e823b-102">Fejlfinding i forbindelse med adgang nægtet meddelelse i Sharepoint/OneDrive Administration</span><span class="sxs-lookup"><span data-stu-id="e823b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="e823b-103">Hvis du modtager en meddelelse, der ikke er nægtet adgang, når du forsøger at gå til en Sharepoint/OneDrive Administration, skal du kontrollere, at du [tildeler en licens til brugeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="e823b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="e823b-104">Hvis brugeren har en licens, skal du også sikre dig, at vedkommende [tildeles en administratorrolle,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) der kan få adgang til administratorcentrene.</span><span class="sxs-lookup"><span data-stu-id="e823b-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="e823b-105">Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugernavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="e823b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e823b-106">Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="e823b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e823b-107">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="e823b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e823b-108">Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed.</span><span class="sxs-lookup"><span data-stu-id="e823b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e823b-109">Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden afdeling og synkroniseres igen med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="e823b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="e823b-110">Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen [Gendan en bruger i Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e823b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="e823b-111">Bemærk: Hvis et OneDrive eller SharePoint Administration ikke er tilgængeligt for flere brugere, der tidligere havde adgang, kan der være et midlertidigt tjenesteproblem.</span><span class="sxs-lookup"><span data-stu-id="e823b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="e823b-112">[Tjek dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e823b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


