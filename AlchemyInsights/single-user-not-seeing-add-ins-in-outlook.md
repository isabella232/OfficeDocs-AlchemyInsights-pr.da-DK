---
title: Enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719659"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ea57d-102">Enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook</span><span class="sxs-lookup"><span data-stu-id="ea57d-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ea57d-103">Brugeren kan være en del af en rolle, der ikke har den korrekte AppsForOfficeEnabled-parameter.</span><span class="sxs-lookup"><span data-stu-id="ea57d-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="ea57d-104">Kør denne cmdlet for at finde ud af, om den rette rolle er knyttet til brugeren:</span><span class="sxs-lookup"><span data-stu-id="ea57d-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="ea57d-105">Get-ManagementRoleAssignment-RoleAssignee user@domain.com-delegere $false | Formatér-tabel-automatisk rolle, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="ea57d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="ea57d-106">Du kan finde flere oplysninger i [angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="ea57d-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
