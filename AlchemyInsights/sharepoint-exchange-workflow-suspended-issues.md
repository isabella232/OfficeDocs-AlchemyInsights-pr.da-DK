---
title: Introduktion til SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751666"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="474c9-102">Arbejdsprocesser i SharePoint</span><span class="sxs-lookup"><span data-stu-id="474c9-102">Workflows in SharePoint</span></span>

<span data-ttu-id="474c9-103">Hvis SharePoint-arbejdsprocesser ikke sender mails, kan din organisation være stødt på grænserne for afsenderens Exchange Online-afsender.</span><span class="sxs-lookup"><span data-stu-id="474c9-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="474c9-104">Fejlmeddelelsen ' arbejdsprocessen er suspenderet ' kan opstå, hvis du har et af følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="474c9-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="474c9-105">Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-arbejdsgangs platforms typen.</span><span class="sxs-lookup"><span data-stu-id="474c9-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="474c9-106">Arbejdsprocessen er konfigureret til at sende en brugerdefineret e-mail-meddelelse til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.</span><span class="sxs-lookup"><span data-stu-id="474c9-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="474c9-107">Når du kører arbejdsprocessen, sendes e-mailen ikke, og du bemærker fejlmeddelelsen, den interne status er indstillet til suspenderet eller ikke kan sendes til en modtager vises.</span><span class="sxs-lookup"><span data-stu-id="474c9-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="474c9-108">Yderligere oplysninger finder du i følgende [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="474c9-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

