---
title: Fejlfinding i forbindelse med meddelelser adgang nægtet
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503521"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c4164-102">Fejlfinding i forbindelse med adgang nægtet meddelelser i Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="c4164-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c4164-103">Hvis du modtager en adgang nægtet vises, når du forsøger at gå til administrationssiden for en Sharepoint/OneDrive, skal du kontrollere, at du [tildeler en licens til brugeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c4164-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="c4164-104">Hvis brugeren har en licens, skal du også sikre dig de er [tildelt en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , der kan få adgang til admin centrum.</span><span class="sxs-lookup"><span data-stu-id="c4164-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="c4164-105">Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme brugerens hovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="c4164-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c4164-106">Den nye konto er oprettet ved hjælp af en anden værdi af PUID (Passport Entydigt ID).</span><span class="sxs-lookup"><span data-stu-id="c4164-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c4164-107">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="c4164-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c4164-108">Et andet scenario omfatter katalogsynkronisering med en Active Directory-organisationsenheden (OU).</span><span class="sxs-lookup"><span data-stu-id="c4164-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c4164-109">Hvis brugerne har allerede logget på SharePoint, og derefter er flyttet til en anden OU og resynced med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="c4164-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c4164-110">Du kan løse dette problem, skal du gendanne den oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c4164-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="c4164-111">Bemærk: Hvis en OneDrive eller SharePoint Administration center ikke er tilgængelig for flere brugere, som tidligere har haft adgang, kan der være et problem med den midlertidige tjeneste.</span><span class="sxs-lookup"><span data-stu-id="c4164-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c4164-112">[Kontroller service sundhed dashboardet](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c4164-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


