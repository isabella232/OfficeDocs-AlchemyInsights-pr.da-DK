---
title: Introduktion til SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700701"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="46baa-102">Arbejdsprocesser i SharePoint</span><span class="sxs-lookup"><span data-stu-id="46baa-102">Workflows in SharePoint</span></span>

<span data-ttu-id="46baa-103">Hvis SharePoint-arbejdsprocesser ikke sender mails, kan din organisation have registreret Exchange Online-afsender grænsen.</span><span class="sxs-lookup"><span data-stu-id="46baa-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="46baa-104">Fejlmeddelelsen "arbejdsprocessen er suspenderet" kan forekomme, hvis du har et af følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="46baa-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="46baa-105">Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-typen arbejdsproces platform.</span><span class="sxs-lookup"><span data-stu-id="46baa-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="46baa-106">Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.</span><span class="sxs-lookup"><span data-stu-id="46baa-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="46baa-107">Når du kører arbejdsprocessen, bliver mail meddelelsen ikke sendt, og du bemærker fejlmeddelelsen, den interne status er sat til suspenderet eller kan ikke sendes til en modtager vises.</span><span class="sxs-lookup"><span data-stu-id="46baa-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="46baa-108">Hvis du vil have mere at vide, skal du se følgende [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="46baa-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

