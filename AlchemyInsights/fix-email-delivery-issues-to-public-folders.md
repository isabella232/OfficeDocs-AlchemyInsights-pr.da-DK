---
title: Løs problemer med levering af mail til offentlige mapper, der er aktiveret til mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366458"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="994bf-102">Løs problemer med levering af mail til offentlige mapper, der er aktiveret til mail</span><span class="sxs-lookup"><span data-stu-id="994bf-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="994bf-103">Hvis eksterne afsendere ikke kan sende meddelelser til dine mailaktiverede offentlige mapper, og afsenderen modtager fejlen: **blev ikke fundet (550 5.4.1)**, skal du kontrollere, at mail domænet for den offentlige mappe er konfigureret som et internt Relay-domæne i stedet for et autoritativt domæne:</span><span class="sxs-lookup"><span data-stu-id="994bf-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="994bf-104">Åbn [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="994bf-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="994bf-105">Gå til **mail flow** \> **accepterede domæner**, Vælg det accepterede domæne, og klik derefter på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="994bf-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="994bf-106">På siden med egenskaber, der åbnes, hvis domæne typen er angivet til **autoritativ**, skal du ændre værdien til **intern relæ** og derefter klikke på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="994bf-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="994bf-107">Hvis eksterne afsendere modtager den fejl, **du ikke har tilladelse (550 5.7.13)**, skal du køre følgende kommando i [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) for at få vist tilladelserne for anonyme brugere i den offentlige mappe:</span><span class="sxs-lookup"><span data-stu-id="994bf-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="994bf-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For eksempel `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="994bf-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="994bf-109">Hvis du vil tillade, at eksterne brugere sender mails til denne offentlige mappe, skal du føje CreateItems adgang til anonyme brugere.</span><span class="sxs-lookup"><span data-stu-id="994bf-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="994bf-110">For eksempel `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="994bf-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
