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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241246"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="9e368-102">Rette meddelelser, der sidder fast i udbakken</span><span class="sxs-lookup"><span data-stu-id="9e368-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="9e368-103">Vi anbefaler, at du starter med at køre scenariet ["Jeg har problemer med at sende, modtage eller finde mails"](https://aka.ms/SaRA-OutlookSendReceive) fra [værktøjet Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="9e368-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="9e368-104">Når en meddelelse sidder fast i udbakken, er den mest sandsynlige årsag en stor vedhæftet fil, eller indstillingen "Send med det samme, når den er tilsluttet" er ikke aktiveret.</span><span class="sxs-lookup"><span data-stu-id="9e368-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="9e368-105">**Fjerne den store vedhæftede fil**</span><span class="sxs-lookup"><span data-stu-id="9e368-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="9e368-106">Vælg **Send/modtag** > **arbejde offline i**Outlook .</span><span class="sxs-lookup"><span data-stu-id="9e368-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="9e368-107">Vælg **Udbakke**i navigationsruden .</span><span class="sxs-lookup"><span data-stu-id="9e368-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="9e368-108">Herfra kan du:</span><span class="sxs-lookup"><span data-stu-id="9e368-108">From here, you can:</span></span> 
    - <span data-ttu-id="9e368-109">Slet meddelelsen (vælg den, og vælg derefter **Slet**).</span><span class="sxs-lookup"><span data-stu-id="9e368-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="9e368-110">Træk meddelelsen til mappen Kladder, dobbeltklik for at åbne den, og fjern markeringen af den vedhæftede fil, og vælg derefter **Slet**).</span><span class="sxs-lookup"><span data-stu-id="9e368-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="9e368-111">Hvis du får vist en fejlmeddelelse om, at Outlook forsøger at sende meddelelsen, skal du lukke Outlook.</span><span class="sxs-lookup"><span data-stu-id="9e368-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="9e368-112">Det kan tage et øjeblik at afslutte.</span><span class="sxs-lookup"><span data-stu-id="9e368-112">It may take a few moments to exit.</span></span> <span data-ttu-id="9e368-113">Hvis Outlook ikke lukker, skal du trykke på Ctrl+Alt+Delete og vælge **Start Jobliste**.</span><span class="sxs-lookup"><span data-stu-id="9e368-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="9e368-114">Vælg fanen **Processer** i Jobliste, rul ned til outlook.exe, og vælg **Afslut proces**.</span><span class="sxs-lookup"><span data-stu-id="9e368-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="9e368-115">Når Outlook er lukket, skal du genstarte den og gentage trin 2 og 3.</span><span class="sxs-lookup"><span data-stu-id="9e368-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="9e368-116">Når du har fjernet den vedhæftede fil, skal du klikke på **Send/modtag** > **arbejde offline** for at fortsætte med at arbejde online.</span><span class="sxs-lookup"><span data-stu-id="9e368-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="9e368-117">Meddelelser sidder også fast i udbakken, når du klikker på **Send**, men du har ikke forbindelse.</span><span class="sxs-lookup"><span data-stu-id="9e368-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="9e368-118">Klik på **Send/modtag,** og se på knappen **Arbejd offline.**</span><span class="sxs-lookup"><span data-stu-id="9e368-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="9e368-119">Hvis den er blå, er forbindelsen afbrudt.</span><span class="sxs-lookup"><span data-stu-id="9e368-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="9e368-120">Klik på den for at oprette forbindelse (knappen bliver hvid), og klik på **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="9e368-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="9e368-121">**Aktiver Send med det samme, når der er oprettet forbindelse**</span><span class="sxs-lookup"><span data-stu-id="9e368-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="9e368-122">Klik på **Indstillinger**under fanen Filer .</span><span class="sxs-lookup"><span data-stu-id="9e368-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="9e368-123">Klik på **Avanceret**i dialogboksen Outlook-indstillinger .</span><span class="sxs-lookup"><span data-stu-id="9e368-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="9e368-124">Klik på i sektionen Send og modtag for at aktivere **Send med det samme, når der er oprettet forbindelse**.</span><span class="sxs-lookup"><span data-stu-id="9e368-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="9e368-125">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="9e368-125">Click **OK**.</span></span>
 
<span data-ttu-id="9e368-126">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="9e368-126">For full details, see:</span></span>
- [<span data-ttu-id="9e368-127">Video: Sende eller slette en fast låst mail</span><span class="sxs-lookup"><span data-stu-id="9e368-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="9e368-128">Mail forbliver i mappen Udbakke, indtil du manuelt starter en send/modtag-handling i Outlook</span><span class="sxs-lookup"><span data-stu-id="9e368-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
