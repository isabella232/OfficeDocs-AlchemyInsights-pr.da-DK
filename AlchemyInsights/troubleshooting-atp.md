---
title: Fejlfinding i forbindelse med avanceret beskyttelse mod office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512584"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="e3ec0-102">Fejlfinding i forbindelse med avanceret beskyttelse mod office 365</span><span class="sxs-lookup"><span data-stu-id="e3ec0-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="e3ec0-103">Bemærker du forsinkelser i leveringen af meddelelser?</span><span class="sxs-lookup"><span data-stu-id="e3ec0-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="e3ec0-104">Brug indstillingen [Dynamisk levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i din politik om attponere for sikre bilag i ATP.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="e3ec0-105">Dette vil hjælpe med at undgå beskedforsinkelser og samtidig beskytte modtagerne mod skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e3ec0-106">Vil du rapportere falske positiver eller falske negativer til Microsoft?</span><span class="sxs-lookup"><span data-stu-id="e3ec0-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="e3ec0-107">Brug dette [link](https://www.microsoft.com/wdsi/filesubmission/) til at sende filer til analyse.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="e3ec0-108">Vidste du, at du kan aktivere beskyttelse af sikre links for interne mails, der sendes mellem modtagere i organisationen?</span><span class="sxs-lookup"><span data-stu-id="e3ec0-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="e3ec0-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="e3ec0-109">Follow these steps:</span></span>

  1. <span data-ttu-id="e3ec0-110">Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator- eller sikkerhedsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e3ec0-111">Vælg **Policy** Politiksikre links i venstre navigationsrude under **Trusselsstyring** \> **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="e3ec0-112">Vælg politikken i sektionen **Politikker, der gælder for hele organisationen,** og klik på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="e3ec0-113">Under **Indstillinger**skal du aktivere **Anvend sikre links på meddelelser, der sendes i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="e3ec0-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
