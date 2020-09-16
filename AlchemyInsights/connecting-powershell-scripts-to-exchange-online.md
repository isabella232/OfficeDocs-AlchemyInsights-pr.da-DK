---
title: Tilslutning af PowerShell-scripts til Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 3a8383a57bc1267311daf03c78841070cca8fb8f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748058"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="9ef1f-102">Tilslutning af PowerShell-scripts til Exchange Online</span><span class="sxs-lookup"><span data-stu-id="9ef1f-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="9ef1f-103">Basisgodkendelse i Exchange Online frarådes, og den måde, som viderestilles på, er at oprette forbindelse ved hjælp af certifikatbaseret godkendelse for scripts og automatiserede opgaver.</span><span class="sxs-lookup"><span data-stu-id="9ef1f-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="9ef1f-104">Hvis du vil have mere at vide, skal du se [kun app-only-godkendelse for automatiserede scripts i EXO v2-modulet](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span><span class="sxs-lookup"><span data-stu-id="9ef1f-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>