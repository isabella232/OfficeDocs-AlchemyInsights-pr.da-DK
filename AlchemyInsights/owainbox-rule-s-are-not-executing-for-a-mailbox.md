---
title: 1332 OWA - Indbakke-regler ikke udføres for en postkasse
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762217"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="f1627-102">En regel for indbakke virker ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="f1627-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="f1627-103">Kontroller følgende indstillinger:</span><span class="sxs-lookup"><span data-stu-id="f1627-103">Verify the following settings:</span></span>

- <span data-ttu-id="f1627-104">En meddelelse kan omdirigeres, videresendte eller besvarede automatisk baseret på indbakkereglerne kun én gang.</span><span class="sxs-lookup"><span data-stu-id="f1627-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="f1627-105">En omdirigere regel (en regel for Indbakke eller flow postregel, også kendt som hovedregel transport) kan tilføje op til ti modtagere i videresende en meddelelse.</span><span class="sxs-lookup"><span data-stu-id="f1627-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="f1627-106">Yderligere oplysninger finder du under [grænser for kladden, Transport, og Indbakke](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="f1627-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="f1627-107">Indbakkeregler fungerer ikke på den alternative journalføring postkasse.</span><span class="sxs-lookup"><span data-stu-id="f1627-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="f1627-108">Yderligere oplysninger om alternative journalføring postkassen, se [alternativ journalføring postkasse](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="f1627-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="f1627-109">Du kan løse disse problemer ved at se [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="f1627-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="f1627-110">Hvis du ikke anvender de tidligere problemer, køre Indbakke regel Diagnosticeringsrapport, før du eskalere problemet til Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="f1627-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="f1627-111">Åbne postkassen i Outlook på internettet, og klik på **Indstillinger for** \> **Indstillinger** \> **Organiser e-mail** \> **af regler for indbakken**.</span><span class="sxs-lookup"><span data-stu-id="f1627-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="f1627-112">Klik på **Hvis reglerne ikke arbejder Klik her for at generere en diagnosticeringsrapport**nederst på siden.</span><span class="sxs-lookup"><span data-stu-id="f1627-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
