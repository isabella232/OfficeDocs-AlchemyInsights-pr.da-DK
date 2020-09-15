---
title: Identificer IP-adresse og klient i overvågningslogge
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668304"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="fc811-102">Identificer IP-adresse og klient i overvågningslogge</span><span class="sxs-lookup"><span data-stu-id="fc811-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="fc811-103">Den IP-adresse, der er knyttet til en aktivitet af en Microsoft 365-bruger eller-administrator, vises i overvågningsloggene.</span><span class="sxs-lookup"><span data-stu-id="fc811-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="fc811-104">Klientoplysningerne logføres også.</span><span class="sxs-lookup"><span data-stu-id="fc811-104">The client information is also logged.</span></span> <span data-ttu-id="fc811-105">Her er de trin, du skal følge for at identificere sådanne oplysninger</span><span class="sxs-lookup"><span data-stu-id="fc811-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="fc811-106">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="fc811-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fc811-107">Gå til søgesiden **Søg i**  >  **overvågningslogfil** .</span><span class="sxs-lookup"><span data-stu-id="fc811-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="fc811-108">Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen **aktiviteter** .</span><span class="sxs-lookup"><span data-stu-id="fc811-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="fc811-109">Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).</span><span class="sxs-lookup"><span data-stu-id="fc811-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="fc811-110">**Bemærk**: visse aktiviteter er muligvis ikke tilgængelige i menuen **aktiviteter** . de revisions elementer returneres dog, hvis **Vis resultater for alle aktiviteter** er markeret (standardindstillingen).</span><span class="sxs-lookup"><span data-stu-id="fc811-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="fc811-111">Angiv brugernavnet i feltet **brugere** , Vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="fc811-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="fc811-112">I resultaterne kan du se IP-adressen for den pågældende aktivitet i ruden resultater.</span><span class="sxs-lookup"><span data-stu-id="fc811-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="fc811-113">Markér revisions posten for at få vist detaljerede oplysninger **i pop op-vinduet (** f. eks. klient, bruger, der har udført handlingen osv.).</span><span class="sxs-lookup"><span data-stu-id="fc811-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="fc811-114">Du kan finde flere oplysninger i [finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="fc811-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
