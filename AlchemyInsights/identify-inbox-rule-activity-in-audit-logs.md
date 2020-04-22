---
title: Identificer aktivitet for indbakkeregel i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716418"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="a70a5-102">Identificer aktivitet for indbakkeregel i overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="a70a5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="a70a5-103">Du kan bruge overvågningslogsøgning i Microsoft 365 Security & Compliance Center til at få vist regelhændelser i indbakken (oprettelse, ændring og sletning af indbakkeregler).</span><span class="sxs-lookup"><span data-stu-id="a70a5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="a70a5-104">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a70a5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a70a5-105">Gå til**søgesiden for søgefilen til søgeovervågning** i **søgefilen** > til søgning i søgeområdet.</span><span class="sxs-lookup"><span data-stu-id="a70a5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="a70a5-106">Vælg datointervallet i felterne **Startdato** **og Slutdato.**</span><span class="sxs-lookup"><span data-stu-id="a70a5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="a70a5-107">Under **Exchange Mailbox Activities**skal du kontrollere , at feltet **Aktiviteter** er angivet til **Ny IndbakkeRegel Opret/rediger/aktiver/deaktiver indbakkereglen**.</span><span class="sxs-lookup"><span data-stu-id="a70a5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="a70a5-108">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="a70a5-108">Click **Search**.</span></span>

<span data-ttu-id="a70a5-109">Vælg en overvågningspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="a70a5-109">In the results, select an audit record.</span></span> <span data-ttu-id="a70a5-110">Klik på Flere oplysninger i pop **op-vinduet med**detaljer .</span><span class="sxs-lookup"><span data-stu-id="a70a5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="a70a5-111">Oplysninger om indstillingerne for indbakkeregel vises i feltet **Parametre.**</span><span class="sxs-lookup"><span data-stu-id="a70a5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="a70a5-112">Du kan finde flere oplysninger [under Bestemme, om en bruger har oprettet en indbakkeregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="a70a5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
