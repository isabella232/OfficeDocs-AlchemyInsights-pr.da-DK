---
title: Fejlfinding i forbindelse med avanceret trusselsbeskyttelse i Office 365
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
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732396"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="07d9f-102">Fejlfinding i forbindelse med avanceret trusselsbeskyttelse i Office 365</span><span class="sxs-lookup"><span data-stu-id="07d9f-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="07d9f-103">Bemærker du forsinkelser i leveringen af meddelelser?</span><span class="sxs-lookup"><span data-stu-id="07d9f-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="07d9f-104">Brug indstillingen [Dynamisk levering](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) i politikken for vedhæftede filer, der er tillid til ATP.</span><span class="sxs-lookup"><span data-stu-id="07d9f-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="07d9f-105">Dette vil hjælpe med at undgå forsinkelser i meddelelserne, samtidig med at modtagerne beskyttes mod skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="07d9f-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="07d9f-106">Vil du rapportere falske positiver eller falske negativer til Microsoft?</span><span class="sxs-lookup"><span data-stu-id="07d9f-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="07d9f-107">Brug dette [link](https://www.microsoft.com/wdsi/filesubmission/) til at sende filer til analyse.</span><span class="sxs-lookup"><span data-stu-id="07d9f-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="07d9f-108">Vidste du, at du kan aktivere Safe Links-beskyttelse for interne mails, der sendes mellem modtagere i organisationen?</span><span class="sxs-lookup"><span data-stu-id="07d9f-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="07d9f-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="07d9f-109">Follow these steps:</span></span>

  1. <span data-ttu-id="07d9f-110">Gå [https://protection.office.com](https://protection.office.com) til og log på med en global administrator- eller sikkerhedsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="07d9f-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="07d9f-111">Vælg **Politiksikre** \> **links**i venstre navigationsrude under **Trusselsstyring**.</span><span class="sxs-lookup"><span data-stu-id="07d9f-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="07d9f-112">Vælg politikken i sektionen **Politikker, der gælder for hele organisationen,** og klik på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="07d9f-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="07d9f-113">Aktiver **Anvend sikre links til meddelelser, der sendes i organisationen ,** under **Indstillinger**.</span><span class="sxs-lookup"><span data-stu-id="07d9f-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
