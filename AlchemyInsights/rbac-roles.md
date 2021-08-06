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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923125"
---
# <a name="rbac-rules"></a>RBAC-regler

Hvis du får tilladelsesfejlen: 

- Klienten med objekt-id har ikke tilladelse til at udføre en handling over omfang **(kode: AuthorizationFailed):** Når du forsøger at oprette en ressource, skal du kontrollere, at du i øjeblikket er logget på med en bruger, der er tildelt en rolle, der har skrivetilladelse til ressourcen i det valgte omfang. Hvis du f.eks. vil administrere virtuelle maskiner i en ressourcegruppe, skal du have [rollen som Virtual Machine-bidragyder](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) på ressourcegruppen (eller det overordnede omfang). Du kan finde en liste over tilladelserne for hver indbygget rolle under [Indbyggede roller for Azure-ressourcer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Du har ikke tilladelse til at oprette en **supportanmodning:** Når du forsøger at oprette eller opdatere en supportanmodning, skal du kontrollere, at du i øjeblikket er logget på med en bruger, der er tildelt en rolle, der har tilladelsen Microsoft.Support/supportTickets/write, f.eks. Supportanmodningsbidragsyder. [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Der kan ikke oprettes flere rolletildelinger **(kode: RoleAssignmentLimitExceeded):** Når du forsøger at tildele en rolle, kan du i stedet prøve at reducere antallet af rolletildelinger ved at tildele roller til grupper. Azure understøtter op til **2000 rolletildelinger** pr. abonnement.

Du kan finde flere oplysninger om Azure RBAC-roller i [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
