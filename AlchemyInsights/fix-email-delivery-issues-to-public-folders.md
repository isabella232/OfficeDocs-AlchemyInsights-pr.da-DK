---
title: Løse problemer med e-mail-levering til postaktiverede offentlige mapper
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910587"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="d9b98-102">Løse problemer med e-mail-levering til postaktiverede offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="d9b98-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="d9b98-103">Hvis eksterne afsendere kan ikke sende meddelelser til dine offentlige mapper med e-mail-aktiveret og afsendere modtager fejl: **ikke fundet (550 5.4.1)**, kontrollere e-mail-domæne til den offentlige mappe er konfigureret som en intern relay domæne i stedet for en autoritative domæne:</span><span class="sxs-lookup"><span data-stu-id="d9b98-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="d9b98-104">Åbn [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="d9b98-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="d9b98-105">Gå til **Poststrøm** \> **godkendte domæner**, Vælg det accepterede domæne, og klik derefter på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="d9b98-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="d9b98-106">Side, der åbnes, hvis domænetype er indstillet til **Authoritative**i egenskaberne, ændre værdien til **interne relay** , og klik derefter på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="d9b98-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="d9b98-107">Hvis eksterne afsendere modtager fejlen **du ikke har tilladelse (550 5.7.13)**, skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) til at få vist tilladelser for anonyme brugere i den offentlige mappe:</span><span class="sxs-lookup"><span data-stu-id="d9b98-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="d9b98-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="d9b98-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="d9b98-109">For at give eksterne brugere at sende e-mail til denne offentlige mappe, kan du tilføje adgang CreateItems ret til brugertypen Anonym.</span><span class="sxs-lookup"><span data-stu-id="d9b98-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="d9b98-110">For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="d9b98-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
