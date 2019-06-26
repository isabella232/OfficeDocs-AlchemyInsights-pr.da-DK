---
title: Fejlfinding af ingen adgang meddelelser til OneDrive for Business-websteder
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223418"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="d1475-102">Fejlfinding af ingen adgang meddelelser til OneDrive for Business-websteder</span><span class="sxs-lookup"><span data-stu-id="d1475-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="d1475-103">Dette problem opstår oftest, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="d1475-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="d1475-104">Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID).</span><span class="sxs-lookup"><span data-stu-id="d1475-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="d1475-105">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="d1475-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="d1475-106">Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU).</span><span class="sxs-lookup"><span data-stu-id="d1475-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="d1475-107">Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="d1475-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="d1475-108">Du kan løse dette problem skal du gendanne den oprindelige UPN med trinnene i artiklen,[gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d1475-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="d1475-109">Når dette er gjort, kan du kontrollere, at brugeren har admin-rettigheder til webstedet OneDrive ved at følge trinnene til [Tilføj admin's for en brugers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="d1475-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="d1475-110">Du kan finde yderligere oplysninger om tilladelsesniveauer finder artikel, [forståelse af tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d1475-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
