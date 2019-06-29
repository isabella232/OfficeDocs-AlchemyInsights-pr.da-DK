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
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383019"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="4d6ec-102">Identificere Indbakke regel aktivitet i overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="4d6ec-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="4d6ec-103">Du kan bruge overvågning log Søg i Security & Overholdelsescenter Indbakke regel hændelser (oprettelse, ændring og sletning af regler for Indbakke).</span><span class="sxs-lookup"><span data-stu-id="4d6ec-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="4d6ec-104">Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="4d6ec-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="4d6ec-105">Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.</span><span class="sxs-lookup"><span data-stu-id="4d6ec-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="4d6ec-106">Vælg datointervallet i felterne **startdato** og **slutdato** .</span><span class="sxs-lookup"><span data-stu-id="4d6ec-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="4d6ec-107">Under **Exchange postkasse aktiviteter**, skal du kontrollere feltet **aktiviteter** er indstillet til **Ny InboxRule Opret/Rediger/aktivere/deaktivere indbakkeregel**.</span><span class="sxs-lookup"><span data-stu-id="4d6ec-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="4d6ec-108">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="4d6ec-108">Click **Search**.</span></span>

<span data-ttu-id="4d6ec-109">Vælg en revisionspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="4d6ec-109">In the results, select an audit record.</span></span> <span data-ttu-id="4d6ec-110">Oplysninger om mærke, klik på **Flere oplysninger**.</span><span class="sxs-lookup"><span data-stu-id="4d6ec-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="4d6ec-111">Oplysninger om indstillinger for regler i Indbakke vises i feltet **parametre** .</span><span class="sxs-lookup"><span data-stu-id="4d6ec-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="4d6ec-112">Yderligere oplysninger finder du [fastlægge, hvis en bruger har oprettet en regel for Indbakke](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="4d6ec-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
