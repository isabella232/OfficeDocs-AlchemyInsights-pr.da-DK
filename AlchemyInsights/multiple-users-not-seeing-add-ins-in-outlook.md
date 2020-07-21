---
title: Flere brugere kan ikke se tilføjelsesprogrammer i Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197839"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="779ef-102">Flere brugere kan ikke se tilføjelsesprogrammer i Outlook</span><span class="sxs-lookup"><span data-stu-id="779ef-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="779ef-103">Hvis du tester Outlook-tilføjelsesprogrammer, og ingen vises, skal du som et første fejlfindingstrin bruge Cmdlet'en **Get-OrganizationConfig** PowerShell til at forespørge på parameteren _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="779ef-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="779ef-104">Hvis forespørgslen returnerer en værdi af **Falsk**, skal du angive denne parameter til **Sand** ved hjælp af **set-OrganizationConfig-cmdlet'en,** så tilføjelsesprogrammer vises som forventet.</span><span class="sxs-lookup"><span data-stu-id="779ef-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="779ef-105">Vi anbefaler ikke, at parameteren _AppsForOfficeEnabled_ er angivet til **False**.</span><span class="sxs-lookup"><span data-stu-id="779ef-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="779ef-106">En værdi af **Falsk** tilsidesætter alle ovenstående indstillinger for administrative og brugeriske rolle og forhindrer, at nye apps aktiveres af en bruger i organisationen.</span><span class="sxs-lookup"><span data-stu-id="779ef-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="779ef-107">Du kan finde flere oplysninger [under Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="779ef-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>