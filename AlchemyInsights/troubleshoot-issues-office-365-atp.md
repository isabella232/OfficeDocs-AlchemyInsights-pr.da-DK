---
title: Fejlfinding af problemer med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766739"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="9569b-102">Fejlfinding af problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="9569b-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="9569b-103">**Bemærk forsinkelser med levering af e-mail-meddelelser?**</span><span class="sxs-lookup"><span data-stu-id="9569b-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="9569b-104">Prøv at bruge indstillingen Dynamisk levering til politikkerne for vedhæftede filer, der er sikkert for ATP.</span><span class="sxs-lookup"><span data-stu-id="9569b-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="9569b-105">Dette vil undgå forsinkelser i leveringen af e-mails, samtidig med at modtagerne beskyttes mod skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="9569b-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="9569b-106">**Vil du rapportere falske positiver eller falske negativer?**</span><span class="sxs-lookup"><span data-stu-id="9569b-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="9569b-107">Brug dette link til at sende filen til analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="9569b-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="9569b-108">**Vidste du, at du kan aktivere ATP Safe Links beskyttelse for e-mail sendt mellem personer i din organisation?**</span><span class="sxs-lookup"><span data-stu-id="9569b-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="9569b-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="9569b-109">Follow these steps:</span></span>
    1. <span data-ttu-id="9569b-110">Gå https://protection.office.comtil , og log på.</span><span class="sxs-lookup"><span data-stu-id="9569b-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="9569b-111">Gå til **Politik for trusselsstyring,** > **Policy** > **Sikre links**.</span><span class="sxs-lookup"><span data-stu-id="9569b-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="9569b-112">Rediger (eller tilføj) en politik **under Politikker, der gælder for bestemte modtagere.**</span><span class="sxs-lookup"><span data-stu-id="9569b-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="9569b-113">Vælg **Anvend sikre links til meddelelser, der sendes i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="9569b-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="9569b-114">Gem din politik, og giv dine ændringer ca. 30 minutter til at fungere gennem datacenteret.</span><span class="sxs-lookup"><span data-stu-id="9569b-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="9569b-115">Du kan få mere hjælp til ATP under [Avanceret trusselsbeskyttelse i Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="9569b-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>