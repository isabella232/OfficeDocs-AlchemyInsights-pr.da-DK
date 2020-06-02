---
title: Fejlfinding i forbindelse med problemer med Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511106"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="79d74-102">Fejlfinding i forbindelse med problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="79d74-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="79d74-103">**Meddelelse forsinkelser med levering af e-mail-besked?**</span><span class="sxs-lookup"><span data-stu-id="79d74-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="79d74-104">Prøv at bruge indstillingen Dynamisk levering til dine politikker for safe attachments for ATP.</span><span class="sxs-lookup"><span data-stu-id="79d74-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="79d74-105">Derved undgås forsinkelser i leveringen af e-mails, samtidig med at modtagerne beskyttes mod skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="79d74-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="79d74-106">**Vil du rapportere falske positiver eller falske negativer?**</span><span class="sxs-lookup"><span data-stu-id="79d74-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="79d74-107">Brug dette link til at sende filen til analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="79d74-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="79d74-108">**Vidste du, at du kan aktivere BESKYTTELSE OM ATP Safe Links for mails, der sendes mellem personer i organisationen?**</span><span class="sxs-lookup"><span data-stu-id="79d74-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="79d74-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="79d74-109">Follow these steps:</span></span>
    1. <span data-ttu-id="79d74-110">Gå til https://protection.office.com , og log på.</span><span class="sxs-lookup"><span data-stu-id="79d74-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="79d74-111">Gå til **Beskyttelseslinks til trusselshåndteringspolitik**  >  **Policy**  >  **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="79d74-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="79d74-112">Under **Politikker, der gælder for bestemte modtagere**, skal du redigere (eller tilføje) en politik.</span><span class="sxs-lookup"><span data-stu-id="79d74-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="79d74-113">Vælg **Anvend sikre links på meddelelser, der sendes i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="79d74-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="79d74-114">Gem din politik, og giv dig ca. 30 minutter til, at ændringerne kan arbejde sig gennem dit datacenter.</span><span class="sxs-lookup"><span data-stu-id="79d74-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="79d74-115">Hvis du vil have mere hjælp til ATP, skal du se [Avanceret beskyttelse mod trusler i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="79d74-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>