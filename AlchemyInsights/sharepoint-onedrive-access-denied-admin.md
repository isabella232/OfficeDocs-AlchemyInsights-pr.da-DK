---
title: Foretag fejlfinding af meddelelser om nægtet adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767654"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="8a5fd-102">Foretag fejlfinding af meddelelser om nægtet adgang i SharePoint/OneDrive administration</span><span class="sxs-lookup"><span data-stu-id="8a5fd-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="8a5fd-103">Hvis du modtager en meddelelse om adgang nægtet, når du forsøger at gå til en SharePoint/OneDrive administration, skal du sørge for, at du [tildeler en licens til brugeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8a5fd-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="8a5fd-104">Hvis brugeren har en licens, skal du også sørge for, at den er [tildelt en administratorrolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , der kan få adgang til administrations centrene.</span><span class="sxs-lookup"><span data-stu-id="8a5fd-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="8a5fd-105">Dette problem kan også opstå, når en bruger slettes og genoprettes med det samme UPN-navn (User Principal Name).</span><span class="sxs-lookup"><span data-stu-id="8a5fd-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8a5fd-106">Den nye konto oprettes ved hjælp af en anden PUID-værdi (entydigt Passport-ID).</span><span class="sxs-lookup"><span data-stu-id="8a5fd-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8a5fd-107">Når brugeren forsøger at få adgang til en gruppe af websteder eller deres OneDrive, har brugeren en forkert PUID.</span><span class="sxs-lookup"><span data-stu-id="8a5fd-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8a5fd-108">En anden situation omfatter Katalogsynkronisering med en Active Directory-afdeling.</span><span class="sxs-lookup"><span data-stu-id="8a5fd-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8a5fd-109">Hvis brugerne allerede har logget på SharePoint, og de derefter flyttes til en anden OU og synkroniseres med SharePoint, kan de opleve dette problem.</span><span class="sxs-lookup"><span data-stu-id="8a5fd-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="8a5fd-110">For at løse dette problem skal du gendanne den oprindelige UPN med trinnene i artiklen, [gendanne en bruger i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="8a5fd-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="8a5fd-111">Bemærk! Hvis en OneDrive-eller SharePoint-Administrationscenter ikke er tilgængelig for flere brugere, der tidligere har haft adgang, kan der være et midlertidigt tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="8a5fd-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="8a5fd-112">[Se dashboardet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8a5fd-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


