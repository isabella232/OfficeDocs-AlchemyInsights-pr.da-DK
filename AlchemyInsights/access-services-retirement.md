---
title: Ydelse af adgangs ydelser
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698676"
---
# <a name="access-services-retirement"></a><span data-ttu-id="2713c-102">Ydelse af adgangs ydelser</span><span class="sxs-lookup"><span data-stu-id="2713c-102">Access services retirement</span></span>

<span data-ttu-id="2713c-103">Som vi oprindeligt har offentliggjort i MC97576, i marts 2017 og fortsat at kommunikere over de seneste års Access-tjenester udgår.</span><span class="sxs-lookup"><span data-stu-id="2713c-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="2713c-104">Den næste fase i denne proces er at fjerne Access-webdatabaser, der bruger SharePoint-lister som underliggende datalager.</span><span class="sxs-lookup"><span data-stu-id="2713c-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="2713c-105">**Hvordan påvirker det mig?**</span><span class="sxs-lookup"><span data-stu-id="2713c-105">**How does this affect me?**</span></span>

<span data-ttu-id="2713c-106">Fra juni 2019 stopper vi med at oprette nye Access-databaser i SharePoint Online og lukker tjenesten og eventuelle resterende apps ved april 2020.</span><span class="sxs-lookup"><span data-stu-id="2713c-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="2713c-107">**Hvad skal jeg gøre for at forberede denne ændring?**</span><span class="sxs-lookup"><span data-stu-id="2713c-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="2713c-108">Vi opfordrer dig til at oprette en overgangsplan for din organisations Access-webdatabaser.</span><span class="sxs-lookup"><span data-stu-id="2713c-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="2713c-109">Administratorer kan bruge [Scannerprogrammet SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over de Access-apps, som websteder bruger.</span><span class="sxs-lookup"><span data-stu-id="2713c-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="2713c-110">Du kan overføre data fra Access-databaser på flere måder:</span><span class="sxs-lookup"><span data-stu-id="2713c-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="2713c-111">Importere til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="2713c-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="2713c-112">Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette gratis virksomhedsløsninger til web-og mobilenheder.</span><span class="sxs-lookup"><span data-stu-id="2713c-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>