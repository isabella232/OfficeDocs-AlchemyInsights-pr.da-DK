---
title: Sidder fast i udbakken på grund af store vedhæftede filer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441300"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="76b4a-102">Ret meddelelser, der sidder fast i udbakken</span><span class="sxs-lookup"><span data-stu-id="76b4a-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="76b4a-103">Vi anbefaler, at du starter med at køre scenariet ["Jeg har problemer med at sende, modtage eller finde mails"](https://aka.ms/SaRA-OutlookSendReceive) fra værktøjet [Microsoft support og genoprettelsesassistent](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="76b4a-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="76b4a-104">Når en meddelelse sidder fast i udbakken, er de mest sandsynlige årsager:</span><span class="sxs-lookup"><span data-stu-id="76b4a-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="76b4a-105">Store vedhæftede filer.</span><span class="sxs-lookup"><span data-stu-id="76b4a-105">Large attachments.</span></span>
- <span data-ttu-id="76b4a-106">Indstillingen **Send med det samme, når** den er tilsluttet er ikke aktiveret.</span><span class="sxs-lookup"><span data-stu-id="76b4a-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="76b4a-107">Sådan fjerner du store vedhæftede filer:</span><span class="sxs-lookup"><span data-stu-id="76b4a-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="76b4a-108">I Outlook skal du vælge **Send/modtag** > **arbejde offline**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="76b4a-109">Vælg **Udbakke**i navigationsruden.</span><span class="sxs-lookup"><span data-stu-id="76b4a-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="76b4a-110">Herfra kan du:</span><span class="sxs-lookup"><span data-stu-id="76b4a-110">From here, you can:</span></span> 
    - <span data-ttu-id="76b4a-111">Slet beskeden (Vælg den, og vælg derefter **Slet**).</span><span class="sxs-lookup"><span data-stu-id="76b4a-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="76b4a-112">Træk beskeden til mappen Kladder, dobbeltklik for at åbne den, og fjern den vedhæftede fil Vælg den, og vælg derefter **Slet**).</span><span class="sxs-lookup"><span data-stu-id="76b4a-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="76b4a-113">Hvis du får vist en fejlmeddelelse om, at Outlook forsøger at overføre meddelelsen, skal du lukke Outlook.</span><span class="sxs-lookup"><span data-stu-id="76b4a-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="76b4a-114">Det kan tage et øjeblik at afslutte.</span><span class="sxs-lookup"><span data-stu-id="76b4a-114">It may take a few moments to exit.</span></span> <span data-ttu-id="76b4a-115">Hvis Outlook ikke lukkes, skal du trykke på Ctrl + Alt + Delete og vælge **Start Jobliste**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="76b4a-116">Vælg fanen **processer** i Jobliste, Rul ned til Outlook. exe, og vælg **Afslut proces**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="76b4a-117">Når Outlook er lukket, skal du genstarte det og gentage trin 2 og 3.</span><span class="sxs-lookup"><span data-stu-id="76b4a-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="76b4a-118">Når du har fjernet den vedhæftede fil, skal du klikke på **Send/modtag** > **arbejde offline** for at genoptage arbejdet online.</span><span class="sxs-lookup"><span data-stu-id="76b4a-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="76b4a-119">Meddelelser går også i stå i udbakken, når du klikker på **Send**, men du har ikke forbindelse.</span><span class="sxs-lookup"><span data-stu-id="76b4a-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="76b4a-120">Klik på **Send/modtag** , og se på knappen **Arbejd offline** .</span><span class="sxs-lookup"><span data-stu-id="76b4a-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="76b4a-121">Hvis det er blåt, er du afbrudt.</span><span class="sxs-lookup"><span data-stu-id="76b4a-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="76b4a-122">Vælg den for at oprette forbindelse (knappen bliver hvid), og klik på **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="76b4a-123">Sådan aktiverer du **Send med det samme, når forbindelsen er oprettet**:</span><span class="sxs-lookup"><span data-stu-id="76b4a-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="76b4a-124">Vælg **filindstillinger** > \*\*\*\* >  **Avanceret**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="76b4a-125">I sektionen **Send og modtag** skal du vælge **Send med det samme, når du er tilsluttet**, og derefter vælge **OK**.</span><span class="sxs-lookup"><span data-stu-id="76b4a-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="76b4a-126">For udførlige oplysninger se:</span><span class="sxs-lookup"><span data-stu-id="76b4a-126">For full details see:</span></span>
- [<span data-ttu-id="76b4a-127">Video: sende eller slette en fast e-mail</span><span class="sxs-lookup"><span data-stu-id="76b4a-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="76b4a-128">Mail forbliver i mappen Udbakke, indtil du manuelt starter en Send/modtag-handling i Outlook</span><span class="sxs-lookup"><span data-stu-id="76b4a-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
