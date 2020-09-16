---
title: Grænsen for daglige mails er overskredet. Arbejdsprocessen er suspenderet.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731557"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="82573-103">Grænsen for daglige mails er overskredet.</span><span class="sxs-lookup"><span data-stu-id="82573-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="82573-104">Arbejdsprocessen er suspenderet.</span><span class="sxs-lookup"><span data-stu-id="82573-104">Workflow is suspended.</span></span>

<span data-ttu-id="82573-105">Denne fejl kan være modtaget i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="82573-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="82573-106">Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010-eller SharePoint 2013-typen arbejdsproces platform.</span><span class="sxs-lookup"><span data-stu-id="82573-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="82573-107">Arbejdsprocessen er konfigureret til at sende en brugerdefineret mail til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.</span><span class="sxs-lookup"><span data-stu-id="82573-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="82573-108">Når du kører arbejdsprocessen, bliver mail meddelelsen ikke sendt, og du bemærker følgende funktionsmåde:</span><span class="sxs-lookup"><span data-stu-id="82573-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="82573-109">For en arbejdsproces, der bruger typen SharePoint 2013-platform, skal du gå til siden **status for arbejdsproces** .</span><span class="sxs-lookup"><span data-stu-id="82573-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="82573-110">På siden status for arbejdsproces er den **interne status** angivet til **Startet**, og oplysnings boblen vises ikke, så du kan **sende til en modtager**.</span><span class="sxs-lookup"><span data-stu-id="82573-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="82573-111">Du kan løse dette problem ved at konfigurere arbejdsprocessen til at sende mails uden at overskride [begrænsningerne for Exchange Online-afsenderen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="82573-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="82573-112">For eksempel skal du bruge en pause i arbejdsprocessen, sende mailen til en Microsoft 365-gruppe, en distributionsgruppe eller en e-mail-aktiveret sikkerhedsgruppe eller sende meddelelsen til færre end 200 modtagere ad gangen.</span><span class="sxs-lookup"><span data-stu-id="82573-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="82573-113">Du kan finde flere oplysninger i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="82573-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="82573-114">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="82573-114">Related topics</span></span>
- [<span data-ttu-id="82573-115">Opret flow</span><span class="sxs-lookup"><span data-stu-id="82573-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="82573-116">SharePoint og flow</span><span class="sxs-lookup"><span data-stu-id="82573-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 