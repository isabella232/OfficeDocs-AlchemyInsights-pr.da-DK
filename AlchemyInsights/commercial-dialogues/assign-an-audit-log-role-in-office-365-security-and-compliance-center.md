---
title: Tildele en overvågningslogrolle i Sikkerheds- og & i Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744600"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Tildele en overvågningslogrolle i Sikkerheds- og & i Office 365

Hvis du vil søge i Office 365-overvågningsloggen, skal en administrator have tildelt rollen Kun **visningslog** eller overvågningsloggen i Exchange Online.  Disse roller tildeles som standard rollegrupperne Administration af overholdelse og Organisationsadministration. Globale administratorer i Office 365 og Microsoft 365 tilføjes automatisk som medlemmer af rollegruppen Organisationsadministration.

Hvis du vil gøre det muligt for en bruger at søge med det mindste niveau af rettigheder, skal du oprette en brugerdefineret rollegruppe i Exchange Online, tilføje rollen Kun **visningslogfiler** eller **Overvågningslogfiler** og derefter tilføje brugeren som medlem af den nye rollegruppe.

Du kan finde flere oplysninger [i Administrere rollegrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) og søge i [overvågningsloggen i Security & Compliance Center.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)