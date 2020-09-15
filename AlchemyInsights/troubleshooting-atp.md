---
title: Fejlfinding af Office 365 Advanced Threat Protection
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658908"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="6850b-102">Fejlfinding af Office 365 Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="6850b-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="6850b-103">Bemærker du forsinkelser i meddelelseslevering?</span><span class="sxs-lookup"><span data-stu-id="6850b-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="6850b-104">Brug indstillingen [dynamisk levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i din politik for sikker sikkerhedstilknytning af DTT.</span><span class="sxs-lookup"><span data-stu-id="6850b-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="6850b-105">Det hjælper med at undgå forsinkelser i meddelelser, mens du beskytter modtagere fra ondsindede filer.</span><span class="sxs-lookup"><span data-stu-id="6850b-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="6850b-106">Vil du rapportere falske positive eller falske negativer til Microsoft?</span><span class="sxs-lookup"><span data-stu-id="6850b-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="6850b-107">Brug dette [link](https://www.microsoft.com/wdsi/filesubmission/) til at sende filer til analyse.</span><span class="sxs-lookup"><span data-stu-id="6850b-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="6850b-108">Vidste du, at du kan aktivere beskyttelse af sikre links for interne mails, der sendes mellem modtagere i din organisation?</span><span class="sxs-lookup"><span data-stu-id="6850b-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="6850b-109">Følg disse trin:</span><span class="sxs-lookup"><span data-stu-id="6850b-109">Follow these steps:</span></span>

  1. <span data-ttu-id="6850b-110">Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator-eller sikkerhedsadministrator konto.</span><span class="sxs-lookup"><span data-stu-id="6850b-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="6850b-111">I venstre navigationsrude under **trussels styring**skal du **Policy** vælge \> **sikre links**til politik.</span><span class="sxs-lookup"><span data-stu-id="6850b-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="6850b-112">I de **politikker, der gælder for hele sektionen organisation** , skal du vælge politikken og klikke på **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="6850b-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="6850b-113">Under **Indstillinger**skal du aktivere **Anvend sikre links til meddelelser, der sendes inden for organisationen**.</span><span class="sxs-lookup"><span data-stu-id="6850b-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
