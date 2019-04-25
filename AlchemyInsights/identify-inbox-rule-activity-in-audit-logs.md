---
title: Identificere Indbakke regel aktivitet i overvågningslogge
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417241"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="dbb02-102">Identificere Indbakke regel aktivitet i overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="dbb02-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="dbb02-103">Du kan bruge overvågning log Søg i Security & Overholdelsescenter Indbakke regel hændelser (oprettelse, ændring og sletning af regler for Indbakke).</span><span class="sxs-lookup"><span data-stu-id="dbb02-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="dbb02-104">Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="dbb02-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="dbb02-105">Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.</span><span class="sxs-lookup"><span data-stu-id="dbb02-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="dbb02-106">Vælg datointervallet i felterne **startdato** og **slutdato** .</span><span class="sxs-lookup"><span data-stu-id="dbb02-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="dbb02-107">Under **Exchange postkasse aktiviteter**, skal du kontrollere feltet **aktiviteter** er indstillet til **Ny InboxRule Opret/Rediger/aktivere/deaktivere indbakkeregel**.</span><span class="sxs-lookup"><span data-stu-id="dbb02-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="dbb02-108">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="dbb02-108">Click **Search**.</span></span>

<span data-ttu-id="dbb02-109">Vælg en revisionspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="dbb02-109">In the results, select an audit record.</span></span> <span data-ttu-id="dbb02-110">Oplysninger om mærke, klik på **Flere oplysninger**.</span><span class="sxs-lookup"><span data-stu-id="dbb02-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="dbb02-111">Oplysninger om indstillinger for regler i Indbakke vises i feltet **parametre** .</span><span class="sxs-lookup"><span data-stu-id="dbb02-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="dbb02-112">Yderligere oplysninger finder du [fastlægge, hvis en bruger har oprettet en regel for Indbakke](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="dbb02-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
