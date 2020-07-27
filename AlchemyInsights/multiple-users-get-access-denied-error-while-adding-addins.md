---
title: Flere brugere får fejlmeddelelsen Adgang nægtet, mens der tilføjes tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423480"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="176cd-102">Flere brugere får fejlmeddelelsen Adgang nægtet, mens der tilføjes tilføjelsesprogrammer i Outlook</span><span class="sxs-lookup"><span data-stu-id="176cd-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="176cd-103">Du kan angive, hvilke administratorer i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til Outlook.</span><span class="sxs-lookup"><span data-stu-id="176cd-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="176cd-104">Du kan også angive, hvilke brugere i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til eget brug.</span><span class="sxs-lookup"><span data-stu-id="176cd-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="176cd-105">Yderligere oplysninger kan finde [oplysninger under Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="176cd-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="176cd-106">Hvis du vil kontrollere, at du har tildelt tilladelser til en bruger, skal du erstatte med navnet på den <Role Name> rolle, der skal bekræftes, og køre følgende kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="176cd-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="176cd-107">Get-ManagementRoleAssignment -Role " <Role Name> -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="176cd-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="176cd-108">I dette eksempel kan du se, hvordan du kan kontrollere, hvem du har tildelt tilladelser til at installere tilføjelsesprogrammer fra Office Store for organisationen.</span><span class="sxs-lookup"><span data-stu-id="176cd-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="176cd-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="176cd-109">PowerShell</span></span>

<span data-ttu-id="176cd-110">-Rolle "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="176cd-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="176cd-111">I resultaterne skal Get-ManagementRoleAssignment gennemse posterne i kolonnen Effektive brugere.</span><span class="sxs-lookup"><span data-stu-id="176cd-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="176cd-112">Yderligere syntaks- og parameteroplysninger [finder du i Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="176cd-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 