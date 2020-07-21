---
title: En enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197831"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="b12d5-102">En enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook</span><span class="sxs-lookup"><span data-stu-id="b12d5-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="b12d5-103">Brugeren kan være en del af en rolle, der ikke har den korrekte Parameter AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="b12d5-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="b12d5-104">Kør denne cmdlet for at finde ud af, om den korrekte rolle er knyttet til brugeren:</span><span class="sxs-lookup"><span data-stu-id="b12d5-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="b12d5-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Uddelegering $false | Format-tabel -auto-rolle,RolleassigneeNavn,RolleassigneeType</span><span class="sxs-lookup"><span data-stu-id="b12d5-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="b12d5-106">Du kan finde flere oplysninger under [Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="b12d5-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
