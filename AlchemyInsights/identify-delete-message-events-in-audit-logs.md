---
title: Identificer slette meddelelseshændelser i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508982"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="86f3b-102">Overvåge logfiler for slettede mails</span><span class="sxs-lookup"><span data-stu-id="86f3b-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="86f3b-103">Fra januar 2019 slår Microsoft som standard loggerføring af postkasseovervågning til.</span><span class="sxs-lookup"><span data-stu-id="86f3b-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="86f3b-104">Hvis du vil gennemse slette meddelelseshændelser for en bestemt bruger, skal du manuelt aktivere slettehandlingerne til overvågning.</span><span class="sxs-lookup"><span data-stu-id="86f3b-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="86f3b-105">Hvis logføring af postkasseovervågning allerede er aktiveret for din organisation eller for den specifikke bruger, skal du følge nedenstående trin.</span><span class="sxs-lookup"><span data-stu-id="86f3b-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="86f3b-106">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="86f3b-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="86f3b-107">Klik på **Søg og undersøg,** og vælg **Søg i overvågningsloggen**.</span><span class="sxs-lookup"><span data-stu-id="86f3b-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="86f3b-108">Vælg datointervallet i felterne **Startdato** og **Slutdato.**</span><span class="sxs-lookup"><span data-stu-id="86f3b-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="86f3b-109">Angiv brugernavn til den bruger, du vil undersøge (den bruger, der har slettet elementerne).</span><span class="sxs-lookup"><span data-stu-id="86f3b-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="86f3b-110">I feltet **Aktiviteter** skal du vælge **Slettede meddelelser fra mappen Slettet post** og **Flyttede meddelelser til mappen Slettet post**.</span><span class="sxs-lookup"><span data-stu-id="86f3b-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="86f3b-111">Klik på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="86f3b-111">Click **Search**.</span></span>

<span data-ttu-id="86f3b-112">Vælg en overvågningspost i resultaterne.</span><span class="sxs-lookup"><span data-stu-id="86f3b-112">In the results, select an audit record.</span></span> <span data-ttu-id="86f3b-113">Klik på **Flere oplysninger**i pop op-vinduet med oplysninger .</span><span class="sxs-lookup"><span data-stu-id="86f3b-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="86f3b-114">Yderligere oplysninger om det slettede element (f.eks. emnelinjen og placeringen af elementet, da det blev slettet) vises i feltet **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="86f3b-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="86f3b-115">Egenskaben **ClientInfoString** viser, om sletningen fandt sted i Outlook, Outlook på internettet (tidligere kaldet Outlook Web App) eller en anden enhed.</span><span class="sxs-lookup"><span data-stu-id="86f3b-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="86f3b-116">Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail til en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="86f3b-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="86f3b-117">**Bemærk:** Du kan ikke hente slettede elementer ved hjælp af overvågningslogfunktionen.</span><span class="sxs-lookup"><span data-stu-id="86f3b-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="86f3b-118">Hvis du vil hente slettede meddelelser i Outlook på internettet, skal du se [Gendanne slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="86f3b-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
