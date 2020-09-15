---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688796"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b4b3e-102">Adgang nægtet, når du får vist en arbejdsproces</span><span class="sxs-lookup"><span data-stu-id="b4b3e-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b4b3e-103">SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med fejlmeddelelsen "adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er indstillet til alle.</span><span class="sxs-lookup"><span data-stu-id="b4b3e-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b4b3e-104">**Du kan løse dette problem ved at følge disse trin:**</span><span class="sxs-lookup"><span data-stu-id="b4b3e-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b4b3e-105">Tillad alle at se medlemmerne af SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="b4b3e-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="b4b3e-106">Fjern SharePoint-gruppen fra linjen til eller CC i mailen.</span><span class="sxs-lookup"><span data-stu-id="b4b3e-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="b4b3e-107">Føj eksplicit brugere til til-eller CC-linjen, hvis medlemskabet af medlemskabet ikke kan ændres for SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="b4b3e-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="b4b3e-108">Hvis du vil have mere at vide, skal du se [http-uautoriseret til/_vti_bin/Client.Svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b4b3e-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  