---
title: Adgang nægtet ved visning af en arbejdsproces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687324"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e327f-102">Adgang nægtet ved visning af en arbejdsproces</span><span class="sxs-lookup"><span data-stu-id="e327f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e327f-103">SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med fejlmeddelelsen "Adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er angivet til Alle.</span><span class="sxs-lookup"><span data-stu-id="e327f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e327f-104">**Du kan lÃ ̧se problemet ved at benytte disse trin:**</span><span class="sxs-lookup"><span data-stu-id="e327f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e327f-105">Giv alle mulighed for at se medlemmerne af SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="e327f-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e327f-106">Fjern SharePoint-gruppen fra linjen Til eller CC i mailen.</span><span class="sxs-lookup"><span data-stu-id="e327f-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e327f-107">Føj eksplicit brugerne til linjen Til eller CC, hvis synligheden af medlemskabet ikke kan ændres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="e327f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e327f-108">Du kan få vist flere oplysninger ved at se [HTTP Uautoriseret til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e327f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  