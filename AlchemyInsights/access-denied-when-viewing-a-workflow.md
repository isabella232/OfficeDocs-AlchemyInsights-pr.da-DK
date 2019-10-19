---
title: Adgang nægtet ved visning af en arbejdsproces
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747742"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="86c63-102">Adgang nægtet ved visning af en arbejdsproces</span><span class="sxs-lookup"><span data-stu-id="86c63-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="86c63-103">SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med en fejlmeddelelse af typen "adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er angivet til alle.</span><span class="sxs-lookup"><span data-stu-id="86c63-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="86c63-104">**Du kan løse dette problem ved at benytte følgende fremgangsmåde:**</span><span class="sxs-lookup"><span data-stu-id="86c63-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="86c63-105">Tillad alle at se medlemmerne af SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="86c63-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="86c63-106">Fjern SharePoint-gruppen fra linjen til eller CC i e-mailen.</span><span class="sxs-lookup"><span data-stu-id="86c63-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="86c63-107">Føj eksplicit brugerne til linjen til eller CC, hvis medlems synlighed ikke kan ændres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="86c63-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="86c63-108">For at se flere oplysninger henvises til [http uautoriseret til/_vti_bin/Client.Svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="86c63-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  