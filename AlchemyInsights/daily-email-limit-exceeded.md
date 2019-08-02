---
title: Daglige e-mail-grænse er overskredet. Arbejdsprocessen er afbrudt.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059633"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="e41c9-103">Daglige e-mail, der er overskredet.</span><span class="sxs-lookup"><span data-stu-id="e41c9-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="e41c9-104">Arbejdsprocessen er afbrudt.</span><span class="sxs-lookup"><span data-stu-id="e41c9-104">Workflow is suspended.</span></span>

<span data-ttu-id="e41c9-105">Denne fejl kan modtages i følgende situationer:</span><span class="sxs-lookup"><span data-stu-id="e41c9-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="e41c9-106">Du har en arbejdsproces i SharePoint Online, der bruger SharePoint 2010 eller SharePoint 2013 platform arbejdsgangstype.</span><span class="sxs-lookup"><span data-stu-id="e41c9-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="e41c9-107">Arbejdsgangen er konfigureret til at sende en brugerdefineret e-mail-meddelelse til mere end 200 brugere ad gangen, mere end 10.000 modtagere pr. dag eller mere end 30 meddelelser pr. minut.</span><span class="sxs-lookup"><span data-stu-id="e41c9-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="e41c9-108">Når du kører arbejdsgangen, sendes e-mailen ikke, og du bemærke følgende funktionsmåde:</span><span class="sxs-lookup"><span data-stu-id="e41c9-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="e41c9-109">For en arbejdsproces ved hjælp af typen SharePoint 2013-platform, kan du gå til **siden arbejdsprocesstatus** .</span><span class="sxs-lookup"><span data-stu-id="e41c9-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="e41c9-110">På siden Status for arbejdsproces **Interne Status** er angivet til **startet**og markeringsboblen oplysninger viser **kunne ikke sendes til en modtager**.</span><span class="sxs-lookup"><span data-stu-id="e41c9-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="e41c9-111">Du kan løse dette problem ved at konfigurere arbejdsgangen til at sende e-mail-meddelelser uden at overskride [grænser for Exchange Online afsender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="e41c9-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="e41c9-112">Brug en pause i arbejdsprocessen, sende e-mailen til en Office 365-gruppe, en distributionsgruppe eller en sikkerhedsgruppe for post, der er aktiveret, eller send meddelelsen til mindre end 200 modtagere på én gang.</span><span class="sxs-lookup"><span data-stu-id="e41c9-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="e41c9-113">Du kan finde flere oplysninger i følgende [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="e41c9-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="e41c9-114">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="e41c9-114">Related topics</span></span>
- [<span data-ttu-id="e41c9-115">Oprette produktionsflow</span><span class="sxs-lookup"><span data-stu-id="e41c9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e41c9-116">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="e41c9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 