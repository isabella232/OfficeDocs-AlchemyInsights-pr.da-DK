---
title: Tip til DLP-politik fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932580"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="81086-102">Problemer med DLP-politiktip</span><span class="sxs-lookup"><span data-stu-id="81086-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="81086-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="81086-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="81086-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="81086-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="81086-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="81086-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="81086-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="81086-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="81086-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="81086-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="81086-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="81086-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="81086-109">**Tip til DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="81086-109">**DLP policy tips**</span></span>

<span data-ttu-id="81086-110">Når brugerne bruger **DLP-politikker**, kan de få besked om en politikovertrædelse med **politiktip**.</span><span class="sxs-lookup"><span data-stu-id="81086-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="81086-111">Administratorer kan konfigurere politiktip, der skal vises, mens de tester deres DLP-politik, eller når politikken er i fuld håndhævelsestilstand.</span><span class="sxs-lookup"><span data-stu-id="81086-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="81086-112">Hvis du vil konfigurere politiktip om din DLP-politik i Center for Sikkerhed og Overholdelse i fuld håndhævelsestilstand, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="81086-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="81086-113">Sørg for, at politiktip er **aktiveret** på DLP-reglen ved hjælp af trinnene [her](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="81086-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="81086-114">Sørg **for,** at dit indhold svarer til det, **der kræves** for at udløse den regel, der er beskrevet i denne artikel [her](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="81086-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="81086-115">Politiktip vises i både OWA og Outlook.</span><span class="sxs-lookup"><span data-stu-id="81086-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="81086-116">Men når du bruger **Outlook 2013 eller nyere**, vises politiktip kun under visse betingelser.</span><span class="sxs-lookup"><span data-stu-id="81086-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="81086-117">Disse betingelser er angivet her: [Understøttede betingelser for Outlook 2013 eller nyere til visning af politiktip](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="81086-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="81086-118">Yderligere oplysninger om Tip til DLP-politik finder du i: [Vis politiktip til DLP-politikker](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="81086-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  