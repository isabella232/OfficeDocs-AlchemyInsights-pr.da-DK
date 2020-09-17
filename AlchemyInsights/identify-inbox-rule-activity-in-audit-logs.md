---
title: Identificere aktivitet for Indbakke regel i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779045"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="9eb67-102">Identificere aktivitet for Indbakke regel i overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="9eb67-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="9eb67-103">Du kan bruge søgning i overvågningsloggen i Microsoft 365 Security & overholdelses Center til at få vist regler for Indbakke-regler (oprette, redigere og slette indbakkeregler).</span><span class="sxs-lookup"><span data-stu-id="9eb67-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="9eb67-104">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9eb67-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9eb67-105">Gå til søgesiden **Søg i**  >  **overvågningslogfil** .</span><span class="sxs-lookup"><span data-stu-id="9eb67-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="9eb67-106">Vælg datointervallet i felterne **Start dato** og **Slutdato** .</span><span class="sxs-lookup"><span data-stu-id="9eb67-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="9eb67-107">Under **aktiviteter for Exchange-postkassen**skal du kontrollere, at feltet **aktiviteter** er indstillet til **New-InboxRule Create/Modify/enable/disable indbakke Rule**.</span><span class="sxs-lookup"><span data-stu-id="9eb67-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="9eb67-108">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="9eb67-108">Click **Search**.</span></span>

<span data-ttu-id="9eb67-109">I resultaterne skal du vælge en revisionspost.</span><span class="sxs-lookup"><span data-stu-id="9eb67-109">In the results, select an audit record.</span></span> <span data-ttu-id="9eb67-110">Klik på **flere oplysninger**i pop op-vinduet detaljer.</span><span class="sxs-lookup"><span data-stu-id="9eb67-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9eb67-111">Oplysninger om indstillingerne for Indbakke-reglen vises i feltet **parametre** .</span><span class="sxs-lookup"><span data-stu-id="9eb67-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="9eb67-112">Du kan finde flere oplysninger under [afgøre, om en bruger har oprettet en indbakke regel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="9eb67-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
