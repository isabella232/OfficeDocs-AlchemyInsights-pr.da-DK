---
title: Løs problemer med levering af mail til mailaktiverede offentlige mapper
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716346"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="c3ed7-102">Løs problemer med levering af mail til mailaktiverede offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="c3ed7-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="c3ed7-103">Hvis eksterne afsendere ikke kan sende meddelelser til dine e-mail-aktiverede offentlige mapper, og afsenderne får vist fejlen: **Blev ikke fundet (550 5.4.1),** skal du kontrollere, at maildomænet for den offentlige mappe er konfigureret som et internt relædomæne i stedet for et autoritativt domæne:</span><span class="sxs-lookup"><span data-stu-id="c3ed7-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="c3ed7-104">Åbn [Exchange Administration (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="c3ed7-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="c3ed7-105">Gå til **Mailflow** \> **Accepterede domæner**, vælg det accepterede domæne, og klik derefter på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="c3ed7-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="c3ed7-106">Hvis domænetypen er angivet til **Autoritativ**på siden egenskaber, der åbnes, skal du ændre værdien til **Internt relæ** og derefter klikke på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="c3ed7-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="c3ed7-107">Hvis eksterne afsendere får vist den **fejl, du ikke har tilladelse til (550 5.7.13),** skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for at få vist tilladelserne for anonyme brugere i den offentlige mappe:</span><span class="sxs-lookup"><span data-stu-id="c3ed7-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="c3ed7-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`F.eks.</span><span class="sxs-lookup"><span data-stu-id="c3ed7-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="c3ed7-109">Hvis du vil give eksterne brugere tilladelse til at sende mail til denne offentlige mappe, skal du føje adgangsrettigheden CreateItems til brugeren Anonym.</span><span class="sxs-lookup"><span data-stu-id="c3ed7-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="c3ed7-110">`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`F.eks.</span><span class="sxs-lookup"><span data-stu-id="c3ed7-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
