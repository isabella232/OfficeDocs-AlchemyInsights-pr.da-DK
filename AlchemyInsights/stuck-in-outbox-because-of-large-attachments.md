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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232624"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e711c-102">Rette meddelelser, der sidder fast i udbakken</span><span class="sxs-lookup"><span data-stu-id="e711c-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e711c-103">Vi anbefaler, at du starter med at køre scenariet ["Jeg har problemer med at sende, modtage eller finde mails"](https://aka.ms/SaRA-OutlookSendReceive) fra [værktøjet Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) på den berørte computer.</span><span class="sxs-lookup"><span data-stu-id="e711c-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="e711c-104">Når en meddelelse sidder fast i udbakken, er den mest sandsynlige årsag en stor vedhæftet fil, eller indstillingen "Send med det samme, når den er tilsluttet" er ikke aktiveret.</span><span class="sxs-lookup"><span data-stu-id="e711c-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e711c-105">**Fjerne den store vedhæftede fil**</span><span class="sxs-lookup"><span data-stu-id="e711c-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e711c-106">Klik på **Send/modtag** > **arbejde offline**.</span><span class="sxs-lookup"><span data-stu-id="e711c-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e711c-107">Klik på **Udbakke**i navigationsruden .</span><span class="sxs-lookup"><span data-stu-id="e711c-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="e711c-108">Herfra kan du:</span><span class="sxs-lookup"><span data-stu-id="e711c-108">From here, you can:</span></span> 
    - <span data-ttu-id="e711c-109">Slet meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="e711c-109">Delete the message.</span></span> <span data-ttu-id="e711c-110">Du skal blot markere den og klikke på **Slet**.</span><span class="sxs-lookup"><span data-stu-id="e711c-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="e711c-111">Træk meddelelsen til **kladdemappen**, dobbeltklik for at åbne meddelelsen, og slet den vedhæftede fil (klik på den, og klik på **Slet**).</span><span class="sxs-lookup"><span data-stu-id="e711c-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="e711c-112">Hvis en fejl fortæller dig, at Outlook forsøger at sende meddelelsen, skal du lukke Outlook.</span><span class="sxs-lookup"><span data-stu-id="e711c-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e711c-113">Det kan tage et øjeblik at afslutte.</span><span class="sxs-lookup"><span data-stu-id="e711c-113">It may take a few moments to exit.</span></span> <span data-ttu-id="e711c-114">Hvis Outlook ikke lukker, skal du trykke **på Ctrl+Alt+Delete** og klikke på **Start Jobliste**.</span><span class="sxs-lookup"><span data-stu-id="e711c-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="e711c-115">Vælg fanen **Processer** i Jobliste, rul ned til outlook.exe, og klik på **Afslut proces**.</span><span class="sxs-lookup"><span data-stu-id="e711c-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="e711c-116">Når Outlook er lukket, skal du genstarte Outlook og gentage trin 2-3.</span><span class="sxs-lookup"><span data-stu-id="e711c-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="e711c-117">Når du har fjernet den vedhæftede fil, skal du klikke på **Send/modtag** > **arbejde offline** for at fravælge knappen og for at fortsætte med at arbejde online.</span><span class="sxs-lookup"><span data-stu-id="e711c-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="e711c-118">Meddelelser sidder også fast i udbakken, når du klikker på **Send**, men du har ikke forbindelse.</span><span class="sxs-lookup"><span data-stu-id="e711c-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e711c-119">Klik på **Send/modtag,** og se på knappen **Arbejd offline.**</span><span class="sxs-lookup"><span data-stu-id="e711c-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e711c-120">Hvis den er blå, er forbindelsen afbrudt.</span><span class="sxs-lookup"><span data-stu-id="e711c-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e711c-121">Klik på den for at oprette forbindelse (knappen bliver hvid), og klik på **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="e711c-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e711c-122">**Aktiver Send med det samme, når der er oprettet forbindelse**</span><span class="sxs-lookup"><span data-stu-id="e711c-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e711c-123">Klik på **Indstillinger**under fanen Filer .</span><span class="sxs-lookup"><span data-stu-id="e711c-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e711c-124">Klik på **Avanceret**i dialogboksen Outlook-indstillinger .</span><span class="sxs-lookup"><span data-stu-id="e711c-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e711c-125">Klik på i sektionen Send og modtag for at aktivere **Send med det samme, når der er oprettet forbindelse**.</span><span class="sxs-lookup"><span data-stu-id="e711c-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e711c-126">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="e711c-126">Click **OK**.</span></span>
 
<span data-ttu-id="e711c-127">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="e711c-127">For full details, see:</span></span>
- [<span data-ttu-id="e711c-128">Video: Sende eller slette en fast låst mail</span><span class="sxs-lookup"><span data-stu-id="e711c-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e711c-129">Mail forbliver i mappen Udbakke, indtil du manuelt starter en send/modtag-handling i Outlook</span><span class="sxs-lookup"><span data-stu-id="e711c-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
