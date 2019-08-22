---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495817"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e2ec8-102">Adgang nægtet, når du får vist en arbejdsproces</span><span class="sxs-lookup"><span data-stu-id="e2ec8-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e2ec8-103">SharePoint 2013 arbejdsprocesser, der forsøger at sende en e-mail til en SharePoint-gruppe kan mislykkes med en "Adgang nægtet"-fejlmeddelelse, hvis medlemskab af gruppen SharePoint ikke er indstillet til alle.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e2ec8-104">**Du kan løse dette problem ved at gøre disse trin:**</span><span class="sxs-lookup"><span data-stu-id="e2ec8-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e2ec8-105">Gør det muligt for alle at se medlemmer af SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e2ec8-106">Fjern SharePoint-gruppen fra boksen til eller CC linje i e-mailen.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e2ec8-107">Tilføj brugerne eksplicit til til eller CC linje, hvis medlemskab synlighed ikke kan ændres for SharePoint-gruppe.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e2ec8-108">For at få vist se flere oplysninger [HTTP med uautoriserede /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e2ec8-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  