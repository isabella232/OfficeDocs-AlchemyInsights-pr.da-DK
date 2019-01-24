---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464120"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="6a28b-102">Adgang nægtet, når du får vist en arbejdsproces</span><span class="sxs-lookup"><span data-stu-id="6a28b-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="6a28b-103">SharePoint 2013 arbejdsprocesser, der forsøger at sende en e-mail til en SharePoint-gruppe kan mislykkes med en "Adgang nægtet"-fejlmeddelelse, hvis medlemskab af gruppen SharePoint ikke er indstillet til alle.</span><span class="sxs-lookup"><span data-stu-id="6a28b-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="6a28b-104">**Du kan løse dette problem ved at gøre disse trin:**</span><span class="sxs-lookup"><span data-stu-id="6a28b-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="6a28b-105">Gør det muligt for alle at se medlemmer af SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="6a28b-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="6a28b-106">Fjern SharePoint-gruppen fra boksen til eller CC linje i e-mailen.</span><span class="sxs-lookup"><span data-stu-id="6a28b-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="6a28b-107">Tilføj brugerne eksplicit til til eller CC linje, hvis medlemskab synlighed ikke kan ændres for SharePoint-gruppe.</span><span class="sxs-lookup"><span data-stu-id="6a28b-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="6a28b-108">For at få vist se flere oplysninger [HTTP med uautoriserede /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="6a28b-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

