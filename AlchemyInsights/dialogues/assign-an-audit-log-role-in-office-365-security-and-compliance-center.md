---
title: Tildel en overvågningslogrolle i Office 365 Security & Compliance Center
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523973"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="50146-102">Tildel en overvågningslogrolle i Office 365 Security & Compliance Center</span><span class="sxs-lookup"><span data-stu-id="50146-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="50146-103">Hvis du vil søge i Office 365-overvågningsloggen, skal en administrator have tildelt rollen Kun **visningslog** eller overvågningsloggen i Exchange Online. </span><span class="sxs-lookup"><span data-stu-id="50146-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="50146-104">Disse roller tildeles som standard rollegrupperne Administration af overholdelse og Organisationsadministration.</span><span class="sxs-lookup"><span data-stu-id="50146-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="50146-105">Globale administratorer i Office 365 og Microsoft 365 tilføjes automatisk som medlemmer af rollegruppen Organisationsadministration.</span><span class="sxs-lookup"><span data-stu-id="50146-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="50146-106">Hvis du vil gøre det muligt for en bruger at søge med det mindste niveau af rettigheder, skal du oprette en brugerdefineret rollegruppe i Exchange Online, tilføje rollen Kun **visningslogfiler** eller **Overvågningslogfiler** og derefter tilføje brugeren som medlem af den nye rollegruppe.</span><span class="sxs-lookup"><span data-stu-id="50146-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="50146-107">Du kan finde flere oplysninger [i Administrere rollegrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) og søge i [overvågningsloggen i Security & Compliance Center.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="50146-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>