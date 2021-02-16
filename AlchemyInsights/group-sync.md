---
title: Gruppesynkronisering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256683"
---
# <a name="group-sync"></a><span data-ttu-id="f3077-102">Gruppesynkronisering</span><span class="sxs-lookup"><span data-stu-id="f3077-102">Group sync</span></span>

<span data-ttu-id="f3077-103">Denne artikel indeholder vejledning om gruppesynkronisering.</span><span class="sxs-lookup"><span data-stu-id="f3077-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="f3077-104">Hvis en global administrator eller gruppeejer ikke kan redigere gruppeegenskaber eller tilføje medlemmer eller tildele ejere i Azure-portalen, skal du sikre dig, at kilden til autoriteten for gruppen er Azure Active Directory (Azure AD) for den globale administrator eller gruppeejeren til at redigere gruppen.</span><span class="sxs-lookup"><span data-stu-id="f3077-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="f3077-105">Før du forsøger at slette en synkroniseret gruppe i Azure AD, skal du sikre dig, at du [har slettet alle tildelte](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) licenser for at undgå fejl.</span><span class="sxs-lookup"><span data-stu-id="f3077-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="f3077-106">Hvis du vil have mere at vide om, hvordan du synkroniserer brugere, grupper og kontakter, skal du se [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)og følge Synkronisering af en lokal gruppe til Azure ved hjælp af Azure AD Connect for at synkronisere efter pr.m-grupper ved hjælp af AD Connect. [](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="f3077-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="f3077-107">Følg denne vejledning til [fejlfinding under synkronisering for at](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) foretage fejlfinding af almindelige fejl under synkronisering.</span><span class="sxs-lookup"><span data-stu-id="f3077-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

