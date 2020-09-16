---
title: Flere brugere får adgang nægtet-fejl under tilføjelse af tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724357"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="dffcf-102">Flere brugere får adgang nægtet-fejl under tilføjelse af tilføjelsesprogrammer i Outlook</span><span class="sxs-lookup"><span data-stu-id="dffcf-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="dffcf-103">Du kan angive, hvilke administratorer i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til Outlook.</span><span class="sxs-lookup"><span data-stu-id="dffcf-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="dffcf-104">Du kan også angive, hvilke brugere i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til deres eget brug.</span><span class="sxs-lookup"><span data-stu-id="dffcf-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="dffcf-105">Hvis du vil have mere at vide, skal du se [angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="dffcf-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="dffcf-106">Hvis du vil bekræfte, at du har fået tildelt tilladelser for en bruger, skal du erstatte <Role Name> med navnet på rollen for at bekræfte og køre følgende kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="dffcf-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="dffcf-107">Get-ManagementRoleAssignment-Role " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="dffcf-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="dffcf-108">I dette eksempel kan du se, hvordan du kan se, hvem du har tildelt tilladelser til at installere tilføjelsesprogrammer fra Office store for organisationen.</span><span class="sxs-lookup"><span data-stu-id="dffcf-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="dffcf-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="dffcf-109">PowerShell</span></span>

<span data-ttu-id="dffcf-110">-Role "org Marketplace-apps"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="dffcf-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="dffcf-111">I resultaterne, Get-ManagementRoleAssignment, skal du gennemgå posterne i kolonnen effektive brugere.</span><span class="sxs-lookup"><span data-stu-id="dffcf-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="dffcf-112">Du kan finde detaljerede oplysninger om syntaks og parameter under [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="dffcf-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 