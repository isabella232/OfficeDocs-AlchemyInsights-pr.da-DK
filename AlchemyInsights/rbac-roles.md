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
# <a name="rbac-rules"></a>RBAC-regler

Hvis du får tilladelses fejlen: 

- **Klienten med objekt-id har ikke tilladelse til at udføre handlingen over område (kode: AuthorizationFailed)**: når du forsøger at oprette en ressource, skal du kontrollere, at du er logget på med en bruger, der er tildelt en rolle, der har skrivetilladelse til ressourcen i det valgte område. Hvis du vil administrere virtuelle maskiner i en ressourcegruppe, skal du have rollen som [virtuel maskines bidragyder](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) i ressourcegruppen (eller det overordnede omfang). Hvis du vil have en liste over tilladelserne for hver indbygget rolle, skal du se [indbyggede roller for Azure-ressourcer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Du har ikke tilladelse til at oprette en supportanmodning**: når du forsøger at oprette eller opdatere en supportanmodning, skal du kontrollere, at du i øjeblikket er logget på med en bruger, der har fået tildelt en rolle, der har Microsoft. support/supportTickets/Write permission, f. eks. [support anmodningens bidragyder](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Der kan ikke oprettes flere rolletildelinger (kode: RoleAssignmentLimitExceeded)**: når du forsøger at tildele en rolle, kan du prøve at reducere antallet af rolletildelinger ved i stedet at tildele roller til grupper. Azure understøtter op til **2000** rolletildelinger pr. abonnement.

Du kan finde flere oplysninger om Azure RBAC-roller i [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
