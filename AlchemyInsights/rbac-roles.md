---
title: 'RBAC-roller '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583350"
---
# <a name="rbac-rules"></a><span data-ttu-id="2b1e5-102">RBAC-regler</span><span class="sxs-lookup"><span data-stu-id="2b1e5-102">RBAC rules</span></span>

<span data-ttu-id="2b1e5-103">Hvis du får tilladelses fejlen:</span><span class="sxs-lookup"><span data-stu-id="2b1e5-103">If you get the permission error:</span></span> 

- <span data-ttu-id="2b1e5-104">**Klienten med objekt-id har ikke tilladelse til at udføre handlingen over område (kode: AuthorizationFailed)**: når du forsøger at oprette en ressource, skal du kontrollere, at du er logget på med en bruger, der er tildelt en rolle, der har skrivetilladelse til ressourcen i det valgte område.</span><span class="sxs-lookup"><span data-stu-id="2b1e5-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="2b1e5-105">Hvis du vil administrere virtuelle maskiner i en ressourcegruppe, skal du have rollen som [virtuel maskines bidragyder](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) i ressourcegruppen (eller det overordnede omfang).</span><span class="sxs-lookup"><span data-stu-id="2b1e5-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="2b1e5-106">Hvis du vil have en liste over tilladelserne for hver indbygget rolle, skal du se [indbyggede roller for Azure-ressourcer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2b1e5-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="2b1e5-107">**Du har ikke tilladelse til at oprette en supportanmodning**: når du forsøger at oprette eller opdatere en supportanmodning, skal du kontrollere, at du i øjeblikket er logget på med en bruger, der har fået tildelt en rolle, der har Microsoft. support/supportTickets/Write permission, f. eks. [support anmodningens bidragyder](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="2b1e5-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="2b1e5-108">**Der kan ikke oprettes flere rolletildelinger (kode: RoleAssignmentLimitExceeded)**: når du forsøger at tildele en rolle, kan du prøve at reducere antallet af rolletildelinger ved i stedet at tildele roller til grupper.</span><span class="sxs-lookup"><span data-stu-id="2b1e5-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="2b1e5-109">Azure understøtter op til **2000** rolletildelinger pr. abonnement.</span><span class="sxs-lookup"><span data-stu-id="2b1e5-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="2b1e5-110">Du kan finde flere oplysninger om Azure RBAC-roller i [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2b1e5-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
