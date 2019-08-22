---
title: Identificere Indbakke regel aktivitet i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539156"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="95e15-102">Identificere Indbakke regel aktivitet i overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="95e15-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="95e15-103">Du kan bruge overvågning log søgning i Office 365 sikkerhed & Overholdelsescenter Indbakke regel hændelser (oprettelse, ændring og sletning af regler for Indbakke).</span><span class="sxs-lookup"><span data-stu-id="95e15-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="95e15-104">Log på [Office 365 sikkerhed & Overholdelsescenter](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="95e15-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="95e15-105">Gå til **Søg** > **revision log** søgeside.</span><span class="sxs-lookup"><span data-stu-id="95e15-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="95e15-106">Vælg datointervallet i felterne **startdato** og **slutdato** .</span><span class="sxs-lookup"><span data-stu-id="95e15-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="95e15-107">Under **Exchange postkasse aktiviteter**, skal du kontrollere feltet **aktiviteter** er indstillet til **Ny InboxRule Opret/Rediger/aktivere/deaktivere indbakkeregel**.</span><span class="sxs-lookup"><span data-stu-id="95e15-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="95e15-108">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="95e15-108">Click **Search**.</span></span>

<span data-ttu-id="95e15-109">Vælg en revisionspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="95e15-109">In the results, select an audit record.</span></span> <span data-ttu-id="95e15-110">Oplysninger om mærke, klik på **Flere oplysninger**.</span><span class="sxs-lookup"><span data-stu-id="95e15-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="95e15-111">Oplysninger om indstillinger for regler i Indbakke vises i feltet **parametre** .</span><span class="sxs-lookup"><span data-stu-id="95e15-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="95e15-112">Yderligere oplysninger finder du [fastlægge, hvis en bruger har oprettet en regel for Indbakke](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="95e15-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
