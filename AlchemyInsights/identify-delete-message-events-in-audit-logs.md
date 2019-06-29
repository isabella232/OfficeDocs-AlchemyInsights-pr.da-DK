---
title: Identificere Slet meddelelse hændelser i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383127"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6d158-102">Overvågningslogge for slettede e-mails</span><span class="sxs-lookup"><span data-stu-id="6d158-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6d158-103">Starter i januar 2019, Microsoft er at aktivere postkassen Overvåg logføring som standard.</span><span class="sxs-lookup"><span data-stu-id="6d158-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6d158-104">Ellers for at få vist Slet meddelelse hændelser for en bestemt bruger, skal du aktivere manuelt slettehandlingerne for overvågning.</span><span class="sxs-lookup"><span data-stu-id="6d158-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6d158-105">Hvis overvågning af postkasse logføring er allerede aktiveret for organisationen, eller for en bestemt bruger, skal du følge nedenstående trin.</span><span class="sxs-lookup"><span data-stu-id="6d158-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6d158-106">Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6d158-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6d158-107">Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.</span><span class="sxs-lookup"><span data-stu-id="6d158-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6d158-108">Vælg datointervallet i felterne **startdato** og **slutdato** .</span><span class="sxs-lookup"><span data-stu-id="6d158-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6d158-109">Angiv brugernavnet for den bruger, du vil undersøge (den bruger, der har slettet elementerne).</span><span class="sxs-lookup"><span data-stu-id="6d158-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6d158-110">I feltet **aktiviteter** , skal du vælge **slettede meddelelser fra mappen Slettet post** og **Moved meddelelser til mappen Slettet post**.</span><span class="sxs-lookup"><span data-stu-id="6d158-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6d158-111">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="6d158-111">Click **Search**.</span></span>

<span data-ttu-id="6d158-112">Vælg en revisionspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="6d158-112">In the results, select an audit record.</span></span> <span data-ttu-id="6d158-113">Oplysninger om mærke, klik på **Flere oplysninger**.</span><span class="sxs-lookup"><span data-stu-id="6d158-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6d158-114">Yderligere oplysninger om elementet slettet (for eksempel, emnelinjen og placeringen af varen, da den blev slettet) vises i feltet **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="6d158-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6d158-115">Egenskaben **ClientInfoString** vises, hvis sletningen opstod i Outlook, Outlook på internettet (tidligere kendt som Outlook Web App), eller en anden enhed.</span><span class="sxs-lookup"><span data-stu-id="6d158-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6d158-116">Yderligere oplysninger finder du [fastlægge, der har konfigureret e-mail videresendes til en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="6d158-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6d158-117">**Bemærk**: Du kan ikke hente slettede emner ved hjælp af funktionen overvågning log.</span><span class="sxs-lookup"><span data-stu-id="6d158-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6d158-118">Hvis du vil hente slettede meddelelser i Outlook på internettet, se [gendanne slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="6d158-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
