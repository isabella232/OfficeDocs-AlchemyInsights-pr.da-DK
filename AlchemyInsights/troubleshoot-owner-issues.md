---
title: Fejlfinding af problemer med ejeren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900863"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="b4dec-102">Fejlfinding af problemer med ejeren</span><span class="sxs-lookup"><span data-stu-id="b4dec-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="b4dec-103">Hvis du vil foretage fejlfinding af problemer med ejeren, skal du udføre følgende trin:</span><span class="sxs-lookup"><span data-stu-id="b4dec-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="b4dec-104">[Tilføje eller ændre Azure-abonnements administratorer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory-grupper (Azure ad)-grupper ejes og administreres af gruppe ejere.</span><span class="sxs-lookup"><span data-stu-id="b4dec-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="b4dec-105">Gruppe ejere kan være brugere eller tjeneste principaler og kan administrere gruppen, herunder medlemskab.</span><span class="sxs-lookup"><span data-stu-id="b4dec-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="b4dec-106">Kun eksisterende gruppe ejere eller gruppe-administrerende administratorer kan tildele gruppe ejere.</span><span class="sxs-lookup"><span data-stu-id="b4dec-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="b4dec-107">Gruppe ejere behøver ikke at være medlem af gruppen.</span><span class="sxs-lookup"><span data-stu-id="b4dec-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="b4dec-108">[Tilføje eller ændre Azure-abonnements administratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): i denne artikel beskrives det, hvordan du kan tilføje eller ændre administratorrollen for en bruger ved hjælp af Azure RBAC på abonnements området.</span><span class="sxs-lookup"><span data-stu-id="b4dec-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="b4dec-109">Brug PowerShell til at tilføje en gruppeejer eller en program ejer.</span><span class="sxs-lookup"><span data-stu-id="b4dec-109">Use PowerShell to add a group owner or an application owner.</span></span>
