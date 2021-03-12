---
title: Fejlfinding af adgang nægtet meddelelser
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707948"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="05d49-102">Fejlfinding af adgang nægtet meddelelser i Sharepoint/OneDrive Administration</span><span class="sxs-lookup"><span data-stu-id="05d49-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="05d49-103">Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til en Sharepoint/OneDrive Administration, skal du sørge for at tildele en licens [til brugeren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="05d49-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="05d49-104">Hvis brugeren har en licens, skal du også sikre dig, at de [er tildelt en administratorrolle,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) der kan få adgang til Administration.</span><span class="sxs-lookup"><span data-stu-id="05d49-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="05d49-105">Dette problem kan også opstå, når en bruger slettes og genoprettes med samme brugerens hovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="05d49-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="05d49-106">Den nye konto oprettes ved hjælp af en anden værdi for PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="05d49-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="05d49-107">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren et forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="05d49-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="05d49-108">Et andet scenarie indebærer katalogsynkronisering med en Active Directory-organisationsenhed (OU).</span><span class="sxs-lookup"><span data-stu-id="05d49-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="05d49-109">Hvis brugerne allerede er logget på SharePoint og derefter flyttes til en anden OU og synkroniseres igen med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="05d49-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="05d49-110">Du kan løse dette problem ved at gendanne det oprindelige UPN ved hjælp af trinnene i artiklen Gendan [en bruger i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="05d49-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="05d49-111">Bemærk! Hvis en OneDrive- eller SharePoint Administration ikke er tilgængelig for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt problem med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="05d49-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="05d49-112">[Kontrollér dashboardet over tjenestetilstand.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="05d49-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


