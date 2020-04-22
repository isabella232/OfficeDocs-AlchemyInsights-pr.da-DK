---
title: Fejlfinding i forbindelse med adgang til afviste meddelelser på OneDrive for Business-websteder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692795"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="59acb-102">Fejlfinding i forbindelse med adgang til afviste meddelelser på OneDrive for Business-websteder</span><span class="sxs-lookup"><span data-stu-id="59acb-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="59acb-103">Dette problem opstår oftest, når en bruger slettes og genoprettes med det samme brugernavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="59acb-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="59acb-104">Den nye konto oprettes ved hjælp af en anden PUID-værdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="59acb-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="59acb-105">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="59acb-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="59acb-106">Et andet scenarie omfatter katalogsynkronisering med en Active Directory-organisationsenhed.</span><span class="sxs-lookup"><span data-stu-id="59acb-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="59acb-107">Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden afdeling og synkroniseres igen med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="59acb-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="59acb-108">Du kan lÃ ̧se problemet ved at gendanne det oprindelige UPN med trinnene i artiklen Gendanne [en bruger i Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="59acb-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="59acb-109">Hvis du ikke kan gendanne den oprindelige bruger, skal du fjerne den gamle bruger fra OneDrive-webstedet ved hjælp af disse trin, [Fjern en bruger fra listen over brugeroplysninger]().</span><span class="sxs-lookup"><span data-stu-id="59acb-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="59acb-110">Når dette er gjort, kan du bekræfte, at brugeren har administratorrettigheder til OneDrive-webstedet, ved at følge trinnene for at [tilføje administratorer til en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="59acb-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="59acb-111">Yderligere oplysninger om tilladelsesniveauer finder du i artiklen [Om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="59acb-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
