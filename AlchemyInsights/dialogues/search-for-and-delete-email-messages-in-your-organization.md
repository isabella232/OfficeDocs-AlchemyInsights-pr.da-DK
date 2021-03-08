---
title: Søge efter og slette mails i din organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523691"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="0eb21-102">Søge efter og slette mails i din organisation</span><span class="sxs-lookup"><span data-stu-id="0eb21-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="0eb21-103">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="0eb21-103">Follow these steps:</span></span>

1. <span data-ttu-id="0eb21-104">Hvis du ikke er global administrator, skal din konto føjes til **rollegruppen for eDiscovery Manager** eller administration af overholdelsessøgning for at søge efter **meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="0eb21-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="0eb21-105">Hvis du vil slette meddelelser, skal du deltage i **rollegruppen Organisationsadministration** eller **administrationsrollen Søg og tøm.**</span><span class="sxs-lookup"><span data-stu-id="0eb21-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="0eb21-106">Tilladelser til disse roller tildeles i [Sikkerheds- & overholdelsescenter.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="0eb21-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="0eb21-107">[Opret en indholdssøgning for](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde den meddelelse, du vil slette.</span><span class="sxs-lookup"><span data-stu-id="0eb21-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="0eb21-108">[Opret forbindelse til Security & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0eb21-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="0eb21-109">Hvis du bruger MFA, skal du se denne vejledning: Opret forbindelse til [Security & Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0eb21-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="0eb21-110">Slet meddelelsen: Kør `New-ComplianceSearchAction` cmdlet'en for at slette meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="0eb21-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="0eb21-111">Slettede meddelelser flyttes til en brugers mappe genoprettelige elementer.</span><span class="sxs-lookup"><span data-stu-id="0eb21-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="0eb21-112">Se trin 3 for at [få en eksempelkommando: Slet meddelelsen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="0eb21-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
