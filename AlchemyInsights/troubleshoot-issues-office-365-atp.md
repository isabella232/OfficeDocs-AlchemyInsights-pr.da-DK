---
title: Fejlfinding af problemer med Microsoft Defender til Office 365 (DTT)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801401"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="1572f-102">Fejlfinding af problemer med Office 365 DTT</span><span class="sxs-lookup"><span data-stu-id="1572f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="1572f-103">**Oplever du forsinkelser med levering af mail** ?</span><span class="sxs-lookup"><span data-stu-id="1572f-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="1572f-104">Prøv at bruge indstillingen dynamisk levering for dine ATP-politikker for sikre vedhæftede filer.</span><span class="sxs-lookup"><span data-stu-id="1572f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="1572f-105">Dette vil undgå forsinkelser i levering af mails, når du beskytter modtagere fra ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="1572f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="1572f-106">**Vil du rapportere falske positive eller falske negativer** ?</span><span class="sxs-lookup"><span data-stu-id="1572f-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="1572f-107">Brug dette link til at sende filen til analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="1572f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="1572f-108">**Vidste du, at du kan aktivere beskyttelse med ATP sikre links for mails, der sendes mellem personer i organisationen** ?</span><span class="sxs-lookup"><span data-stu-id="1572f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="1572f-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="1572f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="1572f-110">Gå til https://protection.office.com , og log på.</span><span class="sxs-lookup"><span data-stu-id="1572f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="1572f-111">Gå til politik for sikre **trusler administration**  >  **Policy**  >  **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="1572f-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="1572f-112">Under **politikker, der gælder for bestemte modtagere** , skal du redigere (eller tilføje) en politik.</span><span class="sxs-lookup"><span data-stu-id="1572f-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="1572f-113">Vælg **Anvend sikre links til meddelelser, der sendes inden for organisationen** .</span><span class="sxs-lookup"><span data-stu-id="1572f-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="1572f-114">Gem din politik, og Tillad ca. 30 minutter, før dine ændringer fungerer på deres måde gennem dit datacenter.</span><span class="sxs-lookup"><span data-stu-id="1572f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="1572f-115">Du kan få mere hjælp til DTT i [Microsoft Defender til Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="1572f-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>