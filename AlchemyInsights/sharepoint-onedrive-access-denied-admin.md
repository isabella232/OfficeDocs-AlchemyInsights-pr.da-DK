---
title: Fejlfinding i forbindelse med adgang nægtet-meddelelser
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751270"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="eb499-102">Fejlfinding i forbindelse med adgang nægtet-meddelelser i SharePoint/OneDrive administration</span><span class="sxs-lookup"><span data-stu-id="eb499-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="eb499-103">Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til et SharePoint/OneDrive-administrations Center, skal du sørge for at [tildele brugeren en licens](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="eb499-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="eb499-104">Hvis brugeren har en licens, skal du også sørge for, at de er [tildelt en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , der kan få adgang til administrations centrene.</span><span class="sxs-lookup"><span data-stu-id="eb499-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="eb499-105">Dette problem kan også opstå, når en bruger slettes og oprettes igen med det samme bruger hovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="eb499-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="eb499-106">Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="eb499-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="eb499-107">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="eb499-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="eb499-108">Et andet scenario involverer Katalogsynkronisering med en Active Directory-organisationsenhed (OU).</span><span class="sxs-lookup"><span data-stu-id="eb499-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="eb499-109">Hvis brugerne allerede er logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres igen med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="eb499-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="eb499-110">Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="eb499-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="eb499-111">Bemærk: Hvis et OneDrive-eller SharePoint-Administrationscenter ikke er tilgængeligt for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt serviceproblem.</span><span class="sxs-lookup"><span data-stu-id="eb499-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="eb499-112">[Kontroller dashboardet for servicetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="eb499-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


