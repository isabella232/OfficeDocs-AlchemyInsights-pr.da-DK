---
title: Identificer IP-adresse og klient i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508910"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="425ff-102">Identificer IP-adresse og klient i overvågningslogfiler</span><span class="sxs-lookup"><span data-stu-id="425ff-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="425ff-103">Den IP-adresse, der svarer til en aktivitet af en Microsoft 365-bruger eller -administrator, vises i overvågningsloggene.</span><span class="sxs-lookup"><span data-stu-id="425ff-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="425ff-104">Klientoplysningerne logføres også.</span><span class="sxs-lookup"><span data-stu-id="425ff-104">The client information is also logged.</span></span> <span data-ttu-id="425ff-105">Her er de skridt til at identificere sådanne oplysninger</span><span class="sxs-lookup"><span data-stu-id="425ff-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="425ff-106">Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="425ff-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="425ff-107">Gå til søgesiden for søgesøgning i søgeloggen søge i søgeloggen **for søgeloggen søge**i søgeloggen for  >  **søgesøgning.**</span><span class="sxs-lookup"><span data-stu-id="425ff-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="425ff-108">Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen **Aktiviteter.**</span><span class="sxs-lookup"><span data-stu-id="425ff-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="425ff-109">Hvis ikke, returneres alle aktiviteter for den valgte bruger (standardindstilling).</span><span class="sxs-lookup"><span data-stu-id="425ff-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="425ff-110">**Bemærk:** Visse aktiviteter er muligvis ikke tilgængelige i menuen **Aktiviteter.** Disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).</span><span class="sxs-lookup"><span data-stu-id="425ff-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="425ff-111">Angiv brugernavnet i feltet **Brugere,** vælg det relevante datointerval for aktiviteten, og klik derefter på **Søg**.</span><span class="sxs-lookup"><span data-stu-id="425ff-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="425ff-112">I resultaterne kan du se IP-adressen for den pågældende aktivitet i resultatruden.</span><span class="sxs-lookup"><span data-stu-id="425ff-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="425ff-113">Vælg overvågningsposten for at få vist detaljerede oplysninger i pop op-vinduet **Detaljer** (f.eks. klient, bruger, der udførte handlingen osv.).</span><span class="sxs-lookup"><span data-stu-id="425ff-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="425ff-114">Du kan finde flere oplysninger [under Finde IP-adressen på den computer, der bruges til at få adgang til en kompromitteret konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="425ff-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
